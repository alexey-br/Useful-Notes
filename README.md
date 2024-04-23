### --- Oracle APEX Installation ---

sqlplus / as sysdba <br>
alter session set container = xepdb1; <br>
@apexins.sql SYSAUX SYSAUX TEMP /i/ <br>
@apxchpwd.sql <br>
* restarting process *
ALTER USER APEX_PUBLIC_USER ACCOUNT UNLOCK; <br>
ALTER USER APEX_PUBLIC_USER IDENTIFIED BY (password) <br>
@apex_rest_config.sql <br>
