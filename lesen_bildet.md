---
layout: default
title: Squeng AG
description: building the right thing right
---

{% include navigation.md %}

## Vom Nicht-Programmierer zum Software-Ingenieur

Auch in der Software-Entwicklung gilt, dass Übung den Meister macht. Und je nach schulischer Ausbildung und beruflicher Weiterbildung hat man vielleicht das Glück, unter Anleitung von Lehrern, Mentoren etc. eine Stufe nach der anderen zu erklimmen. Doch wie wird man autodidaktisch Software-Ingenieur, wenn man noch Software-Entwickler ist, Software-Entwickler, wenn man noch Programmierer ist, oder Programmierer, wenn man noch Nicht-Programmierer ist? *[Thereʼs a book for that!](https://squeng.wordpress.com/2019/03/17/nicht-nur-lesen-bildet/)*

---

Bezeichnen Programmierer, Software-Entwickler und Software-Ingenieur nicht das gleiche? Nein! In den Worten von [Jacobson *et al.*](https://dl.acm.org/doi/book/10.1145/3277669):

- „*Programming* stands for the work related to implementation or coding of source code.“
- „*Software development* is the larger process which, apart from programming, includes working with requirements, design, test, etc.“
- „«*Software engineering* combines engineering techniques with software development practices» (from Wikipedia). Moving from development to engineering means more reliance on science and less on craft, which typically manifests itself in some form of description of a designated way of working and higher-level automation of work. This allows for repeatability and consistency from project to project. Engineering also means that teams, for example, learn as they work and continuously improve their way of working. Thus, stated in simple terms, *software engineering is bringing engineering discipline to software development*.“

---

Bücher zu den Stichworten "programming", "software development" und "software engineering" gibt es wie Sand am Meer. [Viele sind sehr gut oder wenigstens gut, nicht wenige sind jedoch schlecht oder gar sehr schlecht.](https://www.squeng.com/stapel) Man bräuchte also nicht viel Pech, um als Anfänger an ein schlechtes Buch des entsprechenden Themas zu geraten, was die Gefahr bärge, den Stoff gar nicht zu verstehen und deshalb an sich selbst zu zweifeln oder ihn falsch zu verstehen und das falsch Gelernte dereinst mühsam umlernen zu müssen.

### Vom Nicht-Programmierer zum Programmierer

---

Kindern empfehle ich, gemeinsam mit ihren Eltern mit [Scratch](https://scratch.mit.edu/) programmieren zu lernen. Den Eltern lege ich ausserdem [Lifelong Kindergarten](https://mitpress.mit.edu/9780262536134/) nahe als motivierenden & spannenden Lieferanten von Hintergrundinformationen.

---

Es gibt zig Programmiersprachen. Selbst wenn man sich auf diejenigen beschränkt, welche eine gewisse Verbreitung in der Software-Industrie geniessen, kommt man noch auf [ein paar Dutzend](https://survey.stackoverflow.co/2022/#most-popular-technologies-language-prof). Es wäre also illusorisch, alle praxis-relevanten Programmiersprachen erlernen zu wollen; genauso illusorisch wäre es zu glauben, als professioneller Programmierer nur eine beherrschen zu müssen. Deshalb ist die Programmiersprache, mit der man programmieren lernt, sekundär. Viel wichtiger ist es, ein starkes Fundament zu legen; die zukünftig liebste (oder vermeintlich beste) Programmiersprache erlernt sich dann relativ leicht, wenn das Fundament stark ist.

Bücher, die eine Einführung in die Programmierung versprechen, gibt es zumindest in Deutsch gar nicht so viele. ([Amazon listet nur etwa 500 dazu auf.](https://www.amazon.de/s?k=einf%C3%BChrung+in+die+programmierung)) Darunter sind nichtsdestotrotz noch zu viele, welche didaktisch einiges zu wünschen übrig lassen. Beispielsweise werden Spracheigenschaften und -konzepte nicht selten rein mechanistisch beschrieben, ohne wirklich auf ihren Sinn & Zweck einzugehen. (Man stelle sich vor, dass im Deutschunterricht lieblos erwähnt wird, dass es Konjunktiv I und Konjunktiv II gibt sowie zur Illustration ein paar Konjugationstabellen gezeigt werden, ohne jemals darauf einzugehen, wann & wie Konjunktiv I resp. II korrekt verwendet werden.)

Dabei habe ich grundsätzlich nichts gegen Bücher, die kurz & bündig eine Programmier*sprache* einführen. [Horstmanns *… for the Impatient*-Bücher](https://horstmann.com/) z.B. mag ich sehr; er setzt jedoch auch klipp & klar Programmierkenntnisse voraus.

**Auf jeden Fall kann ich [*Introduction to Programming and Problem-Solving Using Scala*](https://www.routledge.com/Introduction-to-Programming-and-Problem-Solving-Using-Scala/Lewis-Lacher/p/book/9781498730952) empfehlen und zwar die Kapitel 1 bis 10 sowie 13, 15 und 16.** Hinweise auf weitere sehr gute Bücher, insbesondere deutschsprachige, nehme [ich](/ingenieure) sehr gerne entgegen. Und da es bei aller Liebe zur Abstraktion hilft, etwas über das Innenleben eines Computers (Hardware, Systemsoftware etc.) zu verstehen, hoffe ich, im Frühling ergänzend auch noch [*Computer verstehen*](https://www.amazon.de/Computer-verstehen-Streifzug-Innenleben-Computers/dp/3658403136/) empfehlen zu können.

### Vom Programmierer zum Software-Entwickler

#### Security as a Forethought

Heutzutage wäre es unverantwortlich, Software ohne Rücksicht auf ihre Sicherheit zu entwickeln. Zwar muss die Betreiberin der Software sich mit Fragen des [Datenschutzes](https://dpunkt.de/produkt/cloud-computing-nach-der-datenschutz-grundverordnung/) und der [Privatheit](http://williamstallings.com/Privacy/) auseinandersetzen und ihre Politik (gegenüber Kunden, Benutzern etc.) festlegen, welche teils mit Sicherheitsmechanismen durchgesetzt wird. Doch Softwaresicherheit (nicht zu verwechseln mit Sicherheitssoftware) ist die Verantwortung jeder einzelnen Software-Entwicklerin und jedes einzelnen Software-Entwicklers.

![eine meiner Unterrichtsfolien aus dem Jahr 2015](SecSWvsSWsec.png)

**[*Designing Secure Software*](https://nostarch.com/designing-secure-software) ist Pflichtlektüre für alle (angehenden) Software-Entwickler.** Darüber hinaus ist es unabdingbar, sich auch mit Softwaresicherheit in Bezug auf die eingesetzte [Programmiersprache](https://wiki.sei.cmu.edu/confluence/display/seccode/) (z.B. [Java](https://www.mhprofessional.com/iron-clad-java-9780071835886-usa)) sowie aller anderen Technologien (z.B. [Web](https://nostarch.com/websecurity)) auseinanderzusetzen.

#### Objektorientierte Programmierung

Heutzutage kommt man typischerweise schon in Berührung mit objektorientierter Programmierung (OOP), wenn man programmieren lernt. Auch [das oben empfohlene Buch](https://www.routledge.com/Introduction-to-Programming-and-Problem-Solving-Using-Scala/Lewis-Lacher/p/book/9781498730952) sowie [sein zweiter Band](https://www.routledge.com/Object-Orientation-Abstraction-and-Data-Structures-Using-Scala/Lewis-Lacher/p/book/9781498732161) bieten eine Einführung in OOP. In den letzten Jahrzehnten hat sich OOP auf breiter Front durchgesetzt, so dass Software-Entwickler sich auch damit auseinandersetzen sollten, wenn sie in erster Linie noch mit einer nicht-objektorientierten Programmiersprache wie z.B. [C](https://www.manning.com/books/modern-c) strukturiert programmieren.

**Mein Lieblingsbuch zu OOP ist [*Objektorientierte Programmierung in Oberon-2*](https://link.springer.com/book/10.1007/978-3-642-58985-0).** Da das Buch jedoch schon etwa ein Vierteljahrhundert auf dem Buckel hat, werde ich in nächster Zeit prüfen, ob [*Objektorientierte Programmierung*](https://www.rheinwerk-verlag.de/objektorientierte-programmierung-das-umfassende-handbuch/) (m)eine Empfehlung wert ist; *stay tuned!*

#### Funktionale Programmierung

Etwa 2003 hat mich [Sebastian Mödersheim](https://www.imm.dtu.dk/~samo/) auf die Vorzüge der funktionalen Programmierung hingewiesen. Als erfahrener [Haskell](https://www.haskell.org/)-Programmierer wusste er, wovon er spricht. Ich hingegen masste mir mit meinen sage & schreibe fast zwei Jahren Industrie-Erfahrung das Urteil an, dass funktionale Programmierung vielleicht für Theoretiker interessant sei, aber doch nicht relevant für Praktiker. Sebastians Hinweis auf [*Beating the Averages*](http://paulgraham.com/avg.html) änderte noch nichts an meiner Fehleinschätzung. (Erst Jahre später, nachdem ich [Paul Graham](http://paulgraham.com/) via [Y Combinator](https://www.ycombinator.com/) [nochmals] kennengelernt und begonnen hatte, [seine Essays](http://paulgraham.com/articles.html) zu lesen, realisierte ich, dass ich doch schon mal etwas von ihm gelesen, aber noch viel zu wenig ernst genommen hatte …)

Heute finden sich glücklicherweise viele Konzepte aus rein funktionalen Programmiersprachen in modernen, hybriden Programmiersprachen. Müsste man sie als Software-Entwickler wieder hergeben, würde man sie schmerzlich vermissen. Umgekehrt kann man immens davon profitieren und grosse Freude daran haben, wenn man sich etwas tiefer mit ihnen auseinandersetzt (und einmal mehr nicht nur mit ihrer Mechanik). Deshalb ist Teil I von **[*Functional and Concurrent Programming*](https://www.fcpbook.org/) Pflicht (und [*Functional Programming in Scala*](https://www.manning.com/books/functional-programming-in-scala-second-edition) Kür)**.

#### Entwurf & Architektur

Wenn sie nicht gerade aus der Feder der gleichen Autoren stammen, findet man kaum zwei Definitionen von Software-Architektur resp. Stellenbeschriebe von Software-Architekten, welche sich einig sind. Im Software-Kontext wird sogar unterschieden zwischen "entwerfen" (*to design*), [das als Verb existiert](https://www.merriam-webster.com/dictionary/design), und "architekten" (*to architect*), [**das auch im Englischen nicht als Verb existiert**](https://www.merriam-webster.com/dictionary/architect) …

Im Geiste von KISS (Keep it simple, Squeng!) würde meine Definition eigentlich lauten: Software-Architekten entwerfen Software resp. Software-Architektur ist das Resultat von Software-Entwurf. Anders ausgedrückt würde ich Designer und Architekt im Kontext von Software als synonym betrachten. (Deshalb riskiere ich auch kein 🤯 bei der Feststellung, dass z.B. Innenarchitektur resp. Innenarchitekt mit [*interior design*](https://de.pons.com/%C3%BCbersetzung/deutsch-englisch/Innenarchitektur) resp. [*interior designer*](https://de.pons.com/%C3%BCbersetzung/deutsch-englisch/Innenarchitekt) übersetzt wird.)

Konsequenterweise dürfte ich auch nicht unterschieden zwischen *design patterns* und *architecture patterns*, aber muss halt akzeptieren, dass damit in der Praxis verschiedene Dimensionen impliziert werden. (Vor Jahrzehnten hatte auch ich mal *"architecture is high-level design and design is low-level architecture"* geschrieben.) Und dass verschiedene Dimensionen unterschieden werden, ist tatsächlich sinnvoll, so wie auch in der Nicht-Software-Architektur z.B. zwischen Stadtarchitekten und Innenarchitekten unterschieden wird. Deshalb folgt nun eine Liste von lesenswerten Büchern:
- "Was sind meine Verantwortlichkeiten, wenn ich als Software-Entwickler die Software-Architekten-Rolle spiele?" [*Software Architecture for Developers*](https://leanpub.com/software-architecture-for-developers)
- "System-Architektur: Entwerfe ich einen modularen Monolithen oder eine Menge von Microservices?" [*Software Architecture Patterns*](https://www.oreilly.com/library/view/software-architecture-patterns/9781098134280/)
- "Applikations-Architektur: Wie entwerfe ich ein Modul oder einen Microservice?" (*Spoiler alert!* Die Antwort lautet [clean](https://blog.cleancoder.com/uncle-bob/2012/08/13/the-clean-architecture.html)/[hexagonal](https://alistair.cockburn.us/hexagonal-architecture/)/[onion](https://jeffreypalermo.com/tag/onion-architecture/).) [*Domain Modeling Made Functional*](https://pragprog.com/titles/swdddf/domain-modeling-made-functional/)
- "Wie entwerfe ich Funktionen oder Klassen eines Moduls oder eines Microservices?" [*Adaptive Code*](https://www.microsoftpressstore.com/store/adaptive-code-agile-coding-with-design-patterns-and-9781509302581) (eine dritte Auflage scheint in Vorbereitung zu sein)

#### Testen

Zwar war ich mir der Wichtigkeit des Testens schon immer bewusst, dennoch musste man mich zwischen 25 und 45 zum Testen verknurren. Zwischen 45 und 65 will ich es viel besser machen, zumal ich mittlerweile grossen Gefallen am Thema gefunden habe, nicht zuletzt, weil Testen nicht nur die Implementation, sondern auch den Entwurf von Software unterstützt. **Allerspätestens seit [*Effective Software Testing*](https://www.manning.com/books/effective-software-testing) hätte ich ohnehin keine Ausrede mehr.**

FORTSETZUNG FOLGT …

### Vom Software-Entwickler zum Software-Ingenieur

FORTSETZUNG FOLGT …

<!--
reminders to myself:

- [Continuous Delivery Pipelines](https://leanpub.com/cd-pipelines)
- [Engineering Management for the Rest of Us](https://www.engmanagement.dev/)
- [Product Management in Practice](https://www.oreilly.com/library/view/product-management-in/9781098119720/)
- [Code](https://www.microsoftpressstore.com/store/code-the-hidden-language-of-computer-hardware-and-software-9780137909100)
-->
