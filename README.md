[ec2-user@web-server ~]$ sudo cat /var/log/cloud-init-output.log
Cloud-init v. 19.3-46.amzn2.0.7 running 'init-local' at Thu, 25 Dec 2025 05:22:08 +0000. Up 4.38 seconds.
Cloud-init v. 19.3-46.amzn2.0.7 running 'init' at Thu, 25 Dec 2025 05:22:09 +0000. Up 5.44 seconds.
ci-info: ++++++++++++++++++++++++++++++++++++++Net device info++++++++++++++++++++++++++++++++++++++
ci-info: +--------+------+----------------------------+---------------+--------+-------------------+
ci-info: | Device |  Up  |          Address           |      Mask     | Scope  |     Hw-Address    |
ci-info: +--------+------+----------------------------+---------------+--------+-------------------+
ci-info: |  eth0  | True |        10.200.0.101        | 255.255.255.0 | global | 06:e9:be:ce:0a:55 |
ci-info: |  eth0  | True | fe80::4e9:beff:fece:a55/64 |       .       |  link  | 06:e9:be:ce:0a:55 |
ci-info: |   lo   | True |         127.0.0.1          |   255.0.0.0   |  host  |         .         |
ci-info: |   lo   | True |          ::1/128           |       .       |  host  |         .         |
ci-info: +--------+------+----------------------------+---------------+--------+-------------------+
ci-info: +++++++++++++++++++++++++++++++Route IPv4 info++++++++++++++++++++++++++++++++
ci-info: +-------+-----------------+------------+-----------------+-----------+-------+
ci-info: | Route |   Destination   |  Gateway   |     Genmask     | Interface | Flags |
ci-info: +-------+-----------------+------------+-----------------+-----------+-------+
ci-info: |   0   |     0.0.0.0     | 10.200.0.1 |     0.0.0.0     |    eth0   |   UG  |
ci-info: |   1   |    10.200.0.0   |  0.0.0.0   |  255.255.255.0  |    eth0   |   U   |
ci-info: |   2   | 169.254.169.254 |  0.0.0.0   | 255.255.255.255 |    eth0   |   UH  |
ci-info: +-------+-----------------+------------+-----------------+-----------+-------+
ci-info: +++++++++++++++++++Route IPv6 info+++++++++++++++++++
ci-info: +-------+-------------+---------+-----------+-------+
ci-info: | Route | Destination | Gateway | Interface | Flags |
ci-info: +-------+-------------+---------+-----------+-------+
ci-info: |   9   |  fe80::/64  |    ::   |    eth0   |   U   |
ci-info: |   11  |    local    |    ::   |    eth0   |   U   |
ci-info: |   12  |   ff00::/8  |    ::   |    eth0   |   U   |
ci-info: +-------+-------------+---------+-----------+-------+
Cloud-init v. 19.3-46.amzn2.0.7 running 'modules:config' at Thu, 25 Dec 2025 05:22:11 +0000. Up 7.02 seconds.
Loaded plugins: extras_suggestions, langpacks, priorities, update-motd
No packages needed for security; 0 packages available
No packages marked for update
Cloud-init v. 19.3-46.amzn2.0.7 running 'modules:final' at Thu, 25 Dec 2025 05:22:20 +0000. Up 14.35 seconds.
Loaded plugins: extras_suggestions, langpacks, priorities, update-motd
Existing lock /var/run/yum.pid: another copy is running as pid 2332.
Another app is currently holding the yum lock; waiting for it to exit...
  The other application is: yum
    Memory :  58 M RSS (285 MB VSZ)
    Started: Thu Dec 25 05:22:13 2025 - 00:07 ago
    State  : Running, pid: 2332
Another app is currently holding the yum lock; waiting for it to exit...
  The other application is: yum
    Memory : 219 M RSS (446 MB VSZ)
    Started: Thu Dec 25 05:22:13 2025 - 00:09 ago
    State  : Running, pid: 2332
Another app is currently holding the yum lock; waiting for it to exit...
  The other application is: yum
    Memory : 232 M RSS (459 MB VSZ)
    Started: Thu Dec 25 05:22:13 2025 - 00:11 ago
    State  : Running, pid: 2332
No packages marked for update
Topic lamp-mariadb10.2-php7.2 has end-of-support date of 2020-11-30
Topic php7.2 has end-of-support date of 2020-11-30
Loaded plugins: extras_suggestions, langpacks, priorities, update-motd
Cleaning repos: amzn2-core amzn2extra-docker amzn2extra-lamp-mariadb10.2-php7.2
              : amzn2extra-php7.2
12 metadata files removed
4 sqlite files removed
0 metadata files removed
Loaded plugins: extras_suggestions, langpacks, priorities, update-motd
Resolving Dependencies
--> Running transaction check
---> Package mariadb.x86_64 3:10.2.38-1.amzn2.0.1 will be installed
--> Processing Dependency: mariadb-libs(x86-64) = 3:10.2.38-1.amzn2.0.1 for package: 3:mariadb-10.2.38-1.amzn2.0.1.x86_64
--> Processing Dependency: mariadb-common(x86-64) = 3:10.2.38-1.amzn2.0.1 for package: 3:mariadb-10.2.38-1.amzn2.0.1.x86_64
---> Package php-cli.x86_64 0:7.2.34-1.amzn2 will be installed
--> Processing Dependency: php-common(x86-64) = 7.2.34-1.amzn2 for package: php-cli-7.2.34-1.amzn2.x86_64
---> Package php-fpm.x86_64 0:7.2.34-1.amzn2 will be installed
---> Package php-json.x86_64 0:7.2.34-1.amzn2 will be installed
---> Package php-mysqlnd.x86_64 0:7.2.34-1.amzn2 will be installed
---> Package php-pdo.x86_64 0:7.2.34-1.amzn2 will be installed
--> Running transaction check
---> Package mariadb-common.x86_64 3:10.2.38-1.amzn2.0.1 will be installed
--> Processing Dependency: /etc/my.cnf for package: 3:mariadb-common-10.2.38-1.amzn2.0.1.x86_64
---> Package mariadb-libs.x86_64 1:5.5.68-1.amzn2.0.1 will be updated
---> Package mariadb-libs.x86_64 3:10.2.38-1.amzn2.0.1 will be an update
---> Package php-common.x86_64 0:7.2.34-1.amzn2 will be installed
--> Processing Dependency: libzip.so.5()(64bit) for package: php-common-7.2.34-1.amzn2.x86_64
--> Running transaction check
---> Package libzip.x86_64 0:1.3.2-1.amzn2.0.1 will be installed
---> Package mariadb-config.x86_64 3:10.2.38-1.amzn2.0.1 will be installed
---> Package mariadb-libs.x86_64 1:5.5.68-1.amzn2.0.1 will be updated
--> Finished Dependency Resolution

Dependencies Resolved

================================================================================
 Package      Arch   Version           Repository                          Size
================================================================================
Installing:
 mariadb      x86_64 3:10.2.38-1.amzn2.0.1
                                       amzn2extra-lamp-mariadb10.2-php7.2 6.1 M
 php-cli      x86_64 7.2.34-1.amzn2    amzn2extra-php7.2                  4.4 M
 php-fpm      x86_64 7.2.34-1.amzn2    amzn2extra-php7.2                  1.5 M
 php-json     x86_64 7.2.34-1.amzn2    amzn2extra-php7.2                   71 k
 php-mysqlnd  x86_64 7.2.34-1.amzn2    amzn2extra-php7.2                  238 k
 php-pdo      x86_64 7.2.34-1.amzn2    amzn2extra-php7.2                  132 k
Installing for dependencies:
 libzip       x86_64 1.3.2-1.amzn2.0.1 amzn2-core                          62 k
 mariadb-common
              x86_64 3:10.2.38-1.amzn2.0.1
                                       amzn2extra-lamp-mariadb10.2-php7.2  58 k
 mariadb-config
              x86_64 3:10.2.38-1.amzn2.0.1
                                       amzn2extra-lamp-mariadb10.2-php7.2  34 k
 php-common   x86_64 7.2.34-1.amzn2    amzn2extra-php7.2                  1.1 M
Updating for dependencies:
 mariadb-libs x86_64 3:10.2.38-1.amzn2.0.1
                                       amzn2extra-lamp-mariadb10.2-php7.2 154 k

Transaction Summary
================================================================================
Install  6 Packages (+4 Dependent packages)
Upgrade             ( 1 Dependent package)

Total download size: 14 M
Downloading packages:
Delta RPMs disabled because /usr/bin/applydeltarpm not installed.
--------------------------------------------------------------------------------
Total                                               34 MB/s |  14 MB  00:00     
Running transaction check
Running transaction test
Transaction test succeeded
Running transaction
  Installing : 3:mariadb-config-10.2.38-1.amzn2.0.1.x86_64                 1/12 
  Installing : 3:mariadb-common-10.2.38-1.amzn2.0.1.x86_64                 2/12 
  Updating   : 3:mariadb-libs-10.2.38-1.amzn2.0.1.x86_64                   3/12 
  Installing : libzip-1.3.2-1.amzn2.0.1.x86_64                             4/12 
  Installing : php-common-7.2.34-1.amzn2.x86_64                            5/12 
  Installing : php-json-7.2.34-1.amzn2.x86_64                              6/12 
  Installing : php-pdo-7.2.34-1.amzn2.x86_64                               7/12 
  Installing : php-mysqlnd-7.2.34-1.amzn2.x86_64                           8/12 
  Installing : php-fpm-7.2.34-1.amzn2.x86_64                               9/12 
  Installing : php-cli-7.2.34-1.amzn2.x86_64                              10/12 
  Installing : 3:mariadb-10.2.38-1.amzn2.0.1.x86_64                       11/12 
  Cleanup    : 1:mariadb-libs-5.5.68-1.amzn2.0.1.x86_64                   12/12 
  Verifying  : php-fpm-7.2.34-1.amzn2.x86_64                               1/12 
  Verifying  : php-cli-7.2.34-1.amzn2.x86_64                               2/12 
  Verifying  : 3:mariadb-common-10.2.38-1.amzn2.0.1.x86_64                 3/12 
  Verifying  : 3:mariadb-libs-10.2.38-1.amzn2.0.1.x86_64                   4/12 
  Verifying  : php-json-7.2.34-1.amzn2.x86_64                              5/12 
  Verifying  : php-common-7.2.34-1.amzn2.x86_64                            6/12 
  Verifying  : libzip-1.3.2-1.amzn2.0.1.x86_64                             7/12 
  Verifying  : 3:mariadb-config-10.2.38-1.amzn2.0.1.x86_64                 8/12 
  Verifying  : php-mysqlnd-7.2.34-1.amzn2.x86_64                           9/12 
  Verifying  : php-pdo-7.2.34-1.amzn2.x86_64                              10/12 
  Verifying  : 3:mariadb-10.2.38-1.amzn2.0.1.x86_64                       11/12 
  Verifying  : 1:mariadb-libs-5.5.68-1.amzn2.0.1.x86_64                   12/12 

Installed:
  mariadb.x86_64 3:10.2.38-1.amzn2.0.1     php-cli.x86_64 0:7.2.34-1.amzn2     
  php-fpm.x86_64 0:7.2.34-1.amzn2          php-json.x86_64 0:7.2.34-1.amzn2    
  php-mysqlnd.x86_64 0:7.2.34-1.amzn2      php-pdo.x86_64 0:7.2.34-1.amzn2     

Dependency Installed:
  libzip.x86_64 0:1.3.2-1.amzn2.0.1                                             
  mariadb-common.x86_64 3:10.2.38-1.amzn2.0.1                                   
  mariadb-config.x86_64 3:10.2.38-1.amzn2.0.1                                   
  php-common.x86_64 0:7.2.34-1.amzn2                                            

Dependency Updated:
  mariadb-libs.x86_64 3:10.2.38-1.amzn2.0.1                                     

Complete!
Installing php-pdo, php-mysqlnd, php-fpm, php-cli, php-json, mariadb
  2  httpd_modules                   available    [ =1.0  =stable ]
  3  memcached1.5                    available    \
        [ =1.5.1  =1.5.16  =1.5.17 ]
  9  R3.4                            available    [ =3.4.3  =stable ]
 15 *php7.2=latest                   enabled      \
        [ =7.2.0  =7.2.4  =7.2.5  =7.2.8  =7.2.11  =7.2.13  =7.2.14
          =7.2.16  =7.2.17  =7.2.19  =7.2.21  =7.2.22  =7.2.23
          =7.2.24  =7.2.26  =stable ]
 17 *lamp-mariadb10.2-php7.2=latest  enabled      \
        [ =10.2.10_7.2.0  =10.2.10_7.2.4  =10.2.10_7.2.5
          =10.2.10_7.2.8  =10.2.10_7.2.11  =10.2.10_7.2.13
          =10.2.10_7.2.14  =10.2.10_7.2.16  =10.2.10_7.2.17
          =10.2.10_7.2.19  =10.2.10_7.2.22  =10.2.10_7.2.23
          =10.2.10_7.2.24  =stable ]
 18  libreoffice                     available    \
        [ =5.0.6.2_15  =5.3.6.1  =stable ]
 19  gimp                            available    [ =2.8.22 ]
 20  docker=latest                   enabled      \
        [ =17.12.1  =18.03.1  =18.06.1  =18.09.9  =stable ]
 21  mate-desktop1.x                 available    \
        [ =1.19.0  =1.20.0  =stable ]
 22  GraphicsMagick1.3               available    \
        [ =1.3.29  =1.3.32  =1.3.34  =stable ]
 25  testing                         available    [ =1.0  =stable ]
 26  ecs                             available    [ =stable ]
 27  corretto8                       available    \
        [ =1.8.0_192  =1.8.0_202  =1.8.0_212  =1.8.0_222  =1.8.0_232
          =1.8.0_242  =stable ]
 32  lustre2.10                      available    \
        [ =2.10.5  =2.10.8  =stable ]
 34  lynis                           available    [ =stable ]
 36  BCC                             available    [ =0.x  =stable ]
 37  mono                            available    [ =5.x  =stable ]
 38  nginx1                          available    [ =stable ]
 40  mock                            available    [ =stable ]
 43  livepatch                       available    [ =stable ]
 45  haproxy2                        available    [ =stable ]
 46  collectd                        available    [ =stable ]
 47  aws-nitro-enclaves-cli          available    [ =stable ]
 48  R4                              available    [ =stable ]
 49  kernel-5.4                      available    [ =stable ]
 50  selinux-ng                      available    [ =stable ]
 52  tomcat9                         available    [ =stable ]
 55  kernel-5.10                     available    [ =stable ]
 56  redis6                          available    [ =stable ]
 60  mock2                           available    [ =stable ]
 62  kernel-5.15                     available    [ =stable ]
 63  postgresql14                    available    [ =stable ]
 64  firefox                         available    [ =stable ]
 65  lustre                          available    [ =stable ]
  _ †php8.1                          available    [ =stable ]
 67  awscli1                         available    [ =stable ]
  _  php8.2                          available    [ =stable ]
 69  dnsmasq                         available    [ =stable ]
 70  unbound1.17                     available    [ =stable ]
 72  collectd-python3                available    [ =stable ]
* Extra topic has reached end of support.
† Note on end-of-support. Use 'info' subcommand.
Loaded plugins: extras_suggestions, langpacks, priorities, update-motd
Existing lock /var/run/yum.pid: another copy is running as pid 2485.
Another app is currently holding the yum lock; waiting for it to exit...
  The other application is: yum
    Memory : 146 M RSS (372 MB VSZ)
    Started: Thu Dec 25 05:22:39 2025 - 00:03 ago
    State  : Running, pid: 2485
Another app is currently holding the yum lock; waiting for it to exit...
  The other application is: yum
    Memory : 234 M RSS (461 MB VSZ)
    Started: Thu Dec 25 05:22:39 2025 - 00:05 ago
    State  : Running, pid: 2485
Another app is currently holding the yum lock; waiting for it to exit...
  The other application is: yum
    Memory : 237 M RSS (464 MB VSZ)
    Started: Thu Dec 25 05:22:39 2025 - 00:07 ago
    State  : Running, pid: 2485
Resolving Dependencies
--> Running transaction check
---> Package httpd.x86_64 0:2.4.65-1.amzn2.0.2 will be installed
--> Processing Dependency: httpd-filesystem = 2.4.65-1.amzn2.0.2 for package: httpd-2.4.65-1.amzn2.0.2.x86_64
--> Processing Dependency: httpd-tools = 2.4.65-1.amzn2.0.2 for package: httpd-2.4.65-1.amzn2.0.2.x86_64
--> Processing Dependency: /etc/mime.types for package: httpd-2.4.65-1.amzn2.0.2.x86_64
--> Processing Dependency: httpd-filesystem for package: httpd-2.4.65-1.amzn2.0.2.x86_64
--> Processing Dependency: mod_http2 for package: httpd-2.4.65-1.amzn2.0.2.x86_64
--> Processing Dependency: system-logos-httpd for package: httpd-2.4.65-1.amzn2.0.2.x86_64
--> Processing Dependency: libapr-1.so.0()(64bit) for package: httpd-2.4.65-1.amzn2.0.2.x86_64
--> Processing Dependency: libaprutil-1.so.0()(64bit) for package: httpd-2.4.65-1.amzn2.0.2.x86_64
---> Package mariadb-server.x86_64 3:10.2.38-1.amzn2.0.1 will be installed
--> Processing Dependency: mariadb-tokudb-engine(x86-64) = 3:10.2.38-1.amzn2.0.1 for package: 3:mariadb-server-10.2.38-1.amzn2.0.1.x86_64
--> Processing Dependency: mariadb-server-utils(x86-64) = 3:10.2.38-1.amzn2.0.1 for package: 3:mariadb-server-10.2.38-1.amzn2.0.1.x86_64
--> Processing Dependency: mariadb-rocksdb-engine(x86-64) = 3:10.2.38-1.amzn2.0.1 for package: 3:mariadb-server-10.2.38-1.amzn2.0.1.x86_64
--> Processing Dependency: mariadb-gssapi-server(x86-64) = 3:10.2.38-1.amzn2.0.1 for package: 3:mariadb-server-10.2.38-1.amzn2.0.1.x86_64
--> Processing Dependency: mariadb-errmsg(x86-64) = 3:10.2.38-1.amzn2.0.1 for package: 3:mariadb-server-10.2.38-1.amzn2.0.1.x86_64
--> Processing Dependency: mariadb-cracklib-password-check(x86-64) = 3:10.2.38-1.amzn2.0.1 for package: 3:mariadb-server-10.2.38-1.amzn2.0.1.x86_64
--> Processing Dependency: mariadb-backup(x86-64) = 3:10.2.38-1.amzn2.0.1 for package: 3:mariadb-server-10.2.38-1.amzn2.0.1.x86_64
--> Processing Dependency: bison for package: 3:mariadb-server-10.2.38-1.amzn2.0.1.x86_64
--> Running transaction check
---> Package apr.x86_64 0:1.7.2-1.amzn2.0.1 will be installed
---> Package apr-util.x86_64 0:1.6.3-1.amzn2.0.1 will be installed
--> Processing Dependency: apr-util-bdb(x86-64) = 1.6.3-1.amzn2.0.1 for package: apr-util-1.6.3-1.amzn2.0.1.x86_64
---> Package bison.x86_64 0:3.0.4-6.amzn2.0.2 will be installed
--> Processing Dependency: m4 >= 1.4 for package: bison-3.0.4-6.amzn2.0.2.x86_64
---> Package generic-logos-httpd.noarch 0:18.0.0-4.amzn2 will be installed
---> Package httpd-filesystem.noarch 0:2.4.65-1.amzn2.0.2 will be installed
---> Package httpd-tools.x86_64 0:2.4.65-1.amzn2.0.2 will be installed
---> Package mailcap.noarch 0:2.1.41-2.amzn2 will be installed
---> Package mariadb-backup.x86_64 3:10.2.38-1.amzn2.0.1 will be installed
---> Package mariadb-cracklib-password-check.x86_64 3:10.2.38-1.amzn2.0.1 will be installed
---> Package mariadb-errmsg.x86_64 3:10.2.38-1.amzn2.0.1 will be installed
---> Package mariadb-gssapi-server.x86_64 3:10.2.38-1.amzn2.0.1 will be installed
---> Package mariadb-rocksdb-engine.x86_64 3:10.2.38-1.amzn2.0.1 will be installed
---> Package mariadb-server-utils.x86_64 3:10.2.38-1.amzn2.0.1 will be installed
--> Processing Dependency: perl(Data::Dumper) for package: 3:mariadb-server-utils-10.2.38-1.amzn2.0.1.x86_64
--> Processing Dependency: perl(DBI) for package: 3:mariadb-server-utils-10.2.38-1.amzn2.0.1.x86_64
--> Processing Dependency: perl(DBI) for package: 3:mariadb-server-utils-10.2.38-1.amzn2.0.1.x86_64
--> Processing Dependency: perl(DBD::mysql) for package: 3:mariadb-server-utils-10.2.38-1.amzn2.0.1.x86_64
---> Package mariadb-tokudb-engine.x86_64 3:10.2.38-1.amzn2.0.1 will be installed
---> Package mod_http2.x86_64 0:1.15.19-1.amzn2.0.2 will be installed
--> Running transaction check
---> Package apr-util-bdb.x86_64 0:1.6.3-1.amzn2.0.1 will be installed
---> Package m4.x86_64 0:1.4.16-10.amzn2.0.2 will be installed
---> Package perl-DBD-MySQL.x86_64 0:4.023-6.amzn2 will be installed
---> Package perl-DBI.x86_64 0:1.627-4.amzn2.0.2 will be installed
--> Processing Dependency: perl(RPC::PlClient) >= 0.2000 for package: perl-DBI-1.627-4.amzn2.0.2.x86_64
--> Processing Dependency: perl(RPC::PlServer) >= 0.2001 for package: perl-DBI-1.627-4.amzn2.0.2.x86_64
---> Package perl-Data-Dumper.x86_64 0:2.145-3.amzn2.0.2 will be installed
--> Running transaction check
---> Package perl-PlRPC.noarch 0:0.2020-14.amzn2 will be installed
--> Processing Dependency: perl(Net::Daemon) >= 0.13 for package: perl-PlRPC-0.2020-14.amzn2.noarch
--> Processing Dependency: perl(Compress::Zlib) for package: perl-PlRPC-0.2020-14.amzn2.noarch
--> Processing Dependency: perl(Net::Daemon::Log) for package: perl-PlRPC-0.2020-14.amzn2.noarch
--> Processing Dependency: perl(Net::Daemon::Test) for package: perl-PlRPC-0.2020-14.amzn2.noarch
--> Running transaction check
---> Package perl-IO-Compress.noarch 0:2.061-2.amzn2 will be installed
--> Processing Dependency: perl(Compress::Raw::Bzip2) >= 2.061 for package: perl-IO-Compress-2.061-2.amzn2.noarch
--> Processing Dependency: perl(Compress::Raw::Zlib) >= 2.061 for package: perl-IO-Compress-2.061-2.amzn2.noarch
---> Package perl-Net-Daemon.noarch 0:0.48-5.amzn2 will be installed
--> Running transaction check
---> Package perl-Compress-Raw-Bzip2.x86_64 0:2.061-3.amzn2.0.2 will be installed
---> Package perl-Compress-Raw-Zlib.x86_64 1:2.061-4.amzn2.0.2 will be installed
--> Finished Dependency Resolution

Dependencies Resolved

================================================================================
 Package                         Arch   Version               Repository   Size
================================================================================
Installing:
 httpd                           x86_64 2.4.65-1.amzn2.0.2    amzn2-core  1.4 M
 mariadb-server                  x86_64 3:10.2.38-1.amzn2.0.1 amzn2extra-lamp-mariadb10.2-php7.2
                                                                           17 M
Installing for dependencies:
 apr                             x86_64 1.7.2-1.amzn2.0.1     amzn2-core  130 k
 apr-util                        x86_64 1.6.3-1.amzn2.0.1     amzn2-core  101 k
 apr-util-bdb                    x86_64 1.6.3-1.amzn2.0.1     amzn2-core   22 k
 bison                           x86_64 3.0.4-6.amzn2.0.2     amzn2-core  674 k
 generic-logos-httpd             noarch 18.0.0-4.amzn2        amzn2-core   19 k
 httpd-filesystem                noarch 2.4.65-1.amzn2.0.2    amzn2-core   25 k
 httpd-tools                     x86_64 2.4.65-1.amzn2.0.2    amzn2-core   90 k
 m4                              x86_64 1.4.16-10.amzn2.0.2   amzn2-core  256 k
 mailcap                         noarch 2.1.41-2.amzn2        amzn2-core   31 k
 mariadb-backup                  x86_64 3:10.2.38-1.amzn2.0.1 amzn2extra-lamp-mariadb10.2-php7.2
                                                                          5.9 M
 mariadb-cracklib-password-check x86_64 3:10.2.38-1.amzn2.0.1 amzn2extra-lamp-mariadb10.2-php7.2
                                                                           37 k
 mariadb-errmsg                  x86_64 3:10.2.38-1.amzn2.0.1 amzn2extra-lamp-mariadb10.2-php7.2
                                                                          222 k
 mariadb-gssapi-server           x86_64 3:10.2.38-1.amzn2.0.1 amzn2extra-lamp-mariadb10.2-php7.2
                                                                           39 k
 mariadb-rocksdb-engine          x86_64 3:10.2.38-1.amzn2.0.1 amzn2extra-lamp-mariadb10.2-php7.2
                                                                          5.5 M
 mariadb-server-utils            x86_64 3:10.2.38-1.amzn2.0.1 amzn2extra-lamp-mariadb10.2-php7.2
                                                                          1.6 M
 mariadb-tokudb-engine           x86_64 3:10.2.38-1.amzn2.0.1 amzn2extra-lamp-mariadb10.2-php7.2
                                                                          833 k
 mod_http2                       x86_64 1.15.19-1.amzn2.0.2   amzn2-core  149 k
 perl-Compress-Raw-Bzip2         x86_64 2.061-3.amzn2.0.2     amzn2-core   32 k
 perl-Compress-Raw-Zlib          x86_64 1:2.061-4.amzn2.0.2   amzn2-core   58 k
 perl-DBD-MySQL                  x86_64 4.023-6.amzn2         amzn2-core  141 k
 perl-DBI                        x86_64 1.627-4.amzn2.0.2     amzn2-core  804 k
 perl-Data-Dumper                x86_64 2.145-3.amzn2.0.2     amzn2-core   48 k
 perl-IO-Compress                noarch 2.061-2.amzn2         amzn2-core  260 k
 perl-Net-Daemon                 noarch 0.48-5.amzn2          amzn2-core   51 k
 perl-PlRPC                      noarch 0.2020-14.amzn2       amzn2-core   36 k

Transaction Summary
================================================================================
Install  2 Packages (+25 Dependent packages)

Total download size: 36 M
Installed size: 150 M
Downloading packages:
--------------------------------------------------------------------------------
Total                                               47 MB/s |  36 MB  00:00     
Running transaction check
Running transaction test
Transaction test succeeded
Running transaction
  Installing : apr-1.7.2-1.amzn2.0.1.x86_64                                1/27 
  Installing : apr-util-bdb-1.6.3-1.amzn2.0.1.x86_64                       2/27 
  Installing : apr-util-1.6.3-1.amzn2.0.1.x86_64                           3/27 
  Installing : perl-Data-Dumper-2.145-3.amzn2.0.2.x86_64                   4/27 
  Installing : httpd-tools-2.4.65-1.amzn2.0.2.x86_64                       5/27 
  Installing : perl-Net-Daemon-0.48-5.amzn2.noarch                         6/27 
  Installing : m4-1.4.16-10.amzn2.0.2.x86_64                               7/27 
  Installing : bison-3.0.4-6.amzn2.0.2.x86_64                              8/27 
  Installing : httpd-filesystem-2.4.65-1.amzn2.0.2.noarch                  9/27 
  Installing : perl-Compress-Raw-Bzip2-2.061-3.amzn2.0.2.x86_64           10/27 
  Installing : generic-logos-httpd-18.0.0-4.amzn2.noarch                  11/27 
  Installing : 3:mariadb-errmsg-10.2.38-1.amzn2.0.1.x86_64                12/27 
  Installing : mailcap-2.1.41-2.amzn2.noarch                              13/27 
  Installing : mod_http2-1.15.19-1.amzn2.0.2.x86_64                       14/27 
  Installing : httpd-2.4.65-1.amzn2.0.2.x86_64                            15/27 
  Installing : 1:perl-Compress-Raw-Zlib-2.061-4.amzn2.0.2.x86_64          16/27 
  Installing : perl-IO-Compress-2.061-2.amzn2.noarch                      17/27 
  Installing : perl-PlRPC-0.2020-14.amzn2.noarch                          18/27 
  Installing : perl-DBI-1.627-4.amzn2.0.2.x86_64                          19/27 
  Installing : perl-DBD-MySQL-4.023-6.amzn2.x86_64                        20/27 
  Installing : 3:mariadb-cracklib-password-check-10.2.38-1.amzn2.0.1.x8   21/27 
  Installing : 3:mariadb-gssapi-server-10.2.38-1.amzn2.0.1.x86_64         22/27 
  Installing : 3:mariadb-tokudb-engine-10.2.38-1.amzn2.0.1.x86_64         23/27 
  Installing : 3:mariadb-rocksdb-engine-10.2.38-1.amzn2.0.1.x86_64        24/27 
  Installing : 3:mariadb-backup-10.2.38-1.amzn2.0.1.x86_64                25/27 
  Installing : 3:mariadb-server-10.2.38-1.amzn2.0.1.x86_64                26/27 
  Installing : 3:mariadb-server-utils-10.2.38-1.amzn2.0.1.x86_64          27/27 
  Verifying  : apr-1.7.2-1.amzn2.0.1.x86_64                                1/27 
  Verifying  : 1:perl-Compress-Raw-Zlib-2.061-4.amzn2.0.2.x86_64           2/27 
  Verifying  : mailcap-2.1.41-2.amzn2.noarch                               3/27 
  Verifying  : 3:mariadb-errmsg-10.2.38-1.amzn2.0.1.x86_64                 4/27 
  Verifying  : 3:mariadb-cracklib-password-check-10.2.38-1.amzn2.0.1.x8    5/27 
  Verifying  : generic-logos-httpd-18.0.0-4.amzn2.noarch                   6/27 
  Verifying  : perl-Compress-Raw-Bzip2-2.061-3.amzn2.0.2.x86_64            7/27 
  Verifying  : perl-DBI-1.627-4.amzn2.0.2.x86_64                           8/27 
  Verifying  : perl-PlRPC-0.2020-14.amzn2.noarch                           9/27 
  Verifying  : 3:mariadb-gssapi-server-10.2.38-1.amzn2.0.1.x86_64         10/27 
  Verifying  : 3:mariadb-tokudb-engine-10.2.38-1.amzn2.0.1.x86_64         11/27 
  Verifying  : httpd-filesystem-2.4.65-1.amzn2.0.2.noarch                 12/27 
  Verifying  : perl-DBD-MySQL-4.023-6.amzn2.x86_64                        13/27 
  Verifying  : apr-util-1.6.3-1.amzn2.0.1.x86_64                          14/27 
  Verifying  : perl-Data-Dumper-2.145-3.amzn2.0.2.x86_64                  15/27 
  Verifying  : 3:mariadb-rocksdb-engine-10.2.38-1.amzn2.0.1.x86_64        16/27 
  Verifying  : 3:mariadb-server-10.2.38-1.amzn2.0.1.x86_64                17/27 
  Verifying  : httpd-tools-2.4.65-1.amzn2.0.2.x86_64                      18/27 
  Verifying  : bison-3.0.4-6.amzn2.0.2.x86_64                             19/27 
  Verifying  : m4-1.4.16-10.amzn2.0.2.x86_64                              20/27 
  Verifying  : mod_http2-1.15.19-1.amzn2.0.2.x86_64                       21/27 
  Verifying  : httpd-2.4.65-1.amzn2.0.2.x86_64                            22/27 
  Verifying  : 3:mariadb-server-utils-10.2.38-1.amzn2.0.1.x86_64          23/27 
  Verifying  : perl-IO-Compress-2.061-2.amzn2.noarch                      24/27 
  Verifying  : perl-Net-Daemon-0.48-5.amzn2.noarch                        25/27 
  Verifying  : apr-util-bdb-1.6.3-1.amzn2.0.1.x86_64                      26/27 
  Verifying  : 3:mariadb-backup-10.2.38-1.amzn2.0.1.x86_64                27/27 

Installed:
  httpd.x86_64 0:2.4.65-1.amzn2.0.2 mariadb-server.x86_64 3:10.2.38-1.amzn2.0.1

Dependency Installed:
  apr.x86_64 0:1.7.2-1.amzn2.0.1                                                
  apr-util.x86_64 0:1.6.3-1.amzn2.0.1                                           
  apr-util-bdb.x86_64 0:1.6.3-1.amzn2.0.1                                       
  bison.x86_64 0:3.0.4-6.amzn2.0.2                                              
  generic-logos-httpd.noarch 0:18.0.0-4.amzn2                                   
  httpd-filesystem.noarch 0:2.4.65-1.amzn2.0.2                                  
  httpd-tools.x86_64 0:2.4.65-1.amzn2.0.2                                       
  m4.x86_64 0:1.4.16-10.amzn2.0.2                                               
  mailcap.noarch 0:2.1.41-2.amzn2                                               
  mariadb-backup.x86_64 3:10.2.38-1.amzn2.0.1                                   
  mariadb-cracklib-password-check.x86_64 3:10.2.38-1.amzn2.0.1                  
  mariadb-errmsg.x86_64 3:10.2.38-1.amzn2.0.1                                   
  mariadb-gssapi-server.x86_64 3:10.2.38-1.amzn2.0.1                            
  mariadb-rocksdb-engine.x86_64 3:10.2.38-1.amzn2.0.1                           
  mariadb-server-utils.x86_64 3:10.2.38-1.amzn2.0.1                             
  mariadb-tokudb-engine.x86_64 3:10.2.38-1.amzn2.0.1                            
  mod_http2.x86_64 0:1.15.19-1.amzn2.0.2                                        
  perl-Compress-Raw-Bzip2.x86_64 0:2.061-3.amzn2.0.2                            
  perl-Compress-Raw-Zlib.x86_64 1:2.061-4.amzn2.0.2                             
  perl-DBD-MySQL.x86_64 0:4.023-6.amzn2                                         
  perl-DBI.x86_64 0:1.627-4.amzn2.0.2                                           
  perl-Data-Dumper.x86_64 0:2.145-3.amzn2.0.2                                   
  perl-IO-Compress.noarch 0:2.061-2.amzn2                                       
  perl-Net-Daemon.noarch 0:0.48-5.amzn2                                         
  perl-PlRPC.noarch 0:0.2020-14.amzn2                                           

Complete!
Created symlink from /etc/systemd/system/multi-user.target.wants/httpd.service to /usr/lib/systemd/system/httpd.service.
Created symlink from /etc/systemd/system/multi-user.target.wants/mariadb.service to /usr/lib/systemd/system/mariadb.service.
--2025-12-25 05:23:00--  https://aws-tc-largeobjects.s3.amazonaws.com/CUR-TF-100-RESTRT-1/173-activity-JAWS-troubleshoot-instance/db-v2.tar.gz
Resolving aws-tc-largeobjects.s3.amazonaws.com (aws-tc-largeobjects.s3.amazonaws.com)... 52.92.138.185, 52.92.243.89, 52.92.224.113, ...
Connecting to aws-tc-largeobjects.s3.amazonaws.com (aws-tc-largeobjects.s3.amazonaws.com)|52.92.138.185|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 1725 (1.7K) [application/x-gzip]
Saving to: 'db-v2.tar.gz'

     0K .                                                     100% 52.1M=0s

2025-12-25 05:23:00 (52.1 MB/s) - 'db-v2.tar.gz' saved [1725/1725]

db/
db/create-db.sh
db/set-root-password.log
db/set-root-password.sh
db/sql/
db/sql/create-db.sql
db/sql/set-root-password.sql
--2025-12-25 05:23:00--  https://aws-tc-largeobjects.s3.amazonaws.com/CUR-TF-100-RESTRT-1/173-activity-JAWS-troubleshoot-instance/cafe-v2.tar.gz
Resolving aws-tc-largeobjects.s3.amazonaws.com (aws-tc-largeobjects.s3.amazonaws.com)... 3.5.76.99, 52.218.179.57, 52.92.250.89, ...
Connecting to aws-tc-largeobjects.s3.amazonaws.com (aws-tc-largeobjects.s3.amazonaws.com)|3.5.76.99|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 6955791 (6.6M) [application/x-gzip]
Saving to: 'cafe-v2.tar.gz'

     0K .......... .......... .......... .......... ..........  0% 25.3M 0s
    50K .......... .......... .......... .......... ..........  1% 90.9M 0s
   100K .......... .......... .......... .......... ..........  2% 71.9M 0s
   150K .......... .......... .......... .......... ..........  2% 88.0M 0s
   200K .......... .......... .......... .......... ..........  3% 18.2M 0s
   250K .......... .......... .......... .......... ..........  4% 68.1M 0s
   300K .......... .......... .......... .......... ..........  5% 75.6M 0s
   350K .......... .......... .......... .......... ..........  5% 78.7M 0s
   400K .......... .......... .......... .......... ..........  6% 90.3M 0s
   450K .......... .......... .......... .......... ..........  7% 78.0M 0s
   500K .......... .......... .......... .......... ..........  8% 20.1M 0s
   550K .......... .......... .......... .......... ..........  8% 78.1M 0s
   600K .......... .......... .......... .......... ..........  9% 79.4M 0s
   650K .......... .......... .......... .......... .......... 10% 80.2M 0s
   700K .......... .......... .......... .......... .......... 11% 79.2M 0s
   750K .......... .......... .......... .......... .......... 11% 47.1M 0s
   800K .......... .......... .......... .......... .......... 12% 19.4M 0s
   850K .......... .......... .......... .......... .......... 13% 79.6M 0s
   900K .......... .......... .......... .......... .......... 13% 75.3M 0s
   950K .......... .......... .......... .......... .......... 14% 77.6M 0s
  1000K .......... .......... .......... .......... .......... 15% 80.8M 0s
  1050K .......... .......... .......... .......... .......... 16% 79.9M 0s
  1100K .......... .......... .......... .......... .......... 16% 18.4M 0s
  1150K .......... .......... .......... .......... .......... 17% 14.4M 0s
  1200K .......... .......... .......... .......... .......... 18% 76.9M 0s
  1250K .......... .......... .......... .......... .......... 19% 86.1M 0s
  1300K .......... .......... .......... .......... .......... 19% 77.9M 0s
  1350K .......... .......... .......... .......... .......... 20% 77.6M 0s
  1400K .......... .......... .......... .......... .......... 21% 77.9M 0s
  1450K .......... .......... .......... .......... .......... 22% 79.0M 0s
  1500K .......... .......... .......... .......... .......... 22% 75.2M 0s
  1550K .......... .......... .......... .......... .......... 23% 76.9M 0s
  1600K .......... .......... .......... .......... .......... 24% 19.0M 0s
  1650K .......... .......... .......... .......... .......... 25% 81.4M 0s
  1700K .......... .......... .......... .......... .......... 25% 76.7M 0s
  1750K .......... .......... .......... .......... .......... 26% 78.6M 0s
  1800K .......... .......... .......... .......... .......... 27% 79.3M 0s
  1850K .......... .......... .......... .......... .......... 27% 78.9M 0s
  1900K .......... .......... .......... .......... .......... 28% 18.5M 0s
  1950K .......... .......... .......... .......... .......... 29% 73.2M 0s
  2000K .......... .......... .......... .......... .......... 30% 78.2M 0s
  2050K .......... .......... .......... .......... .......... 30% 85.2M 0s
  2100K .......... .......... .......... .......... .......... 31% 90.8M 0s
  2150K .......... .......... .......... .......... .......... 32% 73.9M 0s
  2200K .......... .......... .......... .......... .......... 33% 18.5M 0s
  2250K .......... .......... .......... .......... .......... 33% 79.4M 0s
  2300K .......... .......... .......... .......... .......... 34% 73.7M 0s
  2350K .......... .......... .......... .......... .......... 35% 78.1M 0s
  2400K .......... .......... .......... .......... .......... 36% 79.4M 0s
  2450K .......... .......... .......... .......... .......... 36% 81.3M 0s
  2500K .......... .......... .......... .......... .......... 37% 15.0M 0s
  2550K .......... .......... .......... .......... .......... 38% 49.6M 0s
  2600K .......... .......... .......... .......... .......... 39% 80.6M 0s
  2650K .......... .......... .......... .......... .......... 39% 79.2M 0s
  2700K .......... .......... .......... .......... .......... 40% 75.5M 0s
  2750K .......... .......... .......... .......... .......... 41% 77.9M 0s
  2800K .......... .......... .......... .......... .......... 41% 18.8M 0s
  2850K .......... .......... .......... .......... .......... 42% 75.8M 0s
  2900K .......... .......... .......... .......... .......... 43% 81.7M 0s
  2950K .......... .......... .......... .......... .......... 44% 86.9M 0s
  3000K .......... .......... .......... .......... .......... 44% 79.7M 0s
  3050K .......... .......... .......... .......... .......... 45% 78.4M 0s
  3100K .......... .......... .......... .......... .......... 46% 18.6M 0s
  3150K .......... .......... .......... .......... .......... 47% 78.9M 0s
  3200K .......... .......... .......... .......... .......... 47% 80.3M 0s
  3250K .......... .......... .......... .......... .......... 48% 81.0M 0s
  3300K .......... .......... .......... .......... .......... 49% 79.4M 0s
  3350K .......... .......... .......... .......... .......... 50% 81.7M 0s
  3400K .......... .......... .......... .......... .......... 50% 18.8M 0s
  3450K .......... .......... .......... .......... .......... 51% 80.1M 0s
  3500K .......... .......... .......... .......... .......... 52% 76.3M 0s
  3550K .......... .......... .......... .......... .......... 52% 80.8M 0s
  3600K .......... .......... .......... .......... .......... 53% 74.8M 0s
  3650K .......... .......... .......... .......... .......... 54% 80.5M 0s
  3700K .......... .......... .......... .......... .......... 55% 18.6M 0s
  3750K .......... .......... .......... .......... .......... 55% 84.0M 0s
  3800K .......... .......... .......... .......... .......... 56% 87.8M 0s
  3850K .......... .......... .......... .......... .......... 57% 68.9M 0s
  3900K .......... .......... .......... .......... .......... 58% 78.8M 0s
  3950K .......... .......... .......... .......... .......... 58% 80.0M 0s
  4000K .......... .......... .......... .......... .......... 59% 18.4M 0s
  4050K .......... .......... .......... .......... .......... 60% 77.6M 0s
  4100K .......... .......... .......... .......... .......... 61% 71.7M 0s
  4150K .......... .......... .......... .......... .......... 61%  480K 0s
  4200K .......... .......... .......... .......... .......... 62%  208M 0s
  4250K .......... .......... .......... .......... .......... 63%  238M 0s
  4300K .......... .......... .......... .......... .......... 64%  238M 0s
  4350K .......... .......... .......... .......... .......... 64%  246M 0s
  4400K .......... .......... .......... .......... .......... 65%  214M 0s
  4450K .......... .......... .......... .......... .......... 66%  224M 0s
  4500K .......... .......... .......... .......... .......... 66%  214M 0s
  4550K .......... .......... .......... .......... .......... 67%  240M 0s
  4600K .......... .......... .......... .......... .......... 68%  243M 0s
  4650K .......... .......... .......... .......... .......... 69%  269M 0s
  4700K .......... .......... .......... .......... .......... 69%  231M 0s
  4750K .......... .......... .......... .......... .......... 70%  224M 0s
  4800K .......... .......... .......... .......... .......... 71%  236M 0s
  4850K .......... .......... .......... .......... .......... 72%  227M 0s
  4900K .......... .......... .......... .......... .......... 72%  231M 0s
  4950K .......... .......... .......... .......... .......... 73%  231M 0s
  5000K .......... .......... .......... .......... .......... 74%  227M 0s
  5050K .......... .......... .......... .......... .......... 75%  262M 0s
  5100K .......... .......... .......... .......... .......... 75%  231M 0s
  5150K .......... .......... .......... .......... .......... 76%  206M 0s
  5200K .......... .......... .......... .......... .......... 77%  241M 0s
  5250K .......... .......... .......... .......... .......... 78%  229M 0s
  5300K .......... .......... .......... .......... .......... 78%  236M 0s
  5350K .......... .......... .......... .......... .......... 79%  219M 0s
  5400K .......... .......... .......... .......... .......... 80%  228M 0s
  5450K .......... .......... .......... .......... .......... 80%  272M 0s
  5500K .......... .......... .......... .......... .......... 81%  266M 0s
  5550K .......... .......... .......... .......... .......... 82%  222M 0s
  5600K .......... .......... .......... .......... .......... 83%  237M 0s
  5650K .......... .......... .......... .......... .......... 83%  237M 0s
  5700K .......... .......... .......... .......... .......... 84%  232M 0s
  5750K .......... .......... .......... .......... .......... 85%  226M 0s
  5800K .......... .......... .......... .......... .......... 86%  239M 0s
  5850K .......... .......... .......... .......... .......... 86%  237M 0s
  5900K .......... .......... .......... .......... .......... 87%  271M 0s
  5950K .......... .......... .......... .......... .......... 88%  237M 0s
  6000K .......... .......... .......... .......... .......... 89%  236M 0s
  6050K .......... .......... .......... .......... .......... 89%  231M 0s
  6100K .......... .......... .......... .......... .......... 90%  211M 0s
  6150K .......... .......... .......... .......... .......... 91%  256M 0s
  6200K .......... .......... .......... .......... .......... 92%  300M 0s
  6250K .......... .......... .......... .......... .......... 92%  260M 0s
  6300K .......... .......... .......... .......... .......... 93%  304M 0s
  6350K .......... .......... .......... .......... .......... 94%  258M 0s
  6400K .......... .......... .......... .......... .......... 94%  304M 0s
  6450K .......... .......... .......... .......... .......... 95%  247M 0s
  6500K .......... .......... .......... .......... .......... 96%  288M 0s
  6550K .......... .......... .......... .......... .......... 97%  306M 0s
  6600K .......... .......... .......... .......... .......... 97%  294M 0s
  6650K .......... .......... .......... .......... .......... 98%  247M 0s
  6700K .......... .......... .......... .......... .......... 99%  307M 0s
  6750K .......... .......... .......... .......... ..        100%  293M=0.2s

2025-12-25 05:23:01 (33.6 MB/s) - 'cafe-v2.tar.gz' saved [6955791/6955791]

cafe/
cafe/AWSSDK/
cafe/AWSSDK/aws.phar
cafe/css/
cafe/css/menu.css
cafe/css/styles.css
cafe/getAppParameters.php
cafe/images/
cafe/images/Cake-Vitrine.jpg
cafe/images/Chocolate-Chip-Cookies.jpg
cafe/images/Coffee-and-Pastries.jpg
cafe/images/Coffee-Shop.png
cafe/images/Coffee.jpg
cafe/images/Cookies.jpg
cafe/images/Croissants.jpg
cafe/images/Cup-of-Hot-Chocolate.jpg
cafe/images/default-image.jpg
cafe/images/Donuts.jpg
cafe/images/Frank-Martha.jpg
cafe/images/Latte.jpg
cafe/images/Muffins.jpg
cafe/images/Strawberry-Blueberry-Tarts.jpg
cafe/images/Strawberry-Tarts.jpg
cafe/index.php
cafe/menu.php
cafe/orderHistory.php
cafe/processOrder.php
cafe/serverInfo.php

Set Root Password script completed.
Please check the set-root-password.log file to verify successful execution.


Create Database script completed.
Please check the create-db.log file to verify successful execution.

Cloud-init v. 19.3-46.amzn2.0.7 finished at Thu, 25 Dec 2025 05:23:01 +0000. Datasource DataSourceEc2.  Up 55.93 seconds
