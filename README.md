# HANGMAN_SEARCH_GAME_IN_C_Language

 #include<iostream>

#include<string.h>

using namespace std;

int main()

{

    cout<<"_____HANGMAN SEARCH GAME_____\n";

    cout<<"_You Can play Three times this game_\n\n";

    cout<<"~~~Dictionary of Words~~~\n";

    cout<<"Pink\nRed\nYellow\nWhite\nBrown\nBlack\nBlue\nOrange\n\n";

    string x,m;

    int w=0,l=0,at=0;

    a:

    cout<<"Here is a word from dictionary with all hidden characters,\nNow you have to guess the hidden characters:\n";

    cin>>x;

    at++;

    if(x=="Brown")

    {

        cout<<"\n\nCongratulations!you successfully guessed the hidden characters\n";

        w++;

    }else

    {

        cout<<"\n\nYou failed,Good luck for next time\n\n";

        l++;

    }

    if(at<3)

    {

        cout<<"Are you want to play one more time?\n\nPress: ~YES~ for playing\npress: ~NO~ for not playing!!";

        cin>>m;

        if(m=="YES")

            goto a;     

    }

    cout<<"you win the game "<<w<<" time.\n";

    cout<<"And Loss "<<l<<" time";

}
