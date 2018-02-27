# <a name="educationschool-resource-type"></a>Тип ресурса educationSchool

Учебное заведение. Ресурс **EducationSchool** в настоящее время соответствует ресурсу [administrativeUnit](../../beta/resources/administrativeunit.md), и у них общий идентификатор.  

>**Примечание.** Ресурсы **administrativeUnit** и **educationOrganization** представлены в бета-версии. Если вы используете эти ресурсы, не забывайте периодически просматривать [журнал изменений](../../../concepts/changelog.md). Когда ресурсы API Microsoft Graph будут выпущены для версии конечной точки 1.0, мы сообщим об этом в журнале изменений. Если приложение потребляет ресурсы **administrativeUnit** или **educationOrganization**, необходимо будет объявить URL-адреса базового запроса, как показано в блоке кода ниже.  
  ```JavaScript
  var v1BaseUrl = “https://graph.microsoft.com/v1.0/education”;
  var betaBaseUrl = “https://graph.microsoft.com/beta/education”;  // for administrativeUnit and educationOrganization
  ```

Этот ресурс — подтип [educationOrganization](../../beta/resources/educationorganization.md).


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
|[Получение administrativeUnit](../api/educationschool_get_administrativeunit.md) |[administrativeUnit](../../beta/resources/administrativeunit.md)| Получение элемента **administrativeUnit**, соответствующего учебному заведению **educationSchool**.|
|[Обновление](../api/educationschool_update.md) | [educationSchool](educationschool.md) |Обновление объекта **educationSchool**. |
|[Удаление](../api/educationschool_delete.md) | None |Удаление объекта **educationSchool**. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String|GUID этого учебного заведения.|
|displayName| String| Отображаемое имя учебного заведения.| 
|description| String | Описание учебного заведения.| 
|status| string| Только для чтения. Возможные значения: `inactive`, `active`, `expired`, `deleteable`.|
|externalSource| string| Только для чтения.  Возможные значения: `sis`, `manual`, `unknownFutureValue`.|
|principalEmail| String| Адрес электронной почты директора.|
|principalName| String | Имя директора.|
|externalPrincipalId| String | Идентификатор директора в системе синхронизации. |
|highestGrade|String| Самый старший класс. |
|lowestGrade|String| Самый младший класс. |
|schoolNumber|String| Номер школы.|
|externalId|String| Идентификатор учебного заведения в системе синхронизации. |
|phone|String| Номер телефона учебного заведения. |
|fax|String| Номер факса учебного заведения. |
|address|[physicalAddress](physicaladdress.md)| Адрес учебного заведения.|
|createdBy|[identitySet](identityset.md)|Объект, который создал учебное заведение.|


## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|classes|Коллекция [educationClass](educationclass.md)| Классы, которые обучаются в учебном заведении. Допускается значение null.|
|users|Коллекция [educationUser](educationuser.md)| Пользователи в учебном заведении. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
