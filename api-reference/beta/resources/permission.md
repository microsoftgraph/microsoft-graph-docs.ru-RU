# <a name="permission-resource-type"></a>Тип ресурса Permission

Ресурс **Permission** предоставляет сведения о разрешении, предоставленном для ресурса [DriveItem](driveitem.md).

Разрешения могут иметь самые различные формы. Ресурс **Permission** представляет эти различные формы с помощью аспектов в ресурсе.

## <a name="json-representation"></a>Представление JSON

Ниже показано представление JSON ресурса.

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "link", "grantedTo", "invitation", "inheritedFrom", "shareId" ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.permission"
}-->
```json
{
  "id": "string (identifier)",
  "grantedTo": {"@odata.type": "microsoft.graph.identitySet"},
  "inheritedFrom": {"@odata.type": "microsoft.graph.itemReference"},
  "invitation": {"@odata.type": "microsoft.graph.sharingInvitation"},
  "link": {"@odata.type": "microsoft.graph.sharingLink"},
  "roles": ["string"],
  "shareId": "string"
}
```

## <a name="properties"></a>Свойства

| Свойство      | Тип                                      | Описание                                                                                                                           |
|:--------------|:------------------------------------------|:--------------------------------------------------------------------------------------------------------------------------------------|
| id            | Строка                                    | Уникальный идентификатор разрешения среди всех разрешений для элемента. Только для чтения.                                                 |
| grantedTo     | [IdentitySet](identityset.md)             | Для разрешений типа user: сведения о пользователях и приложениях для этого разрешения. Только для чтения.                                    |
| invitation    | [SharingInvitation](sharinginvitation.md) | Сведения обо всех сопоставленных приглашениях к совместному использованию для данного разрешения. Только для чтения.                                                          |
| inheritedFrom | [ItemReference](itemreference.md)         | Предоставляет ссылку на предка текущего разрешения, если оно унаследовано от предка. Только для чтения.                       |
| ссылка          | [SharingLink](sharinglink.md)             | Предоставляет сведения о ссылке для текущего разрешения, если это разрешение типа link. Только для чтения.                                     |
| role          | Коллекция строк.                      | Тип разрешения, например `read`. Полный список ролей см. ниже. Только для чтения.                                                 |
| shareId       | String                                    | Уникальный маркер для этого разрешения. Только для чтения. |

Ресурс [Permission](../resources/permission.md) использует _аспекты_ для предоставления сведений о типе разрешения, представленного ресурсом.

Разрешения с аспектом [**link**](sharinglink.md) представляют ссылки для совместного доступа, созданные в элементе. Ссылки для совместного доступа содержат уникальный токен, предоставляющий доступ к элементу для любого пользователя, у которого есть такая ссылка.

Разрешения с аспектом [**invitation**](sharinginvitation.md) представляют разрешения, добавленные путем приглашения определенных пользователей или групп для доступа к файлу.

## <a name="roles-enumeration"></a>Перечисление ролей

| Роль  | Сведения                                                                        |
|:------|:-------------------------------------------------------------------------------|
| `read`  | Дает возможность считывать метаданные и содержимое элемента.            |
| `write` | Дает возможность считывать и изменять метаданные и содержимое элемента. |

## <a name="methods"></a>Методы

| Метод                                              | Путь REST                            |
|:----------------------------------------------------|:---------------------------------------|
| [Вывод списка разрешений](../api/item_list_permissions.md) | `GET /drive/items/{item-id}/permissions`  |
| [Получение разрешения](../api/permission_get.md)          | `GET /drive/items/{item-id}/permissions/{id}` |
| [Добавление](../api/item_invite.md)                        | `POST /drive/items/{item-id}/invite` |
| [Обновление](../api/permission_update.md)               | `PATH /drive/items/{item-id}/permissions/{id}` |
| [Удаление](../api/permission_delete.md)               | `DELETE /drive/items/{item-id}/permissions/{id}` |


## <a name="remarks"></a>Заметки

Библиотеки документов OneDrive для бизнеса и SharePoint не возвращают свойство **inheritedFrom**.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "permission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
