# Извлечение сущностей из текстовых задач по физике 

### Entities:

1. Object - физическое тело/материальная точка
2. Substance - вещество, из которого сделано тело или в котором находится тело
3. Property - количественный показатель, физическая величина (например, масса, скорость)
4. Value - численное значение физической величины (например, 10 кг, 20 м/с)
5. Phenomena - явление/процесс, по которому можно определить тему задачи
6. Question - вопрос в задаче по поводу свойства какой-либо тела

### Relations:

1. Description  Arg1:Property, Arg2:Object - Property описывает свойство какого-то конкретного тела (масса мячика)
2. Description  Arg1:Property, Arg2:Substance - свойство, описывающее какое-либо вещество (вода массой 3 кг)
3. Description  Arg1:Value, Arg2:Object - значение физической величины, описывающее какое-либо тело (в некоторых задачах не указана физическая величина, вместо этого обозначено просто: "10-ти килограммовый мяч...")
4. Description  Arg1:Value, Arg2:Substance - значение физической величины, описывающее какое-либо вещество (в некоторых задачах не указана физическая величина, вместо этого обозначено просто: "2 литра воды...")
5. Measure  Arg1:Property, Arg2:Value - физическая величина измеряется в ...
6. About  Arg1:Question, Arg2:Property - указание на вопрос задачи, чаще всего это вопрос о каком-либо свойстве объекта
7. Happens Arg1:Phenomena, Arg2:Object - физическое явление/процесс происходит над каким-то объектом (например, мяч падает)
8. Happens Arg1:Phenomena, Arg2:Substance - физическое явление/процесс происходит над каким-то веществом (например, вода нагревается)
9. Material Arg1:Substance, Arg2:Object - указание на материал, из которого состоит физическое тело (например, куб из дерева)
10. Located Arg1:Object, Arg2:Substance - указание на месторасположение тела в какой-то среде (например, мяч находится в керосине)
11. Located Arg1:Substance, Arg2:Substance - указание на месторасположение вещества в какой-то среде (например, стекло в керосине)
12. Do Arg1:Object, Arg2:Phenomena - какое-то тело оказывается воздействие на другое тело (например, кран поднял груз)

### Events: 

Увеличение или уменьшение какой-либо физической величины

1. Increase Changing-Arg:Property, Event-Arg:<EVENT>
2. Decrease Changing-Arg:Property, Event-Arg:<EVENT>

### Attributes: 
  
1. Type_of_changing	Arg:<EVENT>, Value:In|On - изменение какой-либо величины просходит "на" какое-то число или "в/во" сколько-то раз
2. Reference Arg:<ENTITY> - для данной сущности необходимы справочные данные (например, плотность, удельная теплоемкость)
3. Medium Arg:<ENTITY> - вещество является средой (например, в воде находится...)

  
### Задачи

Источники:
  
1. Перышкин 
2. Физика. Задачник. 10-11 кл.: учебное пособие / А.П. Рымкевич. - 23-е изд., стереотип. - М.: Дрофа, 2019. - 188, [4] с.: ил. - (Российский учебник).

Темы:

1. Механика
2. Электричество
3. Термодинамика
