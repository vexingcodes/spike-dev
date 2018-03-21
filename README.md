# spike-dev
A Vagrant/Ansible environment for testing and validating changes to
riscv-isa-sim in a repeatable environment.

# How to run the test.
Install vagrant and run `vagrant up`. Vagrant will boot a clean debian 9.3
virtual machine and run the Ansible script to perform the test.

# What's it do?
* Builds [riscv/riscv-fesvr][1].
* Builds [vexingcodes/riscv-isa-sim][2].
* Builds a RISC-V cross compiler with crosstools-ng.
* Builds [vexingcodes/spike-plugin][3].
* Runs the example spike MMIO plugin and prints its output.

[1]: https://github.com/riscv/riscv-fesvr
[2]: https://github.com/vexingcodes/riscv-isa-sim
[3]: https://github.com/vexingcodes/spike-plugin
