# Ansible Playbook Visual Guide

This document contains ASCII diagrams and visual representations of how the Ansible playbook works and what the output looks like.

## Overview

```
  +---------+      +---------------+      +------------+  
  |  User   |----->| Ansible Play  |----->|  Target    |  
  |         |      |   Book        |      |  Machine   |  
  +---------+      +---------------+      +------------+  
```

## Execution Flow

```
1. User initiates playbook
2. Ansible processes tasks in playbook
3. Tasks are executed on target machines
4. Results are gathered and reported back
```

## Expected Output

```
TASK [Install Apache] *************************************************************************
changed: [target1]

TASK [Start Apache] **************************************************************************
changed: [target1]  

PLAY RECAP ************************************************************************************
target1                    : ok=2    changed=2    unreachable=0    failed=0 
```

---

This guide will help users understand the components and execution of Ansible playbooks effectively.