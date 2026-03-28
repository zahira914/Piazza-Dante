<!DOCTYPE html>
<html lang="it">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Piazza Dante - Il Manoscritto</title>
    <link href="https://fonts.googleapis.com/css2?family=MedievalSharp&family=Spectral:italic,wght@0,400;0,700&display=swap" rel="stylesheet">
    <style>
        :root {
            --pergamena: #f2e3c9;
            --pelle: #3e2723;
            --inchiostro: #1a0f0a;
            --oro: #a67c00;
            --rosso-antico: #7e0000;
        }

        body {
            background-color: var(--pelle);
            background-image: url('https://www.transparenttextures.com/patterns/leather.png');
            color: var(--inchiostro);
            font-family: 'Spectral', serif;
            margin: 0;
            padding: 20px;
            display: flex;
            justify-content: center;
        }

        .manoscritto {
            background-color: var(--pergamena);
            background-image: url('https://www.transparenttextures.com/patterns/paper-fibers.png');
            max-width: 850px;
            width: 100%;
            padding: 50px;
            box-shadow: 0 0 40px rgba(0,0,0,0.8);
            border: 2px solid #8d6e63;
            position: relative;
        }

        .manoscritto::before {
            content: "";
            position: absolute;
            top: 15px; left: 15px; right: 15px; bottom: 15px;
            border: 1px solid var(--oro);
            pointer-events: none;
        }

        header {
            text-align: center;
            border-bottom: 3px double var(--rosso-antico);
            margin-bottom: 40px;
            padding-bottom: 20px;
        }

        h1 {
            font-family: 'MedievalSharp', cursive;
            font-size: 3.5rem;
            color: var(--rosso-antico);
            margin: 0;
            text-shadow: 1px 1px 2px rgba(0,0,0,0.2);
        }

        .img-centrale {
            text-align: center;
            margin: 30px 0;
        }

        /* Stile per l'immagine web di Dante */
        .dante-img {
            max-width: 100%;
            width: 550px;
            height: auto;
            border: 8px solid #fff;
            box-shadow: 0 5px 15px rgba(0,0,0,0.3);
            border-image: linear-gradient(to bottom, var(--oro), #5d4037) 1;
        }

        /* Stile per le immagini della presentazione */
        .foto-progetto {
            max-width: 90%;
            height: auto;
            border: 4px solid var(--inchiostro);
            border-radius: 5px;
            margin: 20px auto;
            display: block;
            box-shadow: 3px 3px 10px rgba(0,0,0,0.4);
            background-color: #e0d4b8; /* Colore di sfondo se manca l'immagine */
            text-align: center;
            line-height: 200px;
            font-style: italic;
            color: #666;
        }

        nav {
            text-align: center;
            margin-bottom: 40px;
            font-family: 'MedievalSharp', cursive;
        }

        nav a {
            color: var(--inchiostro);
            text-decoration: none;
            margin: 0 10px;
            font-size: 1.1rem;
            border-bottom: 1px transparent;
        }

        nav a:hover {
            color: var(--rosso-antico);
            border-bottom: 1px solid var(--rosso-antico);
        }

        h2 {
            font-family: 'MedievalSharp', cursive;
            color: var(--rosso-antico);
            border-bottom: 1px solid var(--oro);
            padding-bottom: 5px;
        }

        .testo-antico {
            font-size: 1.2rem;
            line-height: 1.7;
            text-align: justify;
        }

        .capolettera {
            float: left;
            font-family: 'MedievalSharp', cursive;
            font-size: 4rem;
            line-height: 1;
            padding-right: 10px;
            color: var(--rosso-antico);
        }

        .box-materiali {
            background: rgba(166, 124, 0, 0.1);
            border: 1px dashed var(--inchiostro);
            padding: 15px;
            margin-top: 20px;
            font-style: italic;
        }
    </style>
</head>
<body>

<div class="manoscritto">
    <header>
        <h1>Piazza Dante</h1>
        <p><i>Chronicon del Progetto Artistico Scolastico</i></p>
    </header>

    <nav>
        <a href="#dante">Il Poeta</a> | 
        <a href="#trittico">Il Trittico</a> | 
        <a href="#beatrice">Beatrice</a> | 
        <a href="#ignavia">Riflessione</a>
    </nav>

    <div class="img-centrale">
        <img src="https://www.marcelloveneziani.com/wp-content/uploads/2021/03/32-620x350.jpg" 
             alt="Ritratto di Dante Alighieri" 
             class="dante-img">
    </div>

    <section id="dante">
        <h2>Il Ritratto del Poeta</h2>
        <p class="testo-antico">
            <span class="capolettera">I</span>n un angolo della nostra scuola è nata <b>Piazza Dante</b>, uno spazio speciale dove gli studenti possono ammirare i ritratti del Sommo Poeta e delle visioni celestiali.
            Dante Alighieri (1265-1321) è qui rappresentato con uno sguardo che invita alla riflessione. 
        </p>
    </section>

    <section id="trittico">
        <h2>Il Trittico: Dante - Paradiso - Beatrice</h2>
        
        <img src="trittico.jpg" alt="[Inserisci l'immagine del Trittico salvata come trittico.jpg]" class="foto-progetto">

        <p class="testo-antico">
            Il trittico celebra il settecentenario della morte di Dante. L'idea di dare nuova vita a oggetti eterogenei destinati allo smaltimento ha ispirato la creazione di un'opera straordinaria.
        </p>

        <img src="mia_immagine.jpg" alt="[Inserisci l'immagine salvata come mia_immagine.jpg]" class="foto-progetto">
        
    </section>

    <section id="beatrice">
        <h2>Beatrice Portinari</h2>
        
        <img src="beatrice.jpg" alt="[Inserisci l'immagine di Beatrice salvata come beatrice.jpg]" class="foto-progetto">

        <p class="testo-antico">
            Nata a Firenze nel 1266 e morta nel 1290, è una figura centrale nella cultura medievale, simbolo di purezza, gentilezza e spiritualità. Nel ritratto, Beatrice guarda verso Dante, circondata da fiori, farfalle e luce policroma.
        </p>
        <div class="box-materiali">
            <b>Materiali utilizzati:</b> Capsule del caffè, bottoni, carta, stickers, cannucce e altri materiali di recupero.
        </div>
    </section>

    <section id="ignavia">
        <h2>Ignavia Ieri e Oggi</h2>
        <p class="testo-antico">
            Dante condanna gli ignavi, coloro che non scelgono, non prendono posizione e restano spettatori. Oggi l'ignavia assume forme nuove: indifferenza e passività digitale. Questo progetto ci invita a non restare a guardare.
        </p>
    </section>

</div>

</body>
</html>
