#include <iostream>
#include <sstream>

int main() { //zadanie usu(etap 1) 100p/100p
    std::string wejscie; // format: a b
    std::getline(std::cin, wejscie); // pobierz wejscie i przenies do zmiennej

    int pozycja = wejscie.find(" "); // znajdź pozycje spacji w wejsciu

    long long liczba_a;



    std::stringstream stringstream(wejscie.substr(0, pozycja)); //konwersja string'a do long long
    stringstream >> liczba_a;

    long long liczba_b;

    std::stringstream sstr(wejscie.substr(pozycja, wejscie.size())); //konwersja string'a do long long
    sstr >> liczba_b;

    long int ilosc_liczb_parz = (liczba_b - liczba_a)/2;
    long int ilosc_liczb_nie_parz = (liczba_b - liczba_a)/2;

    if(liczba_a % 2 == 0 && liczba_b % 2 == 0)
    {
        ilosc_liczb_parz++;
    }
    else if(liczba_a % 2 != 0 && liczba_b % 2 != 0)
    {
        ilosc_liczb_nie_parz++;
    }
    else
    {
        ilosc_liczb_parz++;
        ilosc_liczb_nie_parz++;
    } //Obliczanie ilosci liczb parzystych/nieparzystych

    long int wynik = 0;

    if(ilosc_liczb_nie_parz % 2 == 0)
    {
        wynik += ilosc_liczb_nie_parz;
    }
    else
    {
        wynik += ilosc_liczb_nie_parz - 1;
    }

    if(ilosc_liczb_parz % 2 == 0)
    {
        wynik += ilosc_liczb_parz;
    }
    else
    {
        wynik += ilosc_liczb_parz - 1;
    } //obliczanie wyniku

    std::cout << wynik;
}
