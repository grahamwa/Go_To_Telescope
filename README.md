## GoTo Modifier for my Dobsaonian Telescope


The goal of this project is to make a GoTo system for my dobsonian telecope that I got back in the start of 2023. It should be computer controlled and be able to move to a selected target and also automatically track it. To make the GoTo I will primaraly be using an arduino fitted with a cnc shield that controls two NEMA 17 stepper motors witht the help of a rotary encoder. To aid my creation I will be using my schoools lazer vutter and 3d printers.




##
##



### Starting Point
##
The Telescope I bought was a f/5 130mm dobonsian by skywatcher. I bought a dobsonian over a equatorial mount for simplicty reasons as well as for the wooden base and easy to remove hardwear.

<img src="https://usa.all-startelescope.com/cdn/shop/products/S11710_Heritage150_LeftFront_1800x1800_3ac2cdd2-1c1b-43c0-9795-49c9df086e0c-sw_600x600.jpg?v=1645512990" width=50% height=50%>

The telescope moves on two differant mounts, the base (Azimuth); the vertival screw (Altidude). The first step I did was to figure out a way to connect the motor and the axis. The solution was to create two gears that would glue to the bases and allow for the motor to move the gears in any way possible. On the left is the altitude gear, the left- the stepper holder. For the diesing process I used OnShape: A free online softwear creation comapny.

<img src="https://github.com/grahamwa/Go_To_Telescope/assets/88165698/33e6c0f1-e2ff-4fec-838b-c6da134f178a" width="405" hieght =50%/> <img src="https://github.com/grahamwa/Go_To_Telescope/assets/88165698/e596ac78-e1e1-47d0-bab9-f39c3effd581" width="405"/> 
                                                                                                                            
##                                                                                                                          
##


### Arduinio Communication Unit


##


For housing I lazer cut I box from thin wood on the cutter, adding holes for cables and fans as well as an eccesable power supply. This box Icludes a pc fan for cooling and cut out for the USB 2.0 cable port. 

<img src="https://lh3.googleusercontent.com/fife/ALs6j_HqOE5FGkFGbRnOUDfGlTLLntItIJ_7zybg3MNzYXxc7JctSnVTlDL0K-8GUnEUQmipKoGeyesxK_50n3UiybfQEGghqzEk9N_Ydaq7KvGC1CyGley7F-TJAouxqQLv2hZD9Q7KyhME4uQ6c9jikxgEGOGmNyofvihAfdgjP2Oeanl9DEKpg-of-aMVDcC6bxFLgBHRmAdtAW6xYeJXQaTxLmF_IgLpMvOcFpVsY1faOAVkMbYx3s1mQcnRO6p5rLPAWD1BaarmOe5SGTRu24H2ifSDlu3YPudUCwmkegqzCCdmbIMVsHtb11qRt6UflD-6r7oyi4ZhdpNEdvDzNEN1gZsE-P5FrLOMNU0WxnAR1hoxM9oaDRS4EnEXRhqTfQ3HFrIM2Y8HsnET5N6VxsbGShZlLsM9rxFjlMvkiT256cc82606vi5q6WkTjmiyUjNgoEOnNe72ByCSRaEXc7zMHC6H_87vQnjwhTRnyV7dWoMtbDScDSia2KaX4EIzuEwClc0WqzCixv69UTbNKAilyhosmVwZFBQAHFSOWhJtB6_rGiaPp3pfN6i3DDImmka0qh-_8pb0AyhHccqtKB3CMswTY28GMhRAi93jeuChNuP6Hjp0aIIk7C7TQZF2kmq2lxUN7N5F-fke1WOHGkKGBHs9Dk1955P3p6F5P7JKQ6goATgIyDgX7qu4CCJUuNXAOZ_tY6Rt4OH1GExUeaeQkW1pCywcT6WtfwTFoEvdsNRG_lAFois2NjHcwzwwvEafroaFA_AFokoRGvrgD2UU6TW0e_oJMLVSX68vOYPVz1rnAYtMGw_yOKkC73YPpavpHo_13KWtmnuRBbQImvMA0JbBLPLn_tGWbV6zHlL1uTn3fkQXaO9WL-1F9F9L5TeKoEFDAJdbgyNEKsOOcwFrJ1kQXg2o-k9nzPKd0O_Py7CDu82GREnCiGKmj7yfKQnSbdNFGm8cxdow_QA2HBxNMZR7h-gDulhwN_0pXc4EpTI7BY8NNyYbENG6dhxXRbAsYi5V6UJpzqem0c7X1yxVEzTZdSHogwWpwMe6JyDWIM75WcjSUvrznl15axyWvOBV8qULm4E33SqfDm9XMM0Vx8ePTP9m1hcXkJMQFjprnB0OR5j3vqCL1yW174bBRAoBQ9Nbm4xKkeRBcxlW4VYKMgssAfFm243_i34dP5Y_cNA7Rqzkv2lICQsyjm_31N0aSawETxx_Dk3l_5Ji6V8RyIfd3v8ymrntcCLsOlqMk0L7kMhPfoENU6Rk4Kg4yjOOHrQHbqeEwpfZoNnqqwC_FE3nNW1NOopSqbiT03USdyDkpteNbXc0jbXRLDgauudUHIasxRdyElQ8z0DVz4tfOfPaFcc_93nlUx_BDY9TvYgo6QACDayxP6oYbuLSL50YcUGdkQq0MJ8-P1QAAM_7O3UzecEo37HohsiJCt-G6j_AJEkxpBbC2MhsEWDTi621MX6ViLm5YtVcWw-ASjMW2PQPGwndzq_krAXfCvQ2lIlXVvjpBSGWJIKI7SXtObmhn9DfkklulKSP17j4YRn7mU6YLzH6w_INFmSPAaidH9TcVEjwbDyWgi8YNtdvY5am9eWHYIsO=w1365-h615" width="425"/> <img src="https://lh3.googleusercontent.com/u/0/drive-viewer/AKGpihb3ogLCcg7puj3xcdjzUogpKSRvB1wG8HxPhA5akZpf4ji9jKKtNlZyC3eD5n4IT5URzaJ17V8QJXZSs1vcNw5DeVZxDg=w1365-h615" width="425"/> 

The arduino is connected though I2c pins to another arduino running a slave opporation to return readingf=s from rotary encoder. 


<img src="https://lh3.googleusercontent.com/fife/ALs6j_Hdcgk17p7d9O4zLI0hXaeaaZg-5cUC95FuSQ56dacr2d7zhthn3QjllLcnx1FsFL2jmflLjFaJvt-Y59L39nCzA3Je00cUVHi_Trk7GEBpZV_LoKFwTSZ996G8o1vAbdnjV8nTV2Z0Smk3gcz3tdRD__oSOujJmA42i7X8RPXqWqGpnkIPjEqiqg2m7o764WmzqRCUb4gMoc-odbg-dEnlx--cRhMMx-rmfz7fZp5i7Y7quYoGMiGD3v4QXk4FB_bn0w0VmHorVb534Occ9y1VBGH9oN5bGagdHib_ajsCbUje0RdRBw_PrBwtYG6bZ_KQk7uUVRg7sRzmfE2JvdfKs_vfGraClLw_IqtexBTxudr-_4Ayxo96vDATk0K5yognFiTX798Ecrc4-qzctiNACBWD2p4R-ck2OTmBh4LzrRL6oAmp_xhnUC1jgEXgjIIcc_3UI-pxW2vLISKFRpXxQQqZh5SsgKoZ9L7fWtFRlxvXsZWsEsX13Z81aXXnzvOimvoxFLEPNkYWPnjmGBTmjuEQKVl5LzloLxnW22MfJ5iyeiXWWBR10bSuZ6WGTYDq9QB3tOHFzYs7FIXrBNw4tLPTHSUxhVtO8cd-GCgWUhw_HCtUdS5XNgOkA8CYMVaW5ixpyn-IFslYm1enNC1UtkGwLY5GMrJb02FgtoO-vB6d7oeP6znZ_d5ibFZTFvIIfVf8nc6-WtfYYqzldPP4yzVe-n1GwoKHklWF6sxRdZjDOsUmwUJhWv6xWxCAhfcjSn1u2V0fCVjvzFrlVfEPVcNlSxfo2yxMo1MOW0XzAopkvBzo8FaWwZglvGCeLV6V_zCQ2ZAcmymwB9SNpEzTUL4tB7Rk75Lobn55SxPj4hIPgreykkNnl6Ybi6oCCfJn66TSDne609fBamM3xPP8-a_sbvDWHulnMfQMc7ET2MxhToGnu5DC_i9MeXKGUA0Wo8DHY8wE4wts0fT1bUS6CH_KXejs2o5DprnVS6VXI2XQayu9LNtB6903DXvShjIHPFo-3dPbD21oUPEtA4QtrgyCtHwQ66HI08pt8hG3E3D3epdEChcx1_pQprPPQCyvsNuLiS3g_EproSm96EX7rICC0Rf6BweMYAFbTFPB42m0kPd4bcPzoCwlHFCQT6sDdFwNybHVIziA7BdMzHwPpXUdKFq68Bf8vghHbHT4qT1PyctavAAUHG2VBFoPwn3SmWODFXSc5vFTMaUMWLtP90c8X_wYOu1Oxs0uNXRUmOowzwsVB4Nx6Ea2RbP_GYXm4a0I5uIM1tTv6IMvajVRymE1KQxegF9qet4zlCQiYYTbCcJWyAgEDGJbgDlIy8H4OoRneLPNmxDUdQCALrUEYq294zwLmqDTrbAhlJiHyIdqUCmewoB9u7s7zumsRxGJfCdg27xQcb4Qs-ZQnD0rb-nwjIafygP4TBKrnS_dgv9GIoVPZ7qigBTG1nS7lslW0rfvmKdgV45875OjRIkhnD_G_jyZ3-V3BFkmUNOVFo6x74zOSTzR3u2y2-QTiUOlsxwPtW8TaTR56Ef-beopjgfGzCXtoFMGXQpgx1-dDYbyFSRwqp7PzDYxgthrg4aRSqQ13EFHoA=w1365-h615" width=50% height=50%>




