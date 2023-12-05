def planszowka():
    gracz1 = 0
    gracz2 = 0
    rzut = 0
    pozycja1 = 0
    pozycja2 = 0
    d = False
    plansza = 9
    przejscie1 = 0
    przejscie2 = 0
    zwyciezca = 0
    a = 2
    b = 9
    e = 3
    c = 7
    d = 9
    czekaj1 = 0
    czekaj2 = 0
    pulapka1 = False
    pulapka2 = False
    gratrwa = True


    while gratrwa == True:
        if czekaj1 == 0 and gratrwa == True:
            gracz1 = int(input("Gracz 1: Rzut kostka - 1, Koniec gry - 0: "))
            if gracz1 == 1:
                rzut = randint(1, 4)
                print("Wyrzuciles: ", rzut)
                if pulapka1 == True and rzut == 4:
                    pulapka1 = False
                elif pulapka1 == False:
                    pozycja1 += rzut
                    if pozycja1 <= plansza:
                        pozycja1 = pozycja1
                    elif (przejscie1 == 1 and pozycja1 >= plansza):
                        pozycja1 -= 10
                        przejscie1 -= 1
                    else:
                        pozycja1 -= 10
                        przejscie1 += 1
                    if przejscie1 == 0:
                        if pozycja1 == a:
                            print("Stanales na pole podrozy, idziesz 5 pol do przodu")
                            pozycja1 += 5
                        elif pozycja1 == b:
                            czekaj1 = randint(1, 3)
                            print("Czekaj: ", czekaj1, "kolejek")
                    elif przejscie1 == 1:
                        if pozycja1 == e:
                            pulapka1 = True
                            print("Wpadles w pulapke, wylosuj 4 oczka by uciec")
                        elif pozycja1 == c:
                            pozycja1 -= 7
                            przejscie1 -= 1
                        elif pozycja1 == d:
                            print("Gracz 1 WYGRAL")
                            gratrwa = False
                        elif (pozycja1 >= plansza):
                            pozycja1 -= 10
                            przejscie1 -= 1
                    pulapka1 = False
                elif (pulapka1 == True and rzut != 4):
                    pulapka1 = True
                    print("Nie udalo sie uciec z pulapki")
                print("Twoja pozycja to: ", przejscie1, pozycja1)
            else:
                return 0
        if gratrwa == True and czekaj2 == 0:
            gracz2 = int(input("Gracz 2: Rzut kostka - 1, koniec gry - 0: "))
            if gracz2 == 1:
                rzut = randint(1, 4)
                print("Wyrzuciles: ", rzut)
                if pulapka2 == True and rzut == 4:
                    pulapka2 = False
                elif pulapka2 == False:
                    pozycja2 += rzut
                    if pozycja2 <= plansza:
                        pozycja2 = pozycja2
                    elif (przejscie2 == 1 and pozycja2 >= plansza):
                        pozycja2 -= 10
                        przejscie2 -= 1
                    else:
                        pozycja2 -= 10
                        przejscie2 += 1
                    if przejscie2 == 0:
                        if pozycja2 == a:
                            print("Stanales na pole podrozy, idziesz 5 pol do przodu")
                            pozycja2 += 5
                        elif pozycja2 == b:
                            czekaj2 = randint(1, 3)
                            print("Czekasz: ", czekaj2, "tury")
                    elif przejscie2 == 1:
                        if pozycja2 == e:
                            pulapka2 = True
                            print("Wpadles w pulapke, wylosuj 4 oczka by uciec")
                        elif pozycja2 == c:
                            pozycja2 -= 7
                            przejscie2 -= 1
                        elif pozycja2 == d:
                            print("Gracz 2 WYGRAL")
                            gratrwa = False
                        elif (pozycja2 >= plansza):
                            pozycja2 -= 10
                            przejscie2 -= 1
                    pulapka2 = False
                elif (pulapka2 == True and rzut != 4):
                    pulapka2 = True
                    print("Nie udalo sie uciec z pulapki")
                print("Twoja pozycja to: ", przejscie2, pozycja2)
            else:
                return 0

        if czekaj1 > 0:
            czekaj1 -= 1
        if czekaj2 > 0:
            czekaj2 -= 1





planszowka()
