ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~$ export GITHUB_USERNAME=<Lopatukhin>
bash: syntax error near unexpected token `newline'
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~$ export GITHUB_USERNAME=Lopatukhin
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~$ export GIST_TOKEN=https://gist.github.com/Lopatukhin/9c3ab2509df3fcbf6d7d1ec7a68f2412
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~$ mkdir -p $Lopatukhin/workspace
mkdir: cannot create directory ‘/workspace’: Permission denied
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~$ alias edit=<nano|vi|vim|subl>
bash: syntax error near unexpected token `newline'
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~$ mkdir -p ${GITHUB_USERNAME}/workspace
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~$ i
i: command not found
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~$ cd ${GITHUB_USERNAME}/workspace
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace$ pwd
/home/ilia_lopatukhin/Lopatukhin/workspace
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace$ cd ..
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin$ pwd
/home/ilia_lopatukhin/Lopatukhin
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin$ mkdir -p workspace/tasks/
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin$ mkdir -p workspace/projects/
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin$ mkdir -p workspace/reports/
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin$ cd workspace
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace$ wget https://nodejs.org/dist/v6.11.5/node-v6.11.5-linux-x64.tar.xz
--2025-06-14 19:56:03--  https://nodejs.org/dist/v6.11.5/node-v6.11.5-linux-x64.tar.xz
Resolving nodejs.org (nodejs.org)... 172.66.128.70, 104.20.1.252, 2606:4700:10::6814:1fc, ...
Connecting to nodejs.org (nodejs.org)|172.66.128.70|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 9356460 (8.9M) [application/x-xz]
Saving to: ‘node-v6.11.5-linux-x64.tar.xz’

node-v6.11.5-linux-x64.ta 100%[==================================>]   8.92M  2.69MB/s    in 3.4s    

2025-06-14 19:56:08 (2.62 MB/s) - ‘node-v6.11.5-linux-x64.tar.xz’ saved [9356460/9356460]

ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace$ tar -xf node-v6.11.5-linux-x64.tar.xz
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace$ rm -rf node-v6.11.5-linux-x64.tar.xz
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace$  mv node-v6.11.5-linux-x64 node
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace$ ls node/bin
node  npm
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace$ echo ${PATH}
/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/snap/bin:/snap/bin
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace$ export PATH=${PATH}:`pwd`/node/bin
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace$ echo ${PATH}
/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/snap/bin:/snap/bin:/home/ilia_lopatukhin/Lopatukhin/workspace/node/bin
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace$ mkdir scripts
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace$ cat > scripts/activate<<EOF
> export PATH=\${PATH}:`pwd`/node/bin
> EOF
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace$ source scripts/activate
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace$ gem install gist
Command 'gem' not found, but can be installed with:
sudo snap install ruby           # version 3.4.4, or
sudo apt  install ruby-rubygems  # version 3.4.20-1
See 'snap info ruby' for additional versions.
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace$ sudo snap install ruby 
[sudo] password for ilia_lopatukhin: 
error: This revision of snap "ruby" was published using classic confinement and thus may perform
       arbitrary system changes outside of the security sandbox that snaps are usually confined to,
       which may put your system at risk.

       If you understand and want to proceed repeat the command including --classic.
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace$ sudo apt  install ruby-rubygems
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
The following additional packages will be installed:
  fonts-lato javascript-common libjs-jquery libruby libruby3.2 rake ruby ruby-net-telnet ruby-sdbm
  ruby-webrick ruby-xmlrpc ruby3.2 rubygems-integration
Suggested packages:
  apache2 | lighttpd | httpd ri ruby-dev bundler
The following NEW packages will be installed:
  fonts-lato javascript-common libjs-jquery libruby libruby3.2 rake ruby ruby-net-telnet
  ruby-rubygems ruby-sdbm ruby-webrick ruby-xmlrpc ruby3.2 rubygems-integration
0 upgraded, 14 newly installed, 0 to remove and 61 not upgraded.
Need to get 8,926 kB of archives.
After this operation, 41.1 MB of additional disk space will be used.
Do you want to continue? [Y/n] y
Get:1 http://ru.archive.ubuntu.com/ubuntu noble/main amd64 fonts-lato all 2.015-1 [2,781 kB]
Get:2 http://ru.archive.ubuntu.com/ubuntu noble/main amd64 javascript-common all 11+nmu1 [5,936 B]
Get:3 http://ru.archive.ubuntu.com/ubuntu noble/main amd64 libjs-jquery all 3.6.1+dfsg+~3.5.14-1 [328 kB]
Get:4 http://ru.archive.ubuntu.com/ubuntu noble/main amd64 rubygems-integration all 1.18 [5,336 B]
Get:5 http://ru.archive.ubuntu.com/ubuntu noble-updates/main amd64 ruby3.2 amd64 3.2.3-1ubuntu0.24.04.5 [50.7 kB]
Get:6 http://ru.archive.ubuntu.com/ubuntu noble/main amd64 ruby-rubygems all 3.4.20-1 [238 kB]
Get:7 http://ru.archive.ubuntu.com/ubuntu noble/main amd64 ruby amd64 1:3.2~ubuntu1 [3,466 B]
Get:8 http://ru.archive.ubuntu.com/ubuntu noble/main amd64 rake all 13.0.6-3 [61.6 kB]
Get:9 http://ru.archive.ubuntu.com/ubuntu noble/main amd64 ruby-net-telnet all 0.2.0-1 [13.3 kB]
Get:10 http://ru.archive.ubuntu.com/ubuntu noble-updates/main amd64 ruby-webrick all 1.8.1-1ubuntu0.1 [52.6 kB]
Get:11 http://ru.archive.ubuntu.com/ubuntu noble/main amd64 ruby-xmlrpc all 0.3.2-2 [24.8 kB]
Get:12 http://ru.archive.ubuntu.com/ubuntu noble/main amd64 ruby-sdbm amd64 1.0.0-5build4 [16.2 kB]
Get:13 http://ru.archive.ubuntu.com/ubuntu noble-updates/main amd64 libruby3.2 amd64 3.2.3-1ubuntu0.24.04.5 [5,341 kB]
Get:14 http://ru.archive.ubuntu.com/ubuntu noble/main amd64 libruby amd64 1:3.2~ubuntu1 [4,694 B]   
Fetched 8,926 kB in 13s (663 kB/s)                                                                  
Selecting previously unselected package fonts-lato.
(Reading database ... 218651 files and directories currently installed.)
Preparing to unpack .../00-fonts-lato_2.015-1_all.deb ...
Unpacking fonts-lato (2.015-1) ...
Selecting previously unselected package javascript-common.
Preparing to unpack .../01-javascript-common_11+nmu1_all.deb ...
Unpacking javascript-common (11+nmu1) ...
Selecting previously unselected package libjs-jquery.
Preparing to unpack .../02-libjs-jquery_3.6.1+dfsg+~3.5.14-1_all.deb ...
Unpacking libjs-jquery (3.6.1+dfsg+~3.5.14-1) ...
Selecting previously unselected package rubygems-integration.
Preparing to unpack .../03-rubygems-integration_1.18_all.deb ...
Unpacking rubygems-integration (1.18) ...
Selecting previously unselected package ruby3.2.
Preparing to unpack .../04-ruby3.2_3.2.3-1ubuntu0.24.04.5_amd64.deb ...
Unpacking ruby3.2 (3.2.3-1ubuntu0.24.04.5) ...
Selecting previously unselected package ruby-rubygems.
Preparing to unpack .../05-ruby-rubygems_3.4.20-1_all.deb ...
Unpacking ruby-rubygems (3.4.20-1) ...
Selecting previously unselected package ruby.
Preparing to unpack .../06-ruby_1%3a3.2~ubuntu1_amd64.deb ...
Unpacking ruby (1:3.2~ubuntu1) ...
Selecting previously unselected package rake.
Preparing to unpack .../07-rake_13.0.6-3_all.deb ...
Unpacking rake (13.0.6-3) ...
Selecting previously unselected package ruby-net-telnet.
Preparing to unpack .../08-ruby-net-telnet_0.2.0-1_all.deb ...
Unpacking ruby-net-telnet (0.2.0-1) ...
Selecting previously unselected package ruby-webrick.
Preparing to unpack .../09-ruby-webrick_1.8.1-1ubuntu0.1_all.deb ...
Unpacking ruby-webrick (1.8.1-1ubuntu0.1) ...
Selecting previously unselected package ruby-xmlrpc.
Preparing to unpack .../10-ruby-xmlrpc_0.3.2-2_all.deb ...
Unpacking ruby-xmlrpc (0.3.2-2) ...
Selecting previously unselected package ruby-sdbm:amd64.
Preparing to unpack .../11-ruby-sdbm_1.0.0-5build4_amd64.deb ...
Unpacking ruby-sdbm:amd64 (1.0.0-5build4) ...
Selecting previously unselected package libruby3.2:amd64.
Preparing to unpack .../12-libruby3.2_3.2.3-1ubuntu0.24.04.5_amd64.deb ...
Unpacking libruby3.2:amd64 (3.2.3-1ubuntu0.24.04.5) ...
Selecting previously unselected package libruby:amd64.
Preparing to unpack .../13-libruby_1%3a3.2~ubuntu1_amd64.deb ...
Unpacking libruby:amd64 (1:3.2~ubuntu1) ...
Setting up javascript-common (11+nmu1) ...
Setting up fonts-lato (2.015-1) ...
Setting up rubygems-integration (1.18) ...
Setting up ruby-net-telnet (0.2.0-1) ...
Setting up ruby-webrick (1.8.1-1ubuntu0.1) ...
Setting up libjs-jquery (3.6.1+dfsg+~3.5.14-1) ...
Setting up ruby-xmlrpc (0.3.2-2) ...
Setting up ruby3.2 (3.2.3-1ubuntu0.24.04.5) ...
Setting up libruby:amd64 (1:3.2~ubuntu1) ...
Setting up ruby (1:3.2~ubuntu1) ...
Setting up rake (13.0.6-3) ...
Setting up libruby3.2:amd64 (3.2.3-1ubuntu0.24.04.5) ...
Setting up ruby-rubygems (3.4.20-1) ...
Setting up ruby-sdbm:amd64 (1.0.0-5build4) ...
Processing triggers for fontconfig (2.15.0-1.1ubuntu2) ...
Processing triggers for libc-bin (2.39-0ubuntu8.4) ...
Processing triggers for man-db (2.12.0-4build2) ...
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace$ gem install gist
Fetching gist-6.0.0.gem
ERROR:  While executing gem ... (Gem::FilePermissionError)
    You don't have write permissions for the /var/lib/gems/3.2.0 directory.
	/usr/lib/ruby/vendor_ruby/rubygems/installer.rb:713:in `verify_gem_home'
	/usr/lib/ruby/vendor_ruby/rubygems/installer.rb:903:in `pre_install_checks'
	/usr/lib/ruby/vendor_ruby/rubygems/installer.rb:303:in `install'
	/usr/lib/ruby/vendor_ruby/rubygems/resolver/specification.rb:105:in `install'
	/usr/lib/ruby/vendor_ruby/rubygems/request_set.rb:195:in `block in install'
	/usr/lib/ruby/vendor_ruby/rubygems/request_set.rb:183:in `each'
	/usr/lib/ruby/vendor_ruby/rubygems/request_set.rb:183:in `install'
	/usr/lib/ruby/vendor_ruby/rubygems/commands/install_command.rb:215:in `install_gem'
	/usr/lib/ruby/vendor_ruby/rubygems/commands/install_command.rb:231:in `block in install_gems'
	/usr/lib/ruby/vendor_ruby/rubygems/commands/install_command.rb:224:in `each'
	/usr/lib/ruby/vendor_ruby/rubygems/commands/install_command.rb:224:in `install_gems'
	/usr/lib/ruby/vendor_ruby/rubygems/commands/install_command.rb:170:in `execute'
	/usr/lib/ruby/vendor_ruby/rubygems/command.rb:328:in `invoke_with_build_args'
	/usr/lib/ruby/vendor_ruby/rubygems/command_manager.rb:253:in `invoke_command'
	/usr/lib/ruby/vendor_ruby/rubygems/command_manager.rb:193:in `process_args'
	/usr/lib/ruby/vendor_ruby/rubygems/command_manager.rb:151:in `run'
	/usr/lib/ruby/vendor_ruby/rubygems/gem_runner.rb:52:in `run'
	/usr/bin/gem:12:in `<main>'
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace$ (umask 0077 && echo ${GIST_TOKEN} > ~/.gist)
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace$ export LAB_NUMBER=01
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace$ git clone https://github.com/tp-labs/lab${LAB_NUMBER} tasks/lab${LAB_NUMBER}
Cloning into 'tasks/lab01'...
remote: Enumerating objects: 74, done.
remote: Counting objects: 100% (3/3), done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 74 (delta 0), reused 1 (delta 0), pack-reused 71 (from 1)
Receiving objects: 100% (74/74), 945.07 KiB | 1.49 MiB/s, done.
Resolving deltas: 100% (20/20), done.
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace$ mkdir reports/lab${LAB_NUMBER}
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace$ cp tasks/lab${LAB_NUMBER}/README.md reports/lab${LAB_NUMBER}/REPORT.md
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace$ cd reports/lab${LAB_NUMBER}
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/reports/lab01$ edit REPORT.md
Command 'edit' not found, but can be installed with:
sudo apt install mailcap
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/reports/lab01$ sudo apt install mailcap
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
The following NEW packages will be installed:
  mailcap
0 upgraded, 1 newly installed, 0 to remove and 61 not upgraded.
Need to get 23.8 kB of archives.
After this operation, 90.1 kB of additional disk space will be used.
Get:1 http://ru.archive.ubuntu.com/ubuntu noble/main amd64 mailcap all 3.70+nmu1ubuntu1 [23.8 kB]
Fetched 23.8 kB in 10s (2,361 B/s)      
Selecting previously unselected package mailcap.
(Reading database ... 221734 files and directories currently installed.)
Preparing to unpack .../mailcap_3.70+nmu1ubuntu1_all.deb ...
Unpacking mailcap (3.70+nmu1ubuntu1) ...
Setting up mailcap (3.70+nmu1ubuntu1) ...
Processing triggers for man-db (2.12.0-4build2) ...
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/reports/lab01$ edit REPORT.md
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/reports/lab01$ gist REPORT.md
Command 'gist' not found, but can be installed with:
sudo apt install yorick
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/reports/lab01$ sudo apt install yorick
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
The following additional packages will be installed:
  rlwrap yorick-data yorick-z
Suggested packages:
  yorick-full yorick-mpy-openmpi | yorick-mpy-mpich2 emacsen curl
The following NEW packages will be installed:
  rlwrap yorick yorick-data yorick-z
0 upgraded, 4 newly installed, 0 to remove and 61 not upgraded.
Need to get 1,443 kB of archives.
After this operation, 4,538 kB of additional disk space will be used.
Do you want to continue? [Y/n] y
Get:1 http://ru.archive.ubuntu.com/ubuntu noble/universe amd64 rlwrap amd64 0.46.1-1build2 [107 kB]
Get:2 http://ru.archive.ubuntu.com/ubuntu noble/universe amd64 yorick-data all 2.2.04+dfsg1-12build3 [505 kB]
Get:3 http://ru.archive.ubuntu.com/ubuntu noble/universe amd64 yorick amd64 2.2.04+dfsg1-12build3 [795 kB]
Get:4 http://ru.archive.ubuntu.com/ubuntu noble/universe amd64 yorick-z amd64 1.2.0+cvs20080115-5.1build2 [36.7 kB]
Fetched 1,443 kB in 11s (128 kB/s)  
Selecting previously unselected package rlwrap.
(Reading database ... 221756 files and directories currently installed.)
Preparing to unpack .../rlwrap_0.46.1-1build2_amd64.deb ...
Unpacking rlwrap (0.46.1-1build2) ...
Selecting previously unselected package yorick-data.
Preparing to unpack .../yorick-data_2.2.04+dfsg1-12build3_all.deb ...
Unpacking yorick-data (2.2.04+dfsg1-12build3) ...
Selecting previously unselected package yorick.
Preparing to unpack .../yorick_2.2.04+dfsg1-12build3_amd64.deb ...
Unpacking yorick (2.2.04+dfsg1-12build3) ...
Selecting previously unselected package yorick-z.
Preparing to unpack .../yorick-z_1.2.0+cvs20080115-5.1build2_amd64.deb ...
Unpacking yorick-z (1.2.0+cvs20080115-5.1build2) ...
Setting up yorick-data (2.2.04+dfsg1-12build3) ...
Setting up rlwrap (0.46.1-1build2) ...
update-alternatives: using /usr/bin/rlwrap to provide /usr/bin/readline-editor (readline-editor) in a
uto mode
/usr/share/rlwrap/filters/ftp_filter.py:57: SyntaxWarning: invalid escape sequence '\s'
  results = [re.split('\s+', l)[dir_filename_column[where]] for l in lines]
/usr/share/rlwrap/filters/ftp_filter.py:100: SyntaxWarning: invalid escape sequence '\s'
  nwords = len(re.split('\s+', line))
/usr/share/rlwrap/filters/ftp_filter.py:108: SyntaxWarning: invalid escape sequence '\s'
  command = re.search('\s*(\S+)', line).group(1)
/usr/share/rlwrap/filters/rlwrapfilter.py:4: SyntaxWarning: invalid escape sequence '\s'
  """
/usr/share/rlwrap/filters/rlwrapfilter.py:211: SyntaxWarning: invalid escape sequence '\S'
  m = re.match("(\S+) (.*?)\r?\n", sys.stdin.readline())
Setting up yorick (2.2.04+dfsg1-12build3) ...
Setting up yorick-z (1.2.0+cvs20080115-5.1build2) ...
Processing triggers for man-db (2.12.0-4build2) ...
Processing triggers for install-info (7.1-3build2) ...
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/reports/lab01$ gist REPORT.md
gist: (WARNING) fread failed (command) on CGM file REPORT.md
gist: (WARNING) BEGIN METAFILE element missing
gist: (WARNING) REPORT.md is not a binary CGM, cannot open
