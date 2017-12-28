# Cminus-Compiler

A compiler for the C- language </br>
C-Minus is a extremely simplified version of C.</br>
It is a ridiculously trivial  project, which was originally written for a university subject (Queensland University of Technology's course ITB464 Modern Compiler Construction). It implements the C-Minus language, which is the simplest possible conventional imperative language that does something interesting (recursion, arrays, iteration, decision -- that's it)

Here's what a C-Minus program might look like:

    /*
     * A program to perform Euclid's algorithm to computer
     *  the greatest common denominator (GCD) of a pair of integers. 
     */
    
    int gcd(int u, int v)
    {
        if (v == 0) return u ;
        else return gcd(v,u-u/v*v);
        /* u-u/v*v == u mod v */
    }
    
    void main(void)
    {   int x; int y;
        x = input(); y = input();
        output(gcd(x,y));
    }
    
