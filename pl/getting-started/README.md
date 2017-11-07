# Pierwsze kroki

## Instalowanie Go

Mac lub Linux

Zawsze ściągaj i używaj niezmodyfikowanych wersji z golang.org zamiast wersji z homebrew, apt-get, yum etc. Te drugie mogą być zepsute, albo co gorsze - zmodyfikowane przez kogoś.

Ustaw GOPATH w .bashrc, .bash\_profile, .zshrc etc:

```
export GOPATH=$HOME/go
```

Dodaj binarki Go \(kompilator i narzędzia\) do swojego PATH:

```
export PATH=$PATH:/usr/local/go/bin
```

Wyloguj i zaloguj się ponownie lub po prostu wpisz:

```
$ source .bashrc
```

by zastosować zmiany.

## Instalowanie Go

Windows

Ściągnij i zainstaluj Go - użyj instalatorów MSI z oficjalnej strony.

Ustaw GOPATH w Zmiennych Środowiskowych:

```
GOPATH=%userdir%/go
```

Dodaj binarki Go \(kompilator i narzędzia\) do swojego PATH:

```
%userdir%/go/bin    
```

## Zweryfikuj instalację

Z wiersza poleceń:

```
go version
```

Powinieneś zobaczyć coś jak:

```
go version 1.8 linux/amd64
```

## Edytowanie kodu Go

Popularne edytory Go:

vim i neovim z pluginem vim-go

emacs z go-mode.el

Visual Studio Code z vscode-go \(działa z debuggerem!\)

Atom z go-plus

IntelliJ IDEA z Go plugin

## The Go Playground

Nawet jeżeli nie masz skonfigurowanego edytora, wciąż możesz pobawić się Go ze swojej przeglądarki.

[The Go Playground](https://play.golang.org)

Go Playground to serwis, który działa na serwerach golang.org. Otrzymuje on kod źródłowy Go, kompiluje i wykonuje go w kontrolowanym środowisku \("sandbox"\), a następnie zwraca wynik.

## Ograniczenia Go Playground

Są pewne ograniczenia, które dotyczą rzeczy które mogą być wykonywane w Playground:

Playground może używać większość z biblioteki standardowej, z małymi wyjątkami. Jedyna komunikacja Playground posiada do świata zewnętrznego to standard output i standard error.

W Playground czas zaczyna się o 22:00:00 UTC, 10.11.2009 r. \(znaczenie tej daty pozostawiamy do jako ćwiczenie dla czytelnika\). Sprawia to, że łatwiej jest cache'ować programy dając wynik, który jest deterministyczny.

Istnieją również limity dotyczące czasu wykonania programu, użycia procesora i pamięci.

Podsumowując: Brak IO na systemie plików, nic użytecznego z czasem czy datami, nie można używać żadnych bibliotek zewnętrznych.

## The Go Playground

Nawet z tymi wszystkimi ograniczeniami, Go playground jest kochany przez społeczność Go - jest to świetne miejsce do dzielenia się kodem, nawet jeżeli nie da się go uruchomić czy skompilować. Możesz wprowadzić kod i kliknąć przycisk "SHARE", który da Ci link do tego kodu.

Spróbuj teraz z tym linkiem:

[Hello World!](https://play.golang.org/p/992fMmkkxr)

## Komenda Go

All of your command line interaction with Go will be through the `go` command.

Wszystkie interakcje z wierszem poleceń dotyczącym Go będzie poprzez słowo `go` .

Kilka przykładowych i częstych komend:

```
go build some/package
go run main.go
go test some/package
go get github.com/someone/package
go install some/package
```

## Ćwiczenie

From your command prompt type `go` and hit return to see the various tools the `go` command implements.  Try some like:

Wpisz `go` w Twoim wierszu poleceń i naciśnij enter by zobaczyć różne narzędzia, które są dostępne. Spróbuj niektóre, jak:

```
go env
go list
go version
```

## Ściągnij materiały

Użyj komendy `go` z Twojego wiersza poleceń by ściągnąć materiały i ćwiczenia dla tej książki:

```
go get github.com/thewondertwins/learngo
```



