---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Permission
localization_priority: Normal
ms.openlocfilehash: 6a5a0af9c95900232ff87aa7aedb731a83a91cc5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518851"
---
# <a name="permission-resource-type"></a>Тип ресурса Permission

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **Permission** предоставляет сведения о разрешении на совместный доступ, предоставленном для ресурса [DriveItem](driveitem.md).

Разрешения на совместный доступ могут принимать самые различные формы.
Ресурс **Permission** представляет эти формы с помощью аспектов ресурса.

>**Примечание:** OneDrive для бизнеса и SharePoint библиотек документов не возвращают свойство **inheritedFrom** .

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "link",
    "grantedTo",
    "grantedToIdentities",
    "invitation",
    "inheritedFrom",
    "shareId",
    "expirationDateTime",
    "hasPassword"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.permission"
}-->

```json
{
  "id": "string (identifier)",
  "grantedTo": {"@odata.type": "microsoft.graph.identitySet"},
  "grantedToIdentities": [{"@odata.type": "microsoft.graph.identitySet"}],
  "inheritedFrom": {"@odata.type": "microsoft.graph.itemReference"},
  "invitation": {"@odata.type": "microsoft.graph.sharingInvitation"},
  "link": {"@odata.type": "microsoft.graph.sharingLink"},
  "roles": ["string"],
  "shareId": "string",
  "expirationDateTime": "string (timestamp)",
  "hasPassword": "boolean"
}
```

## <a name="properties"></a>Свойства

| Свойство            | Тип                        | Описание
|:--------------------|:----------------------------|:-------------------------
| id                  | String                      | Уникальный идентификатор разрешения среди всех разрешений для элемента. Только для чтения.
| grantedTo           | [IdentitySet][]             | Для разрешений типа user: сведения о пользователях и приложениях для этого разрешения. Только для чтения.
| grantedToIdentities | Коллекции ([IdentitySet][]) | Для разрешения ссылок типа сведения о пользователях, которым были предоставлены разрешения. Только для чтения.
| invitation          | [SharingInvitation][]       | Сведения обо всех сопоставленных приглашениях к совместному использованию для данного разрешения. Только для чтения.
| inheritedFrom       | [ItemReference][]           | Предоставляет ссылку на предка текущего разрешения, если оно унаследовано от предка. Только для чтения.
| ссылка                | [SharingLink][]             | Предоставляет сведения о ссылке для текущего разрешения, если это разрешение типа link. Только для чтения.
| roles               | Collection(String)          | Тип разрешения, например `read`. Полный список ролей см. ниже. Только для чтения.
| shareId             | String                      | Уникальный токен, с помощью которого можно получить доступ к общему элементу через **API [shares][]**. Только для чтения.
| expirationDateTime  | DateTimeOffset              | В формате гггг-мм-Ддвчч DateTimeOffset указывает время истечения срока действия разрешения. DateTime.MinValue указывает на наличие задано без ограничения срока действия для этого разрешения. Необязательный параметр.
| HasPassword         | Логическое                     | Указывает, будет ли для этого разрешения, задать пароль, отображаются в ответ. Необязательный и только для чтения и только личные OneDrive.

### <a name="roles-enumeration-values"></a>Значения перечисления роли

| Значение        | Сведения                                                                        |
|:------------|:-------------------------------------------------------------------------------|
| `read`      | Дает возможность считывать метаданные и содержимое элемента.            |
| `write`     | Дает возможность считывать и изменять метаданные и содержимое элемента. |
| `sp.owner`  | В случае с SharePoint и OneDrive для бизнеса представляет роль владельца.       |
| `sp.member` | В случае с SharePoint и OneDrive для бизнеса представляет роль участника.      |

Ресурс Permission предоставляет сведения о типе разрешения, представленного ресурсом, с помощью _аспектов_.

Общего доступа ссылки содержат уникальный маркер, необходимые для доступа к элементу.

Разрешения с аспектом [**invitation**][SharingInvitation] представляют разрешения, добавленные путем приглашения определенных пользователей или групп для доступа к файлу.

## <a name="sharing-links"></a>Ссылки для общего доступа

Разрешения с помощью представляют аспекта[SharingLink] [**ссылок**], общий доступ к ссылок, созданных для элемента.
Это наиболее распространенных типов разрешений.
Общего доступа к ссылкам уникальных URL-адрес, который можно использовать для доступа к файлу или папки.
Они могут настраиваться для предоставления доступа в различными способами.
Например можно использовать [команду createLink][] API для создания связи, которая работает для всех вошел в вашей организации, или можно создать ссылку, которая работает для всех пользователей, без необходимости входа в.
[Приглашение][] API можно использовать для создания ссылок, который работает только для определенных пользователей ли они в вашей компании или нет.

Ниже приведены некоторые примеры того, общий доступ к ссылки.

### <a name="view-link"></a>Ссылка для просмотра

В этом представлении ссылку предоставляет доступ только для чтения всем пользователям, с помощью ссылки.

<!-- {"blockType": "example", "@odata.type": "microsoft.graph.permission", "name": "permission-view-link" } -->

```json
{
  "id": "1",
  "roles": ["read"],
  "link": {
    "scope": "anonymous",
    "type": "view",
    "webUrl": "https://onedrive.live.com/redir?resid=5D33DD65C6932946!70859&authkey=!AL7N1QAfSWcjNU8&ithint=folder%2cgif",
    "application": { "id": "1234", "displayName": "Sample Application" }
  },
  "shareId": "!LKj1lkdlals90j1nlkascl",
  "expirationDateTime": "0001-01-01T00:00:00Z"
}
```

### <a name="edit-link"></a>Ссылка для редактирования

В этом ссылку Изменение предоставляет доступ на чтение и запись всем пользователям в организации с помощью ссылки.

<!-- {"blockType": "example", "@odata.type": "microsoft.graph.permission", "name": "permission-edit-link" } -->

```json
{
  "id": "2ceefb3g32hh",
  "roles": ["write"],
  "link": {
    "scope": "organization",
    "type": "edit",
    "webUrl": "https://contoso.sharepoint.com/:w:/t/design/fj277ghautbb422707565gnvg23",
    "application": { "id": "1234", "displayName": "Sample Application" }
  },
  "shareId": "!LKj1lkdlals90j1nlkascl",
  "expirationDateTime": "0001-01-01T00:00:00Z"
}
```

### <a name="specific-people-link"></a>Конкретные пользователи ссылок

Ссылка на чтение и запись для конкретных пользователей в `grantedToIdentities` семейства сайтов.

<!-- {"blockType": "example", "@odata.type": "microsoft.graph.permission", "name": "permission-people-link" } -->

```json
{
  "id": "3",
  "grantedToIdentities": [
    {
       "user": {
        "id": "35fij1974gb8832",
        "displayName": "Misty Suarez"
      }
    },
    {
       "user": {
        "id": "9397721fh4hgh73",
        "displayName": "Judith Clemons"
      }
    }
  ],
  "roles": ["write"],
  "link": {
    "webUrl": "https://contoso.sharepoint.com/:w:/t/design/a577ghg9hgh737613bmbjf839026561fmzhsr85ng9f3hjck2t5s",
    "application": { "id": "1234", "displayName": "Sample Application" }
  },
  "shareId": "!LKj1lkdlals90j1nlkascl",
  "expirationDateTime": "0001-01-01T00:00:00Z"
}
```

## <a name="sharing-invitations"></a>Общий доступ к приглашений

Разрешения, отправленные с [Пригласить][] API могут предоставить дополнительную информацию в аспекта[SharingInvitation] [приглашение].
Если приглашение было отправлено на адрес электронной почты, соответствует известной учетной записи, свойство **grantedTo** может не задано, пока погашен приглашение, которое происходит при первом пользователь щелкает ссылку и подписывает.

<!-- {"blockType": "example", "@odata.type": "microsoft.graph.permission", "name": "permission-invite-email" } -->

```json
{
  "id": "1",
  "roles": ["write"],
  "invitation": {
    "email": "jd@fabrikam.com",
    "signInRequired": true
  },
  "shareId": "FWxc1lasfdbEAGM5fI7B67aB5ZMPDMmQ11U",
  "expirationDateTime": "0001-01-01T00:00:00Z"
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
    "email": "jd@fabrikam.com",
    "signInRequired": true
  },
  "shareId": "FWxc1lasfdbEAGM5fI7B67aB5ZMPDMmQ11U",
  "expirationDateTime": "0001-01-01T00:00:00Z"
}
```

## <a name="methods"></a>Методы

| Метод                                                   | Путь REST
|:---------------------------------------------------------|:-----------------------
| [Получение списка разрешений](../api/driveitem-list-permissions.md) | `GET /drive/items/{item-id}/permissions`
| [Получение разрешения](../api/permission-get.md)               | `GET /drive/items/{item-id}/permissions/{id}`
| [Создать ссылку] [команду createLink]                                | `POST /drive/items/{item-id}/createLink`
| [Приглашение пользователей] [приглашение]                                  | `POST /drive/items/{item-id}/invite`
| [Обновление](../api/permission-update.md)                    | `PATCH /drive/items/{item-id}/permissions/{id}`
| [удаление](../api/permission-delete.md);                    | `DELETE /drive/items/{item-id}/permissions/{id}`



[команду createLink]: ../api/driveitem-createlink.md
[IdentitySet]: identityset.md
[Приглашение]: ../api/driveitem-invite.md
[ItemReference]: itemreference.md
[API общих папок]: ../api/shares-get.md
[SharingInvitation]: sharinginvitation.md
[SharingLink]: sharinglink.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The permission object provides information about permissions and roles and sharing information.",
  "keywords": "sharing,permissions,read,write,acl",
  "section": "documentation",
  "tocPath": "Resources/Permission",
  "suppressions": [
    "Error: /api-reference/beta/resources/permission.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
