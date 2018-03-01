# <a name="educationroot-resource-type"></a>Тип ресурса educationRoot

Пространство имен `/education` обеспечивает функциональность, предназначенную для сектора образования. Некоторые объекты пространства имен `/education` можно найти в других частях Microsoft Graph (например, [users](user.md)). Пространство имен для образовательной сферы позволяет использовать специальные свойства и функции для этих объектов.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Создание educationClass](../api/educationroot_post_classes.md) |[educationClass](educationclass.md)| Создание объекта **educationClass** путем публикации в коллекции курсов.|
|[Перечисление курсов](../api/educationroot_list_classes.md) |Коллекция [educationClass](educationclass.md)| Получение коллекции объектов **educationClass**.|
|[Создание educationSchool](../api/educationroot_post_schools.md) |[educationSchool](educationschool.md)| Создание объекта **educationSchool** путем публикации в коллекции учебных заведений.|
|[Перечисление учебных заведений](../api/educationroot_list_schools.md) |Коллекция [educationSchool](educationschool.md)| Получение коллекции объектов **educationSchool**.|
|[Создание educationUser](../api/educationroot_post_users.md) |[educationUser](educationuser.md)| Создание **educationUser** путем публикации в коллекции пользователей.|
|[Перечисление пользователей](../api/educationroot_list_users.md) |Коллекция [educationUser](educationuser.md)| Получение коллекции объектов **educationUser**.|

## <a name="properties"></a>Свойства
Нет

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|classes|Коллекция [educationClass](educationclass.md)| Только для чтения. Допускается значение NULL.|
|me|[educationUser](educationuser.md)| Только для чтения. Допускается значение NULL.|
|schools|Коллекция [educationSchool](educationschool.md)| Только для чтения. Допускается значение NULL.|
|users|Коллекция [educationUser](educationuser.md)| Только для чтения. Допускается значение NULL.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationRoot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->