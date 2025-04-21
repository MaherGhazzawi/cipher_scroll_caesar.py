# 🏛️ Caesar Cipher – Geheimnisse in Buchstaben gehüllt

Ein kleines, aber kraftvolles Python-Tool, um Nachrichten zu **verschlüsseln** und **entschlüsseln** – inspiriert von Julius Caesar, dem Meister der einfachen, aber wirkungsvollen Kryptographie.

## 🔐 Was ist das?

Dieses Programm nutzt die klassische **Caesar-Verschlüsselung**, bei der Buchstaben im Alphabet um eine bestimmte Anzahl verschoben werden.  
Dabei entsteht ein geheimer Code, den nur jene mit dem richtigen "Shift" lesen können.

## 🚀 Features

- Verschlüsseln von Nachrichten mit einem beliebigen Shift
- Entschlüsseln von Nachrichten, wenn der Shift bekannt ist
- Unterstützung von Groß- und Kleinbuchstaben
- Alle anderen Zeichen bleiben unverändert

## 🧠 Wie funktioniert das?

Die Caesar-Verschlüsselung ist simpel:  
Ein `A` mit einem Shift von `3` wird zu `D`, ein `B` zu `E` – und so weiter.  
Bei `Z` springt es wieder auf `A` zurück (modulo 26).

## 🛠️ So funktioniert mein Programm : 
Ich habe zwei Hauptfunktionen implementiert:
Die erste ist encrypt_caesar, die einen Text und einen Verschiebungswert (shift) als Parameter verwendet.
Diese beiden – Text und Shift – bilden das Herzstück der Verschlüsselung.

Statt mit Listen zu arbeiten, habe ich gezielt die ord()-Funktion genutzt, um Zeichen in ihre ASCII-Werte zu verwandeln – und anschließend mit chr() wieder zurück.
So kann ich die Buchstaben präzise um den gewünschten Wert im Alphabet verschieben.

Mit isalpha() prüfe ich, ob die Eingabe tatsächlich Buchstaben enthält – damit der Nutzer echten Text eingibt und nicht etwa Zahlen oder Sonderzeichen, die nicht verschlüsselt werden sollen.

Ein while-Loop sorgt dafür, dass der Nutzer im Programm bleibt und beliebig viele Nachrichten ver- oder entschlüsseln kann – bis er es bewusst beendet. 

