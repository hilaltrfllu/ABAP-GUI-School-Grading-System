# SAP ABAP-Internship-project
Simple ABAP dialog program creation- step by step process
Steps
1)Create dialog program using se38 transaction and giving type as module pool e.g ztest_prog
2)Create screen after clicking on display objects and then by right clicking on the module pool program e.g screen 1000. Remember to do save after every step
3)Create include files ztest_prog_o01(PBO process before include ztest_prog_o01) and ztest_prog_a01(PAI process after include file)
4)Uncomment the commented part in screen 1000 and double click on STATUS_1000(to create PBO module remember to associate include file ztest_prog_o01 file). similarly double click on USER_COMMAND_1000 (to create PAI module remember to associate include file ztest_prog_a01 file).
5)Uncomment the commented part in STATUS_1000(PBO module)and give some name to status bar and title bar
SET PF-STATUS 'TESTSTATUS'.
SET TITLEBAR 'TESTTITLE'.
Double click on TESTSTATUS and TESTTITLE to create status bar and title bar
6)Write the code for PBO and PAI module. Sample code for PBO and PAI module is below.
Create the layout for screen
7)Enter text boxes(for display purpose only can give any name) . Then enter input/output boxes(use the name of the box the same as used in the User_COMMAND_1000(PAI module)). Then enter push buttons give name like change, create and display but remember to give FCTCODE as given in the PBO module STATUS_1000.
8)Create transaction using the same name as used in PBO module give program name(ztest_prog main module program) and screen number (1000)while creating the transaction and check all three boxes for GUI support (HTML, java and windows). Create all three transactions
9)Finally activate everything by right clicking on the module and then execute the program by writing the transaction name in the command box for example( /oztest_create2)

---

## Contributors
- Hilal Turfullu <turfullu.hilal@gmail.com>

---

## License & Copyright
© Hilal Turfullu

Licensed under the [MIT LICENSE](LICENSE).
