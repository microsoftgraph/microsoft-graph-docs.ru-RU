---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Permission
ms.openlocfilehash: 9f73684d51ab4cee047219e142f72edf778cb171
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="permission-resource-type"></a>Тип ресурса Permission

Ресурс **Permission** содержит сведения о разрешении на совместный доступ, предоставленном для ресурса [DriveItem](driveitem.md).

Разрешения на совместный доступ могут иметь самые различные формы.
Ресурс **Permission** представляет эти формы с помощью аспектов в ресурсе.

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

## <a name="sharing-links"></a>Ссылки для общего доступа
Наиболее распространенный тип разрешений — ссылки для общего доступа.
Ссылки для общего доступа предоставляют уникальный URL-адрес, включающий ресурс, к которому предоставляется доступ, и маркер аутентификации, предоставляющий доступ к ресурсу. Пользователям не требуется выполнять вход для доступа к содержимому, предоставленному с помощью ссылки для общего доступа. Пользователи могут поделиться ссылкой, предоставляющей доступ к содержимому только для чтения или для чтения и записи.

### <a name="view-link"></a>Ссылка для просмотра
Ссылка для просмотра предоставляет доступ к элементу только для чтения.

<!-- {"blockType": "example", "@odata.type": "microsoft.graph.permission", "name": "permission-view-link" } -->
```json
{
  "id": "1",
  "roles": ["read"],
  "link": {
    "type": "view",
    "webUrl": "https://onedrive.live.com/redir?resid=5D33DD65C6932946!70859&authkey=!AL7N1QAfSWcjNU8&ithint=folder%2cgif",
    "application": { "id": "1234", "displayName": "Sample Application" }
  },
  "shareId": "!LKj1lkdlals90j1nlkascl"
}
```

### <a name="edit-link"></a>Ссылка для редактирования
Ссылка для редактирования предоставляет доступ к элементу для чтения и записи.

<!-- {"blockType": "example", "@odata.type": "microsoft.graph.permission", "name": "permission-edit-link" } -->
```json
{
  "id": "2",
  "roles": ["write"],
  "link": {
    "type": "edit",
    "webUrl": "https://onedrive.live.com/redir?resid=5D33DD65C6932946!70859&authkey=!AL7N1QAfSWcjNU8&ithint=folder%2cgif",
    "application": { "id": "1234", "displayName": "Sample Application" }
  },
  "shareId": "!LKj1lkdlals90j1nlkascl"
}
```

### <a name="sharing-invitation"></a>Приглашение к совместному использованию
Вы можете не только создавать ссылки для общего доступа, но и пригласить пользователя по электронному адресу.
В этом случае разрешение создает приглашение, отправляемое пользователю по электронной почте.

#### <a name="invitation-to-an-email-address"></a>Приглашение на электронный адрес
Если разрешение было отправлено по электронной почте получателю, у которого нет соответствующей учетной записи, то свойство **grantedTo** может быть не задано, пока приглашение не будет активировано (это происходит, когда пользователь впервые переходит по ссылке и выполняет вход).

<!-- {"blockType": "example", "@odata.type": "microsoft.graph.permission", "name": "permission-invite-email" } -->
```json
{
  "id": "1",
  "roles": ["write"],
  "invitation": {
    "email": "jd@gmail.com",
    "signInRequired": true
  },
  "shareId": "FWxc1lasfdbEAGM5fI7B67aB5ZMPDMmQ11U"
}
```

Когда пользователь активирует приглашение к совместному использованию, в свойстве **grantedTo** появятся сведения об учетной записи, которая активировала разрешения:

<!-- {"blockType": "example", "@odata.type": "microsoft.graph.permission", "name": "permission-invite-redeemed" } -->
```json
{
  "id": "1",
  "roles": ["write"],
  "grantedTo": {
    "user": {
      "id": "5D33DD65C6932946",
      "displayName": "John Doe"
    }
  },
  "invitation": {
    "email": "jd@outlook.com",
    "signInRequired": true
  },
  "shareId": "FWxc1lasfdbEAGM5fI7B67aB5ZMPDMmQ11U"
}
```

## <a name="methods"></a>Методы

| Метод                                                   | Путь REST
|:---------------------------------------------------------|:-----------------------
| [Получение списка разрешений](../api/driveitem_list_permissions.md) | `GET /drive/items/{item-id}/permissions`
| [Получение разрешения](../api/permission_get.md)               | `GET /drive/items/{item-id}/permissions/{id}`
| [Добавление](../api/driveitem_invite.md)                        | `POST /drive/items/{item-id}/invite`
| [Обновление](../api/permission_update.md)                    | `PATCH /drive/items/{item-id}/permissions/{id}`
| [Удаление](../api/permission_delete.md)                    | `DELETE /drive/items/{item-id}/permissions/{id}`


## <a name="remarks"></a>Заметки

Библиотеки документов OneDrive для бизнеса и SharePoint не возвращают свойство **inheritedFrom**.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The permission object provides information about permissions and roles and sharing information.",
  "keywords": "sharing,permissions,read,write,acl",
  "section": "documentation",
  "tocPath": "Resources/Permission"
} -->
