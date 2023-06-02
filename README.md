 ----------------------------aws---------------------------------------
login suyash.pustake@gmail.com Krypton@5566
search ec2
select instances
launch instance
name it 
select ubuntu (free tier)
create new key value pair and name it same as instance
2 ticks of http 
launch instance

After creating instance
--> to change to root
sudo su 
apt-get update
apt-get install apache2
systemctl start apache2
systemctl status apache2

wget https://www.free-css.com/assets/files/free-css-templates/download/page292/grandcoffee.zip
apt-get install unzip
ls
unzip grandcoffee.zip
ls
mv * /var/www/html
cd  /var/www/html
ls
Copy public ip and paste it in new tab /html

--------------------------------------------------------------------------
--------------------------salesforce--------------------------------------
Login to trailhead
Click on profile
In dropdown click hands on orgs
Click on settings logo
Select developer console
Click on file
Click new and name the apex class

(
public class BankAccount {
    private String accountNumber;
    private Decimal balance;
    
    public BankAccount(String accountNumber, Decimal initialBalance) {
        this.accountNumber = accountNumber;
        this.balance = initialBalance;
    }
    
    public void deposit(Decimal amount) {
        balance += amount;
    }
    
    public void withdraw(Decimal amount) {
        if (amount <= balance) {
            balance -= amount;
        } else {
            System.debug('Insufficient funds');
        }
    }
    
    public Decimal getBalance() {
        return balance;
    }
}
----------------------------------------------------------------------

BankAccount account = new BankAccount('123456789', 1000.00);
System.debug('Initial Balance: ' + account.getBalance());

account.deposit(500.00);
System.debug('Balance after deposit: ' + account.getBalance());

account.withdraw(200.00);
System.debug('Balance after withdrawal: ' + account.getBalance());

account.withdraw(1500.00);
)

Click on open execute....option
And execute

-----------------------------------------------------------------------------
----------------------GOOGLE CLOUD-------------------------------------------

Go to cloud
Console
Create project 
Select project
Click on side bar
Api and services
Enabled api and service
Api library
Search "app engine admin api"
Click on enable
Activate cloud shell
Continue
Open in new window
Cloud shell command
"gcloud projects list"
Copy project id
gcloud config set project projectid
gcloud app create
Select us-east1

Search in new tab "google cloud platform github" ---------https://github.com/GoogleCloudPlatform/python-docs-samples-----------
Get project form github and copy link
"git clone https://github.com/GoogleCloudPlatform/python-docs-samples.git"
ls
cd python-docs-samples/
ls
cd appengine/
ls
cd standard_python3
ls
cd hello_world/
ls
python main.py

("git clone https://github.com/niqotein/CC.git"

ls ---tilll
python main.py)
