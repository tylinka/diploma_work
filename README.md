# Извлечение сущностей из текстовых задач по физике 

### Entities:

1. Object - физическое тело/материальная точка
2. Property - количественный показатель, физическая величина 
3. Phenomena - явление/процесс, по которому можно определить тему задачи
4. Question - вопрос в задаче по поводу свойства какой-либо тела

### Relations:

1. Description	Arg1:Property, Arg2:Object - Property описывает свойство какого-то конкретного тела
2. Belonging 	  Arg1:Property, Arg2:Property - показывает связь между численными значениями физической величины и самой физической величиной, если в тексте есть разрыв (Первоначальная **частота** падающего света была равна **0,75*10^15 Гц**)
3. About        Arg1:Question, Arg2:Property - вопрос о свойстве

### Events: 

Увеличение или уменьшение какой-либо физической величины

1. Increase Changing-Arg:Property, Event-Arg:<EVENT>
2. Decrease Changing-Arg:Property, Event-Arg:<EVENT>

### Attributes: 

Изменение какой-либо величины "на" или "в"
  
1. Type_of_changing	Arg:<EVENT>, Value:In|On
2. Negation		Arg:<EVENT>

