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

| Свойство      | Тип                                      | Описание
|:--------------|:------------------------------------------|:-----------------
| id            | Строка                                    | Уникальный идентификатор разрешения среди всех разрешений для элемента. Только для чтения.
| grantedTo     | [IdentitySet](identityset.md)             | Для разрешений типа user: сведения о пользователях и приложениях для этого разрешения. Только для чтения.
| invitation    | [SharingInvitation][]                     | Сведения обо всех сопоставленных приглашениях к совместному использованию для данного разрешения. Только для чтения.
| inheritedFrom | [ItemReference](itemreference.md)         | Предоставляет ссылку на предка текущего разрешения, если оно унаследовано от предка. Только для чтения.
| ссылка          | [SharingLink][]                           | Предоставляет сведения о ссылке для текущего разрешения, если это разрешение типа link. Только для чтения.
| role          | Коллекция строк.                      | Тип разрешения, например `read`. Полный список ролей см. ниже. Только для чтения.
| shareId       | String                                    | Уникальный токен, с помощью которого можно получить доступ к общему элементу через [API **shares**](../api/shares_get.md). Только для чтения.

Ресурс Permission предоставляет сведения о типе разрешения, представленного ресурсом, с помощью _аспектов_.

Разрешения с аспектом [**link**][SharingLink] представляют ссылки для совместного доступа, созданные в элементе. Ссылки для совместного доступа содержат уникальный токен, предоставляющий доступ к элементу любому пользователю, у которого есть такая ссылка.

Разрешения с аспектом [**invitation**][SharingInvitation] представляют разрешения, добавленные путем приглашения определенных пользователей или групп для доступа к файлу.

[SharingInvitation]: sharinginvitation.md
[SharingLink]: sharinglink.md

## <a name="roles-enumeration"></a>Перечисление ролей

| Роль        | Сведения                                                                        |
|:------------|:-------------------------------------------------------------------------------|
| `read`      | Дает возможность считывать метаданные и содержимое элемента.            |
| `write`     | Дает возможность считывать и изменять метаданные и содержимое элемента. |
| `sp.owner`  | В случае с SharePoint и OneDrive для бизнеса представляет роль владельца.       |
| `sp.member` | В случае с SharePoint и OneDrive для бизнеса представляет роль участника.      |

## <a name="methods"></a>Методы

| Метод                                              | Путь REST
|:----------------------------------------------------|:-----------------------
| [Вывод списка разрешений](../api/item_list_permissions.md) | `GET /drive/items/{item-id}/permissions`
| [Получение разрешения](../api/permission_get.md)          | `GET /drive/items/{item-id}/permissions/{id}`
| [Добавление](../api/item_invite.md)                        | `POST /drive/items/{item-id}/invite`
| [Обновление](../api/permission_update.md)               | `PATCH /drive/items/{item-id}/permissions/{id}`
| [Удаление](../api/permission_delete.md)               | `DELETE /drive/items/{item-id}/permissions/{id}`


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
