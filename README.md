# ReckonExample

<b>Useful Info</b>

<li>Development tools: IntelliJ Ultimate</li>

<li>Server: Wildfly</li>

<li>localhost to internet: pagekite.me</li>

<li>api reference: https://apiexplorersandbox.openbankproject.com</li>

<li>json to java object: http://pojo.sodhanalibrary.com</li>

<li>JUnit test: Refer to jTest.java</li>



<br/>
<br/>

<b>HeroKu API (cloud) - Active</b>

<li>GetBank list:</li>
https://myreckoning.herokuapp.com/ReckonINGExample/getBanks

<li>Get all accounts for user bennettzhou1</li>
https://myreckoning.herokuapp.com/ReckonINGExample/getMyAccounts?user_name=bennettzhou1

<li>Get all accounts for user superhero</li>
https://myreckoning.herokuapp.com/ReckonINGExample/getMyAccounts?user_name=superhero

<li>Get balance for user bennettzhou1, bank_id = rbs(RBS Bank), Account name=BenAccount_1</li>
https://myreckoning.herokuapp.com/ReckonINGExample/getAccountById?user_name=bennettzhou1&bank_id=rbs&account=BenAccount_1

<li>Get balance for user superhero, bank_id = hsbc-test(HSBC Bank), Account name=superhsbc</li>
https://myreckoning.herokuapp.com/ReckonINGExample/getAccountById?user_name=superhero&bank_id=hsbc-test&account=superhsbc

<li>Get balance for user superhero, bank_id = at02-1465–01(ING Bank), Account name=supering</li>
https://myreckoning.herokuapp.com/ReckonINGExample/getAccountById?user_name=superhero&bank_id=at02-1465--01&account=supering


<li>Transfer 10 dollar from ING bank account to HSBC account under user_name superhero</li>
https://myreckoning.herokuapp.com/ReckonINGExample/createTransaction/superhero?frombank_id=at02-1465--01&fromid=supering&amount=10&tobank_id=hsbc-test&toid=superhsbc


<li>Check Transaction history for account superhsbc in HSBC bank, under user superhero</li>
https://myreckoning.herokuapp.com/ReckonINGExample/getTransactionHistoryById?user_name=superhero&bank_id=hsbc-test&account=superhsbc


<li>Check ALL Transaction history of user superhero (sorted by completion datetime in descendent)</li>
https://myreckoning.herokuapp.com/ReckonINGExample/getMyTransactionHistory?user_name=superhero

<li>Loan Calculator for comparing the offering package based on the provided information
Input Required:
loanAmount(int): Loan Principal
numYears(int): loan duration
currentAge(int): Current age of borrower
totalMonthlyDebt(double): Currently monthly debt of borrower
totalMonthlyIncome(double): Currently monthly salary income of borrower
Loantype: loan offered by which bank

https://myreckoning.herokuapp.com/ReckonINGExample/loan-calculator?loanAmount=500000&numYears=15&currentAge=35&totalMonthlyDebt=3600&totalMonthlyIncome=8888&LoanType=ING

https://myreckoning.herokuapp.com/ReckonINGExample/loan-calculator?loanAmount=500000&numYears=15&currentAge=35&totalMonthlyDebt=3600&totalMonthlyIncome=8888&LoanType=SCB

https://myreckoning.herokuapp.com/ReckonINGExample/loan-calculator?loanAmount=500000&numYears=15&currentAge=35&totalMonthlyDebt=3600&totalMonthlyIncome=8888&LoanType=OCBC

https://myreckoning.herokuapp.com/ReckonINGExample/loan-calculator?loanAmount=500000&numYears=15&currentAge=35&totalMonthlyDebt=3600&totalMonthlyIncome=8888&LoanType=CITI

https://myreckoning.herokuapp.com/ReckonINGExample/loan-calculator?loanAmount=500000&numYears=15&currentAge=35&totalMonthlyDebt=3600&totalMonthlyIncome=8888&LoanType=HSBC



