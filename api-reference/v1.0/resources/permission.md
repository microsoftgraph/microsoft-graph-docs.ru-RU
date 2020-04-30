---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Разрешение
localization_priority: Priority
description: Ресурс Permission содержит сведения о разрешении на совместный доступ, предоставленном для ресурса DriveItem.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 5c4b881aaf10a56b65342dccebd417867c2b7b26
ms.sourcegitcommit: 9b507499fb1ec61b4de47f36f915ae29c8594459
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2020
ms.locfileid: "43934705"
---
# <a name="permission-resource-type"></a><span data-ttu-id="e9a86-103">Тип ресурса Permission</span><span class="sxs-lookup"><span data-stu-id="e9a86-103">Permission resource type</span></span>

<span data-ttu-id="e9a86-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9a86-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e9a86-105">Ресурс **Permission** содержит сведения о разрешении на совместный доступ, предоставленном для ресурса [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="e9a86-105">The **Permission** resource provides information about a sharing permission granted for a [DriveItem](driveitem.md) resource.</span></span>

<span data-ttu-id="e9a86-106">Разрешения на совместный доступ могут иметь самые различные формы.</span><span class="sxs-lookup"><span data-stu-id="e9a86-106">Sharing permissions have a number of different forms.</span></span>
<span data-ttu-id="e9a86-107">Ресурс **Permission** представляет эти формы с помощью аспектов в ресурсе.</span><span class="sxs-lookup"><span data-stu-id="e9a86-107">The **Permission** resource represents these different forms through facets on the resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e9a86-108">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e9a86-108">JSON representation</span></span>

<span data-ttu-id="e9a86-109">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="e9a86-109">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="e9a86-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="e9a86-110">Properties</span></span>

| <span data-ttu-id="e9a86-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="e9a86-111">Property</span></span>      | <span data-ttu-id="e9a86-112">Тип</span><span class="sxs-lookup"><span data-stu-id="e9a86-112">Type</span></span>                                      | <span data-ttu-id="e9a86-113">Описание</span><span class="sxs-lookup"><span data-stu-id="e9a86-113">Description</span></span>
|:--------------|:------------------------------------------|:-----------------
| <span data-ttu-id="e9a86-114">id</span><span class="sxs-lookup"><span data-stu-id="e9a86-114">id</span></span>            | <span data-ttu-id="e9a86-115">Строка</span><span class="sxs-lookup"><span data-stu-id="e9a86-115">String</span></span>                                    | <span data-ttu-id="e9a86-p102">Уникальный идентификатор разрешения среди всех разрешений для элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e9a86-p102">The unique identifier of the permission among all permissions on the item. Read-only.</span></span>
| <span data-ttu-id="e9a86-118">grantedTo</span><span class="sxs-lookup"><span data-stu-id="e9a86-118">grantedTo</span></span>     | [<span data-ttu-id="e9a86-119">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="e9a86-119">IdentitySet</span></span>](identityset.md)             | <span data-ttu-id="e9a86-p103">Для разрешений типа user: сведения о пользователях и приложениях для этого разрешения. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e9a86-p103">For user type permissions, the details of the users & applications for this permission. Read-only.</span></span>
| <span data-ttu-id="e9a86-122">grantedToIdentities</span><span class="sxs-lookup"><span data-stu-id="e9a86-122">grantedToIdentities</span></span> | <span data-ttu-id="e9a86-123">Collection([IdentitySet](identityset.md))</span><span class="sxs-lookup"><span data-stu-id="e9a86-123">Collection([IdentitySet](identityset.md))</span></span> | <span data-ttu-id="e9a86-124">Для разрешений типа link: сведения о пользователях, которым предоставлено разрешение.</span><span class="sxs-lookup"><span data-stu-id="e9a86-124">For link type permissions, the details of the users to whom permission was granted.</span></span> <span data-ttu-id="e9a86-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e9a86-125">Read-only.</span></span>
| <span data-ttu-id="e9a86-126">invitation</span><span class="sxs-lookup"><span data-stu-id="e9a86-126">invitation</span></span>    | <span data-ttu-id="e9a86-127">[SharingInvitation][]</span><span class="sxs-lookup"><span data-stu-id="e9a86-127">[SharingInvitation][]</span></span>                     | <span data-ttu-id="e9a86-p105">Сведения обо всех сопоставленных приглашениях к совместному использованию для данного разрешения. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e9a86-p105">Details of any associated sharing invitation for this permission. Read-only.</span></span>
| <span data-ttu-id="e9a86-130">inheritedFrom</span><span class="sxs-lookup"><span data-stu-id="e9a86-130">inheritedFrom</span></span> | [<span data-ttu-id="e9a86-131">ItemReference</span><span class="sxs-lookup"><span data-stu-id="e9a86-131">ItemReference</span></span>](itemreference.md)         | <span data-ttu-id="e9a86-p106">Предоставляет ссылку на предка текущего разрешения, если оно унаследовано от предка. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e9a86-p106">Provides a reference to the ancestor of the current permission, if it is inherited from an ancestor. Read-only.</span></span>
| <span data-ttu-id="e9a86-134">ссылка</span><span class="sxs-lookup"><span data-stu-id="e9a86-134">link</span></span>          | <span data-ttu-id="e9a86-135">[SharingLink][]</span><span class="sxs-lookup"><span data-stu-id="e9a86-135">[SharingLink][]</span></span>                           | <span data-ttu-id="e9a86-p107">Предоставляет сведения о ссылке для текущего разрешения, если это разрешение типа link. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e9a86-p107">Provides the link details of the current permission, if it is a link type permissions. Read-only.</span></span>
| <span data-ttu-id="e9a86-138">roles</span><span class="sxs-lookup"><span data-stu-id="e9a86-138">roles</span></span>         | <span data-ttu-id="e9a86-139">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="e9a86-139">Collection of String</span></span>                      | <span data-ttu-id="e9a86-p108">Тип разрешения, например `read`. Полный список ролей см. ниже. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e9a86-p108">The type of permission, e.g. `read`. See below for the full list of roles. Read-only.</span></span>
| <span data-ttu-id="e9a86-143">shareId</span><span class="sxs-lookup"><span data-stu-id="e9a86-143">shareId</span></span>       | <span data-ttu-id="e9a86-144">Строка</span><span class="sxs-lookup"><span data-stu-id="e9a86-144">String</span></span>                                    | <span data-ttu-id="e9a86-p109">Уникальный токен, с помощью которого можно получить доступ к общему элементу через [API **shares**](../api/shares-get.md). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e9a86-p109">A unique token that can be used to access this shared item via the [**shares** API](../api/shares-get.md). Read-only.</span></span>
| <span data-ttu-id="e9a86-147">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="e9a86-147">expirationDateTime</span></span>  | <span data-ttu-id="e9a86-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e9a86-148">DateTimeOffset</span></span>              | <span data-ttu-id="e9a86-149">Формат гггг-ММ-ддTЧЧ:мм:ссZ свойства DateTimeOffset указывает время окончания срока действия разрешения.</span><span class="sxs-lookup"><span data-stu-id="e9a86-149">A format of yyyy-MM-ddTHH:mm:ssZ of DateTimeOffset indicates the expiration time of the permission.</span></span> <span data-ttu-id="e9a86-150">DateTime.MinValue указывает, что для этого разрешения не установлен срок действия.</span><span class="sxs-lookup"><span data-stu-id="e9a86-150">DateTime.MinValue indicates there is no expiration set for this permission.</span></span> <span data-ttu-id="e9a86-151">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="e9a86-151">Optional.</span></span>
| <span data-ttu-id="e9a86-152">hasPassword</span><span class="sxs-lookup"><span data-stu-id="e9a86-152">hasPassword</span></span>         | <span data-ttu-id="e9a86-153">Логическое</span><span class="sxs-lookup"><span data-stu-id="e9a86-153">Boolean</span></span>                     | <span data-ttu-id="e9a86-154">Указывает, настроен ли для этого разрешения пароль. Отображается только в отклике.</span><span class="sxs-lookup"><span data-stu-id="e9a86-154">This indicates whether password is set for this permission, it's only showing in response.</span></span> <span data-ttu-id="e9a86-155">Необязательно, только для чтения и предназначено только для OneDrive персональный.</span><span class="sxs-lookup"><span data-stu-id="e9a86-155">Optional and Read-only and for OneDrive Personal only.</span></span>

<span data-ttu-id="e9a86-156">Ресурс Permission предоставляет сведения о типе разрешения, представленного ресурсом, с помощью _аспектов_.</span><span class="sxs-lookup"><span data-stu-id="e9a86-156">The permission resource uses _facets_ to provide information about the kind of permission represented by the resource.</span></span>

<span data-ttu-id="e9a86-p112">Разрешения с аспектом [**link**][SharingLink] представляют ссылки для совместного доступа, созданные в элементе. Ссылки для совместного доступа содержат уникальный токен, предоставляющий доступ к элементу любому пользователю, у которого есть такая ссылка.</span><span class="sxs-lookup"><span data-stu-id="e9a86-p112">Permissions with a [**link**][SharingLink] facet represent sharing links created on the item. Sharing links contain a unique token that provides access to the item for anyone with the link.</span></span>

<span data-ttu-id="e9a86-159">Разрешения с аспектом [**invitation**][SharingInvitation] представляют разрешения, добавленные путем приглашения определенных пользователей или групп для доступа к файлу.</span><span class="sxs-lookup"><span data-stu-id="e9a86-159">Permissions with an [**invitation**][SharingInvitation] facet represent permissions added by inviting specific users or groups to have access to the file.</span></span>

[SharingInvitation]: sharinginvitation.md
[SharingLink]: sharinglink.md

### <a name="roles-property-values"></a><span data-ttu-id="e9a86-162">Значения свойств роли</span><span class="sxs-lookup"><span data-stu-id="e9a86-162">Roles property values</span></span>

| <span data-ttu-id="e9a86-163">Роль</span><span class="sxs-lookup"><span data-stu-id="e9a86-163">Role</span></span>        | <span data-ttu-id="e9a86-164">Сведения</span><span class="sxs-lookup"><span data-stu-id="e9a86-164">Details</span></span>                                                                        |
|:------------|:-------------------------------------------------------------------------------|
| `read`      | <span data-ttu-id="e9a86-165">Дает возможность считывать метаданные и содержимое элемента.</span><span class="sxs-lookup"><span data-stu-id="e9a86-165">Provides the ability to read the metadata and contents of the item.</span></span>            |
| `write`     | <span data-ttu-id="e9a86-166">Дает возможность считывать и изменять метаданные и содержимое элемента.</span><span class="sxs-lookup"><span data-stu-id="e9a86-166">Provides the ability to read and modify the metadata and contents of the item.</span></span> |
| `sp.owner`  | <span data-ttu-id="e9a86-167">В случае с SharePoint и OneDrive для бизнеса представляет роль владельца.</span><span class="sxs-lookup"><span data-stu-id="e9a86-167">For SharePoint and OneDrive for Business this represents the owner role.</span></span>       |
| `sp.member` | <span data-ttu-id="e9a86-168">В случае с SharePoint и OneDrive для бизнеса представляет роль участника.</span><span class="sxs-lookup"><span data-stu-id="e9a86-168">For SharePoint and OneDrive for Business this represents the member role.</span></span>      |

## <a name="sharing-links"></a><span data-ttu-id="e9a86-169">Предоставление ссылок</span><span class="sxs-lookup"><span data-stu-id="e9a86-169">Sharing links</span></span>
<span data-ttu-id="e9a86-p113">Наиболее распространенный тип разрешений — ссылки для общего доступа. Ссылки для общего доступа предоставляют уникальный URL-адрес, включающий ресурс, к которому предоставляется доступ, и маркер аутентификации, предоставляющий доступ к ресурсу. Пользователям не требуется выполнять вход для доступа к содержимому, предоставленному с помощью ссылки для общего доступа. Пользователи могут поделиться ссылкой, предоставляющей доступ к содержимому только для чтения или для чтения и записи.</span><span class="sxs-lookup"><span data-stu-id="e9a86-p113">The most common type of permissions are sharing links. Sharing links provide a unique URL that includes both the resource being shared and an authentication token that provides access to the resource. Users don't need to sign-in to access the content shared with a sharing link. Users can share a link that gives read-only access to the content or writable access to the content.</span></span>

### <a name="view-link"></a><span data-ttu-id="e9a86-174">Ссылка для просмотра</span><span class="sxs-lookup"><span data-stu-id="e9a86-174">View Link</span></span>
<span data-ttu-id="e9a86-175">Ссылка для просмотра предоставляет доступ к элементу только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e9a86-175">A view link provides read-only access to an item.</span></span>

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
  "expirationDateTime": "0001-01-01T00:00:00Z"
}
```

### <a name="edit-link"></a><span data-ttu-id="e9a86-176">Ссылка для редактирования</span><span class="sxs-lookup"><span data-stu-id="e9a86-176">Edit link</span></span>
<span data-ttu-id="e9a86-177">Ссылка для редактирования предоставляет доступ к элементу для чтения и записи.</span><span class="sxs-lookup"><span data-stu-id="e9a86-177">An edit link provides read and write access to an item.</span></span>

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
  "expirationDateTime": "0001-01-01T00:00:00Z"
}
```
### <a name="specific-people-link"></a><span data-ttu-id="e9a86-178">Ссылка для определенных пользователей</span><span class="sxs-lookup"><span data-stu-id="e9a86-178">Specific people link</span></span>

<span data-ttu-id="e9a86-179">Эта ссылка предоставляет доступ для чтения и записи определенным пользователям в коллекции `grantedToIdentities`.</span><span class="sxs-lookup"><span data-stu-id="e9a86-179">This link provides read and write access to the specific people in the `grantedToIdentities` collection.</span></span>

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

### <a name="existing-access-link"></a><span data-ttu-id="e9a86-180">Существующая ссылка для доступа</span><span class="sxs-lookup"><span data-stu-id="e9a86-180">Existing access link</span></span>

<span data-ttu-id="e9a86-181">Эта ссылка не предоставляет пользователю никаких дополнительных прав.</span><span class="sxs-lookup"><span data-stu-id="e9a86-181">This link does not grant any additional privileges to the user.</span></span>

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

### <a name="sharing-invitation"></a><span data-ttu-id="e9a86-182">Приглашение к совместному использованию</span><span class="sxs-lookup"><span data-stu-id="e9a86-182">Sharing Invitation</span></span>
<span data-ttu-id="e9a86-p114">Вы можете не только создавать ссылки для общего доступа, но и пригласить пользователя по электронному адресу. В этом случае разрешение создает приглашение, отправляемое пользователю по электронной почте.</span><span class="sxs-lookup"><span data-stu-id="e9a86-p114">In addition to creating sharing links, a user can be invited by e-mail address. In this scenario the permission creates an invitation that is sent to the user's email.</span></span>

#### <a name="invitation-to-an-email-address"></a><span data-ttu-id="e9a86-185">Приглашение на электронный адрес</span><span class="sxs-lookup"><span data-stu-id="e9a86-185">Invitation to an email address</span></span>
<span data-ttu-id="e9a86-186">Если разрешение было отправлено по электронной почте получателю, у которого нет соответствующей учетной записи, то свойство **grantedTo** может быть не задано, пока приглашение не будет активировано (это происходит, когда пользователь впервые переходит по ссылке и выполняет вход).</span><span class="sxs-lookup"><span data-stu-id="e9a86-186">If the permission was sent via an email address to a recipient who does not have a matching account, the **grantedTo** property may not be set until the invitation is redeemed, which occurs the first time a user clicks the link and signs in.</span></span>

<!-- {"blockType": "example", "@odata.type": "microsoft.graph.permission", "name": "permission-invite-email" } -->
```json
{
  "id": "1",
  "roles": ["write"],
  "invitation": {
    "email": "jd@gmail.com",
    "signInRequired": true
  },
  "shareId": "FWxc1lasfdbEAGM5fI7B67aB5ZMPDMmQ11U",
  "expirationDateTime": "0001-01-01T00:00:00Z"
}
```

<span data-ttu-id="e9a86-187">Когда пользователь активирует приглашение к совместному использованию, в свойстве **grantedTo** появятся сведения об учетной записи, которая активировала разрешения:</span><span class="sxs-lookup"><span data-stu-id="e9a86-187">After the sharing invitation has been redeemed by a user, the **grantedTo** property will contain the information about the account that redeemed the permissions:</span></span>

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
  "shareId": "FWxc1lasfdbEAGM5fI7B67aB5ZMPDMmQ11U",
  "expirationDateTime": "0001-01-01T00:00:00Z"
}
```

## <a name="methods"></a><span data-ttu-id="e9a86-188">Методы</span><span class="sxs-lookup"><span data-stu-id="e9a86-188">Methods</span></span>

| <span data-ttu-id="e9a86-189">Метод</span><span class="sxs-lookup"><span data-stu-id="e9a86-189">Method</span></span>                                                   | <span data-ttu-id="e9a86-190">Путь REST</span><span class="sxs-lookup"><span data-stu-id="e9a86-190">REST Path</span></span>
|:---------------------------------------------------------|:-----------------------
| [<span data-ttu-id="e9a86-191">Получение списка разрешений</span><span class="sxs-lookup"><span data-stu-id="e9a86-191">List permissions</span></span>](../api/driveitem-list-permissions.md) | `GET /drive/items/{item-id}/permissions`
| [<span data-ttu-id="e9a86-192">Получение разрешения</span><span class="sxs-lookup"><span data-stu-id="e9a86-192">Get permission</span></span>](../api/permission-get.md)               | `GET /drive/items/{item-id}/permissions/{id}`
| [<span data-ttu-id="e9a86-193">Добавление</span><span class="sxs-lookup"><span data-stu-id="e9a86-193">Add</span></span>](../api/driveitem-invite.md)                        | `POST /drive/items/{item-id}/invite`
| [<span data-ttu-id="e9a86-194">Обновление</span><span class="sxs-lookup"><span data-stu-id="e9a86-194">Update</span></span>](../api/permission-update.md)                    | `PATCH /drive/items/{item-id}/permissions/{id}`
| <span data-ttu-id="e9a86-195">[удаление](../api/permission-delete.md);</span><span class="sxs-lookup"><span data-stu-id="e9a86-195">[Delete](../api/permission-delete.md)</span></span>                    | `DELETE /drive/items/{item-id}/permissions/{id}`
| [<span data-ttu-id="e9a86-196">Добавление пользователей в ссылку совместного доступа</span><span class="sxs-lookup"><span data-stu-id="e9a86-196">Add users to sharing link</span></span>](../api/permission-grant.md)  | `POST /shares/{encoded-sharing-url}/permission/grant`


## <a name="remarks"></a><span data-ttu-id="e9a86-197">Примечания</span><span class="sxs-lookup"><span data-stu-id="e9a86-197">Remarks</span></span>

<span data-ttu-id="e9a86-198">Библиотеки документов OneDrive для бизнеса и SharePoint не возвращают свойство **inheritedFrom**.</span><span class="sxs-lookup"><span data-stu-id="e9a86-198">OneDrive for Business and SharePoint document libraries do not return the **inheritedFrom** property.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The permission object provides information about permissions and roles and sharing information.",
  "keywords": "sharing,permissions,read,write,acl",
  "section": "documentation",
  "tocPath": "Resources/Permission"
} -->
