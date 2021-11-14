### Zapis ER diagrama
```mermaid
classDiagram
class ENTITETA{
	atribut1 tip lastnosti
	atribut2 tip lastnosti
	atribut3 tip lastnosti
	() ...
}
ENTITETA-->DIJAK
class DIJAK{
	ID_dijaka* integer NN PK
	ime Char(15) NN
	priimek Char(25) NN
	() ...
}