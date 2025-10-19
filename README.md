# make.include-for-vasp-5.4.4-using-ifx
Updated VASP make.include for Intel oneAPI compilers (ifx/icx/icpx). Minimal changes applied to replace deprecated Intel compilers and flags while maintaining full MKL and MPI functionality.
Customized make.include for VASP, updated for compatibility with the Intel oneAPI compiler suite (ifx/icx/icpx).

Changes made:

mpiifort → mpiifx

-mkl=sequential → -qmkl=sequential

icc → icx

icpc → icpx -Wno-register

This update preserves the original structure of the VASP make.include file while ensuring full support for MKL and MPI using the new Intel compilers. It improves compatibility with modern oneAPI environments and removes deprecated flags.
