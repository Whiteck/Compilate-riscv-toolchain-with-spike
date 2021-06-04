# Compilate-riscv-toolchain-with-spike

# Installation 

Download the tar file from GDrive : https://drive.google.com/file/d/1pcwRpcoK2rO6ALekvHwzZqUXNn4iO87S/view?usp=sharing
cp /home/user/Download/riscv_toolchain.tar.xf to /home/user/
tar -xf riscv_toolchain.tar.xf

# Export PATH 

export RISCV=/home/user/riscv_toolchain/
export PATH=$PATH:$RISCV/bin/
export PATH=$PATH:$RISCV/riscv32-unknown-elf/bin/

# Compilate

riscv32-unknown-elf-gcc -o nameofexecutable nameofsourcefiles.c

# Use spike 

spike $(which pk) nameofexecutable
