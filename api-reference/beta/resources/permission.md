---
author: JeremyKelley
ms.author: JeremyKelley
title: Тип ресурса разрешения
description: ресурс Permission, представляющий разрешение на совместный доступ, предоставленное для объекта driveItem
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 29b4c7aaccc62afa16057388758e1a62f05db41e
ms.sourcegitcommit: 577bfd3bb8a2e2679ef1c5942a4a496c2aa3a277
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/17/2020
ms.locfileid: "48582354"
---
# <a name="permission-resource-type"></a><span data-ttu-id="96185-103">Тип ресурса разрешения</span><span class="sxs-lookup"><span data-stu-id="96185-103">permission resource type</span></span>

<span data-ttu-id="96185-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96185-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96185-105">Ресурс **Permission** предоставляет сведения о разрешении на совместный доступ, предоставленном для ресурса [driveItem](driveitem.md) .</span><span class="sxs-lookup"><span data-stu-id="96185-105">The **permission** resource provides information about a sharing permission granted for a [driveItem](driveitem.md) resource.</span></span>

<span data-ttu-id="96185-106">Разрешения на совместный доступ могут иметь самые различные формы.</span><span class="sxs-lookup"><span data-stu-id="96185-106">Sharing permissions have a number of different forms.</span></span>
<span data-ttu-id="96185-107">Ресурс **Permission** представляет эти различные формы с помощью аспектов ресурса.</span><span class="sxs-lookup"><span data-stu-id="96185-107">The **permission** resource represents these different forms through facets on the resource.</span></span>

><span data-ttu-id="96185-108">**Примечание:** Библиотеки документов OneDrive для бизнеса и SharePoint не возвращают свойство **inheritedFrom** .</span><span class="sxs-lookup"><span data-stu-id="96185-108">**Note:** OneDrive for Business and SharePoint document libraries do not return the **inheritedFrom** property.</span></span>

## <a name="json-representation"></a><span data-ttu-id="96185-109">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="96185-109">JSON representation</span></span>

<span data-ttu-id="96185-110">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="96185-110">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="96185-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="96185-111">Properties</span></span>

| <span data-ttu-id="96185-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="96185-112">Property</span></span>            | <span data-ttu-id="96185-113">Тип</span><span class="sxs-lookup"><span data-stu-id="96185-113">Type</span></span>                        | <span data-ttu-id="96185-114">Описание</span><span class="sxs-lookup"><span data-stu-id="96185-114">Description</span></span>
|:--------------------|:----------------------------|:-------------------------
| <span data-ttu-id="96185-115">id</span><span class="sxs-lookup"><span data-stu-id="96185-115">id</span></span>                  | <span data-ttu-id="96185-116">Строка</span><span class="sxs-lookup"><span data-stu-id="96185-116">String</span></span>                      | <span data-ttu-id="96185-p102">Уникальный идентификатор разрешения среди всех разрешений для элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="96185-p102">The unique identifier of the permission among all permissions on the item. Read-only.</span></span>
| <span data-ttu-id="96185-119">grantedTo</span><span class="sxs-lookup"><span data-stu-id="96185-119">grantedTo</span></span>           | <span data-ttu-id="96185-120">[IdentitySet][]</span><span class="sxs-lookup"><span data-stu-id="96185-120">[IdentitySet][]</span></span>             | <span data-ttu-id="96185-p103">Для разрешений типа user: сведения о пользователях и приложениях для этого разрешения. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="96185-p103">For user type permissions, the details of the users & applications for this permission. Read-only.</span></span>
| <span data-ttu-id="96185-123">grantedToIdentities</span><span class="sxs-lookup"><span data-stu-id="96185-123">grantedToIdentities</span></span> | <span data-ttu-id="96185-124">Collection([IdentitySet][])</span><span class="sxs-lookup"><span data-stu-id="96185-124">Collection([IdentitySet][])</span></span> | <span data-ttu-id="96185-125">Для разрешений типа link: сведения о пользователях, которым предоставлено разрешение.</span><span class="sxs-lookup"><span data-stu-id="96185-125">For link type permissions, the details of the users to whom permission was granted.</span></span> <span data-ttu-id="96185-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="96185-126">Read-only.</span></span>
| <span data-ttu-id="96185-127">invitation</span><span class="sxs-lookup"><span data-stu-id="96185-127">invitation</span></span>          | <span data-ttu-id="96185-128">[SharingInvitation][]</span><span class="sxs-lookup"><span data-stu-id="96185-128">[SharingInvitation][]</span></span>       | <span data-ttu-id="96185-p105">Сведения обо всех сопоставленных приглашениях к совместному использованию для данного разрешения. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="96185-p105">Details of any associated sharing invitation for this permission. Read-only.</span></span>
| <span data-ttu-id="96185-131">inheritedFrom</span><span class="sxs-lookup"><span data-stu-id="96185-131">inheritedFrom</span></span>       | <span data-ttu-id="96185-132">[ItemReference][]</span><span class="sxs-lookup"><span data-stu-id="96185-132">[ItemReference][]</span></span>           | <span data-ttu-id="96185-p106">Предоставляет ссылку на предка текущего разрешения, если оно унаследовано от предка. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="96185-p106">Provides a reference to the ancestor of the current permission, if it is inherited from an ancestor. Read-only.</span></span>
| <span data-ttu-id="96185-135">ссылка</span><span class="sxs-lookup"><span data-stu-id="96185-135">link</span></span>                | <span data-ttu-id="96185-136">[SharingLink][]</span><span class="sxs-lookup"><span data-stu-id="96185-136">[SharingLink][]</span></span>             | <span data-ttu-id="96185-p107">Предоставляет сведения о ссылке для текущего разрешения, если это разрешение типа link. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="96185-p107">Provides the link details of the current permission, if it is a link type permissions. Read-only.</span></span>
| <span data-ttu-id="96185-139">roles</span><span class="sxs-lookup"><span data-stu-id="96185-139">roles</span></span>               | <span data-ttu-id="96185-140">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="96185-140">Collection(String)</span></span>          | <span data-ttu-id="96185-p108">Тип разрешения, например `read`. Полный список ролей см. ниже. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="96185-p108">The type of permission, e.g. `read`. See below for the full list of roles. Read-only.</span></span>
| <span data-ttu-id="96185-144">shareId</span><span class="sxs-lookup"><span data-stu-id="96185-144">shareId</span></span>             | <span data-ttu-id="96185-145">String</span><span class="sxs-lookup"><span data-stu-id="96185-145">String</span></span>                      | <span data-ttu-id="96185-146">Уникальный маркер, с помощью которого можно получить доступ к общему элементу через **[API общих папок][]**.</span><span class="sxs-lookup"><span data-stu-id="96185-146">A unique token that can be used to access this shared item via the **[shares API][]**.</span></span> <span data-ttu-id="96185-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="96185-147">Read-only.</span></span>
| <span data-ttu-id="96185-148">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="96185-148">expirationDateTime</span></span>  | <span data-ttu-id="96185-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96185-149">DateTimeOffset</span></span>              | <span data-ttu-id="96185-150">Формат гггг-ММ-ддTЧЧ:мм:ссZ свойства DateTimeOffset указывает время окончания срока действия разрешения.</span><span class="sxs-lookup"><span data-stu-id="96185-150">A format of yyyy-MM-ddTHH:mm:ssZ of DateTimeOffset indicates the expiration time of the permission.</span></span> <span data-ttu-id="96185-151">DateTime.MinValue указывает, что для этого разрешения не установлен срок действия.</span><span class="sxs-lookup"><span data-stu-id="96185-151">DateTime.MinValue indicates there is no expiration set for this permission.</span></span> <span data-ttu-id="96185-152">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="96185-152">Optional.</span></span>
| <span data-ttu-id="96185-153">hasPassword</span><span class="sxs-lookup"><span data-stu-id="96185-153">hasPassword</span></span>         | <span data-ttu-id="96185-154">Логическое</span><span class="sxs-lookup"><span data-stu-id="96185-154">Boolean</span></span>                     | <span data-ttu-id="96185-155">Указывает, настроен ли для этого разрешения пароль. Отображается только в отклике.</span><span class="sxs-lookup"><span data-stu-id="96185-155">This indicates whether password is set for this permission, it's only showing in response.</span></span> <span data-ttu-id="96185-156">Необязательно, только для чтения и предназначено только для OneDrive персональный.</span><span class="sxs-lookup"><span data-stu-id="96185-156">Optional and Read-only and for OneDrive Personal only.</span></span>

### <a name="roles-property-values"></a><span data-ttu-id="96185-157">Значения свойств роли</span><span class="sxs-lookup"><span data-stu-id="96185-157">Roles property values</span></span>

| <span data-ttu-id="96185-158">Роль</span><span class="sxs-lookup"><span data-stu-id="96185-158">Role</span></span>              | <span data-ttu-id="96185-159">Сведения</span><span class="sxs-lookup"><span data-stu-id="96185-159">Details</span></span>                                                                        |
|:------------------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="96185-160">read</span><span class="sxs-lookup"><span data-stu-id="96185-160">read</span></span>            | <span data-ttu-id="96185-161">Дает возможность считывать метаданные и содержимое элемента.</span><span class="sxs-lookup"><span data-stu-id="96185-161">Provides the ability to read the metadata and contents of the item.</span></span>            |
| <span data-ttu-id="96185-162">write</span><span class="sxs-lookup"><span data-stu-id="96185-162">write</span></span>           | <span data-ttu-id="96185-163">Дает возможность считывать и изменять метаданные и содержимое элемента.</span><span class="sxs-lookup"><span data-stu-id="96185-163">Provides the ability to read and modify the metadata and contents of the item.</span></span> |
| <span data-ttu-id="96185-164">sp.full control</span><span class="sxs-lookup"><span data-stu-id="96185-164">sp.full control</span></span> | <span data-ttu-id="96185-165">В случае с SharePoint и OneDrive для бизнеса представляет роль владельца.</span><span class="sxs-lookup"><span data-stu-id="96185-165">For SharePoint and OneDrive for Business this represents the owner role.</span></span>       |

<span data-ttu-id="96185-166">Ресурс Permission предоставляет сведения о типе разрешения, представленного ресурсом, с помощью _аспектов_.</span><span class="sxs-lookup"><span data-stu-id="96185-166">The permission resource uses _facets_ to provide information about the kind of permission represented by the resource.</span></span>

<span data-ttu-id="96185-167">Ссылки совместного доступа содержат уникальный маркер, необходимый для доступа к элементу.</span><span class="sxs-lookup"><span data-stu-id="96185-167">Sharing links contain a unique token required to access the item.</span></span>

<span data-ttu-id="96185-168">Разрешения с аспектом [**invitation**][SharingInvitation] представляют разрешения, добавленные путем приглашения определенных пользователей или групп для доступа к файлу.</span><span class="sxs-lookup"><span data-stu-id="96185-168">Permissions with an [**invitation**][SharingInvitation] facet represent permissions added by inviting specific users or groups to have access to the file.</span></span>

## <a name="sharing-links"></a><span data-ttu-id="96185-169">Ссылки совместного доступа</span><span class="sxs-lookup"><span data-stu-id="96185-169">Sharing links</span></span>

<span data-ttu-id="96185-170">Разрешения с аспектом [**link**][SharingLink] представляют ссылки для совместного доступа, созданные в элементе.</span><span class="sxs-lookup"><span data-stu-id="96185-170">Permissions with a [**link**][SharingLink] facet represent sharing links created on the item.</span></span>
<span data-ttu-id="96185-171">Это наиболее распространенные типы разрешений.</span><span class="sxs-lookup"><span data-stu-id="96185-171">These are the most common kinds of permissions.</span></span>
<span data-ttu-id="96185-172">Ссылки для совместного доступа предоставляют уникальный URL-адрес, который можно использовать для доступа к файлу или папке.</span><span class="sxs-lookup"><span data-stu-id="96185-172">Sharing links provide a unique URL that can be used to access a file or folder.</span></span>
<span data-ttu-id="96185-173">Их можно настроить для предоставления доступа различными способами.</span><span class="sxs-lookup"><span data-stu-id="96185-173">They can be set up to grant access in a variety of ways.</span></span>
<span data-ttu-id="96185-174">Например, вы можете использовать API [createLink][], чтобы создать ссылку, доступную любым пользователям, вошедшим в вашу организацию, или вы можете создать ссылку, доступную всем пользователями без необходимости входа.</span><span class="sxs-lookup"><span data-stu-id="96185-174">For example, you can use the [createLink][] API to create a link that works for anyone signed into your organization, or you can create a link that works for anyone, without needing to sign in.</span></span>
<span data-ttu-id="96185-175">Вы можете использовать API [приглашения][], чтобы создать ссылку, доступную только определенным пользователям, независимо от того, относятся ли они к вашей организации или нет.</span><span class="sxs-lookup"><span data-stu-id="96185-175">You can use the [invite][] API to create a link that only works for specific people, whether they're in your company or not.</span></span>

<span data-ttu-id="96185-176">Вот несколько примеров ссылок совместного доступа.</span><span class="sxs-lookup"><span data-stu-id="96185-176">Here are some examples of sharing links.</span></span>

### <a name="view-link"></a><span data-ttu-id="96185-177">Ссылка для просмотра</span><span class="sxs-lookup"><span data-stu-id="96185-177">View link</span></span>

<span data-ttu-id="96185-178">Эта ссылка для просмотра предоставляет доступ только для чтения любому пользователю с ссылкой.</span><span class="sxs-lookup"><span data-stu-id="96185-178">This view link provides read-only access to anyone with the link.</span></span>

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

### <a name="edit-link"></a><span data-ttu-id="96185-179">Ссылка для редактирования</span><span class="sxs-lookup"><span data-stu-id="96185-179">Edit link</span></span>

<span data-ttu-id="96185-180">Эта ссылка для редактирования предоставляет доступ для чтения и записи любому пользователю в организации, у которого есть ссылка.</span><span class="sxs-lookup"><span data-stu-id="96185-180">This edit link provides read and write access to anyone in the organization with the link.</span></span>

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

### <a name="existing-access-link"></a><span data-ttu-id="96185-181">Существующая ссылка для доступа</span><span class="sxs-lookup"><span data-stu-id="96185-181">Existing access link</span></span>

<span data-ttu-id="96185-182">Эта ссылка не предоставляет пользователю никаких дополнительных прав.</span><span class="sxs-lookup"><span data-stu-id="96185-182">This link does not grant any additional privileges to the user.</span></span>

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

### <a name="specific-people-link"></a><span data-ttu-id="96185-183">Ссылка для определенных пользователей</span><span class="sxs-lookup"><span data-stu-id="96185-183">Specific people link</span></span>

<span data-ttu-id="96185-184">Эта ссылка предоставляет доступ для чтения и записи определенным пользователям в коллекции `grantedToIdentities`.</span><span class="sxs-lookup"><span data-stu-id="96185-184">This link provides read and write access to the specific people in the `grantedToIdentities` collection.</span></span>

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

## <a name="sharing-invitations"></a><span data-ttu-id="96185-185">Приглашение на общий доступ</span><span class="sxs-lookup"><span data-stu-id="96185-185">Sharing invitations</span></span>

<span data-ttu-id="96185-186">Разрешения, отправляемые API [INVITE][] или [предоставления][] , могут содержать дополнительные сведения в [invitation][SharingInvitation] аспекта приглашения для адресов электронной почты, которые не совпадают с известной учетной записью.</span><span class="sxs-lookup"><span data-stu-id="96185-186">Permissions sent by the [invite][] or [grant][] API can have additional information in the [invitation][SharingInvitation] facet for email addresses that don't match a known account.</span></span> <span data-ttu-id="96185-187">В таких случаях свойство **грантедто** может быть настроено до тех пор, пока не будет активирована ссылка приглашения, которая возникает при первом щелчке ссылки и входе в систему.</span><span class="sxs-lookup"><span data-stu-id="96185-187">In such cases, the **grantedTo** property might not be set until the invitation link is redeemed, which occurs the first time the user clicks the link and signs in.</span></span>

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

<span data-ttu-id="96185-188">Когда пользователь активирует приглашение к совместному использованию, в свойстве **grantedTo** появятся сведения об учетной записи, которая активировала разрешения:</span><span class="sxs-lookup"><span data-stu-id="96185-188">After the sharing invitation has been redeemed by a user, the **grantedTo** property will contain the information about the account that redeemed the permissions:</span></span>

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

## <a name="methods"></a><span data-ttu-id="96185-189">Методы</span><span class="sxs-lookup"><span data-stu-id="96185-189">Methods</span></span>

| <span data-ttu-id="96185-190">Метод</span><span class="sxs-lookup"><span data-stu-id="96185-190">Method</span></span>                                                   | <span data-ttu-id="96185-191">Путь REST</span><span class="sxs-lookup"><span data-stu-id="96185-191">REST Path</span></span>
|:---------------------------------------------------------|:-----------------------
| [<span data-ttu-id="96185-192">Получение списка разрешений</span><span class="sxs-lookup"><span data-stu-id="96185-192">List permissions</span></span>](../api/driveitem-list-permissions.md) | `GET /drive/items/{item-id}/permissions`
| [<span data-ttu-id="96185-193">Получение разрешения</span><span class="sxs-lookup"><span data-stu-id="96185-193">Get permission</span></span>](../api/permission-get.md)               | `GET /drive/items/{item-id}/permissions/{id}`
| <span data-ttu-id="96185-194">[Создание ссылки][createLink]</span><span class="sxs-lookup"><span data-stu-id="96185-194">[Create link][createLink]</span></span>                                | `POST /drive/items/{item-id}/createLink`
| <span data-ttu-id="96185-195">[Приглашение участников][invite]</span><span class="sxs-lookup"><span data-stu-id="96185-195">[Invite people][invite]</span></span>                                  | `POST /drive/items/{item-id}/invite`
| [<span data-ttu-id="96185-196">Обновление</span><span class="sxs-lookup"><span data-stu-id="96185-196">Update</span></span>](../api/permission-update.md)                    | `PATCH /drive/items/{item-id}/permissions/{id}`
| <span data-ttu-id="96185-197">[удаление](../api/permission-delete.md);</span><span class="sxs-lookup"><span data-stu-id="96185-197">[Delete](../api/permission-delete.md)</span></span>                    | `DELETE /drive/items/{item-id}/permissions/{id}`
| [<span data-ttu-id="96185-198">Добавление пользователей в ссылку совместного доступа</span><span class="sxs-lookup"><span data-stu-id="96185-198">Add users to sharing link</span></span>](../api/permission-grant.md)  | `POST /shares/{encoded-sharing-url}/permission/grant`
| [<span data-ttu-id="96185-199">Отзыв разрешений</span><span class="sxs-lookup"><span data-stu-id="96185-199">Revoke grants</span></span>](../api/permission-revokegrants.md)   | `POST /drive/items/{item-id}/permissions/{id}/revokeGrants`

[createLink]: ../api/driveitem-createlink.md
[обладают]: ../api/permission-grant.md
[grant]: ../api/permission-grant.md
[IdentitySet]: identityset.md
[invite]: ../api/driveitem-invite.md
[ItemReference]: itemreference.md
[API общих папок]: ../api/shares-get.md
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
