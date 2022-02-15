Zadaca 1 za QAmp








public class zadaca1 {
    public static void main(String[] args){
        Scanner key = new Scanner(System.in);
        System.out.println("Insert your bill: ");
        int racun = key.nextInt();
        System.out.println("Insert your money: ");
        int money = key.nextInt();

        int kusur = money - racun;

           if ((money<=100) && (racun>0)) {

               int dvadesetMaraka;
               int desetMaraka;
               int dvijeMarke;
               int jednaMarka;
               double polaMarke;
               double dvadesetFeninga;
               double desetFeninga;
               double jedanFening;

               NumberFormat format = new DecimalFormat("0.00 ");
               System.out.println("Your change is: " + format.format(kusur) + '\n');

               dvadesetMaraka = kusur / 20;
               kusur = kusur % 20;
               desetMaraka = kusur / 10;
               kusur = kusur % 10;
               dvijeMarke = kusur / 2;
               kusur = kusur % 2;
               jednaMarka = kusur / 1;
               kusur = kusur % 1;
               polaMarke = kusur / 0.5;
               kusur = (int) (kusur % 0.5);
               dvadesetFeninga = kusur / 0.2;
               kusur = (int) (kusur % 0.2);
               desetFeninga = kusur / 0.1;
               kusur = (int) (kusur % 0.1);
               jedanFening = kusur / 0.01;
               kusur = (int) (kusur % 0.01);

               System.out.println("You'll get: " + (double) dvadesetMaraka + " 20KM");
               System.out.println("You'll get: " + (double) desetMaraka + " 10KM");
               System.out.println("You'll get: " + (double) dvijeMarke + " 2KM");
               System.out.println("You'll get: " + (double) jednaMarka + " 1KM");
               System.out.println("You'll get: " + (float) polaMarke + " 0.5KM");
               System.out.println("You'll get: " + (float) dvadesetFeninga + " 0.2KM");
               System.out.println("You'll get: " + (float) desetFeninga + " 0.1KM");
               System.out.println("You'll get: " + (float) jedanFening + " 0.01KM");
           }
           else if (racun==0) {
               System.out.println("You didn't buy anything did you?");
           }
           else if (money>100) {
               System.out.println("You have too much money");
           }
           else if (racun<0) {
            System.out.println("Did you maybe break something?");
        }

           }
    }
