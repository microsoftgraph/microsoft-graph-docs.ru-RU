# <a name="directoryrole-resource-type"></a>Тип ресурса directoryRole

Представляет роль directory Azure AD. Каталог роли Azure AD также называются *ролями администратора*. Дополнительные сведения о ролях каталогов (администратор) можно [Назначение ролей администратора в Azure AD](http://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/). Microsoft Graph можно назначить роли каталог, чтобы предоставлять им разрешения целевой роли пользователей. Для чтения роли каталога или обновите его члены, необходимо активировать в клиентов. Только роль directory Администраторы организации активируется по умолчанию. Активация других ролей доступны directory отправить запрос POST с Идентификатором [directoryRoleTemplate](directoryroletemplate.md) , лежащие в основе роли каталога. Наследуется от [directoryObject](directoryobject.md).
Этот ресурс поддерживает:

- отслеживание дополнений, удалений и обновлений с помощью [запроса изменений](../../../concepts/delta_query_overview.md) (функция [delta](../api/directoryrole_delta.md)).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение directoryRole](../api/directoryrole_get.md) | [directoryRole](directoryrole.md) | Считывание свойств и отношений объекта directoryRole. |
|[Перечисление объектов directoryRole](../api/directoryrole_list.md) | Коллекция объектов [directoryRole](directoryrole.md) | Перечисление ролей каталога, активированных в клиенте. |
|[Добавление элемента](../api/directoryrole_post_members.md) |[directoryObject](directoryobject.md)| Добавление пользователя в роль каталога путем записи данных в свойство навигации members.|
|[Список членов](../api/directoryrole_list_members.md) |Коллекция [directoryObject](directoryobject.md)| Получение пользователей, которые относятся к членам роли каталога, из свойства навигации members.|
|[Удаление члена](../api/directoryrole_delete_member.md) |[directoryObject](directoryobject.md)| Удаление ресурса user из роли каталога.|
|[Активация directoryRole](../api/directoryrole_post_directoryroles.md) |[directoryRole](directoryrole.md) | Активация роли каталога.|
|[delta](../api/directoryrole_delta.md)|Коллекция объектов directoryRole| Получите добавочные изменения для каталога ролей. |

## <a name="properties"></a>Свойства
| Свойство   | Тип | Описание |
|:---------------|:--------|:----------|
|описание|String|Описание роли каталога. Только для чтения. |
|displayName|String|Отображаемое имя роли каталога. Только для чтения. |
|id|String|Уникальный идентификатор роли каталога. Наследуется из [directoryObject](directoryobject.md). Ключ, значение null не допускается, только для чтения.|
|roleTemplateId|String| Свойство **id** ресурса [directoryRoleTemplate](directoryroletemplate.md), определяющего значения свойств для этой роли. При активации роли каталога на клиенте следует указать свойство с помощью операции POST. После активации роли каталога свойство доступно только для чтения. |

## <a name="relationships"></a>Связи
| Связь | Тип |Описание|
|:---------------|:--------|:----------|
|members|Коллекция [directoryObject](directoryobject.md)|Пользователи, которые относятся к членам этой роли каталога. Методы HTTP: GET, POST, DELETE. Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [
    "memberOf",
    "members",
    "ownedObjects",
    "owners"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.directoryObject",
  "@odata.type": "microsoft.graph.directoryRole",
  "@odata.annotations": [
    {
      "capabilities": {
        "toppable": false
      }
    }
  ]
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
  "roleTemplateId": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
