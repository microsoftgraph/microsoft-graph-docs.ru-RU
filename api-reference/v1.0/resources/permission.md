---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Permission
localization_priority: Priority
ms.openlocfilehash: f2781726be786c5eb0d4ed8103dc3b9a62137597
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482226"
---
# <a name="permission-resource-type"></a><span data-ttu-id="fa3c1-102">Тип ресурса Permission</span><span class="sxs-lookup"><span data-stu-id="fa3c1-102">Permission resource type</span></span>

<span data-ttu-id="fa3c1-103">Ресурс **Permission** содержит сведения о разрешении на совместный доступ, предоставленном для ресурса [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="fa3c1-103">The **Permission** resource provides information about a sharing permission granted for a [DriveItem](driveitem.md) resource.</span></span>

<span data-ttu-id="fa3c1-104">Разрешения на совместный доступ могут иметь самые различные формы.</span><span class="sxs-lookup"><span data-stu-id="fa3c1-104">Sharing permissions have a number of different forms.</span></span>
<span data-ttu-id="fa3c1-105">Ресурс **Permission** представляет эти формы с помощью аспектов в ресурсе.</span><span class="sxs-lookup"><span data-stu-id="fa3c1-105">The **Permission** resource represents these different forms through facets on the resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fa3c1-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fa3c1-106">JSON representation</span></span>

<span data-ttu-id="fa3c1-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="fa3c1-107">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "link",
    "grantedTo",
    "invitation",
    "inheritedFrom",
    "shareId"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
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

## <a name="properties"></a><span data-ttu-id="fa3c1-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="fa3c1-108">Properties</span></span>

| <span data-ttu-id="fa3c1-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="fa3c1-109">Property</span></span>      | <span data-ttu-id="fa3c1-110">Тип</span><span class="sxs-lookup"><span data-stu-id="fa3c1-110">Type</span></span>                                      | <span data-ttu-id="fa3c1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="fa3c1-111">Description</span></span>
|:--------------|:------------------------------------------|:-----------------
| <span data-ttu-id="fa3c1-112">id</span><span class="sxs-lookup"><span data-stu-id="fa3c1-112">id</span></span>            | <span data-ttu-id="fa3c1-113">Строка</span><span class="sxs-lookup"><span data-stu-id="fa3c1-113">String</span></span>                                    | <span data-ttu-id="fa3c1-p102">Уникальный идентификатор разрешения среди всех разрешений для элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fa3c1-p102">The unique identifier of the permission among all permissions on the item. Read-only.</span></span>
| <span data-ttu-id="fa3c1-116">grantedTo</span><span class="sxs-lookup"><span data-stu-id="fa3c1-116">grantedTo</span></span>     | [<span data-ttu-id="fa3c1-117">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="fa3c1-117">IdentitySet</span></span>](identityset.md)             | <span data-ttu-id="fa3c1-p103">Для разрешений типа user: сведения о пользователях и приложениях для этого разрешения. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fa3c1-p103">For user type permissions, the details of the users & applications for this permission. Read-only.</span></span>
| <span data-ttu-id="fa3c1-120">invitation</span><span class="sxs-lookup"><span data-stu-id="fa3c1-120">invitation</span></span>    | <span data-ttu-id="fa3c1-121">[SharingInvitation][]</span><span class="sxs-lookup"><span data-stu-id="fa3c1-121">[SharingInvitation][]</span></span>                     | <span data-ttu-id="fa3c1-p104">Сведения обо всех сопоставленных приглашениях к совместному использованию для данного разрешения. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fa3c1-p104">Details of any associated sharing invitation for this permission. Read-only.</span></span>
| <span data-ttu-id="fa3c1-124">inheritedFrom</span><span class="sxs-lookup"><span data-stu-id="fa3c1-124">inheritedFrom</span></span> | [<span data-ttu-id="fa3c1-125">ItemReference</span><span class="sxs-lookup"><span data-stu-id="fa3c1-125">ItemReference</span></span>](itemreference.md)         | <span data-ttu-id="fa3c1-p105">Предоставляет ссылку на предка текущего разрешения, если оно унаследовано от предка. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fa3c1-p105">Provides a reference to the ancestor of the current permission, if it is inherited from an ancestor. Read-only.</span></span>
| <span data-ttu-id="fa3c1-128">ссылка</span><span class="sxs-lookup"><span data-stu-id="fa3c1-128">link</span></span>          | <span data-ttu-id="fa3c1-129">[SharingLink][]</span><span class="sxs-lookup"><span data-stu-id="fa3c1-129">[SharingLink][]</span></span>                           | <span data-ttu-id="fa3c1-p106">Предоставляет сведения о ссылке для текущего разрешения, если это разрешение типа link. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fa3c1-p106">Provides the link details of the current permission, if it is a link type permissions. Read-only.</span></span>
| <span data-ttu-id="fa3c1-132">roles</span><span class="sxs-lookup"><span data-stu-id="fa3c1-132">roles</span></span>         | <span data-ttu-id="fa3c1-133">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="fa3c1-133">Collection of String</span></span>                      | <span data-ttu-id="fa3c1-p107">Тип разрешения, например `read`. Полный список ролей см. ниже. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fa3c1-p107">The type of permission, e.g. `read`. See below for the full list of roles. Read-only.</span></span>
| <span data-ttu-id="fa3c1-137">shareId</span><span class="sxs-lookup"><span data-stu-id="fa3c1-137">shareId</span></span>       | <span data-ttu-id="fa3c1-138">Строка</span><span class="sxs-lookup"><span data-stu-id="fa3c1-138">String</span></span>                                    | <span data-ttu-id="fa3c1-p108">Уникальный токен, с помощью которого можно получить доступ к общему элементу через [API **shares**](../api/shares-get.md). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fa3c1-p108">A unique token that can be used to access this shared item via the [**shares** API](../api/shares-get.md). Read-only.</span></span>

<span data-ttu-id="fa3c1-141">Ресурс Permission предоставляет сведения о типе разрешения, представленного ресурсом, с помощью _аспектов_.</span><span class="sxs-lookup"><span data-stu-id="fa3c1-141">The permission resource uses _facets_ to provide information about the kind of permission represented by the resource.</span></span>

<span data-ttu-id="fa3c1-p109">Разрешения с аспектом [**link**][SharingLink] представляют ссылки для совместного доступа, созданные в элементе. Ссылки для совместного доступа содержат уникальный токен, предоставляющий доступ к элементу любому пользователю, у которого есть такая ссылка.</span><span class="sxs-lookup"><span data-stu-id="fa3c1-p109">Permissions with a [**link**][SharingLink] facet represent sharing links created on the item. Sharing links contain a unique token that provides access to the item for anyone with the link.</span></span>

<span data-ttu-id="fa3c1-144">Разрешения с аспектом [**invitation**][SharingInvitation] представляют разрешения, добавленные путем приглашения определенных пользователей или групп для доступа к файлу.</span><span class="sxs-lookup"><span data-stu-id="fa3c1-144">Permissions with an [**invitation**][SharingInvitation] facet represent permissions added by inviting specific users or groups to have access to the file.</span></span>

[SharingInvitation]: sharinginvitation.md
[SharingLink]: sharinglink.md

## <a name="roles-enumeration"></a><span data-ttu-id="fa3c1-147">Перечисление ролей</span><span class="sxs-lookup"><span data-stu-id="fa3c1-147">Roles enumeration</span></span>

| <span data-ttu-id="fa3c1-148">Роль</span><span class="sxs-lookup"><span data-stu-id="fa3c1-148">Role</span></span>        | <span data-ttu-id="fa3c1-149">Сведения</span><span class="sxs-lookup"><span data-stu-id="fa3c1-149">Details</span></span>                                                                        |
|:------------|:-------------------------------------------------------------------------------|
| `read`      | <span data-ttu-id="fa3c1-150">Дает возможность считывать метаданные и содержимое элемента.</span><span class="sxs-lookup"><span data-stu-id="fa3c1-150">Provides the ability to read the metadata and contents of the item.</span></span>            |
| `write`     | <span data-ttu-id="fa3c1-151">Дает возможность считывать и изменять метаданные и содержимое элемента.</span><span class="sxs-lookup"><span data-stu-id="fa3c1-151">Provides the ability to read and modify the metadata and contents of the item.</span></span> |
| `sp.owner`  | <span data-ttu-id="fa3c1-152">В случае с SharePoint и OneDrive для бизнеса представляет роль владельца.</span><span class="sxs-lookup"><span data-stu-id="fa3c1-152">For SharePoint and OneDrive for Business this represents the owner role.</span></span>       |
| `sp.member` | <span data-ttu-id="fa3c1-153">В случае с SharePoint и OneDrive для бизнеса представляет роль участника.</span><span class="sxs-lookup"><span data-stu-id="fa3c1-153">For SharePoint and OneDrive for Business this represents the member role.</span></span>      |

## <a name="sharing-links"></a><span data-ttu-id="fa3c1-154">Предоставление ссылок</span><span class="sxs-lookup"><span data-stu-id="fa3c1-154">Sharing links</span></span>
<span data-ttu-id="fa3c1-p110">Наиболее распространенный тип разрешений — ссылки для общего доступа. Ссылки для общего доступа предоставляют уникальный URL-адрес, включающий ресурс, к которому предоставляется доступ, и маркер аутентификации, предоставляющий доступ к ресурсу. Пользователям не требуется выполнять вход для доступа к содержимому, предоставленному с помощью ссылки для общего доступа. Пользователи могут поделиться ссылкой, предоставляющей доступ к содержимому только для чтения или для чтения и записи.</span><span class="sxs-lookup"><span data-stu-id="fa3c1-p110">The most common type of permissions are sharing links. Sharing links provide a unique URL that includes both the resource being shared and an authentication token that provides access to the resource. Users don't need to sign-in to access the content shared with a sharing link. Users can share a link that gives read-only access to the content or writable access to the content.</span></span>

### <a name="view-link"></a><span data-ttu-id="fa3c1-159">Ссылка для просмотра</span><span class="sxs-lookup"><span data-stu-id="fa3c1-159">View Link</span></span>
<span data-ttu-id="fa3c1-160">Ссылка для просмотра предоставляет доступ к элементу только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fa3c1-160">A view link provides read-only access to an item.</span></span>

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

### <a name="edit-link"></a><span data-ttu-id="fa3c1-161">Ссылка для редактирования</span><span class="sxs-lookup"><span data-stu-id="fa3c1-161">Edit link</span></span>
<span data-ttu-id="fa3c1-162">Ссылка для редактирования предоставляет доступ к элементу для чтения и записи.</span><span class="sxs-lookup"><span data-stu-id="fa3c1-162">An edit link provides read and write access to an item.</span></span>

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

### <a name="sharing-invitation"></a><span data-ttu-id="fa3c1-163">Приглашение к совместному использованию</span><span class="sxs-lookup"><span data-stu-id="fa3c1-163">Sharing Invitation</span></span>
<span data-ttu-id="fa3c1-p111">Вы можете не только создавать ссылки для общего доступа, но и пригласить пользователя по электронному адресу. В этом случае разрешение создает приглашение, отправляемое пользователю по электронной почте.</span><span class="sxs-lookup"><span data-stu-id="fa3c1-p111">In addition to creating sharing links, a user can be invited by e-mail address. In this scenario the permission creates an invitation that is sent to the user's email.</span></span>

#### <a name="invitation-to-an-email-address"></a><span data-ttu-id="fa3c1-166">Приглашение на электронный адрес</span><span class="sxs-lookup"><span data-stu-id="fa3c1-166">Invitation to an email address</span></span>
<span data-ttu-id="fa3c1-167">Если разрешение было отправлено по электронной почте получателю, у которого нет соответствующей учетной записи, то свойство **grantedTo** может быть не задано, пока приглашение не будет активировано (это происходит, когда пользователь впервые переходит по ссылке и выполняет вход).</span><span class="sxs-lookup"><span data-stu-id="fa3c1-167">If the permission was sent via an email address to a recipient who does not have a matching account, the **grantedTo** property may not be set until the invitation is redeemed, which occurs the first time a user clicks the link and signs in.</span></span>

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

<span data-ttu-id="fa3c1-168">Когда пользователь активирует приглашение к совместному использованию, в свойстве **grantedTo** появятся сведения об учетной записи, которая активировала разрешения:</span><span class="sxs-lookup"><span data-stu-id="fa3c1-168">After the sharing invitation has been redeemed by a user, the **grantedTo** property will contain the information about the account that redeemed the permissions:</span></span>

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

## <a name="methods"></a><span data-ttu-id="fa3c1-169">Методы</span><span class="sxs-lookup"><span data-stu-id="fa3c1-169">Methods</span></span>

| <span data-ttu-id="fa3c1-170">Метод</span><span class="sxs-lookup"><span data-stu-id="fa3c1-170">Method</span></span>                                                   | <span data-ttu-id="fa3c1-171">Путь REST</span><span class="sxs-lookup"><span data-stu-id="fa3c1-171">REST Path</span></span>
|:---------------------------------------------------------|:-----------------------
| [<span data-ttu-id="fa3c1-172">Получение списка разрешений</span><span class="sxs-lookup"><span data-stu-id="fa3c1-172">List permissions</span></span>](../api/driveitem-list-permissions.md) | `GET /drive/items/{item-id}/permissions`
| [<span data-ttu-id="fa3c1-173">Получение разрешения</span><span class="sxs-lookup"><span data-stu-id="fa3c1-173">Get permission</span></span>](../api/permission-get.md)               | `GET /drive/items/{item-id}/permissions/{id}`
| [<span data-ttu-id="fa3c1-174">Добавление</span><span class="sxs-lookup"><span data-stu-id="fa3c1-174">Add</span></span>](../api/driveitem-invite.md)                        | `POST /drive/items/{item-id}/invite`
| [<span data-ttu-id="fa3c1-175">Обновление</span><span class="sxs-lookup"><span data-stu-id="fa3c1-175">Update</span></span>](../api/permission-update.md)                    | `PATCH /drive/items/{item-id}/permissions/{id}`
| [<span data-ttu-id="fa3c1-176">Удаление</span><span class="sxs-lookup"><span data-stu-id="fa3c1-176">Delete</span></span>](../api/permission-delete.md)                    | `DELETE /drive/items/{item-id}/permissions/{id}`


## <a name="remarks"></a><span data-ttu-id="fa3c1-177">Заметки</span><span class="sxs-lookup"><span data-stu-id="fa3c1-177">Remarks</span></span>

<span data-ttu-id="fa3c1-178">Библиотеки документов OneDrive для бизнеса и SharePoint не возвращают свойство **inheritedFrom**.</span><span class="sxs-lookup"><span data-stu-id="fa3c1-178">OneDrive for Business and SharePoint document libraries do not return the **inheritedFrom** property.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The permission object provides information about permissions and roles and sharing information.",
  "keywords": "sharing,permissions,read,write,acl",
  "section": "documentation",
  "tocPath": "Resources/Permission"
} -->
