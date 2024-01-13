class Heroi {
    constructor(nomeDoHeroi, idadeDoHeroi, classeDoHeroi) {
        this.nomeDoHeroi = nomeDoHeroi;
        this.idadeDoHeroi = idadeDoHeroi;
        this.classeDoHeroi = classeDoHeroi;
    }

    atacar() {
        let ataque;

        switch (this.classeDoHeroi) {
            case 'mago':
                ataque = "Magia";
                break;
            case 'guerreiro':
                ataque = "Espada";
                break;
            case 'monge':
                ataque = "Artes Marciais";
                break;
            case 'ninja':
                ataque = "Shuriken";
                break;
            default:
                ataque = "Ataque indefinido";
        }

        console.log(`O ${this.classeDoHeroi} atacou usando ${ataque}`);
    }
}

let heroiMago = new Heroi("Dumbledore", 120, "mago");
let heroiGuerreiro = new Heroi("Guts", 31, "guerreiro");
let heroiMonge = new Heroi("Tanaka", 22, "monge");
let heroiNinja = new Heroi("Gabimaru", 20, "ninja");

heroiMago.atacar();
heroiGuerreiro.atacar();
heroiMonge.atacar();
heroiNinja.atacar();
