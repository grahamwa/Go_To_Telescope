## GoTo Modifier for my Dobsaonian Telescope


The goal of this project is to create a GoTo system for my Dobsonian telescope that I acquired at the beginning of 2023. It should be computer-controlled and capable of moving to a selected target while also automatically tracking it. To achieve this, I will primarily use an Arduino fitted with a CNC shield that controls two NEMA 17 stepper motors with the help of a rotary encoder. To aid in my creation, I will utilize my school's laser cutter and 3D printers.




##
##



### Starting Point
##
The telescope I purchased is a f/5 130mm Dobsonian by SkyWatcher. I chose a Dobsonian over an equatorial mount for simplicity reasons, as well as for the wooden base and easy-to-remove hardware.

<img src="https://usa.all-startelescope.com/cdn/shop/products/S11710_Heritage150_LeftFront_1800x1800_3ac2cdd2-1c1b-43c0-9795-49c9df086e0c-sw_600x600.jpg?v=1645512990" width=50% height=50%>

The telescope moves on two different mounts: the base (Azimuth) and the vertical screw (Altitude). The first step I took was to figure out a way to connect the motor and the axis. The solution was to create two gears that would attach to the bases and allow the motor to move the gears in any direction. On the left is the altitude gear, and on the right is the stepper holder. For the designing process, I used OnShape, a free online software creation company.

<img src="https://github.com/grahamwa/Go_To_Telescope/assets/88165698/33e6c0f1-e2ff-4fec-838b-c6da134f178a" width="405" hieght =50%/> <img src="https://github.com/grahamwa/Go_To_Telescope/assets/88165698/e596ac78-e1e1-47d0-bab9-f39c3effd581" width="405"/> 
                                                                                                                            
##                                                                                                                          
##


### Arduinio Communication Unit


##


For housing, I laser-cut a box from thin wood using the cutter, adding holes for cables and fans, as well as an accessible power supply. This box includes a PC fan for cooling and a cutout for the USB 2.0 cable port.



<img src="https://lh3.googleusercontent.com/fife/ALs6j_HqOE5FGkFGbRnOUDfGlTLLntItIJ_7zybg3MNzYXxc7JctSnVTlDL0K-8GUnEUQmipKoGeyesxK_50n3UiybfQEGghqzEk9N_Ydaq7KvGC1CyGley7F-TJAouxqQLv2hZD9Q7KyhME4uQ6c9jikxgEGOGmNyofvihAfdgjP2Oeanl9DEKpg-of-aMVDcC6bxFLgBHRmAdtAW6xYeJXQaTxLmF_IgLpMvOcFpVsY1faOAVkMbYx3s1mQcnRO6p5rLPAWD1BaarmOe5SGTRu24H2ifSDlu3YPudUCwmkegqzCCdmbIMVsHtb11qRt6UflD-6r7oyi4ZhdpNEdvDzNEN1gZsE-P5FrLOMNU0WxnAR1hoxM9oaDRS4EnEXRhqTfQ3HFrIM2Y8HsnET5N6VxsbGShZlLsM9rxFjlMvkiT256cc82606vi5q6WkTjmiyUjNgoEOnNe72ByCSRaEXc7zMHC6H_87vQnjwhTRnyV7dWoMtbDScDSia2KaX4EIzuEwClc0WqzCixv69UTbNKAilyhosmVwZFBQAHFSOWhJtB6_rGiaPp3pfN6i3DDImmka0qh-_8pb0AyhHccqtKB3CMswTY28GMhRAi93jeuChNuP6Hjp0aIIk7C7TQZF2kmq2lxUN7N5F-fke1WOHGkKGBHs9Dk1955P3p6F5P7JKQ6goATgIyDgX7qu4CCJUuNXAOZ_tY6Rt4OH1GExUeaeQkW1pCywcT6WtfwTFoEvdsNRG_lAFois2NjHcwzwwvEafroaFA_AFokoRGvrgD2UU6TW0e_oJMLVSX68vOYPVz1rnAYtMGw_yOKkC73YPpavpHo_13KWtmnuRBbQImvMA0JbBLPLn_tGWbV6zHlL1uTn3fkQXaO9WL-1F9F9L5TeKoEFDAJdbgyNEKsOOcwFrJ1kQXg2o-k9nzPKd0O_Py7CDu82GREnCiGKmj7yfKQnSbdNFGm8cxdow_QA2HBxNMZR7h-gDulhwN_0pXc4EpTI7BY8NNyYbENG6dhxXRbAsYi5V6UJpzqem0c7X1yxVEzTZdSHogwWpwMe6JyDWIM75WcjSUvrznl15axyWvOBV8qULm4E33SqfDm9XMM0Vx8ePTP9m1hcXkJMQFjprnB0OR5j3vqCL1yW174bBRAoBQ9Nbm4xKkeRBcxlW4VYKMgssAfFm243_i34dP5Y_cNA7Rqzkv2lICQsyjm_31N0aSawETxx_Dk3l_5Ji6V8RyIfd3v8ymrntcCLsOlqMk0L7kMhPfoENU6Rk4Kg4yjOOHrQHbqeEwpfZoNnqqwC_FE3nNW1NOopSqbiT03USdyDkpteNbXc0jbXRLDgauudUHIasxRdyElQ8z0DVz4tfOfPaFcc_93nlUx_BDY9TvYgo6QACDayxP6oYbuLSL50YcUGdkQq0MJ8-P1QAAM_7O3UzecEo37HohsiJCt-G6j_AJEkxpBbC2MhsEWDTi621MX6ViLm5YtVcWw-ASjMW2PQPGwndzq_krAXfCvQ2lIlXVvjpBSGWJIKI7SXtObmhn9DfkklulKSP17j4YRn7mU6YLzH6w_INFmSPAaidH9TcVEjwbDyWgi8YNtdvY5am9eWHYIsO=w1365-h615" width="425"/> <img src="https://lh3.googleusercontent.com/u/0/drive-viewer/AKGpihb3ogLCcg7puj3xcdjzUogpKSRvB1wG8HxPhA5akZpf4ji9jKKtNlZyC3eD5n4IT5URzaJ17V8QJXZSs1vcNw5DeVZxDg=w1365-h615" width="425"/> 

##
The Arduino is connected through I2C pins to another Arduino running a slave operation to return readings from the rotary encoder. This will allow the user to use a method know as polar aligning. THe rotary encoders are used to move the mtors untill the star is in view, then the tlescope can use the coords of the star to slew to any other night sky object. I used a format in which a press of the rotary encoder switches the motors and left is negative rotation and rigt is posotive rotation.
##

<img src="https://lh3.googleusercontent.com/fife/ALs6j_Hdcgk17p7d9O4zLI0hXaeaaZg-5cUC95FuSQ56dacr2d7zhthn3QjllLcnx1FsFL2jmflLjFaJvt-Y59L39nCzA3Je00cUVHi_Trk7GEBpZV_LoKFwTSZ996G8o1vAbdnjV8nTV2Z0Smk3gcz3tdRD__oSOujJmA42i7X8RPXqWqGpnkIPjEqiqg2m7o764WmzqRCUb4gMoc-odbg-dEnlx--cRhMMx-rmfz7fZp5i7Y7quYoGMiGD3v4QXk4FB_bn0w0VmHorVb534Occ9y1VBGH9oN5bGagdHib_ajsCbUje0RdRBw_PrBwtYG6bZ_KQk7uUVRg7sRzmfE2JvdfKs_vfGraClLw_IqtexBTxudr-_4Ayxo96vDATk0K5yognFiTX798Ecrc4-qzctiNACBWD2p4R-ck2OTmBh4LzrRL6oAmp_xhnUC1jgEXgjIIcc_3UI-pxW2vLISKFRpXxQQqZh5SsgKoZ9L7fWtFRlxvXsZWsEsX13Z81aXXnzvOimvoxFLEPNkYWPnjmGBTmjuEQKVl5LzloLxnW22MfJ5iyeiXWWBR10bSuZ6WGTYDq9QB3tOHFzYs7FIXrBNw4tLPTHSUxhVtO8cd-GCgWUhw_HCtUdS5XNgOkA8CYMVaW5ixpyn-IFslYm1enNC1UtkGwLY5GMrJb02FgtoO-vB6d7oeP6znZ_d5ibFZTFvIIfVf8nc6-WtfYYqzldPP4yzVe-n1GwoKHklWF6sxRdZjDOsUmwUJhWv6xWxCAhfcjSn1u2V0fCVjvzFrlVfEPVcNlSxfo2yxMo1MOW0XzAopkvBzo8FaWwZglvGCeLV6V_zCQ2ZAcmymwB9SNpEzTUL4tB7Rk75Lobn55SxPj4hIPgreykkNnl6Ybi6oCCfJn66TSDne609fBamM3xPP8-a_sbvDWHulnMfQMc7ET2MxhToGnu5DC_i9MeXKGUA0Wo8DHY8wE4wts0fT1bUS6CH_KXejs2o5DprnVS6VXI2XQayu9LNtB6903DXvShjIHPFo-3dPbD21oUPEtA4QtrgyCtHwQ66HI08pt8hG3E3D3epdEChcx1_pQprPPQCyvsNuLiS3g_EproSm96EX7rICC0Rf6BweMYAFbTFPB42m0kPd4bcPzoCwlHFCQT6sDdFwNybHVIziA7BdMzHwPpXUdKFq68Bf8vghHbHT4qT1PyctavAAUHG2VBFoPwn3SmWODFXSc5vFTMaUMWLtP90c8X_wYOu1Oxs0uNXRUmOowzwsVB4Nx6Ea2RbP_GYXm4a0I5uIM1tTv6IMvajVRymE1KQxegF9qet4zlCQiYYTbCcJWyAgEDGJbgDlIy8H4OoRneLPNmxDUdQCALrUEYq294zwLmqDTrbAhlJiHyIdqUCmewoB9u7s7zumsRxGJfCdg27xQcb4Qs-ZQnD0rb-nwjIafygP4TBKrnS_dgv9GIoVPZ7qigBTG1nS7lslW0rfvmKdgV45875OjRIkhnD_G_jyZ3-V3BFkmUNOVFo6x74zOSTzR3u2y2-QTiUOlsxwPtW8TaTR56Ef-beopjgfGzCXtoFMGXQpgx1-dDYbyFSRwqp7PzDYxgthrg4aRSqQ13EFHoA=w1365-h615" width="400" /> <img src="https://lh3.googleusercontent.com/u/1/drive-viewer/AKGpihZPKmQMdnu8GO7JTU3M0Lvmn9zVohIor7gG5O6rodfTDETwwssMNCTBIzqP03n3bPuHBXeOcDw0heqdkFFDIP8UtrQD=w1920-h945-v01" width="405"/>

## 
### Physical Adaptation
## 

After some testing, I found that direct gear mounts yeilded the best result as far as stability and function compared to beld driven modles. The Form I used was one which had two motors connected to gears of 250 teeth and 550 teeth to build a aconstant ratio between the cog and gear diatmeter. Luckily OnShape has this feature built in so I simply pluged in my values for both and it gave me a design. For the altidude motor the cut out mehtod worked well for powering the heavy telescope around its base. I simply screwed through the wall into the motor to get the correct angle.


<img src="https://lh3.googleusercontent.com/fife/ALs6j_HLFFDQyuIDDHjAbRIIweIwuUBi6DPW09Hg-7iaKnoHuBrD7EO1XnFhIRsZhcLhwUPo-n8PZh0pH2oCABYmkkHM2HLzS9gU1C4XLrtszMLCTGGOnUbHDPu6-u42FSCXPIwurUEHvsAAhoT-quzM0S9wSZfWwbTTDBJvbhfWC51gaBsLje8TNoIShUtpOEHHZiT4blpEwp6mdN2n0w6PwzZRoeusgq1SklZzTBn_p_D0XJldrZKn1f9kdsaNQ7C8NNLpUlcwESu157qDKTq7reP4DL07IpDjfmF4udN8ZTkTG86TRpv6SaH-NU1zmOMe3NgamdbhU2y1edMoGMOdni9bIHLvMqozeyRFp__c88_gE7vSWqlDi6rx9MpTD_ZHRTdmBGnVsdzT70rCX1tciaDnL0RCcrVwDW28LLT_WABO-evI95xi_hmo9lR3wJDonEksMPWvZkkv6j_R2Z_q6I4bhlUGhJ_ruoj-hoHZJKk7dHmsLMbkXxc90ZHFNTvqVX7heV2lRNCSsO25OW0Tvr5U97TWPMB-U1aBUNEwF1Y1v6c15NPb1-ttZR_eaKIi1V6yDPxN2ziq6hJfd6xZb7KIorPrm-ITZcWfzl7YxqABx2EDmcF4PUoEX5x6x_PTXQpIrnsOE__yw51Hri1QvDEXJeCIEgpyvUUWU-_GI1h36pd8mK2uHqORZojtMOxcdjQ4Vx67iEBTATisKUYVMb0nA7I9ZKs133jLYx8UHXpxEqJzuh2N96ThaMdV7l8OwYavJGFrDb3EjSOfKqau3ItyBfKz53Yz0IaX4_h1FnefRIrQ9HCfOf6Dbiq-VajDYKxCvGF-yAkiPbqartl0G_8yU5SL75EIw4RZhgS3278bxTd_P72EEMbmLIlX-uSBJCVnGVKVjapZ_j87mJm9YClcPQwP3dTQOf0gAGqUB3jQ28cXMTPhBDitorOZZWrHK_cIYZCfJe_AyNjckpEq7jT0SPJLIOaq5GwUYt3MrpgeU-IO_p4sgms185YBVLIG-U7my7aLSUqL7vYXQFOpmCu0Wwt6qrFWZNHpAYgJ2K-cA20QmxjhTAFgNOHjmCg7vpi-i9Qm8RuBzYS3wqpewgo98xuH62Po_kTgST6iyl4LRPgt8BjeKpwAnN9IjfxJn55YvW-7NuY0Bgz1ab_4ihjmpdxzzb7ZGc-Bikd8K6ql9LbrAoIaB6I1neb28PIN7FsN3hZYMxcAooQgilwCCbPi0k2sv02Lb1HsQHQZDGWdsvXgeT8G48ZbL4eYEwnbTZF6BEUXXpfxr3WmFd3iAfTH0s9rFSigV9XNHdcFhhCZYLrkvw2PstbHAi61hgM8OP7W_CD4R3YGB7MnSWHbuenmRgQ6lh2R7Gq8cqk-xb1-2hTNsPonFMedWGyc1gZDS_crVK2sjS0M9FQQpap7NGTsfEmqmyOIwrj6-tmlDS3yer_FLoItgs0UHwM9qis3oOqkYIT8uLYqhL9mBt88xOSVnapnZONsYxr_1FqQwDH89bClvxf0eYiyyeWnPcwlqY4acrTUSRick0l7lyCtAl2pPPHdrMypa2_KOtl9EbSzHdrK3iaZ9y8zh88e8nNtai4BYekqK5IduVzydTdud6px3aIjoIIuRILw7ZwWZrJrLbumuDQ=w1920-h945" width=50% height=50%>

##

To print a large enough base gear I had to split my prints into four even parts whch later were glued and screwed together. The gear has 550 teeth an perfects overlaps the bracket for the motor and the base. This means that you can simply slide in the motor into the holder and everything fits tightly.

##

<img src="https://lh3.googleusercontent.com/fife/ALs6j_G5NWpC3JY5fw5uqOdH9dcLwbefhNr7vNBGLCr7vpNmO6rEzPD9vrzK8kpNn3-BRJiaMW7Q4mVOC00H40IGvsEwSA4ZjLzl04U-VfVTWiAu61JjfDqiUPAl4ZJLwLAlwfBaIrnKimIJJgVAlf46lWGCfno6wZtHuDKtZX0lPPUPGoptmEUYQBTTIhX7iFp_Io2Oa8GOG9wD2aZ1KS5Ku5l9kGGXSFgvP6aKt4v-lauMsv2YNNLPMwba1tQK4NF5c704K3152BIjG-749u52LhAvsRKX3zV2zQdFBEqJZ4_KLzCP2ElokKwaBREK-aR40kqhCoF1AniprgG-BKdHLk9574zjZAr-VHSwp6cyECUC77eVjsUBF8K3ZmurgJKKEAOgrziof5wTzD01wNEhrVWtDIcuA4on7D46as9Hhc8lBsBgLOLm_OZ0YCyf9VlK-y1uQ4vEWvd7PTMa1mwj4yzZz_ireNPSW14irLvGP3JnjeeDsGJPGTvOxEm7b65_qSJ3nqqQ7VHvSpGBdq7mD54faICJv8l4dupHhcQrrKgUESx1qHmkS6zGV1VN-DsyVOalTTqOcJoKiubRmQ-Z3B6dmAD2uMnxmEU8Q69LTOS6ZCJW9MZFvWqIyEsYBPUNPNxRnVYTbRXJjnzpSofqdfaE3BF0XlfOZ-hhQQYvaQgHQeU7KZdckthzWS492nsq979qIQWojVWzMvwfmqK2iXAnPf15geETQwiJx5sKxXpwcpiSH7-TrAKPqo_rfXcqeaTS6v8gm8bnnMxcjQInoEtx37Gd6O82jutkeEgQscQ0zijMWBhs-wHBwtZ_ICrA_JGFYTatymWPb_N9W_qsUM4iqeRU1pbwiiAuziojA-Uau9Sp_MaA8jqM8VvTtDuxVpEhHbrb_vXlBtgDXBWBQrFetHCxla-SH6LR_gFwDWx2halSYdkiH3GOg9qhi2U7xTeNi-eR7Ceu__fUnsHx0WZ0U7-V6pfnyU3bNQfXzQoRU8Cpi77axyDw-_xNDHXjxDA5fzzdS2OxskXPsnIJ_N7P0tt-73UbB4D0bQyx09-nSqg9P_6VeuYAbESiPskhTuQR-6_-nb-ZMI-fhbkHKHkcVTcK8TaujfcYCCK9JHb0lBrohldL4XZejn8W4Pzm_m16Smibsk4MwEYqc_u4F4VEl_HT3ggc7vvbzYtLozLvJxb37kRtbPYQ4J2_x59nGntq3igIjtbvzV7UZZjZOEKYe06SFhRva5ufpHetTf3F3r1PfpnEJ66azIuyZvKnB1UTxhcFYhLEvH7Bwh08x-6XlYKomvdpnC-07AZ8x-dYkKAszZtulhqTDoCO6cW0sZqKzXV1hQ1cO6Kt-2whHXAUabn8j8aAulztz14H-w0RWNz98VB0yXrUMU6HpiVF86AhnthyqS25SYe15RO9CoSnt4mtzx__vEp0IMJvn_X4yvAGeYytZAS2EHWtOyXYLlCwZL78hAt5Mjq7pIt47dIWx7W8zluR5XWLF3D0qOOICFk4NmQIpCk6eDeRV6hTn9UhllITeukaa_Ja_6GlgXsl_qKy9tPY7lNY6yCkHB4v_ef3zwdpWNAd4-KmG1EwsA0kwiAq06IvUN-wxqfxUhWLzUaHsULU8EJMaKuMpGsifCWA1nMn=w1920-h945" width="400" /> <img src="https://lh3.googleusercontent.com/fife/ALs6j_FNTLkHHWPOSTRPnuYL_9RdFsvfDtMF0IgGRsoppf0VOKbbIi575VGyYTLPOqkP7K7WLFAm3V-nFLdh04ldlWL7RxPGs3x3UElE8DBq9RJ1oEVarDHtPvLSw5IXNkg8lTJwspJrYmjNfankzRyveroVXAn322c2YbpwH1eGDVj-4Ye0sz498Dcy692UZNHMS70LIDwtGWRYp7xXpJtkC5ZrUi7HMor3DteBD603dKn5AXkXZ7wAHfTptCkqMarnk_jDaaLnDbm5xgzFYt3GcbR9eZgqCilC8-MvfFa_KjMIiTVwQMw_7Ad1M7QzWO_p95umP89DUVlG5R9vxIPe2U_Gs-R6-8pgaYWJXSokLasTRoAVPW4PRyP__xMZbuko7u8wR7ARQcqonxWznJleNl_JQBWJbsjJvUwzy5zpQ-hi7gaNTDzFNHeS8AmrGob6Kfpvp8SwL3--mNaWB76nPfpulfx6sJ75kEmOvaIWGxhfStU8Fye1NqaQof7Gbr3aZ-V6tmu0D7FEo3SW1fNDzb-Px4_LK3TKgVqkafPmTZT2ZSnya2HrQY9-wjyidCEno4bPE9rvz0Sr4LccN5MG1mnUGTzYomYytfeWrOBA8JyJBVd6LNQRYmKXJXobqihNW2zkmm3bZCDd4etkEATfH9nmCgUfQVjnZSXw3vmNGOC7mDFVWcZvRotRkjl5djgfBafViAtdtIKc7KZJKddQcaVk-ki0l2AD5NBiapxFXchCI2QfpmjOuWkHi4W3RcSIsJIOqL51jeHEN5lBQYhZCZlAhb8-UBK31kUdN-Ui50iwLnoQp3x2pFuEqo9uktZA62x38992Ki92xx-491Z0DVu1W6Q_6XQQNLcVnyZ3BTFTJ1BhaTUQA1bBwcNiMQ03TyUiqJLcZHID5icVl_773MmDMUxGIrbA9XjXHEoeDHD_Asl6C8UjGax7rxTH_Sow-Q5LrB_7P3xVTm2fPpBUCroa-4TpTCuH5oOhOcGOTzQeINqiQQqK88gg4pWJBMucWMt2zHFLvwaX6T9Fu7lFCeIwK3jXoQm0gxwwd8Ti3uqZfLyzaiBEk3pCtkIPCO311YO8xPq6KPRQk4yZjXn0SyaSCQBAtgk7VSFQobXI9GYIL_7DMjIX5gD7RXhS8GHhSU-cajrYOnG5ixzOUEIYNiK1in2CgFBfShII2NQcGec67fYxskymohps4hHx0hnJQ2IOov1KsVivaT3tAwIP5fVppSx2jmwmH2vVww2olpM5fUMAm4WGK8odV8_vZISnux40gXc5TlGOZDSkckjZ5HHtbfPDuhdIRG64dhJEFDHU8E9vwbdchbMmVWWwGfo4XNRdQ4I69AUSItyQF2m5nYtGov7QfdyAfXWpmvwUdmywaZXRk6wWnfiw5zYIlksvEK1gZPZMjy4Af6uMM8prT3-SpSqgy0NwruGgN3mqy5haE_N7dExE8BG51xPhBpk9oqK9tvOSKJF6IRarHEjbOY-rjuy8HVtuY3DvS5QktZdW_yxl26wMd3o7xmgYRM1-45IVAQ5rRGc9szJsUAKT-v_dufrsupB0oqXXECrmnbhaVKtiGi9aI3COPPQjNqOfdojNhRH577Go7c6SY04vWOX1maZT3746rzOGRlCUunt7GyDQlwrA=w1920-h945" width="405"/>

## 
### Code and Communication
## 

Furhter Impleemtation is linked and I will produced video when I create my Jekkl website-

STAY TUNED!
