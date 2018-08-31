# <a name="educationschool-resource-type"></a>Тип ресурса educationSchool

Ресурс представляет учебное заведение и используется для управления классами, преподавателями и учащимися данного учебного заведения.  


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Get](../api/educationschool_get.md) | [educationSchool](educationschool.md) |Считывание свойств и отношений объекта **educationSchool**.|
|[Добавление класса](../api/educationschool_post_classes.md) |[educationClass](educationclass.md)| Добавление нового объекта **educationClass** в учебное заведение через публикацию в свойстве навигации classes.|
|[Перечисление классов](../api/educationschool_list_classes.md) |Коллекция [educationClass](educationclass.md)| Получение коллекции объектов **educationClass**.|
|[Удаление класса](../api/educationschool_delete_classes.md) |[educationClass](educationclass.md)| Удаление **educationClass** из учебного заведения через свойство навигации classes.|
|[Добавление пользователя](../api/educationschool_post_users.md) |[educationUser](educationuser.md)| Добавление нового объекта **educationClass** в учебное заведение через публикацию в свойстве навигации **users**.|
|[Перечисление пользователей](../api/educationschool_list_users.md) |Коллекция [educationUser](educationuser.md)| Получение коллекции объектов **educationUser**.|
|[Удаление пользователя](../api/educationschool_delete_users.md) |[educationUser](educationuser.md)| Удаление **educationUser** из учебного заведения через свойство навигации **users**.|
|[Обновление](../api/educationschool_update.md) | [educationSchool](educationschool.md) |Обновление объекта **educationSchool**. |
|[Удаление](../api/educationschool_delete.md) | Нет |Удаление объекта **educationSchool**. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String (строка)|GUID этого учебного заведения.|
|displayName| String (строка)| Отображаемое имя учебного заведения.| 
|description| String (строка) | Описание учебного заведения.| 
|status| string (строка)| Только для чтения. Возможные значения: `inactive`, `active`, `expired`, `deleteable`.|
|externalSource| educationExternalSource| Только для чтения.  Возможные значения: `sis`, `manual`, `unknownFutureValue`.|
|principalEmail| String (строка)| Адрес электронной почты директора.|
|principalName| String (строка) | Имя директора.|
|externalPrincipalId| String (строка) | Идентификатор директора в системе синхронизации. |
|highestGrade|String (строка)| Самый старший класс. |
|lowestGrade|String (строка)| Самый младший класс. |
|schoolNumber|String (строка)| Номер школы.|
|externalId|String (строка)| Идентификатор учебного заведения в системе синхронизации. |
|phone|String (строка)| Номер телефона учебного заведения. |
|fax|String (строка)| Номер факса учебного заведения. |
|address|[physicalAddress](physicaladdress.md)| Адрес учебного заведения.|
|createdBy|[identitySet](identityset.md)|Объект, который создал учебное заведение.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|classes|Коллекция [educationClass](educationclass.md)| Классы, которые обучаются в учебном заведении. Допускается значение null.|
|users|Коллекция [educationUser](educationuser.md)| Пользователи в учебном заведении. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.educationOrganization",
  "@odata.type": "microsoft.graph.educationSchool"
}-->

```json
{
  "id": "String",
  "displayName": "String",
  "description": "String",
  "status": "String",
  "externalSource": "String",
  "principalEmail": "String",
  "principalName": "String",
  "externalPrincipalId": "String",
  "highestGrade": "String",
  "lowestGrade": "String",
  "schoolNumber": "String",
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "externalId": "String",
  "fax": "String",
  "phone": "String",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationSchool resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
