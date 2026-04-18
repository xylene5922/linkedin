LinkedIn : Browsergate pour Firefox, en moins pire
===================================================

Ne croyez pas que, parce que vous êtes sur Firefox, Microsoft ne s’est pas donné les moyens de récupérer les informations autour de votre navigateur.  D’ailleurs, rien de plus simple sous n’importe quel navigateur – y compris Firefox – à utiliser l’objet navigator et ses méthodes intrusives ! Au moment de la connexion à la page d’accueil de LinkedIn, j’ai tenu à ouvrir le plus gros script pour y voir les méthodes utilisées par Microsoft pour récupérer les informations relatives à l’environnement matériel du navigateur (RAM, processeurs, etc).


* * *

Tester la perméabilité de votre navigateur au BrowserGate
-----------

J’ai créé une page,  reprenant le code du script le plus lourd. Vous pouvez la consulter quel que soit le navigateur  https://dsfc.net/browsergate.html utilisé. Il est assez amusant de voir que Chromium renvoie beaucoup plus d’informations que Firefox. Le nombre de cœurs remonté à partir du navigateur de la fondation Mozilla est faux. La quantité de mémoire utilisée n’est pas remontée par Firefox.

Je n’ai pas fait le test avec Google Chrome. Jamais, au grand jamais, je ne ferai cette folie d’installer Google Chrome sur ma machine de production. Il faut d’ailleurs en avoir un sérieux coup dans le caisson de la part d’informaticiens et autres pseudo-experts en sécurité pour utiliser cette bouse de Google Chrome, n’est-ce pas ?

Chromium
<img width="928" height="862" alt="Chromium" src="https://github.com/user-attachments/assets/936b7a1e-b1db-4ee0-abbf-a5fcf01090a8" />

Firefox
<img width="1117" height="877" alt="Firefox" src="https://github.com/user-attachments/assets/d96c81d5-7c8b-4876-ba7b-0164fb8afc46" />



La résistance de Firefox au fingerprinting
------------------------------------------

Dans le configurateur de Firefox accessible en tapant about:config dans la barre d’adresses, vous pouvez renforcer le navigateur face à la prise d’empreintes. Ce n’est pas le cas dans Chromium. L’avantage de Firefox est de changer l’empreinte Canvas qui identifie de manière unique votre navigateur. Vive Firefox !

<img width="1003" height="684" alt="fingerprinting" src="https://github.com/user-attachments/assets/a1f496b9-6605-48ba-8775-7a6f6bdb1552" />




