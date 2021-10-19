---
author: JeremyKelley
title: Тип ресурса разрешений
description: ресурс разрешений, представляющий разрешение общего доступа, выданного для driveItem
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: f2b58acc06b1a7478c2728f8e371fee67e917d3e
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/19/2021
ms.locfileid: "60493475"
---
# <a name="permission-resource-type"></a>Тип ресурса разрешений

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **разрешений** предоставляет сведения о разрешении общего доступа, предоставленного для [ресурса driveItem.](driveitem.md)

Разрешения на совместный доступ могут иметь самые различные формы.
Ресурс **разрешений** представляет эти различные формы с помощью аспектов на ресурсе.

>**Примечание.** OneDrive для бизнеса и SharePoint библиотеки документов не возвращают **наследуемую собственность.**

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
| id                  | Строка                      | Уникальный идентификатор разрешения среди всех разрешений для элемента. Только для чтения.
| grantedTo           | [IdentitySet][]             | Для разрешений типа user: сведения о пользователях и приложениях для этого разрешения. Только для чтения.
| grantedToIdentities | Collection([IdentitySet][]) | Для разрешений типа link: сведения о пользователях, которым предоставлено разрешение. Только для чтения.
| invitation          | [SharingInvitation][]       | Сведения обо всех сопоставленных приглашениях к совместному использованию для данного разрешения. Только для чтения.
| inheritedFrom       | [ItemReference][]           | Предоставляет ссылку на предка текущего разрешения, если оно унаследовано от предка. Только для чтения.
| ссылка                | [SharingLink][]             | Предоставляет сведения о ссылке для текущего разрешения, если это разрешение типа link. Только для чтения.
| roles               | Collection(String)          | Тип разрешения, например `read`. Полный список ролей см. ниже. Только для чтения.
| shareId             | String                      | Уникальный маркер, с помощью которого можно получить доступ к общему элементу с помощью **[API общих папок][]**. Только для чтения.
| expirationDateTime  | DateTimeOffset              | Формат гггг-ММ-ддTЧЧ:мм:ссZ свойства DateTimeOffset указывает время окончания срока действия разрешения. DateTime.MinValue указывает, что для этого разрешения не установлен срок действия. Необязательно.
| hasPassword         | Логическое                     | Указывает, настроен ли для этого разрешения пароль. Отображается только в отклике. Необязательно, только для чтения и предназначено только для OneDrive персональный.

### <a name="roles-property-values"></a>Значения свойств роли

| Значение              | Описание                                                                        |
|:------------------|:-------------------------------------------------------------------------------|
| read            | Дает возможность считывать метаданные и содержимое элемента.            |
| write           | Дает возможность считывать и изменять метаданные и содержимое элемента. |
| owner           | В случае с SharePoint и OneDrive для бизнеса представляет роль владельца.       |

Ресурс Permission предоставляет сведения о типе разрешения, представленного ресурсом, с помощью _аспектов_.

Ссылки совместного доступа содержат уникальный маркер, необходимый для доступа к элементу.

Разрешения с аспектом [**invitation**][SharingInvitation] представляют разрешения, добавленные путем приглашения определенных пользователей или групп для доступа к файлу.

## <a name="sharing-links"></a>Ссылки совместного доступа

Разрешения с аспектом [**link**][SharingLink] представляют ссылки для совместного доступа, созданные в элементе.
Это наиболее распространенные типы разрешений.
Ссылки для совместного доступа предоставляют уникальный URL-адрес, который можно использовать для доступа к файлу или папке.
Их можно настроить для предоставления доступа различными способами.
Например, вы можете использовать API [createLink][], чтобы создать ссылку, доступную любым пользователям, вошедшим в вашу организацию, или вы можете создать ссылку, доступную всем пользователями без необходимости входа.
Вы можете использовать API [приглашения][], чтобы создать ссылку, доступную только определенным пользователям, независимо от того, относятся ли они к вашей организации или нет.

Вот несколько примеров ссылок совместного доступа.

### <a name="view-link"></a>Просмотр ссылки

Эта ссылка для просмотра предоставляет доступ только для чтения любому пользователю с ссылкой.

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

Эта ссылка для редактирования предоставляет доступ для чтения и записи любому пользователю в организации, у которого есть ссылка.

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

### <a name="existing-access-link"></a>Существующая ссылка для доступа

Эта ссылка не предоставляет пользователю никаких дополнительных прав.

<!-- {"blockType": "example", "@odata.type": "microsoft.graph.permission", "name": "permission-existing-link" } -->

```json
{
  "id": "00000000-0000-0000-0000-000000000000",
  "roles": ["read"],
  "link": {
    "scope": "existingAccess",
    "type": "view",
    "webUrl": "https://contoso.sharepoint.com/:w:/t/design/Shared%20Documents/SampleDoc.docx?d=w12345",
  },
  "expirationDateTime": "0001-01-01T00:00:00Z"
}
```

### <a name="specific-people-link"></a>Ссылка для определенных пользователей

Эта ссылка предоставляет доступ для чтения и записи определенным пользователям в коллекции `grantedToIdentities`.

<!-- {"blockType": "example", truncated: true, "@odata.type": "microsoft.graph.permission", "name": "permission-people-link" } -->

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

## <a name="sharing-invitations"></a>Обмен приглашениями

Разрешения, отправленные [][] API приглашения или гранта, []могут иметь дополнительные сведения в аспекте[sharingInvitation] для адресов электронной почты, которые не соответствуют известной учетной записи. [][] В таких случаях свойство **grantedTo** не может быть установлено до тех пор, пока не будет выкуплена ссылка приглашения, что произойдет при первом щелчке пользователя по ссылке и вошел в нее.

<!-- {"blockType": "example", truncated: true, "@odata.type": "microsoft.graph.permission", "name": "permission-invite-email" } -->

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

<!-- {"blockType": "example", truncated: true,"@odata.type": "microsoft.graph.permission", "name": "permission-invite-redeemed" } -->

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
| [Создание ссылки][createLink]                                | `POST /drive/items/{item-id}/createLink`
| [Приглашение участников][invite]                                  | `POST /drive/items/{item-id}/invite`
| [Обновление](../api/permission-update.md)                    | `PATCH /drive/items/{item-id}/permissions/{id}`
| [удаление](../api/permission-delete.md);                    | `DELETE /drive/items/{item-id}/permissions/{id}`
| [Добавление пользователей в ссылку совместного доступа](../api/permission-grant.md)  | `POST /shares/{encoded-sharing-url}/permission/grant`
| [Отоимка грантов](../api/permission-revokegrants.md)   | `POST /drive/items/{item-id}/permissions/{id}/revokeGrants`

[createLink]: ../api/driveitem-createlink.md
[грант]: ../api/permission-grant.md
[IdentitySet]: identityset.md
[invite]: ../api/driveitem-invite.md
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
  "suppressions": []
}
-->
