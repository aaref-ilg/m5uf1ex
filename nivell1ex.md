# Spring framework

L'**Spring framework** (abreviant, **Spring**), és un [marc de treball](https://ca.wikipedia.org/wiki/Entorn_de_treball_(inform%C3%A0tica)) de [codi obert](https://ca.wikipedia.org/wiki/Codi_obert) per [la plataforma Java](https://ca.wikipedia.org/wiki/Plataforma_Java). La primera versió va ser escrita per Rod Johnson, que inicialment va llençar el producte juntament amb el llibre _One-on-One Java EE Design and Development_.

## Funcionalitats clau

* Gestió de la configuració basada en JavaBeans, aplicant-hi principis d'Inversió de Control, més específicament usant la tècnica d'Injecció de Dependència. Això ajuda a reduir les dependències de components, en implementacions específiques, sobre altres components.
* Una factoria de Beans central, que és usada globalment.
* Capa genèrica d'abstracció per la gestió de transaccions de la base de dades.
* Estratègies preincorporades per la JTA i un sol DataSource de JDBC. Això elimina la dependència en un entorn Java EE pel suport a les transaccions
* Integració amb entorns de persistència com Hibernate, JDO, iBatis i db4o.
* Entorn d'aplicació web MVC, construït al nucli de la funcionalitat de Spring. suportant moltes tecnologies per generar vistes, incloent-hi JSP, FreeMaker, Velocity, Tiles, iText i POI.
* Entorn extensiu de programació orientada a aspectes per proveir serveis, com ara gestió de les transaccions. Amb això es millora la modularitat dels sistemes.

### Entorn d'accés remot

* Protocols basats en HTTP
  * Hessian : protocol de serialització binària de codi obert i mantingut per protocols basats en Corba
  * RMI (1) : mètode d'invocacions usant infraestructura RMI
  * RMI (2) : mètode d'invocacions usant interfícies que acomplien amb l'ús regular d'RMI
  * RMI-IIOP (Corba) : mètode d'invocacions usant RMI-IIOP/Corba
* Integració amb client Enterprise javaBean
  * Connectivitat amb bean local sense estat EJB : connectant amb beans de sessió locals sense estat
  * Connectivitat amb bean remot sense estat EJB : connectant amb beans de sessió remots sense estat
* SOAP
  * Integració amb l'entorn de serveis web Apache Axis

> Spring Framework té el seu propi entorn de programació orientada a l'aspecte que modularitza problemàtiques multicapa en aspectes. La motivació de crear un entorn AOP ve de la consideració que hauria de ser possible proveir funcionalitats bàsiques AOP sense massa complexitat ni al disseny ni la implementació ni la configuració.

```// Hola.java
import java.io.IOException;
public class Hola {
    public static void main(String[] args)throws IOException {
        System.out.println("Hola, món!"); 
    }
}
```

[![spring](https://programaenlinea.net/wp-content/uploads/2019/11/spring-framework.png)](https://programaenlinea.net/wp-content/uploads/2019/11/spring-framework.png)