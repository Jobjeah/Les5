# Les5
Java les 5 

public class Les5{
  private Beer biertje;
  private Whiskey whiskeytje;
  private Vodka vodkatje;
  private Wijn wijntje;
  public static void main(String[] args) {
    	Les5 self = new Les5();
      self.runLesson();
  }
  private void runLesson(){
    biertje = new Beer();
    biertje.drink();
    whiskeytje = new Whiskey();
    whiskeytje.drink();
    whiskeytje.burn();
    whiskeytje.drink();

    //Opdracht 1
    //Maak nu zelf een nieuwe class aan met de naam Vodka
    //Kijk goed naar de syntax van de andere classes Beer en Whiskey

    //done

    //Opdracht 2
    //Zorg ervoor d.m.v overerving dat je met Vodka alles kunt wat je ook met Alcohol kunt (drinken)

    //done

    //Opdracht 3
    //Maak van de Vodka class een object aan. Noem deze "vodkatje"
    //Drink je vodkatje leeg.
    vodkatje = new Vodka();
    vodkatje.drink();

    //Opdracht 4
    //Zowel Vodka als Whiskey kan lekker branden.
    //Het is dus handig als ze allebei overerven van een class waarin het branden is geprogrammeerd
    //Maak een class met de naam BurningAlcohol en zet daarin de burn() method uit de Whiskey class.
    //Verwijder ook de burn() method uit de Whiskey class.
    //Laat de classes Whiskey en Vodka overerven van de BurningAlcohol class
    //Laat BurningAlcohol class overerven van de Alcohol class

    //done

    //Opdracht 5
    //Vul je biertje, vodkatje en je whiskeytje weer met de refil() method
    //verbrand je whiskeytje en drink je vodka leeg.
    //Neem 5 slokken bier.

    biertje.refil();
    vodkatje.refil();
    whiskeytje.refil();

    whiskeytje.burn();

    vodkatje.drink();

    for(int i=0; i<5; i++){
      biertje.drink();
    }

    //Opdracht 6
    //Maak 30 glazen vodka aan en verbrand ze allemaal.

    for(int i=1; i<31; i++){
      vodkatje.refil();
      vodkatje.burn();
      System.out.println("Glas " + i + " van 30 is verbrand. BURN IT LIKE FIREEE!!!");
    }

    //Opdracht 7
    //Maak een nieuwe class aan voor Wijn
    //Wijn is niet brandbaar en je moet het kunnen drinken
    //Zorg dat de Wijn van de juiste class overerft
    //Een glas wijn bevat 250ml
    //maak een glaasje wijn aan en drink deze leeg
    wijntje = new Wijn();

    wijntje.refil();
    wijntje.drink();

  }
}
