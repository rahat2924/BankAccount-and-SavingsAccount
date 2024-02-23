 class BankAccount {
 protected double balance;
 public BankAccount(double
 initialBalance) {
 this.balance = initialBalance;
 }
 public void deposit(double amount)
 {
 balance += amount;
 }
 public void withdraw(double
 amount) {
 balance-= amount;
}
 }
 class SavingsAccount extends
 BankAccount {
 public SavingsAccount(double
 initialBalance) {
 super(initialBalance);
 }
 @Override
 public void withdraw(double
 amount) {
 if (balance- amount >= 100) {
 balance-= amount;
 } else {
 System.out.println("Withdrawal
 denied: Insufficient funds");
 }
 }
 }
 public class Main {
 public static void main(String[]
 args) {
 SavingsAccount savingsAccount
 = new SavingsAccount(500);
 savingsAccount.withdraw(400); //
 Should be denied
savingsAccount.withdraw(200); //
 Should be allowed
 System.out.println("Remaining
 balance: " +
 savingsAccount.balance);
 }
 }
