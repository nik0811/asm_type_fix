# asm_type_fix
Missing asm/types.h file in `Ubuntu` Version `VERSION="20.04.2 LTS (Focal Fossa)"`
```
cd  /usr/include/
sudo vi linux/bpf.h 
sudo vi netatalk/at.h 
sudo vi netatalk/at.h 
sudo vi iproute2//bpf_elf.h 
sudo vi net/ppp_defs.h 
sudo vi linux/types.h 
sudo vi asm-generic/int-ll64.h 
sudo vi linux/posix_types.h 
sudo vi asm-generic/posix_types.h 
sudo vi asm-generic/posix_types.h

Above in each file if you finding,

#include <asm/*>

replace it with

#include <asm-generic/*>
```

In `Ubuntu 20.04.2` `<asm/types.h>` exists in `<asm-generic/types.h>`
