---
author: JeremyKelley
ms.author: JeremyKelley
title: Тип ресурса разрешения
description: ресурс Permission, представляющий разрешение на совместный доступ, предоставленное для объекта driveItem
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: c35134e39618121f9aa7b29c490a6d8427b4a373
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2020
ms.locfileid: "43108202"
---
# <a name="permission-resource-type"></a>Тип ресурса разрешения

Пространство имен: microsoft.graph

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
| id                  | Строка                      | Уникальный идентификатор разрешения среди всех разрешений для элемента. Только для чтения.
| grantedTo           | [IdentitySet][]             | Для разрешений типа user: сведения о пользователях и приложениях для этого разрешения. Только для чтения.
| grantedToIdentities | Collection([IdentitySet][]) | Для разрешений типа link: сведения о пользователях, которым предоставлено разрешение. Только для чтения.
| invitation          | [SharingInvitation][]       | Сведения обо всех сопоставленных приглашениях к совместному использованию для данного разрешения. Только для чтения.
| inheritedFrom       | [ItemReference][]           | Предоставляет ссылку на предка текущего разрешения, если оно унаследовано от предка. Только для чтения.
| ссылка                | [SharingLink][]             | Предоставляет сведения о ссылке для текущего разрешения, если это разрешение типа link. Только для чтения.
| roles               | Collection(String)          | Тип разрешения, например `read`. Полный список ролей см. ниже. Только для чтения.
| shareId             | String                      | Уникальный маркер, с помощью которого можно получить доступ к общему элементу через **[API общих папок][]**. Только для чтения.
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

### <a name="view-link"></a>Ссылка для просмотра

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

### <a name="specific-people-link"></a>Ссылка для определенных пользователей

Эта ссылка предоставляет доступ для чтения и записи определенным пользователям в коллекции `grantedToIdentities`.

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

Разрешения, отправляемые API [INVITE][] или [предоставления][] , могут содержать дополнительные сведения в [invitation][SharingInvitation] аспекта приглашения для адресов электронной почты, которые не совпадают с известной учетной записью. В таких случаях свойство **грантедто** может быть настроено до тех пор, пока не будет активирована ссылка приглашения, которая возникает при первом щелчке ссылки и входе в систему.

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
| [Создание ссылки][createLink]                                | `POST /drive/items/{item-id}/createLink`
| [Приглашение участников][invite]                                  | `POST /drive/items/{item-id}/invite`
| [Обновление](../api/permission-update.md)                    | `PATCH /drive/items/{item-id}/permissions/{id}`
| [Удаление](../api/permission-delete.md)                    | `DELETE /drive/items/{item-id}/permissions/{id}`
| [Добавление пользователей в ссылку для общего доступа](../api/permission-grant.md)  | `POST /shares/{encoded-sharing-url}/permission/grant`


[createLink]: ../api/driveitem-createlink.md
[обладают]: ../api/permission-grant.md
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
