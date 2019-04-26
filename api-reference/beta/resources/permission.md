---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Permission
localization_priority: Normal
ms.openlocfilehash: e8a4adaa3c1d41270e172f9d0b0e1bf3829927c5
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344984"
---
# <a name="permission-resource-type"></a><span data-ttu-id="84bd8-102">Тип ресурса разрешения</span><span class="sxs-lookup"><span data-stu-id="84bd8-102">permission resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84bd8-103">Ресурс **Permission** предоставляет сведения о разрешении на совместный доступ, предоставленном для ресурса [driveItem](driveitem.md) .</span><span class="sxs-lookup"><span data-stu-id="84bd8-103">The **permission** resource provides information about a sharing permission granted for a [driveItem](driveitem.md) resource.</span></span>

<span data-ttu-id="84bd8-104">Разрешения на совместный доступ могут иметь самые различные формы.</span><span class="sxs-lookup"><span data-stu-id="84bd8-104">Sharing permissions have a number of different forms.</span></span>
<span data-ttu-id="84bd8-105">Ресурс **Permission** представляет эти различные формы с помощью аспектов ресурса.</span><span class="sxs-lookup"><span data-stu-id="84bd8-105">The **permission** resource represents these different forms through facets on the resource.</span></span>

><span data-ttu-id="84bd8-106">**Примечание:** Библиотеки документов OneDrive для бизнеса и SharePoint не возвращают свойство **inheritedFrom** .</span><span class="sxs-lookup"><span data-stu-id="84bd8-106">**Note:** OneDrive for Business and SharePoint document libraries do not return the **inheritedFrom** property.</span></span>

## <a name="json-representation"></a><span data-ttu-id="84bd8-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="84bd8-107">JSON representation</span></span>

<span data-ttu-id="84bd8-108">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="84bd8-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="84bd8-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="84bd8-109">Properties</span></span>

| <span data-ttu-id="84bd8-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="84bd8-110">Property</span></span>            | <span data-ttu-id="84bd8-111">Тип</span><span class="sxs-lookup"><span data-stu-id="84bd8-111">Type</span></span>                        | <span data-ttu-id="84bd8-112">Описание</span><span class="sxs-lookup"><span data-stu-id="84bd8-112">Description</span></span>
|:--------------------|:----------------------------|:-------------------------
| <span data-ttu-id="84bd8-113">id</span><span class="sxs-lookup"><span data-stu-id="84bd8-113">id</span></span>                  | <span data-ttu-id="84bd8-114">String</span><span class="sxs-lookup"><span data-stu-id="84bd8-114">String</span></span>                      | <span data-ttu-id="84bd8-p102">Уникальный идентификатор разрешения среди всех разрешений для элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="84bd8-p102">The unique identifier of the permission among all permissions on the item. Read-only.</span></span>
| <span data-ttu-id="84bd8-117">grantedTo</span><span class="sxs-lookup"><span data-stu-id="84bd8-117">grantedTo</span></span>           | <span data-ttu-id="84bd8-118">[IdentitySet][]</span><span class="sxs-lookup"><span data-stu-id="84bd8-118">[IdentitySet][]</span></span>             | <span data-ttu-id="84bd8-p103">Для разрешений типа user: сведения о пользователях и приложениях для этого разрешения. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="84bd8-p103">For user type permissions, the details of the users & applications for this permission. Read-only.</span></span>
| <span data-ttu-id="84bd8-121">Грантедтоидентитиес</span><span class="sxs-lookup"><span data-stu-id="84bd8-121">grantedToIdentities</span></span> | <span data-ttu-id="84bd8-122">Collection ([Identity][])</span><span class="sxs-lookup"><span data-stu-id="84bd8-122">Collection([IdentitySet][])</span></span> | <span data-ttu-id="84bd8-123">Для разрешений типа ссылки — сведения о пользователях, которым предоставлено разрешение.</span><span class="sxs-lookup"><span data-stu-id="84bd8-123">For link type permissions, the details of the users to whom permission was granted.</span></span> <span data-ttu-id="84bd8-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="84bd8-124">Read-only.</span></span>
| <span data-ttu-id="84bd8-125">invitation</span><span class="sxs-lookup"><span data-stu-id="84bd8-125">invitation</span></span>          | <span data-ttu-id="84bd8-126">[SharingInvitation][]</span><span class="sxs-lookup"><span data-stu-id="84bd8-126">[SharingInvitation][]</span></span>       | <span data-ttu-id="84bd8-p105">Сведения обо всех сопоставленных приглашениях к совместному использованию для данного разрешения. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="84bd8-p105">Details of any associated sharing invitation for this permission. Read-only.</span></span>
| <span data-ttu-id="84bd8-129">inheritedFrom</span><span class="sxs-lookup"><span data-stu-id="84bd8-129">inheritedFrom</span></span>       | <span data-ttu-id="84bd8-130">[ItemReference][]</span><span class="sxs-lookup"><span data-stu-id="84bd8-130">[ItemReference][]</span></span>           | <span data-ttu-id="84bd8-p106">Предоставляет ссылку на предка текущего разрешения, если оно унаследовано от предка. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="84bd8-p106">Provides a reference to the ancestor of the current permission, if it is inherited from an ancestor. Read-only.</span></span>
| <span data-ttu-id="84bd8-133">ссылка</span><span class="sxs-lookup"><span data-stu-id="84bd8-133">link</span></span>                | <span data-ttu-id="84bd8-134">[SharingLink][]</span><span class="sxs-lookup"><span data-stu-id="84bd8-134">[SharingLink][]</span></span>             | <span data-ttu-id="84bd8-p107">Предоставляет сведения о ссылке для текущего разрешения, если это разрешение типа link. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="84bd8-p107">Provides the link details of the current permission, if it is a link type permissions. Read-only.</span></span>
| <span data-ttu-id="84bd8-137">roles</span><span class="sxs-lookup"><span data-stu-id="84bd8-137">roles</span></span>               | <span data-ttu-id="84bd8-138">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="84bd8-138">Collection(String)</span></span>          | <span data-ttu-id="84bd8-p108">Тип разрешения, например `read`. Полный список ролей см. ниже. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="84bd8-p108">The type of permission, e.g. `read`. See below for the full list of roles. Read-only.</span></span>
| <span data-ttu-id="84bd8-142">shareId</span><span class="sxs-lookup"><span data-stu-id="84bd8-142">shareId</span></span>             | <span data-ttu-id="84bd8-143">Строка</span><span class="sxs-lookup"><span data-stu-id="84bd8-143">String</span></span>                      | <span data-ttu-id="84bd8-144">Уникальный маркер, который можно использовать для доступа к общему элементу через **[API shares][]**.</span><span class="sxs-lookup"><span data-stu-id="84bd8-144">A unique token that can be used to access this shared item via the **[shares API][]**.</span></span> <span data-ttu-id="84bd8-145">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="84bd8-145">Read-only.</span></span>
| <span data-ttu-id="84bd8-146">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="84bd8-146">expirationDateTime</span></span>  | <span data-ttu-id="84bd8-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84bd8-147">DateTimeOffset</span></span>              | <span data-ttu-id="84bd8-148">Формат YYYY – MM – ДДВчч: mm: ССЧП of DateTimeOffset указывает срок действия разрешения.</span><span class="sxs-lookup"><span data-stu-id="84bd8-148">A format of yyyy-MM-ddTHH:mm:ssZ of DateTimeOffset indicates the expiration time of the permission.</span></span> <span data-ttu-id="84bd8-149">DateTime. MinValue указывает, что для этого разрешения не задано действие срока действия.</span><span class="sxs-lookup"><span data-stu-id="84bd8-149">DateTime.MinValue indicates there is no expiration set for this permission.</span></span> <span data-ttu-id="84bd8-150">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="84bd8-150">Optional.</span></span>
| <span data-ttu-id="84bd8-151">hasPassword</span><span class="sxs-lookup"><span data-stu-id="84bd8-151">hasPassword</span></span>         | <span data-ttu-id="84bd8-152">Логический</span><span class="sxs-lookup"><span data-stu-id="84bd8-152">Boolean</span></span>                     | <span data-ttu-id="84bd8-153">Указывает, задан ли для этого разрешения пароль, который отображается в ответе.</span><span class="sxs-lookup"><span data-stu-id="84bd8-153">This indicates whether password is set for this permission, it's only showing in response.</span></span> <span data-ttu-id="84bd8-154">НеОбязательный и только для чтения и только для OneDrive персональный.</span><span class="sxs-lookup"><span data-stu-id="84bd8-154">Optional and Read-only and for OneDrive Personal only.</span></span>

### <a name="roles-enumeration-values"></a><span data-ttu-id="84bd8-155">Значения перечислений ролей</span><span class="sxs-lookup"><span data-stu-id="84bd8-155">Roles enumeration values</span></span>

| <span data-ttu-id="84bd8-156">Значение</span><span class="sxs-lookup"><span data-stu-id="84bd8-156">Value</span></span>        | <span data-ttu-id="84bd8-157">Сведения</span><span class="sxs-lookup"><span data-stu-id="84bd8-157">Details</span></span>                                                                        |
|:------------|:-------------------------------------------------------------------------------|
| `read`      | <span data-ttu-id="84bd8-158">Дает возможность считывать метаданные и содержимое элемента.</span><span class="sxs-lookup"><span data-stu-id="84bd8-158">Provides the ability to read the metadata and contents of the item.</span></span>            |
| `write`     | <span data-ttu-id="84bd8-159">Дает возможность считывать и изменять метаданные и содержимое элемента.</span><span class="sxs-lookup"><span data-stu-id="84bd8-159">Provides the ability to read and modify the metadata and contents of the item.</span></span> |
| `sp.owner`  | <span data-ttu-id="84bd8-160">В случае с SharePoint и OneDrive для бизнеса представляет роль владельца.</span><span class="sxs-lookup"><span data-stu-id="84bd8-160">For SharePoint and OneDrive for Business this represents the owner role.</span></span>       |
| `sp.member` | <span data-ttu-id="84bd8-161">В случае с SharePoint и OneDrive для бизнеса представляет роль участника.</span><span class="sxs-lookup"><span data-stu-id="84bd8-161">For SharePoint and OneDrive for Business this represents the member role.</span></span>      |

<span data-ttu-id="84bd8-162">Ресурс Permission предоставляет сведения о типе разрешения, представленного ресурсом, с помощью _аспектов_.</span><span class="sxs-lookup"><span data-stu-id="84bd8-162">The permission resource uses _facets_ to provide information about the kind of permission represented by the resource.</span></span>

<span data-ttu-id="84bd8-163">Ссылки для общего доступа содержат уникальный маркер, необходимый для доступа к элементу.</span><span class="sxs-lookup"><span data-stu-id="84bd8-163">Sharing links contain a unique token required to access the item.</span></span>

<span data-ttu-id="84bd8-164">Разрешения с аспектом [**invitation**][SharingInvitation] представляют разрешения, добавленные путем приглашения определенных пользователей или групп для доступа к файлу.</span><span class="sxs-lookup"><span data-stu-id="84bd8-164">Permissions with an [**invitation**][SharingInvitation] facet represent permissions added by inviting specific users or groups to have access to the file.</span></span>

## <a name="sharing-links"></a><span data-ttu-id="84bd8-165">Предоставление ссылок</span><span class="sxs-lookup"><span data-stu-id="84bd8-165">Sharing links</span></span>

<span data-ttu-id="84bd8-166">Разрешения с аспектом [**link**][SharingLink] представляют ссылки для совместного доступа, созданные в элементе.</span><span class="sxs-lookup"><span data-stu-id="84bd8-166">Permissions with a [**link**][SharingLink] facet represent sharing links created on the item.</span></span>
<span data-ttu-id="84bd8-167">Это наиболее распространенные типы разрешений.</span><span class="sxs-lookup"><span data-stu-id="84bd8-167">These are the most common kinds of permissions.</span></span>
<span data-ttu-id="84bd8-168">Ссылки для общего доступа предоставляют уникальный URL-адрес, который можно использовать для доступа к файлу или папке.</span><span class="sxs-lookup"><span data-stu-id="84bd8-168">Sharing links provide a unique URL that can be used to access a file or folder.</span></span>
<span data-ttu-id="84bd8-169">Их можно настроить для предоставления доступа различными способами.</span><span class="sxs-lookup"><span data-stu-id="84bd8-169">They can be set up to grant access in a variety of ways.</span></span>
<span data-ttu-id="84bd8-170">Например, вы можете использовать API [CreateLink][] , чтобы создать ссылку для всех пользователей, которые вошли в организацию, или создать ссылку, которая будет работать для всех пользователей, не требуя входа в систему.</span><span class="sxs-lookup"><span data-stu-id="84bd8-170">For example, you can use the [createLink][] API to create a link that works for anyone signed into your organization, or you can create a link that works for anyone, without needing to sign in.</span></span>
<span data-ttu-id="84bd8-171">Вы можете использовать API [INVITE][] , чтобы создать ссылку, которая работает только для определенных пользователей, независимо от того, находитесь ли они в вашей компании.</span><span class="sxs-lookup"><span data-stu-id="84bd8-171">You can use the [invite][] API to create a link that only works for specific people, whether they're in your company or not.</span></span>

<span data-ttu-id="84bd8-172">Ниже приведено несколько примеров ссылок для общего доступа.</span><span class="sxs-lookup"><span data-stu-id="84bd8-172">Here are some examples of sharing links.</span></span>

### <a name="view-link"></a><span data-ttu-id="84bd8-173">Ссылка для просмотра</span><span class="sxs-lookup"><span data-stu-id="84bd8-173">View link</span></span>

<span data-ttu-id="84bd8-174">Эта ссылка для просмотра предоставляет доступ только для чтения всем пользователям, у которых есть ссылка.</span><span class="sxs-lookup"><span data-stu-id="84bd8-174">This view link provides read-only access to anyone with the link.</span></span>

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

### <a name="edit-link"></a><span data-ttu-id="84bd8-175">Ссылка для редактирования</span><span class="sxs-lookup"><span data-stu-id="84bd8-175">Edit link</span></span>

<span data-ttu-id="84bd8-176">Эта ссылка для редактирования предоставляет доступ для чтения и записи ко всем пользователям в Организации со ссылкой.</span><span class="sxs-lookup"><span data-stu-id="84bd8-176">This edit link provides read and write access to anyone in the organization with the link.</span></span>

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

### <a name="specific-people-link"></a><span data-ttu-id="84bd8-177">Ссылка на конкретные люди</span><span class="sxs-lookup"><span data-stu-id="84bd8-177">Specific people link</span></span>

<span data-ttu-id="84bd8-178">Эта ссылка обеспечивает доступ для чтения и записи к определенным пользователям в `grantedToIdentities` коллекции.</span><span class="sxs-lookup"><span data-stu-id="84bd8-178">This link provides read and write access to the specific people in the `grantedToIdentities` collection.</span></span>

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

## <a name="sharing-invitations"></a><span data-ttu-id="84bd8-179">Приглашение на общий доступ</span><span class="sxs-lookup"><span data-stu-id="84bd8-179">Sharing invitations</span></span>

<span data-ttu-id="84bd8-180">Разрешения, отправляемые API-интерфейсом [INVITE][] , могут содержать []дополнительные сведения в аспекте[SharingInvitation] .</span><span class="sxs-lookup"><span data-stu-id="84bd8-180">Permissions sent by the [invite][] API may have additional information in the [invitation][SharingInvitation] facet.</span></span>
<span data-ttu-id="84bd8-181">Если приглашение было отправлено на адрес электронной почты, который не отвечает на известную учетную запись, свойство **грантедто** не может быть установлено до тех пор, пока не будет активировано приглашение, которое возникает при первом щелчке ссылки и входе в систему.</span><span class="sxs-lookup"><span data-stu-id="84bd8-181">If an invitation was sent to an email address that doesn't match a known account, the **grantedTo** property may not be set until the invitation is redeemed, which occurs the first time the user clicks the link and signs in.</span></span>

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

<span data-ttu-id="84bd8-182">Когда пользователь активирует приглашение к совместному использованию, в свойстве **grantedTo** появятся сведения об учетной записи, которая активировала разрешения:</span><span class="sxs-lookup"><span data-stu-id="84bd8-182">After the sharing invitation has been redeemed by a user, the **grantedTo** property will contain the information about the account that redeemed the permissions:</span></span>

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

## <a name="methods"></a><span data-ttu-id="84bd8-183">Методы</span><span class="sxs-lookup"><span data-stu-id="84bd8-183">Methods</span></span>

| <span data-ttu-id="84bd8-184">Метод</span><span class="sxs-lookup"><span data-stu-id="84bd8-184">Method</span></span>                                                   | <span data-ttu-id="84bd8-185">Путь REST</span><span class="sxs-lookup"><span data-stu-id="84bd8-185">REST Path</span></span>
|:---------------------------------------------------------|:-----------------------
| [<span data-ttu-id="84bd8-186">Получение списка разрешений</span><span class="sxs-lookup"><span data-stu-id="84bd8-186">List permissions</span></span>](../api/driveitem-list-permissions.md) | `GET /drive/items/{item-id}/permissions`
| [<span data-ttu-id="84bd8-187">Получение разрешения</span><span class="sxs-lookup"><span data-stu-id="84bd8-187">Get permission</span></span>](../api/permission-get.md)               | `GET /drive/items/{item-id}/permissions/{id}`
| <span data-ttu-id="84bd8-188">[Создание ссылки] [CreateLink]</span><span class="sxs-lookup"><span data-stu-id="84bd8-188">[Create link][createLink]</span></span>                                | `POST /drive/items/{item-id}/createLink`
| <span data-ttu-id="84bd8-189">[Приглашение пользователей] [пригласить]</span><span class="sxs-lookup"><span data-stu-id="84bd8-189">[Invite people][invite]</span></span>                                  | `POST /drive/items/{item-id}/invite`
| [<span data-ttu-id="84bd8-190">Обновление</span><span class="sxs-lookup"><span data-stu-id="84bd8-190">Update</span></span>](../api/permission-update.md)                    | `PATCH /drive/items/{item-id}/permissions/{id}`
| [<span data-ttu-id="84bd8-191">Удаление</span><span class="sxs-lookup"><span data-stu-id="84bd8-191">Delete</span></span>](../api/permission-delete.md)                    | `DELETE /drive/items/{item-id}/permissions/{id}`



[createLink]: ../api/driveitem-createlink.md
[IdentitySet]: identityset.md
[ложите]: ../api/driveitem-invite.md
[invite]: ../api/driveitem-invite.md
[ItemReference]: itemreference.md
[API общих ресурсов]: ../api/shares-get.md
[shares API]: ../api/shares-get.md
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
