
### Qu'est ce que l'on teste ? 

L'interface *publique* d'une classe définit "un contrat" entre celui qui fournit la classe et celui qui l'utilise. ( Toutes les méthodes / propriétés publiques de la classe.)

Ce contrat définit : 
	- Les services proposés par la classe.
	- La manière dont ces services doivent être utilisés. 

**Tester une classe consiste à vérifier la validité de ce contrat**


### Le TDD (Test Driven Development)

1. Ecrire un premier test.
2. Vérifier qu'il échoue (car le code qu'il test n'existe pas encore), afin de vérifier que le test est valide.
3. Ecrire juste le code suffisant pour passer le test.
4. Vérifier que le test passe.
5. Réviser le code (refacto), i.e. l'améliorer tout en gardant les mêmes fonctionnalités. 

### JUnit5

Terminologie JUnit : 
	- Test Unitaire (Unit test): Test d'une classe.
	- ... A Compléter 

*Annotation :*
Avant  chaque test @BeforeEach 
Après  chaque test @AfterEach
Pour   chaque test @Test
Avant  le premier test @BeforeAll
Après  le dernier test @AfterAll
Ne sera pas lancée comme test @Disabled

*Asserts :* 
AssertTrue(bool)
AssertFalse(bool)
AssertEquals(expect, actual)
AssertNotEqual(expect, actual)
AssertSame(expect, actual)
assertNotSame(expect, actual)
AssertTimeout(timeout, executable)
AssertThrows(ExceptionType, executable)
AssertNull(Object)
AssertNotNull(Object)
Fail() -> Provoque l'echec d'un test.
AssertAll(...)

https://www.jmdoudoux.fr/java/dej/chap-junit.htm