# Hello Micro:bit

## Czeg nauczysz się w tym rozdziale?

* Pokazywać tekst na swoim Micro:bicie
* Pętli

## Jak poprosić swojego Micro:bita, żeby powiedział ,,Hello!"

Twój Micro:bit może robić wiele róznych rzeczy, ale musisz mu wytlumaczyć, jak ma je robić. To tak jakbyś coś czytał, uczył się, i musiał ,,zaimportować" to, co przeczytałeś do mózgu.

A teraz czas, by otworzyć **Mu Editor** i wpisać kilka pierwszych linijek kodu:

```python
# This is a COMMENT
from microbit import display
```

STOP !

Pomyślmy o 2 pierwszych linijkach. Pierwsza linijka zaczyna się znakiem # i oznacza, że to, co jest za tym znakiem, jest komentarzem. Komentarz jest ,,niewidoczną" dla komputera częścią kodu, która jest przydatna tylko dla człowieka, bo tylko on ją widzi. Komentarz to taka notatka dla nas, albo dla innych ludzi, opisująca co dzieje się w danym fragmencie kodu.

Kolejna linijka jest już dużo ważniejsza. Prosimy w niej Pythona, żeby zimportował nam moduł __display__ z modułu microbit.

Czym jest moduł? Jest to paczka zawierająca różne małe programy i funkcje przygotowane przez kogoś, które możemy zaimportować do naszego programu i wykorzystać jak swoje (no prawie - wszystko zależy od licencji na której udostępniany jest dany modół). W uproszczeniu można powiedzieć, że moduł to poprostu przygotowany przez kogoś kod pythona, który możemy zaimportować i wykorzystać w swoim kodzie. 

Teraz możemy poprosić Micro:bita, by wyświetlił nam poniższy tekst:

```python
# To jest ZNÓW komentarz, moglibyśmy tu wpisać jakąś notatkę, albo cokolwiek innego, to widzi tylko człowiek
from microbit import display

display.show("Hello WpiszSwojeImie, I am your Micro:bit")
```

Co tym razem tutaj się dzieje?

Pierwsza i druga linijka nie są niczym nowym.

A o co chodzi w trzeciej linijce kodu?

Używamy fragmentu kodu, którym jest słowo show występujące wewnątrz kodu, fragemntu kodu, jakim jest słowo display.

Display po angielsku oznacza: wyświetl, lub też wyświetlacz, a słowo show = pokaż.

Spróbujmy teraz napisać podobny kod, ale z innym tekstem:

```python
from microbit import display

display.show("Helloo Poland!)
```

Skopiuj ten tekst do swojego edytora Mu i naciśnij Flash!

Mmmm.... czemu otrzymujemy Error, czyli błąd?

* Wykrzyknik na końcu zdania powoduje problem?
* Tekst jest za krótki?
* Potrzebujemy znaku " na końcu tekstu?
* Helloo (po angielsku powinno być ,,Hello") nie jest zapisane poprawnie?

## Ale czemu robić to tylko jeden raz?

W naszym kodzie przesłaliśmy Micro:bitowi tekt, który ma wyświetlać. Micro:bit wyświetla ten tekst tylko raz.
Co zrobić, jeśli chceby, by nasz Micro:bit wyświetlał nasz tekst cały czas? Musimy przedstawić Wam koncepcję pętli (pętla po angielsku to ,,loop").

Za pomocą ,,pętli" mówimy Micro:bitowi, żeby robił coś dopóki jakiś warunek jest spełniony.

W Pythonie mamy różne rodzaje pętli (czyli różne loops). Teraz zaczniemy używać jednej z tych pętli. Pętla ta nazywa się: while.

Komenda ,,while" jest komunikatem, który brzmi dokładnie tak: rób coś, dopóki warunek, czy też inaczej nasze założenia są prawdziwe.

```python
from microbit import display

while True:
  display.show("Hello Poland!")
```

Teraz spróbujmy w takim kodem:

```python
from microbit import display

while False:
  display.show("Hello Poland!")
```

Właśnie zmieniliśmy warunek na coś, co jest zawsze nieprawdziwe.

## Jaka jest różnica między tymi dwoma fragmentami kodu?

## Czemu komenda ,,display" nie jest napisana tuż pod słowem ,,while"?
