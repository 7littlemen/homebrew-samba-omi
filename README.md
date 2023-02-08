Build dynamic libsmbclient with homebrew

```
$ brew uninstall samba-omi
$ rm -rf /opt/homebrew/Library/Taps/7littlemen/homebrew-samba-omi
$ brew tap 7littlemen/samba-omi git@github.com:7littlemen/homebrew-samba-omi.git
$ brew install samba-omi
```

### change library dependencies
```console
$ other/change_lib_dependencies.rb "$(brew --prefix)" "$(brew --prefix samba-omi)/lib/libsmbclient.dylib"
```

### homebrew libraries path
/opt/homebrew/Cellar
or
/usr/local/Cellar/