---
author: JeremyKelley
ms.author: JeremyKelley
title: Тип ресурса разрешения
description: ресурс Permission, представляющий разрешение на совместный доступ, предоставленное для объекта driveItem
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: e43889f3dcab5c887cffe58cfcc4ac632389f980
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932467"
---
# <a name="permission-resource-type"></a><span data-ttu-id="fd79c-103">Тип ресурса разрешения</span><span class="sxs-lookup"><span data-stu-id="fd79c-103">permission resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd79c-104">Ресурс **Permission** предоставляет сведения о разрешении на совместный доступ, предоставленном для ресурса [driveItem](driveitem.md) .</span><span class="sxs-lookup"><span data-stu-id="fd79c-104">The **permission** resource provides information about a sharing permission granted for a [driveItem](driveitem.md) resource.</span></span>

<span data-ttu-id="fd79c-105">Разрешения на совместный доступ могут иметь самые различные формы.</span><span class="sxs-lookup"><span data-stu-id="fd79c-105">Sharing permissions have a number of different forms.</span></span>
<span data-ttu-id="fd79c-106">Ресурс **Permission** представляет эти различные формы с помощью аспектов ресурса.</span><span class="sxs-lookup"><span data-stu-id="fd79c-106">The **permission** resource represents these different forms through facets on the resource.</span></span>

><span data-ttu-id="fd79c-107">**Примечание:** Библиотеки документов OneDrive для бизнеса и SharePoint не возвращают свойство **inheritedFrom** .</span><span class="sxs-lookup"><span data-stu-id="fd79c-107">**Note:** OneDrive for Business and SharePoint document libraries do not return the **inheritedFrom** property.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fd79c-108">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fd79c-108">JSON representation</span></span>

<span data-ttu-id="fd79c-109">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fd79c-109">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="fd79c-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="fd79c-110">Properties</span></span>

| <span data-ttu-id="fd79c-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="fd79c-111">Property</span></span>            | <span data-ttu-id="fd79c-112">Тип</span><span class="sxs-lookup"><span data-stu-id="fd79c-112">Type</span></span>                        | <span data-ttu-id="fd79c-113">Описание</span><span class="sxs-lookup"><span data-stu-id="fd79c-113">Description</span></span>
|:--------------------|:----------------------------|:-------------------------
| <span data-ttu-id="fd79c-114">id</span><span class="sxs-lookup"><span data-stu-id="fd79c-114">id</span></span>                  | <span data-ttu-id="fd79c-115">String</span><span class="sxs-lookup"><span data-stu-id="fd79c-115">String</span></span>                      | <span data-ttu-id="fd79c-p102">Уникальный идентификатор разрешения среди всех разрешений для элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fd79c-p102">The unique identifier of the permission among all permissions on the item. Read-only.</span></span>
| <span data-ttu-id="fd79c-118">grantedTo</span><span class="sxs-lookup"><span data-stu-id="fd79c-118">grantedTo</span></span>           | <span data-ttu-id="fd79c-119">[IdentitySet][]</span><span class="sxs-lookup"><span data-stu-id="fd79c-119">[IdentitySet][]</span></span>             | <span data-ttu-id="fd79c-p103">Для разрешений типа user: сведения о пользователях и приложениях для этого разрешения. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fd79c-p103">For user type permissions, the details of the users & applications for this permission. Read-only.</span></span>
| <span data-ttu-id="fd79c-122">Грантедтоидентитиес</span><span class="sxs-lookup"><span data-stu-id="fd79c-122">grantedToIdentities</span></span> | <span data-ttu-id="fd79c-123">Collection ([Identity][])</span><span class="sxs-lookup"><span data-stu-id="fd79c-123">Collection([IdentitySet][])</span></span> | <span data-ttu-id="fd79c-124">Для разрешений типа ссылки — сведения о пользователях, которым предоставлено разрешение.</span><span class="sxs-lookup"><span data-stu-id="fd79c-124">For link type permissions, the details of the users to whom permission was granted.</span></span> <span data-ttu-id="fd79c-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fd79c-125">Read-only.</span></span>
| <span data-ttu-id="fd79c-126">invitation</span><span class="sxs-lookup"><span data-stu-id="fd79c-126">invitation</span></span>          | <span data-ttu-id="fd79c-127">[SharingInvitation][]</span><span class="sxs-lookup"><span data-stu-id="fd79c-127">[SharingInvitation][]</span></span>       | <span data-ttu-id="fd79c-p105">Сведения обо всех сопоставленных приглашениях к совместному использованию для данного разрешения. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fd79c-p105">Details of any associated sharing invitation for this permission. Read-only.</span></span>
| <span data-ttu-id="fd79c-130">inheritedFrom</span><span class="sxs-lookup"><span data-stu-id="fd79c-130">inheritedFrom</span></span>       | <span data-ttu-id="fd79c-131">[ItemReference][]</span><span class="sxs-lookup"><span data-stu-id="fd79c-131">[ItemReference][]</span></span>           | <span data-ttu-id="fd79c-p106">Предоставляет ссылку на предка текущего разрешения, если оно унаследовано от предка. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fd79c-p106">Provides a reference to the ancestor of the current permission, if it is inherited from an ancestor. Read-only.</span></span>
| <span data-ttu-id="fd79c-134">ссылка</span><span class="sxs-lookup"><span data-stu-id="fd79c-134">link</span></span>                | <span data-ttu-id="fd79c-135">[SharingLink][]</span><span class="sxs-lookup"><span data-stu-id="fd79c-135">[SharingLink][]</span></span>             | <span data-ttu-id="fd79c-p107">Предоставляет сведения о ссылке для текущего разрешения, если это разрешение типа link. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fd79c-p107">Provides the link details of the current permission, if it is a link type permissions. Read-only.</span></span>
| <span data-ttu-id="fd79c-138">roles</span><span class="sxs-lookup"><span data-stu-id="fd79c-138">roles</span></span>               | <span data-ttu-id="fd79c-139">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="fd79c-139">Collection(String)</span></span>          | <span data-ttu-id="fd79c-p108">Тип разрешения, например `read`. Полный список ролей см. ниже. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fd79c-p108">The type of permission, e.g. `read`. See below for the full list of roles. Read-only.</span></span>
| <span data-ttu-id="fd79c-143">shareId</span><span class="sxs-lookup"><span data-stu-id="fd79c-143">shareId</span></span>             | <span data-ttu-id="fd79c-144">Строка</span><span class="sxs-lookup"><span data-stu-id="fd79c-144">String</span></span>                      | <span data-ttu-id="fd79c-145">Уникальный маркер, который можно использовать для доступа к общему элементу через **[API shares][]**.</span><span class="sxs-lookup"><span data-stu-id="fd79c-145">A unique token that can be used to access this shared item via the **[shares API][]**.</span></span> <span data-ttu-id="fd79c-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fd79c-146">Read-only.</span></span>
| <span data-ttu-id="fd79c-147">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="fd79c-147">expirationDateTime</span></span>  | <span data-ttu-id="fd79c-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd79c-148">DateTimeOffset</span></span>              | <span data-ttu-id="fd79c-149">Формат YYYY – MM – ДДВчч: mm: ССЧП of DateTimeOffset указывает срок действия разрешения.</span><span class="sxs-lookup"><span data-stu-id="fd79c-149">A format of yyyy-MM-ddTHH:mm:ssZ of DateTimeOffset indicates the expiration time of the permission.</span></span> <span data-ttu-id="fd79c-150">DateTime. MinValue указывает, что для этого разрешения не задано действие срока действия.</span><span class="sxs-lookup"><span data-stu-id="fd79c-150">DateTime.MinValue indicates there is no expiration set for this permission.</span></span> <span data-ttu-id="fd79c-151">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="fd79c-151">Optional.</span></span>
| <span data-ttu-id="fd79c-152">hasPassword</span><span class="sxs-lookup"><span data-stu-id="fd79c-152">hasPassword</span></span>         | <span data-ttu-id="fd79c-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="fd79c-153">Boolean</span></span>                     | <span data-ttu-id="fd79c-154">Указывает, задан ли для этого разрешения пароль, который отображается в ответе.</span><span class="sxs-lookup"><span data-stu-id="fd79c-154">This indicates whether password is set for this permission, it's only showing in response.</span></span> <span data-ttu-id="fd79c-155">Необязательный и только для чтения и только для OneDrive персональный.</span><span class="sxs-lookup"><span data-stu-id="fd79c-155">Optional and Read-only and for OneDrive Personal only.</span></span>

### <a name="roles-enumeration-values"></a><span data-ttu-id="fd79c-156">Значения перечислений ролей</span><span class="sxs-lookup"><span data-stu-id="fd79c-156">Roles enumeration values</span></span>

| <span data-ttu-id="fd79c-157">Значение</span><span class="sxs-lookup"><span data-stu-id="fd79c-157">Value</span></span>        | <span data-ttu-id="fd79c-158">Сведения</span><span class="sxs-lookup"><span data-stu-id="fd79c-158">Details</span></span>                                                                        |
|:------------|:-------------------------------------------------------------------------------|
| `read`      | <span data-ttu-id="fd79c-159">Дает возможность считывать метаданные и содержимое элемента.</span><span class="sxs-lookup"><span data-stu-id="fd79c-159">Provides the ability to read the metadata and contents of the item.</span></span>            |
| `write`     | <span data-ttu-id="fd79c-160">Дает возможность считывать и изменять метаданные и содержимое элемента.</span><span class="sxs-lookup"><span data-stu-id="fd79c-160">Provides the ability to read and modify the metadata and contents of the item.</span></span> |
| `sp.owner`  | <span data-ttu-id="fd79c-161">В случае с SharePoint и OneDrive для бизнеса представляет роль владельца.</span><span class="sxs-lookup"><span data-stu-id="fd79c-161">For SharePoint and OneDrive for Business this represents the owner role.</span></span>       |
| `sp.member` | <span data-ttu-id="fd79c-162">В случае с SharePoint и OneDrive для бизнеса представляет роль участника.</span><span class="sxs-lookup"><span data-stu-id="fd79c-162">For SharePoint and OneDrive for Business this represents the member role.</span></span>      |

<span data-ttu-id="fd79c-163">Ресурс Permission предоставляет сведения о типе разрешения, представленного ресурсом, с помощью _аспектов_.</span><span class="sxs-lookup"><span data-stu-id="fd79c-163">The permission resource uses _facets_ to provide information about the kind of permission represented by the resource.</span></span>

<span data-ttu-id="fd79c-164">Ссылки для общего доступа содержат уникальный маркер, необходимый для доступа к элементу.</span><span class="sxs-lookup"><span data-stu-id="fd79c-164">Sharing links contain a unique token required to access the item.</span></span>

<span data-ttu-id="fd79c-165">Разрешения с аспектом [**invitation**][SharingInvitation] представляют разрешения, добавленные путем приглашения определенных пользователей или групп для доступа к файлу.</span><span class="sxs-lookup"><span data-stu-id="fd79c-165">Permissions with an [**invitation**][SharingInvitation] facet represent permissions added by inviting specific users or groups to have access to the file.</span></span>

## <a name="sharing-links"></a><span data-ttu-id="fd79c-166">Предоставление ссылок</span><span class="sxs-lookup"><span data-stu-id="fd79c-166">Sharing links</span></span>

<span data-ttu-id="fd79c-167">Разрешения с аспектом [**link**][SharingLink] представляют ссылки для совместного доступа, созданные в элементе.</span><span class="sxs-lookup"><span data-stu-id="fd79c-167">Permissions with a [**link**][SharingLink] facet represent sharing links created on the item.</span></span>
<span data-ttu-id="fd79c-168">Это наиболее распространенные типы разрешений.</span><span class="sxs-lookup"><span data-stu-id="fd79c-168">These are the most common kinds of permissions.</span></span>
<span data-ttu-id="fd79c-169">Ссылки для общего доступа предоставляют уникальный URL-адрес, который можно использовать для доступа к файлу или папке.</span><span class="sxs-lookup"><span data-stu-id="fd79c-169">Sharing links provide a unique URL that can be used to access a file or folder.</span></span>
<span data-ttu-id="fd79c-170">Их можно настроить для предоставления доступа различными способами.</span><span class="sxs-lookup"><span data-stu-id="fd79c-170">They can be set up to grant access in a variety of ways.</span></span>
<span data-ttu-id="fd79c-171">Например, вы можете использовать API [CreateLink][] , чтобы создать ссылку для всех пользователей, которые вошли в организацию, или создать ссылку, которая будет работать для всех пользователей, не требуя входа в систему.</span><span class="sxs-lookup"><span data-stu-id="fd79c-171">For example, you can use the [createLink][] API to create a link that works for anyone signed into your organization, or you can create a link that works for anyone, without needing to sign in.</span></span>
<span data-ttu-id="fd79c-172">Вы можете использовать API [INVITE][] , чтобы создать ссылку, которая работает только для определенных пользователей, независимо от того, находитесь ли они в вашей компании.</span><span class="sxs-lookup"><span data-stu-id="fd79c-172">You can use the [invite][] API to create a link that only works for specific people, whether they're in your company or not.</span></span>

<span data-ttu-id="fd79c-173">Ниже приведено несколько примеров ссылок для общего доступа.</span><span class="sxs-lookup"><span data-stu-id="fd79c-173">Here are some examples of sharing links.</span></span>

### <a name="view-link"></a><span data-ttu-id="fd79c-174">Ссылка для просмотра</span><span class="sxs-lookup"><span data-stu-id="fd79c-174">View link</span></span>

<span data-ttu-id="fd79c-175">Эта ссылка для просмотра предоставляет доступ только для чтения всем пользователям, у которых есть ссылка.</span><span class="sxs-lookup"><span data-stu-id="fd79c-175">This view link provides read-only access to anyone with the link.</span></span>

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

### <a name="edit-link"></a><span data-ttu-id="fd79c-176">Ссылка для редактирования</span><span class="sxs-lookup"><span data-stu-id="fd79c-176">Edit link</span></span>

<span data-ttu-id="fd79c-177">Эта ссылка для редактирования предоставляет доступ для чтения и записи ко всем пользователям в Организации со ссылкой.</span><span class="sxs-lookup"><span data-stu-id="fd79c-177">This edit link provides read and write access to anyone in the organization with the link.</span></span>

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

### <a name="existing-access-link"></a><span data-ttu-id="fd79c-178">Существующая ссылка доступа</span><span class="sxs-lookup"><span data-stu-id="fd79c-178">Existing access link</span></span>

<span data-ttu-id="fd79c-179">Эта ссылка не предоставляет пользователю никаких дополнительных привилегий.</span><span class="sxs-lookup"><span data-stu-id="fd79c-179">This link does not grant any additional privileges to the user.</span></span>

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

### <a name="specific-people-link"></a><span data-ttu-id="fd79c-180">Ссылка на конкретные люди</span><span class="sxs-lookup"><span data-stu-id="fd79c-180">Specific people link</span></span>

<span data-ttu-id="fd79c-181">Эта ссылка обеспечивает доступ для чтения и записи к определенным пользователям в `grantedToIdentities` коллекции.</span><span class="sxs-lookup"><span data-stu-id="fd79c-181">This link provides read and write access to the specific people in the `grantedToIdentities` collection.</span></span>

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

## <a name="sharing-invitations"></a><span data-ttu-id="fd79c-182">Приглашение на общий доступ</span><span class="sxs-lookup"><span data-stu-id="fd79c-182">Sharing invitations</span></span>

<span data-ttu-id="fd79c-183">Разрешения, отправляемые API [INVITE][] или [предоставления][] , могут содержать дополнительные сведения в [][SharingInvitation] аспекта приглашения для адресов электронной почты, которые не совпадают с известной учетной записью.</span><span class="sxs-lookup"><span data-stu-id="fd79c-183">Permissions sent by the [invite][] or [grant][] API can have additional information in the [invitation][SharingInvitation] facet for email addresses that don't match a known account.</span></span> <span data-ttu-id="fd79c-184">В таких случаях свойство **грантедто** может быть настроено до тех пор, пока не будет активирована ссылка приглашения, которая возникает при первом щелчке ссылки и входе в систему.</span><span class="sxs-lookup"><span data-stu-id="fd79c-184">In such cases, the **grantedTo** property might not be set until the invitation link is redeemed, which occurs the first time the user clicks the link and signs in.</span></span>

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

<span data-ttu-id="fd79c-185">Когда пользователь активирует приглашение к совместному использованию, в свойстве **grantedTo** появятся сведения об учетной записи, которая активировала разрешения:</span><span class="sxs-lookup"><span data-stu-id="fd79c-185">After the sharing invitation has been redeemed by a user, the **grantedTo** property will contain the information about the account that redeemed the permissions:</span></span>

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

## <a name="methods"></a><span data-ttu-id="fd79c-186">Методы</span><span class="sxs-lookup"><span data-stu-id="fd79c-186">Methods</span></span>

| <span data-ttu-id="fd79c-187">Метод</span><span class="sxs-lookup"><span data-stu-id="fd79c-187">Method</span></span>                                                   | <span data-ttu-id="fd79c-188">Путь REST</span><span class="sxs-lookup"><span data-stu-id="fd79c-188">REST Path</span></span>
|:---------------------------------------------------------|:-----------------------
| [<span data-ttu-id="fd79c-189">Получение списка разрешений</span><span class="sxs-lookup"><span data-stu-id="fd79c-189">List permissions</span></span>](../api/driveitem-list-permissions.md) | `GET /drive/items/{item-id}/permissions`
| [<span data-ttu-id="fd79c-190">Получение разрешения</span><span class="sxs-lookup"><span data-stu-id="fd79c-190">Get permission</span></span>](../api/permission-get.md)               | `GET /drive/items/{item-id}/permissions/{id}`
| <span data-ttu-id="fd79c-191">[Создание ссылки] [CreateLink]</span><span class="sxs-lookup"><span data-stu-id="fd79c-191">[Create link][createLink]</span></span>                                | `POST /drive/items/{item-id}/createLink`
| <span data-ttu-id="fd79c-192">[Приглашение пользователей] [пригласить]</span><span class="sxs-lookup"><span data-stu-id="fd79c-192">[Invite people][invite]</span></span>                                  | `POST /drive/items/{item-id}/invite`
| [<span data-ttu-id="fd79c-193">Обновление</span><span class="sxs-lookup"><span data-stu-id="fd79c-193">Update</span></span>](../api/permission-update.md)                    | `PATCH /drive/items/{item-id}/permissions/{id}`
| <span data-ttu-id="fd79c-194">[удаление](../api/permission-delete.md);</span><span class="sxs-lookup"><span data-stu-id="fd79c-194">[Delete](../api/permission-delete.md)</span></span>                    | `DELETE /drive/items/{item-id}/permissions/{id}`



[createLink]: ../api/driveitem-createlink.md
[обладают]: ../api/permission-grant.md
[grant]: ../api/permission-grant.md
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
