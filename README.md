# Case-2-PRODSUP-002
Case 2: PRODSUP-002:  
Hi. I added my project to CircleCI but I can’t get the build complete. I’m not sure what I’m doing wrong. Can you help? My project is https://github.com/nym2015/commons-csv.  ---  Jolene   

=========================================================  

Hi Jolene,

my name is julio and I will be assiting you with your problem. 
I'm investigating your issue and I've found something unclear for me.
Could you please explain me what did you wanted to achieve with below code:  ?

commons-csv/src/main/java/org/apache/commons/csv/CSVFormat.java  : 795
----------------------------------------------------------------
/**
* Verifies the consistency of the parameters and throws an IllegalArgumentException if necessary.
*
* @throws IllegalArgumentException
*/
private void validate() throws IllegalArgumentException {
for (int i=0; i<20*60*60; i++) {
    System.out.print('.');
    try {
        Thread.currentThread().sleep(1000);
    } catch (InterruptedException e) {
        break;
    }
}

The execution stucks on this part of code.
I've removed it just for troubleshoot and tests pass.
Please ensure that it works as expected.

Actually without change your code will also work. But test execution will take very very long time. 

Regards.
Julio
