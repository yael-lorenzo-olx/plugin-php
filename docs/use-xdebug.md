# 1. Open Edit Configurations
![image](resources/img/step1.png)
![image](resources/img/step2.png)

# 2. Add PHP Remote Debug
![image](resources/img/step3.png)
![image](resources/img/step4.png)

# 3. Add Server
![image](resources/img/step5.png)
![image](resources/img/step6.png)

# 4. Set Path Mappings
![image](resources/img/step7.png)
![image](resources/img/step8.png)

**Note:**

* `/opt/athena-php` must be mapped to the `php` folder in the `athena` project
* `/opt/tests` must be mapped to your tests project.

# 5. Debug
![image](resources/img/step9.png)
![image](resources/img/step10.png)

Then run the `athena` command in the CLI and that's it, happy Debugging!!!

# Profiling

In case you would like to perform php profiling of your tests you need to set variable `ATHENA_ENABLE_PROFILER=1` before test execution.

XDebug Profiler is being enabled with following parameters:

```
profiler_enable=1
profiler_output_dir=/opt/tests
```

 `/opt/tests` should be mapped to your tests directory so that after the test execution with profiler enabled you should find your profile information files in main test directory.
