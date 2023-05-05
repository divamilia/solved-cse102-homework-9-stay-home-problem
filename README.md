Download Link: https://assignmentchef.com/product/solved-cse102-homework-9-stay-home-problem
<br>
<strong>Part 1.</strong><strong> Stay Home Problem  </strong>

As you know, everyone should stay at home because of the Covid-19 pandemic. Cin Ali, who goes out before the curfew, must run to his home the fastest way before the ban begins.

Let’s assume that Cin Ali is in the bakery at the intersection of Street 2 and Avenue 3, as shown in the diagram, and that he wants to return to his home at the intersection of Street 1 and Avenue 1. Even though Cin Ali wants to avoid getting out of the way, there are equally short cuts.

For example, there are three possible ways in this diagram, as follows:

<ul>

 <li>Move left, then left, then down.</li>

 <li>Move left then down, then left.</li>

 <li>Move down, then left, then left.</li>

</ul>

Your job in this issue is to write an <strong><u>recursive function:</u></strong><strong> [Solutions made without using the recursive function will not be evaluated!]</strong>

int numPathsHome(int street, int avenue)that returns the number of paths Cin Ali could take back to the origin from the specified starting position, subject to the condition that Cin Ali doesn’t want to take any unnecessary steps and can therefore only move west or south (left or down in the diagram).

<strong>Part 2.</strong><strong> COVID-19 Health Coverage </strong>

Imagine that you are hired as Minister of Health of Turkey. Turkey as well as in the whole world there was a need of a national network of hospitals against the pandemic. As the Minister of Health, you need to investigate possible locations for these new hospitals. Your consultants have prepared a list of potential hospital areas for you.Each of these hospitals has a cost and will provide coverage to some nearby cities. We can represent each potential hospital area as a <strong>struct </strong>as follows:




<strong>struct Hospital </strong>

<strong>{ </strong>

char* name;     char citiesServed[3];

<strong>}; </strong>




Although you are interested in providing health care to all, you do not have funds to build an unlimited number of hospitals. <strong><u>Using recursion</u></strong>, you are interested in seeing whether or not it is possible to provide quality health care to every city given a limit on the number of hospitals you can construct. <strong>[Solutions made without using recursion will not be evaluated!]</strong>

Suppose that you are given a char array representing the names of all of the cities in your country. You are also provided with a list of all the proposed hospital locations, each of which is represented by the set of cities that the hospital could service.  Given your funding restrictions, you can purchase at most numHospitals total hospitals.

Write a function:

int canOfferCovidCoverage(char _cities[6], char _locations[4][3], int _numHospitals, struct Hospital results[4]) that accepts as input the set of all cities and a list of the cities that would be covered by each hospital, along with the maximum number of hospitals that can be constructed, and returns whether or not it is possible to provide coverage to all cities using the limited number of hospitals.  If so, your function should update the result parameter to contain one such choice of hospitals.

As an example, consider the country below, where each city is represented by a letter and each potential hospital location is represented with a black dot:

Here, each hospital is can cover all the cities within their circle of coverage.  This would represented as follows:

<ul>

 <li><strong>cities = { “A”, “B”, “C”, “D”, “E”, “F” } </strong></li>

 <li><strong>locations = { {“A”, “B”, “C”}, {“A”, “C”, “D”}, {“B”, “F”}, {“C”, “E”, “F”} }</strong></li>

</ul>

The topmost hospital would serve cities A, B, and C. The hospital on the left would cover A, C, and D. The hospital on the right covers just B and F, and the hospital on the bottom covers C, E, and F. If you can only purchase two hospitals, then there is no way to guarantee coverage to everyone.  However, if you can purchase three hospitals, then you can cover everyone – purchase the top hospital to cover A, B, and C, the bottom hospital to cover C, E, and F, and the leftmost hospital to cover A, C, and D.

<strong>Part 3.</strong><strong> </strong>In quarantine days, people get bored more than standing at home and many people spend time with their playing games for fun! In games played with playing cards, it is essential to mix the decks well. Let us mix the cards in the deck with code!

The deck of cards contains 52 cards which have 4 basic suits. These suits:

<strong>“Hearts”, “Diamonds”, “Clubs”, “Spades” </strong>

There are 13 faces belonging to each suit from 4 suits. These are:

<strong>“Ace”, “Deuce”, “Three”, “Four”, “Five”, “Six”, “Seven”, “Eight”, “Nine”, “Ten”, “Jack”, “Queen”, “King”</strong>




We should represent each card as a <strong>struct </strong>as follows:

<strong>struct card { </strong>const char *face; const char *suit;

<strong>}; </strong>

<strong> </strong>

<strong><u>The steps to be taken are listed below:</u> </strong>

<ul>

 <li>You must place strings in Card structures</li>

 <li>Cards in the deck must be replaced randomly so that the deck is shuffled.</li>

 <li>The elements of the mixed deck should be printed on the screen as in the format below.</li>

</ul>


