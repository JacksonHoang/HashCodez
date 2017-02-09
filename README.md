# HashCodez
Creating Hash values with strings.



import java.util.*;

public class HashCodez {

public static Random r = new Random(26);

public static int hashcode(String s)
    {

        int hash = 0;
        for (int i = 0; i < s.length(); i++)
        {
            hash = (hash*31) + s.charAt(i);
        }
        return hash;

    }


public static void main (String [] args)
    {

        int z = r.nextInt(52);
        System.out.println(z);



        int hashco = hashcode("h");
        int hashco1 = hashcode("o");
        int hashco2 = hashcode("a");
        int hashco3 = hashcode("n");
        int hashco4 = hashcode("g");
        int hashco5 = hashcode("hoang");

        System.out.println("The hashco value of h is: " + hashco);
        System.out.println("The hashco value of o is: " + hashco1);
        System.out.println("The hashco value of a is: " + hashco2);
        System.out.println("The hashco value of n is: " + hashco3);
        System.out.println("The hashco value of g is: " + hashco4);
        System.out.println("The hashco value of hoang is: " + hashco5);

        int hashco6 = hashcode("baaa");
        System.out.println("The hashco value of aaaa is: " + hashco6);

        StringBuilder a = new StringBuilder();
        StringBuilder b = new StringBuilder();


        String alphabet = "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ";

        /*

        for(int i=0; i<1; i++)
        {
            a.insert(i, alphabet.charAt(r.nextInt(alphabet.length())));
        }
            System.out.println(a);
        for(int i=0; i<1; i++)
        {
            b.insert(i, alphabet.charAt(r.nextInt(alphabet.length())));
        }
            System.out.println(b); 


            int hashco7 = 0;
            int hashco8 = 1;

            for(int i=0; i<1; i++)
            {
                a.insert(i, alphabet.charAt(r.nextInt(alphabet.length())));
            }
            hashco7 = hashcode("a");

                do{

                for(int i=0; i<1; i++)
                    {
                        b.insert(i, alphabet.charAt(r.nextInt(alphabet.length())));
                    }
                hashco8 = hashcode("b");


                } while (hashco7 != hashco8);



                System.out.println(a);
                System.out.println(b); 
                System.out.println("The hashco value 7: " + hashco7);
                System.out.println("The hashco value 8: " + hashco8); 


        */
}
}
