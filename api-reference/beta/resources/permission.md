---
author: JeremyKelley
ms.author: JeremyKelley
title: Тип ресурса разрешения
description: ресурс Permission, представляющий разрешение на совместный доступ, предоставленное для объекта driveItem
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 3f74ecd71a9f411a336c7fb4b5720208ca0ffa42
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966183"
---
# <a name="permission-resource-type"></a>Тип ресурса разрешения

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **Permission** предоставляет сведения о разрешении на совместный доступ, предоставленном для ресурса [driveItem](driveitem.md) .

Разрешения на совместный доступ могут иметь самые различные формы.
Ресурс **Permission** представляет эти различные формы с помощью аспектов ресурса.

>**Примечание:** Библиотеки документов OneDrive для бизнеса и SharePoint не возвращают свойство **inheritedFrom** .

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
| Грантедтоидентитиес | Collection ([Identity][]) | Для разрешений типа ссылки — сведения о пользователях, которым предоставлено разрешение. Только для чтения.
| invitation          | [SharingInvitation][]       | Сведения обо всех сопоставленных приглашениях к совместному использованию для данного разрешения. Только для чтения.
| inheritedFrom       | [ItemReference][]           | Предоставляет ссылку на предка текущего разрешения, если оно унаследовано от предка. Только для чтения.
| ссылка                | [SharingLink][]             | Предоставляет сведения о ссылке для текущего разрешения, если это разрешение типа link. Только для чтения.
| roles               | Collection(String)          | Тип разрешения, например `read`. Полный список ролей см. ниже. Только для чтения.
| shareId             | Строка                      | Уникальный маркер, который можно использовать для доступа к общему элементу через **[API shares][]**. Только для чтения.
| expirationDateTime  | DateTimeOffset              | Формат YYYY – MM – ДДВчч: mm: ССЧП of DateTimeOffset указывает срок действия разрешения. DateTime. MinValue указывает, что для этого разрешения не задано действие срока действия. Необязательно.
| hasPassword         | Boolean                     | Указывает, задан ли для этого разрешения пароль, который отображается в ответе. Необязательный и только для чтения и только для OneDrive персональный.

### <a name="roles-enumeration-values"></a>Значения перечислений ролей

| Значение        | Сведения                                                                        |
|:------------|:-------------------------------------------------------------------------------|
| `read`      | Дает возможность считывать метаданные и содержимое элемента.            |
| `write`     | Дает возможность считывать и изменять метаданные и содержимое элемента. |
| `sp.owner`  | В случае с SharePoint и OneDrive для бизнеса представляет роль владельца.       |
| `sp.member` | В случае с SharePoint и OneDrive для бизнеса представляет роль участника.      |

Ресурс Permission предоставляет сведения о типе разрешения, представленного ресурсом, с помощью _аспектов_.

Ссылки для общего доступа содержат уникальный маркер, необходимый для доступа к элементу.

Разрешения с аспектом [**invitation**][SharingInvitation] представляют разрешения, добавленные путем приглашения определенных пользователей или групп для доступа к файлу.

## <a name="sharing-links"></a>Предоставление ссылок

Разрешения с аспектом [**link**][SharingLink] представляют ссылки для совместного доступа, созданные в элементе.
Это наиболее распространенные типы разрешений.
Ссылки для общего доступа предоставляют уникальный URL-адрес, который можно использовать для доступа к файлу или папке.
Их можно настроить для предоставления доступа различными способами.
Например, вы можете использовать API [CreateLink][] , чтобы создать ссылку для всех пользователей, которые вошли в организацию, или создать ссылку, которая будет работать для всех пользователей, не требуя входа в систему.
Вы можете использовать API [INVITE][] , чтобы создать ссылку, которая работает только для определенных пользователей, независимо от того, находитесь ли они в вашей компании.

Ниже приведено несколько примеров ссылок для общего доступа.

### <a name="view-link"></a>Ссылка для просмотра

Эта ссылка для просмотра предоставляет доступ только для чтения всем пользователям, у которых есть ссылка.

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

Эта ссылка для редактирования предоставляет доступ для чтения и записи ко всем пользователям в Организации со ссылкой.

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

### <a name="existing-access-link"></a>Существующая ссылка доступа

Эта ссылка не предоставляет пользователю никаких дополнительных привилегий.

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

### <a name="specific-people-link"></a>Ссылка на конкретные люди

Эта ссылка обеспечивает доступ для чтения и записи к определенным пользователям в `grantedToIdentities` коллекции.

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

## <a name="sharing-invitations"></a>Приглашение на общий доступ

Разрешения, отправляемые API [INVITE][] или [предоставления][] , могут содержать дополнительные сведения в [][SharingInvitation] аспекта приглашения для адресов электронной почты, которые не совпадают с известной учетной записью. В таких случаях свойство **грантедто** может быть настроено до тех пор, пока не будет активирована ссылка приглашения, которая возникает при первом щелчке ссылки и входе в систему.

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
| [Создание ссылки] [CreateLink]                                | `POST /drive/items/{item-id}/createLink`
| [Приглашение пользователей] [пригласить]                                  | `POST /drive/items/{item-id}/invite`
| [Обновление](../api/permission-update.md)                    | `PATCH /drive/items/{item-id}/permissions/{id}`
| [удаление](../api/permission-delete.md);                    | `DELETE /drive/items/{item-id}/permissions/{id}`



[createLink]: ../api/driveitem-createlink.md
[обладают]: ../api/permission-grant.md
[IdentitySet]: identityset.md
[ложите]: ../api/driveitem-invite.md
[ItemReference]: itemreference.md
[API общих ресурсов]: ../api/shares-get.md
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
