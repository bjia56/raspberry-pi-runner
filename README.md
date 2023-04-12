<!-- start title -->

# GitHub Action: Raspberry Pi VM Runner

<!-- end title -->
<!-- start description -->

Action to execute commands within a Raspberry Pi VM running on QEMU

<!-- end description -->
<!-- start contents -->
<!-- end contents -->
<!-- start usage -->

```yaml
- uses: bjia56/raspberry-pi-runner@main
  with:
    # Commands to run on the Pi, executed with /bin/bash
    # Default: uname -a
    commands: ""

    # User to run commands on the Pi, either pi or root
    # Default: pi
    user: ""

    # Path on the host to copy into the VM, before commands are executed
    # Default:
    prerun_copy_from: ""

    # Path on the VM to copy files to, before commands are executed
    # Default: /home/pi
    prerun_copy_to: ""

    # Path on the VM to copy to the host, after commands are executed
    # Default:
    postrun_copy_from: ""

    # Path on the host to copy files to, after commands are executed
    # Default: .
    postrun_copy_to: ""

    # Print debugging output from VM initialization and teardown
    # Default: no
    debug: ""
```

<!-- end usage -->
<!-- start inputs -->

| **Input**                          | **Description**                                                    | **Default**           | **Required** |
| ---------------------------------- | ------------------------------------------------------------------ | --------------------- | ------------ |
| **<code>commands</code>**          | Commands to run on the Pi, executed with /bin/bash                 | <code>uname -a</code> | **true**     |
| **<code>user</code>**              | User to run commands on the Pi, either pi or root                  | <code>pi</code>       | **true**     |
| **<code>prerun_copy_from</code>**  | Path on the host to copy into the VM, before commands are executed |                       | **false**    |
| **<code>prerun_copy_to</code>**    | Path on the VM to copy files to, before commands are executed      | <code>/home/pi</code> | **false**    |
| **<code>postrun_copy_from</code>** | Path on the VM to copy to the host, after commands are executed    |                       | **false**    |
| **<code>postrun_copy_to</code>**   | Path on the host to copy files to, after commands are executed     | <code>.</code>        | **false**    |
| **<code>debug</code>**             | Print debugging output from VM initialization and teardown         | <code>no</code>       | **false**    |

<!-- end inputs -->
<!-- start outputs -->
<!-- end outputs -->
<!-- start [.github/ghadocs/examples/] -->
<!-- end [.github/ghadocs/examples/] -->
