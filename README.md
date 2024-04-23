### --- Oracle APEX Installation ---

sqlplus / as sysdba <br>
alter session set container = xepdb1;
@apexins.sql SYSAUX SYSAUX TEMP /i/
@apxchpwd.sql
-- restarting process --
ALTER USER APEX_PUBLIC_USER ACCOUNT UNLOCK;
ALTER USER APEX_PUBLIC_USER IDENTIFIED BY (password)
@apex_rest_config.sql
