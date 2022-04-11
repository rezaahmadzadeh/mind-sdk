It is best to use windows Powershell for working with Hexa.

1. The first step is to login to the Developer bridge

```shell
> mind login <user_name> <passwd>
```

*Note:* your Developer bridge ID might be different than your Simualtor ID.

2. Now you should switch to robot's wifi. The security code is the last 8 digits on the network name.

3. Make sure the robot is on and the led is blue/purple?

4. Find the robot using

```shell
> mind scan
```
you will see robot's IP and name.

5. Now, you should set the default robot

```shell
> mind set-default-robot <robot_name>
```

6. You can initialize a project 

```shell
> mind init <project_name> --robottype <robot_name>
```

7. You then change directory to the project directory and build the project

```shell
> cd <project_name>
> mind build
> mind pack
```

8. Then you can run the .mpk file built in the previous step.

```shell
> mind run
```



