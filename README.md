# rails_pracrice

- environment 
  - rails 6.1.4.1
  - yarn 1.22.5
  - ruby 2.7.0p0 (2019-12-25 revision 647ee6f091) [x86_64-linux-gnu]
  - node v14.17.5
  - ubuntu 20.04
```bash
rails new app
```
- If you see below log 
```bash
rails aborted!
TypeError: superclass mismatch for class Command
/var/lib/gems/2.7.0/gems/thor-1.1.0/lib/thor/command.rb:2:in `<class:Thor>'
/var/lib/gems/2.7.0/gems/thor-1.1.0/lib/thor/command.rb:1:in `<main>'
/var/lib/gems/2.7.0/gems/bootsnap-1.7.7/lib/bootsnap/load_path_cache/core_ext/kernel_require.rb:23:in `require'
/var/lib/gems/2.7.0/gems/bootsnap-1.7.7/lib/bootsnap/load_path_cache/core_ext/kernel_require.rb:23:in `block in require_with_bootsnap_lfi'
/var/lib/gems/2.7.0/gems/bootsnap-1.7.7/lib/bootsnap/load_path_cache/loaded_features_index.rb:92:in `register'
/var/lib/gems/2.7.0/gems/bootsnap-1.7.7/lib/bootsnap/load_path_cache/core_ext/kernel_require.rb:22:in `require_with_bootsnap_lfi'
/var/lib/gems/2.7.0/gems/bootsnap-1.7.7/lib/bootsnap/load_path_cache/core_ext/kernel_require.rb:31:in `require'
....
```

- Solution 
``` bash
dpkg -r --force-depends  ruby-thor
gem install thor
```
