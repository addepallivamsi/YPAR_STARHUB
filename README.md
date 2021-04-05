# YPAR_STARHUB
StarHub Repository

REPORT  z_vammise_test.
*
Tables tbtcjob.
data: gv_binc_jobname               like tbtcjob-jobname,
      w_jobname like tbtcjob-jobname.
data: gv_binc_jobcount              like tbtcjob-jobcount.
RANGES: lr_matnr FOR vbap-matnr.

  lr_matnr-sign   = 'I'.
  lr_matnr-option = 'EQ'.
  lr_matnr-low    = 'A0000700146'.
  APPEND lr_matnr.
