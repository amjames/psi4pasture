set(ccsort_sources local.cc local_polar.cc transpert.cc cc_memcheck.cc classify.cc f_spinad.cc cache.cc build_F_RHF.cc local_magnetic.cc sort_tei.cc cphf_F.cc fock.cc get_params.cc scf_check.cc f_sort.cc cphf_B.cc idx_permute_multipass.cc d_sort.cc b_sort.cc build_B_RHF.cc build_abcd_packed.cc c_sort.cc distribute.cc sort_oei.cc idx_permute.cc e_spinad.cc file_build_multipass.cc get_moinfo.cc file_build.cc ccsort.cc d_spinad.cc file_build_presort.cc e_sort.cc idx_error.cc denom.cc sort_pert.cc domain_print.cc idx_permute_presort.cc)

add_psi4_plugin(ccsort ${ccsort_sources})
#target_include_directories(ccsort SYSTEM PRIVATE ${psi4_INCLUDE_DIR})

install(TARGETS ccsort
        LIBRARY DESTINATION ${install_loc})
