<!DOCTYPE html>
<html lang="es">
<head>

<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>BRASI MODS</title>

<style>

* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

body {
    background: #000;
    color: white;
    font-family: Arial, sans-serif;
    min-height: 100vh;
}

.oculto {
    display: none !important;
}

.pantalla {
    min-height: 100vh;
    padding: 25px 18px;
}

/* FONDO PAYASO */

#acceso {
    background:
        linear-gradient(
            rgba(0,0,0,0.62),
            rgba(0,0,0,0.86)
        ),
        url("payaso.jpg") center center / cover no-repeat;
}

/* LOGO */

.logo {
    text-align: center;
    padding-top: 45px;
}

.logo h1 {
    font-size: 45px;
    letter-spacing: 5px;
    text-shadow: 0 0 18px rgba(255,212,71,0.35);
}

.logo h2 {
    color: #ffd447;
    letter-spacing: 8px;
    font-size: 18px;
    margin-top: 3px;
}

.logo p {
    color: #aaa;
    font-size: 11px;
    letter-spacing: 2px;
    margin-top: 12px;
}

/* TARJETA */

.tarjeta {
    width: 100%;
    max-width: 480px;
    margin: 35px auto;
    padding: 23px;

    background: rgba(16,16,16,0.92);
    border: 1px solid #292929;
    border-radius: 20px;

    backdrop-filter: blur(5px);
}

/* KEY */

.key-titulo {
    text-align: center;
    color: #fff;
    font-size: 16px;
    font-weight: bold;
    margin-bottom: 15px;
}

/* INPUT */

input,
select {
    width: 100%;
    height: 52px;

    background: #080808;
    color: white;

    border: 1px solid #292929;
    border-radius: 13px;

    padding: 0 14px;

    outline: none;

    margin-bottom: 15px;
}

input:focus,
select:focus {
    border-color: #d8a72d;
}

/* BOTONES */

button {
    border: none;
    cursor: pointer;

    font-family: Arial, sans-serif;
    font-weight: bold;
}

.boton {
    width: 100%;
    height: 54px;

    border-radius: 14px;

    background: #d8a72d;
    color: #000;

    font-size: 13px;
}

.entrar {
    background: #00e676;
    margin-top: 4px;
}

#error {
    text-align: center;
    color: #ff4444;
    font-size: 12px;
    margin-top: 12px;
    min-height: 18px;
}

/* GENERADOR */

header {
    max-width: 600px;
    margin: auto;

    display: flex;
    justify-content: space-between;
    align-items: center;

    margin-bottom: 28px;
}

header strong {
    display: block;
    font-size: 20px;
}

header small {
    color: #d8a72d;
    font-size: 10px;
}

.volver {
    width: 45px;
    height: 45px;

    border-radius: 13px;

    background: #151515;
    color: white;

    font-size: 22px;
}

main {
    width: 100%;
    max-width: 600px;
    margin: auto;
}

main h1 {
    font-size: 27px;
}

.descripcion {
    color: #777;
    font-size: 12px;
    margin: 7px 0 20px;
}

/* PESTAÑAS */

.pestanas {
    display: grid;
    grid-template-columns: 1fr 1fr;

    gap: 7px;

    padding: 5px;

    background: #0b0b0b;

    border: 1px solid #222;

    border-radius: 16px;

    margin-bottom: 17px;
}

.pestana {
    height: 47px;

    border-radius: 12px;

    background: transparent;

    color: #777;
}

.pestana.activa {
    background: #d8a72d;
    color: #000;
}

/* PANEL */

.panel {
    background: #101010;

    border: 1px solid #222;

    border-radius: 19px;

    padding: 20px;
}

label {
    display: block;

    color: #aaa;

    font-size: 10px;

    font-weight: bold;

    margin-bottom: 8px;
}

/* GENERAR */

.generar {
    width: 100%;

    height: 55px;

    border-radius: 14px;

    background: #00e676;

    color: #001b0c;

    margin-top: 5px;
}

/* RESTAURAR */

.restaurar {
    width: 100%;

    height: 50px;

    border-radius: 14px;

    background: #222;

    color: #ddd;

    margin-top: 10px;

    border: 1px solid #333;
}

.restaurar:active {
    transform: scale(.98);
}

/* NOTA */

.nota {
    padding: 13px;

    margin-bottom: 15px;

    background: #18140a;

    border: 1px solid #493c16;

    border-radius: 12px;

    color: #bbb;

    font-size: 11px;
}

/* RESULTADO */

.resultado {
    margin-top: 17px;

    padding: 18px;

    background: #0e0e0e;

    border: 1px solid #292929;

    border-radius: 18px;
}

.titulo-resultado {
    color: #d8a72d;

    font-weight: bold;

    margin-bottom: 12px;
}

.linea {
    display: flex;

    justify-content: space-between;

    padding: 10px 0;

    border-bottom: 1px solid #1d1d1d;

    font-size: 13px;
}

.linea span:first-child {
    color: #aaa;
}

.linea span:last-child {
    color: #45ff95;

    font-weight: bold;
}

/* TIKTOKER */

.tiktoker-titulo {
    color: #d8a72d;

    font-size: 17px;

    font-weight: bold;

    margin-bottom: 15px;
}

</style>

</head>

<body>


<!-- =========================
     PANTALLA DE ACCESO
========================= -->

<div id="acceso" class="pantalla">

    <div class="logo">

        <h1>BRASI</h1>

        <h2>MODS</h2>

        <p>GENERADOR DE SENSIBILIDAD</p>

    </div>

    <div class="tarjeta">

        <div class="key-titulo">
            🔐 INGRESAR KEY
        </div>

        <input
            id="key"
            type="password"
            placeholder="KEY"
            autocomplete="off"
        >

        <button
            id="entrar"
            class="boton entrar"
        >
            🔓 ENTRAR
        </button>

        <p id="error"></p>

    </div>

</div>


<!-- =========================
     GENERADOR
========================= -->

<div id="generador" class="pantalla oculto">

<header>

    <div>

        <strong>BRASI MODS</strong>

        <small>GENERADOR</small>

    </div>

    <button
        id="volver"
        class="volver"
    >
        ←
    </button>

</header>


<main>

    <h1>🎯 Generador</h1>

    <p class="descripcion">
        Elegí Android o TikToker FF.
    </p>


    <!-- PESTAÑAS -->

    <div class="pestanas">

        <button
            id="androidTab"
            class="pestana activa"
        >
            📱 ANDROID
        </button>

        <button
            id="tiktokerTab"
            class="pestana"
        >
            🎵 TIKTOKER FF
        </button>

    </div>


    <!-- ANDROID -->

    <section
        id="androidPanel"
        class="panel"
    >

        <label>MARCA</label>

        <select id="marca">

            <option value="">
                Seleccionar marca
            </option>

            <option>Samsung</option>
            <option>Motorola</option>
            <option>Xiaomi</option>
            <option>Redmi</option>
            <option>POCO</option>
            <option>Realme</option>
            <option>OPPO</option>
            <option>Vivo</option>
            <option>ZTE</option>
            <option>TCL</option>
            <option>Tecno</option>
            <option>Infinix</option>
            <option>Honor</option>
            <option>OnePlus</option>
            <option>Nokia</option>
            <option>ASUS</option>
            <option>Google</option>
            <option>Sony</option>
            <option>Huawei</option>

        </select>

        <label>MODELO</label>

        <input
            id="modelo"
            type="text"
            placeholder="Ej: TCL 501"
        >

        <button
            id="generarAndroid"
            class="generar"
        >
            🔥 GENERAR SENSIBILIDAD
        </button>

    </section>


    <!-- TIKTOKER -->

    <section
        id="tiktokerPanel"
        class="panel oculto"
    >

        <div class="tiktoker-titulo">
            🎵 TIKTOKER FF
        </div>

        <label>
            TIKTOKER
        </label>

        <select id="tiktoker">

            <option value="">
                Seleccionar TikToker
            </option>

            <option value="nobru">NOBRU</option>
            <option value="coringa">CORINGA</option>
            <option value="waski">WASKI</option>
            <option value="cerol">CEROL</option>
            <option value="biela">BIELA</option>
            <option value="playhard">PLAYHARD</option>
            <option value="jota">JOTA</option>
            <option value="raone">RAONE</option>
            <option value="thurzin">THURZIN</option>
            <option value="elgato">EL GATO</option>
            <option value="loud">LOUD</option>
            <option value="bruno">BRUNO PLAY HARD</option>
            <option value="souz">SOUZ</option>
            <option value="two9">TWO9</option>
            <option value="yago">YAGO</option>
            <option value="nativa">NATIVA</option>
            <option value="bak">BAK</option>
            <option value="machado">MACHADO</option>
            <option value="k1ng">K1NG</option>
            <option value="fluxo">FLUXO</option>

        </select>

        <div class="nota">

            🎯 Configuración fija para cada creador.
            <br><br>
            Los valores son configuraciones
            inspiradas en el estilo del creador.

        </div>

        <button
            id="generarTiktoker"
            class="generar"
        >
            🎵 VER SENSIBILIDAD
        </button>

    </section>


    <!-- RESULTADO -->

    <div
        id="resultado"
        class="resultado oculto"
    >

        <div class="titulo-resultado">
            🎯 RESULTADO
        </div>

        <div id="datos"></div>

        <button
            id="restaurar"
            class="restaurar"
        >
            🔄 RESTAURAR
        </button>

    </div>

</main>

</div>


<script>

/* =========================
   CONFIGURACIÓN
========================= */

var KEY = "BRASI-21E58";


/* =========================
   MÚSICA DOMA
========================= */

var audioDoma = null;

function iniciarMusica() {

    if (audioDoma) return;

    try {

        audioDoma = new Audio("doma.mp3");

        audioDoma.loop = true;

        audioDoma.volume = 1.0;

        audioDoma.preload = "auto";

        var reproduccion = audioDoma.play();

        if (reproduccion !== undefined) {

            reproduccion.catch(function() {

                audioDoma = null;

            });

        }

    } catch (e) {

        audioDoma = null;

    }

}


/* =========================
   DETENER MÚSICA
========================= */

function detenerMusica() {

    if (audioDoma) {

        audioDoma.pause();

        audioDoma.currentTime = 0;

        audioDoma.src = "";

        audioDoma.load();

        audioDoma = null;

    }

}


/* =========================
   ACTIVAR AL TOCAR
========================= */

document.addEventListener(
    "click",
    function() {

        if (
            !document.hidden &&
            acceso &&
            !acceso.classList.contains("oculto")
        ) {

            iniciarMusica();

        }

    }
);


/* =========================
   SI SE PONE EN SEGUNDO PLANO
========================= */

document.addEventListener(
    "visibilitychange",
    function() {

        if (document.hidden) {

            detenerMusica();

        }

    }
);


/* =========================
   AL SALIR DE LA PÁGINA
========================= */

window.addEventListener(
    "pagehide",
    detenerMusica
);

window.addEventListener(
    "beforeunload",
    detenerMusica
);


/* ELEMENTOS */

var acceso =
document.getElementById("acceso");

var generador =
document.getElementById("generador");

var key =
document.getElementById("key");

var entrar =
document.getElementById("entrar");

var error =
document.getElementById("error");

var volver =
document.getElementById("volver");

var androidTab =
document.getElementById("androidTab");

var tiktokerTab =
document.getElementById("tiktokerTab");

var androidPanel =
document.getElementById("androidPanel");

var tiktokerPanel =
document.getElementById("tiktokerPanel");

var marca =
document.getElementById("marca");

var modelo =
document.getElementById("modelo");

var tiktoker =
document.getElementById("tiktoker");

var generarAndroid =
document.getElementById("generarAndroid");

var generarTiktoker =
document.getElementById("generarTiktoker");

var resultado =
document.getElementById("resultado");

var datos =
document.getElementById("datos");

var restaurar =
document.getElementById("restaurar");


/* =========================
   ENTRAR
========================= */

function ingresar() {

    iniciarMusica();

    var valor =
        key.value.trim().toUpperCase();

    if (valor === KEY) {

        error.innerHTML =
            "✅ BIENVENIDO A BRASI MODS";

        error.style.color =
            "#00e676";

        setTimeout(function() {

            detenerMusica();

            acceso.classList.add("oculto");

            generador.classList.remove("oculto");

            error.innerHTML = "";

        }, 700);

    } else {

        error.innerHTML =
            "❌ KEY INCORRECTA";

        error.style.color =
            "#ff4444";

    }

}

entrar.onclick = ingresar;


/* ENTER */

key.onkeydown = function(e) {

    if (e.key === "Enter") {

        ingresar();

    }

};


/* =========================
   VOLVER
========================= */

volver.onclick = function() {

    detenerMusica();

    generador.classList.add("oculto");

    acceso.classList.remove("oculto");

    key.value = "";

    error.innerHTML = "";

    restaurarSensibilidad();

};


/* =========================
   PESTAÑA ANDROID
========================= */

androidTab.onclick = function() {

    androidTab.classList.add("activa");

    tiktokerTab.classList.remove("activa");

    androidPanel.classList.remove("oculto");

    tiktokerPanel.classList.add("oculto");

};


/* =========================
   PESTAÑA TIKTOKER
========================= */

tiktokerTab.onclick = function() {

    tiktokerTab.classList.add("activa");

    androidTab.classList.remove("activa");

    tiktokerPanel.classList.remove("oculto");

    androidPanel.classList.add("oculto");

};


/* =========================
   ALEATORIO
========================= */

function aleatorio(min, max) {

    return Math.floor(
        Math.random() * (max - min + 1)
    ) + min;

}


/* =========================
   GENERAR ANDROID
========================= */

function generarAndroidOriginal() {

    if (marca.value === "") {

        alert("Seleccioná una marca.");

        return;

    }

    if (modelo.value.trim() === "") {

        alert("Escribí el modelo.");

        return;

    }

    var general =
        aleatorio(175, 200);

    var rojo =
        aleatorio(165, 195);

    var mira2 =
        aleatorio(155, 185);

    var mira4 =
        aleatorio(145, 175);

    var awm =
        aleatorio(90, 120);

    var camara =
        aleatorio(160, 195);

    var boton =
        aleatorio(43, 52);

    var dpi =
        aleatorio(400, 600);

    mostrar(

        marca.value +
        " " +
        modelo.value,

        "ANDROID",

        general,
        rojo,
        mira2,
        mira4,
        awm,
        camara,
        boton,
        dpi

    );

}


/* =========================
   TIKTOKERS
========================= */

var tiktokers = {

    nobru: [195,190,180,168,110,185,48,480],

    coringa: [200,195,185,172,115,190,50,520],

    waski: [190,185,175,165,108,180,47,460],

    cerol: [185,180,170,160,105,175,46,450],

    biela: [198,193,182,170,112,188,49,500],

    playhard: [192,187,177,165,108,182,48,470],

    jota: [200,190,180,170,110,190,51,520],

    raone: [188,183,173,162,103,178,46,450],

    thurzin: [196,191,181,169,112,187,49,490],

    elgato: [194,189,179,167,109,184,48,480],

    loud: [199,194,184,171,114,189,50,510],

    bruno: [191,186,176,164,106,181,47,470],

    souz: [187,182,172,161,104,177,46,440],

    two9: [197,192,183,170,113,188,49,500],

    yago: [193,188,178,166,107,183,48,480],

    nativa: [189,184,174,163,105,179,47,460],

    bak: [200,196,186,173,116,192,51,530],

    machado: [196,190,181,168,111,186,49,490],

    k1ng: [198,193,183,171,114,189,50,510],

    fluxo: [192,187,177,165,108,182,48,470]

};


/* =========================
   GENERAR TIKTOKER
========================= */

function generarTiktokerOriginal() {

    var nombre =
        tiktoker.value;

    if (nombre === "") {

        alert("Seleccioná un TikToker.");

        return;

    }

    var c =
        tiktokers[nombre];

    mostrar(

        nombre.toUpperCase(),

        "TIKTOKER FF",

        c[0],
        c[1],
        c[2],
        c[3],
        c[4],
        c[5],
        c[6],
        c[7]

    );

}


/* =========================
   BOTÓN GENERAR ANDROID
========================= */

generarAndroid.onclick = function() {

    generarAndroidOriginal();

};


/* =========================
   BOTÓN GENERAR TIKTOKER
========================= */

generarTiktoker.onclick = function() {

    generarTiktokerOriginal();

};


/* =========================
   MOSTRAR RESULTADO
========================= */

function mostrar(

    nombre,
    tipo,
    general,
    rojo,
    mira2,
    mira4,
    awm,
    camara,
    boton,
    dpi

) {

    datos.innerHTML =

        linea("Perfil", nombre) +

        linea("Tipo", tipo) +

        linea("General", general) +

        linea("Punto rojo", rojo) +

        linea("Mira 2X", mira2) +

        linea("Mira 4X", mira4) +

        linea("Mira AWM", awm) +

        linea("Cámara libre", camara) +

        linea(
            "Botón de disparo",
            boton + "%"
        ) +

        linea("DPI", dpi);

    resultado.classList.remove("oculto");

}


/* =========================
   RESTAURAR
========================= */

function restaurarSensibilidad() {

    resultado.classList.add("oculto");

    datos.innerHTML = "";

}


/* BOTÓN RESTAURAR */

restaurar.onclick = function() {

    restaurarSensibilidad();

};


/* =========================
   LÍNEA
========================= */

function linea(nombre, valor) {

    return (

        "<div class='linea'>" +

        "<span>" +
        nombre +
        "</span>" +

        "<span>" +
        valor +
        "</span>" +

        "</div>"

    );

}

</script>

</body>
</html>
