if ! in_depends $MODULE asciidoc || ! in_depends $MODULE xmlto; then
   OPTS+=" --disable-documentation"
fi

default_build &&

# remove the static lib
rm /usr/lib/libbtrfs.a &&

if module_installed bash-completion ; then
   # install bash completion
   install -Dm644 btrfs-completion /usr/share/bash-completion/completions/btrfs
fi
