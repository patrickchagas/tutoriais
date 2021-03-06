## Constantes Mágicas

O PHP fornece um grande número de constantes predefinidas para qualquer script que execute. A maioria dessas constantes, entretanto, são criadas por várias extensões, e estarão presentes somente quando essas extensões estiverem disponíveis, tanto por carregamento dinâmico quanto por compilação direta.

Há nove constantes mágicas, que mudam dependendo de onde são utilizadas. Por exemplo, o valor de __LINE__ depende da linha em que é utilizada em seu script. Todas essas constantes "mágicas" são resolvidas em tempo de compilação, ao contrário das constantes regulares que são resolvidas em tempo de execução. Essas constantes especiais são case-insentitive e estão descritas a seguir:

Algumas constantes "mágicas" do PHP Nome 	Descrição
```php
__LINE__ 	O número da linha corrente do arquivo.
__FILE__ 	O caminho completo e nome do arquivo com links simbólicos resolvidos. Se utilizado dentro de um include, o nome do arquivo incluído será retornado.
__DIR__ 	O diretório do arquivo. Se usado dentro de um include, o diretório do arquivo incluído é retornado. É equivalente a dirname(__FILE__). O nome do diretório não possui barra no final, a não ser que seja o diretório raiz.
__FUNCTION__ 	O nome da função, or {closure} para funções anônimas.
__CLASS__ 	O nome da classe. O nome da classe inclui o namespace em que foi declarado (por exemplo, Foo\Bar). Note que a partir do PHP 5.4, __CLASS__ também funcionará em traits. Quando utilizada em um método trait, __CLASS__ é o nome da classe que está utilizando a trait.
__TRAIT__ 	O nome do trait. O nome do trait inclui o namespace em que foi declarado (por exemplo, Foo\Bar).
__METHOD__ 	O nome do método da classe.
__NAMESPACE__ 	O nome do namespace corrente.
```
NomeDaClasse::class 	O nome completo da classe. Veja também ::class.

Veja também get_class(), get_object_vars(), file_exists() e function_exists(). 
