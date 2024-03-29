---
author: JeremyKelley
ms.date: 09/10/2017
title: Разрешение
ms.localizationpriority: high
description: Ресурс Permission содержит сведения о разрешении на совместный доступ, предоставленном для ресурса DriveItem.
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: ef2d30f7c239bdca21a3b9d643a91c83c7999b30
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2021
ms.locfileid: "61241424"
---
# <a name="permission-resource-type"></a>Тип ресурса Permission

Пространство имен: microsoft.graph

Ресурс **Permission** содержит сведения о разрешении на совместный доступ, предоставленном для ресурса [DriveItem](driveitem.md).

Разрешения на совместный доступ могут иметь самые различные формы.
Ресурс **permission** представляет эти формы с помощью аспектов в ресурсе.

Библиотеки документов OneDrive для бизнеса и SharePoint не возвращают свойство **inheritedFrom**.
Свойства **grantedTo** и **grantedToIdentities** в дальнейшем станут нерекомендуемыми, а отклик будет перенесен в **grantedToV2** и **grantedToIdentitiesV2** под соответствующими именами свойств.

## <a name="json-representation"></a>Представление JSON

Ниже показано представление JSON ресурса.

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "link",
    "grantedTo",
    "grantedToIdentities",
    "grantedToV2",
    "grantedToIdentitiesV2",
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
  "grantedToV2": {"@odata.type": "microsoft.graph.sharePointIdentitySet"},
  "grantedToIdentitiesV2": [{"@odata.type": "microsoft.graph.sharePointIdentitySet"}],
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

| Свойство                         | Тип                                      | Описание |
|:---------------------------------|:------------------------------------------|:-----------------
| id                               | Строка                                    | Уникальный идентификатор разрешения среди всех разрешений для элемента. Только для чтения. |
| grantedToV2                      | [SharePointIdentitySet][]                 | Для разрешений типа user: сведения о пользователях и приложениях для этого разрешения. Только для чтения. |
| grantedToIdentitiesV2            | Коллекция ([SharePointIdentitySet][]) | Для разрешений типа link: сведения о пользователях, которым предоставлено разрешение. Только для чтения. |
| invitation                       | [SharingInvitation][]                     | Сведения обо всех сопоставленных приглашениях к совместному использованию для данного разрешения. Только для чтения. |
| inheritedFrom                    | [ItemReference](itemreference.md)         | Предоставляет ссылку на предка текущего разрешения, если оно унаследовано от предка. Только для чтения. |
| ссылка                             | [SharingLink][]                           | Предоставляет сведения о ссылке для текущего разрешения, если это разрешение типа link. Только для чтения. |
| roles                            | Коллекция строк                      | Тип разрешения, например `read`. Полный список ролей см. ниже. Только для чтения. |
| shareId                          | Строка                                    | Уникальный токен, с помощью которого можно получить доступ к общему элементу через [API **shares**](../api/shares-get.md). Только для чтения. |
| expirationDateTime               | DateTimeOffset                            | Формат гггг-ММ-ддTЧЧ:мм:ссZ свойства DateTimeOffset указывает время окончания срока действия разрешения. DateTime.MinValue указывает, что для этого разрешения не установлен срок действия. Необязательно. |
| hasPassword                      | Логическое                                   | Указывает, установлен ли пароль для этого разрешения. Это свойство отображается только в отклике. Необязательно. Только для чтения. Только для личного хранилища OneDrive. |
| grantedTo (нерекомендуемое)           | [IdentitySet](identityset.md)             | Для разрешений типа user: сведения о пользователях и приложениях для этого разрешения. Только для чтения. |
| grantedToIdentities (нерекомендуемое) | Collection([IdentitySet](identityset.md)) | Для разрешений типа: сведения о пользователях, которым предоставлено разрешение. Только для чтения. |

Ресурс Permission предоставляет сведения о типе разрешения, представленного ресурсом, с помощью _аспектов_.

Разрешения с аспектом [**link**][SharingLink] представляют ссылки для совместного доступа, созданные в элементе. Ссылки для совместного доступа содержат уникальный токен, предоставляющий доступ к элементу любому пользователю, у которого есть такая ссылка.

Разрешения с аспектом [**invitation**][SharingInvitation] представляют разрешения, добавленные путем приглашения определенных пользователей или групп для доступа к файлу.

[SharingInvitation]: sharinginvitation.md
[SharingLink]: sharinglink.md
[SharePointIdentitySet]: sharePointIdentitySet.md

### <a name="roles-property-values"></a>Значения свойств роли

| Значение           | Описание                                                                        |
|:----------------|:-------------------------------------------------------------------------------|
| read            | Дает возможность считывать метаданные и содержимое элемента.            |
| write           | Дает возможность считывать и изменять метаданные и содержимое элемента. |
| owner           | В случае с SharePoint и OneDrive для бизнеса представляет роль владельца.       |

## <a name="sharing-links"></a>Предоставление ссылок
Наиболее распространенный тип разрешений — ссылки для общего доступа. Ссылки для общего доступа предоставляют уникальный URL-адрес, включающий ресурс, к которому предоставляется доступ, и маркер аутентификации, предоставляющий доступ к ресурсу. Пользователям не требуется выполнять вход для доступа к содержимому, предоставленному с помощью ссылки для общего доступа. Пользователи могут поделиться ссылкой, предоставляющей доступ к содержимому только для чтения или для чтения и записи.

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
  "shareId": "!LKj1lkdlals90j1nlkascl",
  "expirationDateTime&quot;: &quot;0001-01-01T00:00:00Z"
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
  "shareId": "!LKj1lkdlals90j1nlkascl",
  "expirationDateTime&quot;: &quot;0001-01-01T00:00:00Z"
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
        "displayName&quot;: &quot;Misty Suarez"
      }
    },
    {
       "user": {
        "id": "9397721fh4hgh73",
        "displayName&quot;: &quot;Judith Clemons"
      }
    }
  ],
  "grantedToIdentitiesV2": [
    {
       "user": {
        "id": "35fij1974gb8832",
        "displayName&quot;: &quot;Misty Suarez"
      },
      "siteUser": {
        "id": "1",
        "displayName": "Misty Suarez",
        "loginName&quot;: &quot;Misty Suarez"
      }
    },
    {
       "user": {
        "id": "9397721fh4hgh73",
        "displayName&quot;: &quot;Judith Clemons"
      },
      "siteUser": {
        "id": "2",
        "displayName": "Judith Clemons",
        "loginName&quot;: &quot;Judith Clemons"
      }
    }
  ],
  "roles": ["write"],
  "link": {
    "webUrl": "https://contoso.sharepoint.com/:w:/t/design/a577ghg9hgh737613bmbjf839026561fmzhsr85ng9f3hjck2t5s",
    "application": { "id": "1234", "displayName": "Sample Application" }
  },
  "shareId": "!LKj1lkdlals90j1nlkascl",
  "expirationDateTime&quot;: &quot;0001-01-01T00:00:00Z"
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
  "expirationDateTime&quot;: &quot;0001-01-01T00:00:00Z"
}
```

### <a name="sharing-invitation"></a>Приглашение к совместному использованию
Вы можете не только создавать ссылки для общего доступа, но и пригласить пользователя по электронному адресу. В этом случае разрешение создает приглашение, отправляемое пользователю по электронной почте.

#### <a name="invitation-to-an-email-address"></a>Приглашение на электронный адрес
Если разрешение было отправлено по электронной почте получателю, у которого нет соответствующей учетной записи, то свойство **grantedTo** может быть не задано, пока приглашение не будет активировано (это происходит, когда пользователь впервые переходит по ссылке и выполняет вход).

<!-- {"blockType": "example", "@odata.type": "microsoft.graph.permission", "name": "permission-invite-email" } -->
```json
{
  "id": "1",
  "roles": ["write"],
  "invitation": {
    "email": "jd@contoso.com",
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
      "displayName": "Robin Danielsen"
    }
  },
  "grantedToV2": {
    "user": {
      "id": "5D33DD65C6932946",
      "displayName": "Robin Danielsen"
    },
    "siteUser": {
      "id": "1",
      "displayName": "Robin Danielsen",
      "loginName": "Robin Danielsen"
    }
  },
  "invitation": {
    "email": "rd@contoso.com",
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
| [Добавление](../api/driveitem-invite.md)                        | `POST /drive/items/{item-id}/invite`
| [Обновление](../api/permission-update.md)                    | `PATCH /drive/items/{item-id}/permissions/{id}`
| [удаление](../api/permission-delete.md);                    | `DELETE /drive/items/{item-id}/permissions/{id}`
| [Добавление пользователей в ссылку совместного доступа](../api/permission-grant.md)  | `POST /shares/{encoded-sharing-url}/permission/grant`

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The permission object provides information about permissions and roles and sharing information.",
  "keywords": "sharing,permissions,read,write,acl",
  "section": "documentation",
  "tocPath": "Resources/Permission"
} -->
