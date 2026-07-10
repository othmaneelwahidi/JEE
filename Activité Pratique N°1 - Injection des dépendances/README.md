# Activite pratique 1 - Injection des dependances

## Objectif

Illustrer l'inversion de controle : la couche metier depend d'une abstraction
DAO et recoit son implementation sans couplage fort.

## Travaux realises

- Instanciation statique des composants.
- Instanciation dynamique depuis `config.txt` avec la reflection.
- Injection Spring par XML et par annotations.
- Creation d'un mini-framework IoC compatible XML et annotations.

## Sous-projets

`tp1-injection` contient `IDao`, `IMetier`, leurs implementations et les
presentations `Pres1`, `Pres2`, `PresSpringXML` et `PresSpringAnnotations`.

`tp1-mini-framework` analyse des definitions XML ou les annotations
`@Component` et `@Autowired`, construit les objets et injecte leurs dependances.

## Compilation

```bash
cd tp1-injection
mvn clean compile
cd ../tp1-mini-framework
mvn clean compile
```

Lancez ensuite la classe de presentation souhaitee depuis l'IDE.

## Concepts acquis

Couplage faible, interfaces, inversion de controle, injection, reflection,
configuration XML et detection par annotations.
