Puoi [saltare questa sezione](http://tutorial.djangogirls.org/en/installation/#install-python) se non utilizzi un Chromebook. L'installazione su Chromebook segue una procedura un po' diversa. Il resto delle istruzioni di installazione puó essere ignorato.

### Cloud IDE (PaizaCloud Cloud IDE, AWS Cloud9)

Cloud IDE è uno strumento che mette a disposizione un editor di codice e l'accesso ad un computer virtuale su cui installare, scrivere ed eseguire il software. In questo tutorial, Cloud IDE avrà la funzione di un *computer locale*. Digiterai i comandi sull'interfaccia di un terminale, come le tue compagne di corso che utilizzano OS X, Ubuntu o Windows, ma il tuo terminale sarà connesso a un computer remoto che Cloud IDE ha creato per te. Di seguito trovi le istruzioni per i cloud IDE (PaizaCloud Cloud IDE, AWS Cloud9). Puoi selezionare uno dei Cloud IDE e seguire le relative istruzioni.

#### PaizaCloud Cloud IDE

1. Andare su [PaizaCloud Cloud IDE](https://paiza.cloud/)
2. Creare un account
3. Cliccare su *New Server*
4. Fare click sul pulsante Terminal (sul lato sinistro della finestra)

Ora dovresti vedere un'interfaccia con una barra laterale e dei pulsanti sulla sinistra. Fai click sul pulante "Terminal" per aprire la finestra del terminale con il prompt, così:

{% filename %}Terminal{% endfilename %}

    $
    

Il terminale su PaizaCloud Cloud IDE è pronto a ricevere istruzioni. Puoi ridimensionare la finestra o renderla un po' più più grande.

#### AWS Cloud9

1. Andare su [AWS Cloud9](https://aws.amazon.com/cloud9/)
2. Creare un account
3. Fare click su *Create Environment*

Ora dovresti vedere un'interfaccia con una barra laterale, una finestra principale con del testo e una finestra più piccola in basso che assomiglia a questa:

{% filename %}bash{% endfilename %}

    yourusername:~/workspace $
    

Questa finestra in basso è il tuo terminale. Puoi usare il terminale per inviare istuzioni al computer remoto Cloud9. Puoi cambiare le dimesioni della finestra e renderla più grande.

### Ambiente virtuale

Un ambiente virtuale (in inglese virtual environment, abbreviato spesso in virtualenv) è come una scatola privata in cui possiamo mettere del codice per un progetto su cui stiamo lavorando. Lo usiamo per tenere separate le diverse parti di codice che ci servono per i nostri progetti, in modo da non creare confusione tra un progetto e l'altro.

Nel terminale, in fondo all'interfaccia Cloud9, esegui il seguente codice:

{% filename %}Cloud 9{% endfilename %}

    sudo apt update 
    sudo apt install python3.6-venv
    

Se non funziona, chiedi aiuto al tuo coach.

Poi esegui:

{% filename %}Cloud 9{% endfilename %}

    mkdir djangogirls 
    cd djangogirls
    python3.6 -mvenv myvenv 
    source myvenv/bin/activate 
    pip install django~={{ book.django_version }}
    

(nota che nell'ultima linea abbiamo usato una tilde seguita dal segno 'uguale':`~=`).

### GitHub

Crea un account [GitHub](https://github.com).

### PythonAnywhere

Il tutorial Django Girls comprende una sezione della cosiddetta distribuzione, che consiste nel prendere il codice della tua nuova applicazione web e spostarlo su un computer pubblicamente accessibile (chiamato server) in modo che altre persone possano vedere il tuo lavoro.

Questa parte risulterà un po' strana se segui il tutorial su un Chromebook, in quanto stiamo già usando un computer collegato a Internet (a differenza, ad esempio, di un laptop). Tuttavia è importante, se pensiamo al nostro Cloud9 come a uno spazio dove abbiamo il nostro "lavoro in corso", e a Python Anywhere come a uno spazio dove mostrare i nostri programmi quando sono più completi.

Quindi, crea un nuovo account Python Anywhere su [www.pythonanywhere.com](https://www.pythonanywhere.com).