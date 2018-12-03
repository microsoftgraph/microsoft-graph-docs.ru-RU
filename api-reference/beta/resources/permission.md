---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Permission
ms.openlocfilehash: 195d4840fdb25339eda3858c0bac2395ee9b1c4a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081638"
---
# <a name="permission-resource-type"></a><span data-ttu-id="38ea2-102">Тип ресурса разрешения</span><span class="sxs-lookup"><span data-stu-id="38ea2-102">permission resource type</span></span>

> <span data-ttu-id="38ea2-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="38ea2-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="38ea2-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38ea2-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="38ea2-105">**Разрешение** ресурсов предоставляет сведения о общего доступа разрешение дается для [driveItem](driveitem.md) ресурсов.</span><span class="sxs-lookup"><span data-stu-id="38ea2-105">The **permission** resource provides information about a sharing permission granted for a [driveItem](driveitem.md) resource.</span></span>

<span data-ttu-id="38ea2-106">Разрешения на совместный доступ могут принимать самые различные формы.</span><span class="sxs-lookup"><span data-stu-id="38ea2-106">Sharing permissions have a number of different forms.</span></span>
<span data-ttu-id="38ea2-107">**Разрешение** ресурсов представляет этих различных форм через аспектов для ресурса.</span><span class="sxs-lookup"><span data-stu-id="38ea2-107">The **permission** resource represents these different forms through facets on the resource.</span></span>

><span data-ttu-id="38ea2-108">**Примечание:** OneDrive для бизнеса и SharePoint библиотек документов не возвращают свойство **inheritedFrom** .</span><span class="sxs-lookup"><span data-stu-id="38ea2-108">**Note:** OneDrive for Business and SharePoint document libraries do not return the **inheritedFrom** property.</span></span>

## <a name="json-representation"></a><span data-ttu-id="38ea2-109">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="38ea2-109">JSON representation</span></span>

<span data-ttu-id="38ea2-110">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="38ea2-110">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="38ea2-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="38ea2-111">Properties</span></span>

| <span data-ttu-id="38ea2-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="38ea2-112">Property</span></span>            | <span data-ttu-id="38ea2-113">Тип</span><span class="sxs-lookup"><span data-stu-id="38ea2-113">Type</span></span>                        | <span data-ttu-id="38ea2-114">Описание</span><span class="sxs-lookup"><span data-stu-id="38ea2-114">Description</span></span>
|:--------------------|:----------------------------|:-------------------------
| <span data-ttu-id="38ea2-115">id</span><span class="sxs-lookup"><span data-stu-id="38ea2-115">id</span></span>                  | <span data-ttu-id="38ea2-116">Строка</span><span class="sxs-lookup"><span data-stu-id="38ea2-116">String</span></span>                      | <span data-ttu-id="38ea2-p103">Уникальный идентификатор разрешения среди всех разрешений для элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="38ea2-p103">The unique identifier of the permission among all permissions on the item. Read-only.</span></span>
| <span data-ttu-id="38ea2-119">grantedTo</span><span class="sxs-lookup"><span data-stu-id="38ea2-119">grantedTo</span></span>           | <span data-ttu-id="38ea2-120">[IdentitySet][]</span><span class="sxs-lookup"><span data-stu-id="38ea2-120">[IdentitySet][]</span></span>             | <span data-ttu-id="38ea2-p104">Для разрешений типа user: сведения о пользователях и приложениях для этого разрешения. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="38ea2-p104">For user type permissions, the details of the users & applications for this permission. Read-only.</span></span>
| <span data-ttu-id="38ea2-123">grantedToIdentities</span><span class="sxs-lookup"><span data-stu-id="38ea2-123">grantedToIdentities</span></span> | <span data-ttu-id="38ea2-124">Коллекции ([IdentitySet][])</span><span class="sxs-lookup"><span data-stu-id="38ea2-124">Collection([IdentitySet][])</span></span> | <span data-ttu-id="38ea2-125">Для разрешения ссылок типа сведения о пользователях, которым были предоставлены разрешения.</span><span class="sxs-lookup"><span data-stu-id="38ea2-125">For link type permissions, the details of the users to whom permission was granted.</span></span> <span data-ttu-id="38ea2-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="38ea2-126">Read-only.</span></span>
| <span data-ttu-id="38ea2-127">invitation</span><span class="sxs-lookup"><span data-stu-id="38ea2-127">invitation</span></span>          | <span data-ttu-id="38ea2-128">[SharingInvitation][]</span><span class="sxs-lookup"><span data-stu-id="38ea2-128">[SharingInvitation][]</span></span>       | <span data-ttu-id="38ea2-p106">Сведения обо всех сопоставленных приглашениях к совместному использованию для данного разрешения. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="38ea2-p106">Details of any associated sharing invitation for this permission. Read-only.</span></span>
| <span data-ttu-id="38ea2-131">inheritedFrom</span><span class="sxs-lookup"><span data-stu-id="38ea2-131">inheritedFrom</span></span>       | <span data-ttu-id="38ea2-132">[ItemReference][]</span><span class="sxs-lookup"><span data-stu-id="38ea2-132">[ItemReference][]</span></span>           | <span data-ttu-id="38ea2-p107">Предоставляет ссылку на предка текущего разрешения, если оно унаследовано от предка. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="38ea2-p107">Provides a reference to the ancestor of the current permission, if it is inherited from an ancestor. Read-only.</span></span>
| <span data-ttu-id="38ea2-135">ссылка</span><span class="sxs-lookup"><span data-stu-id="38ea2-135">link</span></span>                | <span data-ttu-id="38ea2-136">[SharingLink][]</span><span class="sxs-lookup"><span data-stu-id="38ea2-136">[SharingLink][]</span></span>             | <span data-ttu-id="38ea2-p108">Предоставляет сведения о ссылке для текущего разрешения, если это разрешение типа link. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="38ea2-p108">Provides the link details of the current permission, if it is a link type permissions. Read-only.</span></span>
| <span data-ttu-id="38ea2-139">roles</span><span class="sxs-lookup"><span data-stu-id="38ea2-139">roles</span></span>               | <span data-ttu-id="38ea2-140">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="38ea2-140">Collection(String)</span></span>          | <span data-ttu-id="38ea2-p109">Тип разрешения, например `read`. Полный список ролей см. ниже. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="38ea2-p109">The type of permission, e.g. `read`. See below for the full list of roles. Read-only.</span></span>
| <span data-ttu-id="38ea2-144">shareId</span><span class="sxs-lookup"><span data-stu-id="38ea2-144">shareId</span></span>             | <span data-ttu-id="38ea2-145">String</span><span class="sxs-lookup"><span data-stu-id="38ea2-145">String</span></span>                      | <span data-ttu-id="38ea2-146">Уникальный маркер, который можно использовать для доступа к этой общий элемент через **[общий API][]**.</span><span class="sxs-lookup"><span data-stu-id="38ea2-146">A unique token that can be used to access this shared item via the **[shares API][]**.</span></span> <span data-ttu-id="38ea2-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="38ea2-147">Read-only.</span></span>
| <span data-ttu-id="38ea2-148">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="38ea2-148">expirationDateTime</span></span>  | <span data-ttu-id="38ea2-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38ea2-149">DateTimeOffset</span></span>              | <span data-ttu-id="38ea2-150">В формате гггг-мм-Ддвчч DateTimeOffset указывает время истечения срока действия разрешения.</span><span class="sxs-lookup"><span data-stu-id="38ea2-150">A format of yyyy-MM-ddTHH:mm:ssZ of DateTimeOffset indicates the expiration time of the permission.</span></span> <span data-ttu-id="38ea2-151">DateTime.MinValue указывает на наличие задано без ограничения срока действия для этого разрешения.</span><span class="sxs-lookup"><span data-stu-id="38ea2-151">DateTime.MinValue indicates there is no expiration set for this permission.</span></span> <span data-ttu-id="38ea2-152">Необязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="38ea2-152">Optional.</span></span>
| <span data-ttu-id="38ea2-153">hasPassword</span><span class="sxs-lookup"><span data-stu-id="38ea2-153">hasPassword</span></span>         | <span data-ttu-id="38ea2-154">Логический</span><span class="sxs-lookup"><span data-stu-id="38ea2-154">Boolean</span></span>                     | <span data-ttu-id="38ea2-155">Указывает, будет ли для этого разрешения, задать пароль, отображаются в ответ.</span><span class="sxs-lookup"><span data-stu-id="38ea2-155">This indicates whether password is set for this permission, it's only showing in response.</span></span> <span data-ttu-id="38ea2-156">Необязательный и только для чтения и только личные OneDrive.</span><span class="sxs-lookup"><span data-stu-id="38ea2-156">Optional and Read-only and for OneDrive Personal only.</span></span>

### <a name="roles-enumeration-values"></a><span data-ttu-id="38ea2-157">Значения перечисления роли</span><span class="sxs-lookup"><span data-stu-id="38ea2-157">Roles enumeration values</span></span>

| <span data-ttu-id="38ea2-158">Значение</span><span class="sxs-lookup"><span data-stu-id="38ea2-158">Value</span></span>        | <span data-ttu-id="38ea2-159">Сведения</span><span class="sxs-lookup"><span data-stu-id="38ea2-159">Details</span></span>                                                                        |
|:------------|:-------------------------------------------------------------------------------|
| `read`      | <span data-ttu-id="38ea2-160">Дает возможность считывать метаданные и содержимое элемента.</span><span class="sxs-lookup"><span data-stu-id="38ea2-160">Provides the ability to read the metadata and contents of the item.</span></span>            |
| `write`     | <span data-ttu-id="38ea2-161">Дает возможность считывать и изменять метаданные и содержимое элемента.</span><span class="sxs-lookup"><span data-stu-id="38ea2-161">Provides the ability to read and modify the metadata and contents of the item.</span></span> |
| `sp.owner`  | <span data-ttu-id="38ea2-162">В случае с SharePoint и OneDrive для бизнеса представляет роль владельца.</span><span class="sxs-lookup"><span data-stu-id="38ea2-162">For SharePoint and OneDrive for Business this represents the owner role.</span></span>       |
| `sp.member` | <span data-ttu-id="38ea2-163">В случае с SharePoint и OneDrive для бизнеса представляет роль участника.</span><span class="sxs-lookup"><span data-stu-id="38ea2-163">For SharePoint and OneDrive for Business this represents the member role.</span></span>      |

<span data-ttu-id="38ea2-164">Ресурс Permission предоставляет сведения о типе разрешения, представленного ресурсом, с помощью _аспектов_.</span><span class="sxs-lookup"><span data-stu-id="38ea2-164">The permission resource uses _facets_ to provide information about the kind of permission represented by the resource.</span></span>

<span data-ttu-id="38ea2-165">Общего доступа ссылки содержат уникальный маркер, необходимые для доступа к элементу.</span><span class="sxs-lookup"><span data-stu-id="38ea2-165">Sharing links contain a unique token required to access the item.</span></span>

<span data-ttu-id="38ea2-166">Разрешения с аспектом [**invitation**][SharingInvitation] представляют разрешения, добавленные путем приглашения определенных пользователей или групп для доступа к файлу.</span><span class="sxs-lookup"><span data-stu-id="38ea2-166">Permissions with an [**invitation**][SharingInvitation] facet represent permissions added by inviting specific users or groups to have access to the file.</span></span>

## <a name="sharing-links"></a><span data-ttu-id="38ea2-167">Ссылки для общего доступа</span><span class="sxs-lookup"><span data-stu-id="38ea2-167">Sharing links</span></span>

<span data-ttu-id="38ea2-168">Разрешения с помощью представляют аспекта[SharingLink] [**ссылок**], общий доступ к ссылок, созданных для элемента.</span><span class="sxs-lookup"><span data-stu-id="38ea2-168">Permissions with a [**link**][SharingLink] facet represent sharing links created on the item.</span></span>
<span data-ttu-id="38ea2-169">Это наиболее распространенных типов разрешений.</span><span class="sxs-lookup"><span data-stu-id="38ea2-169">These are the most common kinds of permissions.</span></span>
<span data-ttu-id="38ea2-170">Общего доступа к ссылкам уникальных URL-адрес, который можно использовать для доступа к файлу или папки.</span><span class="sxs-lookup"><span data-stu-id="38ea2-170">Sharing links provide a unique URL that can be used to access a file or folder.</span></span>
<span data-ttu-id="38ea2-171">Они могут настраиваться для предоставления доступа в различными способами.</span><span class="sxs-lookup"><span data-stu-id="38ea2-171">They can be set up to grant access in a variety of ways.</span></span>
<span data-ttu-id="38ea2-172">Например можно использовать [команду createLink][] API для создания связи, которая работает для всех вошел в вашей организации, или можно создать ссылку, которая работает для всех пользователей, без необходимости входа в.</span><span class="sxs-lookup"><span data-stu-id="38ea2-172">For example, you can use the [createLink][] API to create a link that works for anyone signed into your organization, or you can create a link that works for anyone, without needing to sign in.</span></span>
<span data-ttu-id="38ea2-173">[Приглашение][] API можно использовать для создания ссылок, который работает только для определенных пользователей ли они в вашей компании или нет.</span><span class="sxs-lookup"><span data-stu-id="38ea2-173">You can use the [invite][] API to create a link that only works for specific people, whether they're in your company or not.</span></span>

<span data-ttu-id="38ea2-174">Ниже приведены некоторые примеры того, общий доступ к ссылки.</span><span class="sxs-lookup"><span data-stu-id="38ea2-174">Here are some examples of sharing links.</span></span>

### <a name="view-link"></a><span data-ttu-id="38ea2-175">Просмотр ссылки</span><span class="sxs-lookup"><span data-stu-id="38ea2-175">View link</span></span>

<span data-ttu-id="38ea2-176">В этом представлении ссылку предоставляет доступ только для чтения всем пользователям, с помощью ссылки.</span><span class="sxs-lookup"><span data-stu-id="38ea2-176">This view link provides read-only access to anyone with the link.</span></span>

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

### <a name="edit-link"></a><span data-ttu-id="38ea2-177">Ссылка для редактирования</span><span class="sxs-lookup"><span data-stu-id="38ea2-177">Edit link</span></span>

<span data-ttu-id="38ea2-178">В этом ссылку Изменение предоставляет доступ на чтение и запись всем пользователям в организации с помощью ссылки.</span><span class="sxs-lookup"><span data-stu-id="38ea2-178">This edit link provides read and write access to anyone in the organization with the link.</span></span>

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

### <a name="specific-people-link"></a><span data-ttu-id="38ea2-179">Конкретные пользователи ссылок</span><span class="sxs-lookup"><span data-stu-id="38ea2-179">Specific people link</span></span>

<span data-ttu-id="38ea2-180">Ссылка на чтение и запись для конкретных пользователей в `grantedToIdentities` семейства сайтов.</span><span class="sxs-lookup"><span data-stu-id="38ea2-180">This link provides read and write access to the specific people in the `grantedToIdentities` collection.</span></span>

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

## <a name="sharing-invitations"></a><span data-ttu-id="38ea2-181">Общий доступ к приглашений</span><span class="sxs-lookup"><span data-stu-id="38ea2-181">Sharing invitations</span></span>

<span data-ttu-id="38ea2-182">Разрешения, отправленные с [Пригласить][] API могут предоставить дополнительную информацию в аспекта[SharingInvitation] [приглашение].</span><span class="sxs-lookup"><span data-stu-id="38ea2-182">Permissions sent by the [invite][] API may have additional information in the [invitation][SharingInvitation] facet.</span></span>
<span data-ttu-id="38ea2-183">Если приглашение было отправлено на адрес электронной почты, соответствует известной учетной записи, свойство **grantedTo** может не задано, пока погашен приглашение, которое происходит при первом пользователь щелкает ссылку и подписывает.</span><span class="sxs-lookup"><span data-stu-id="38ea2-183">If an invitation was sent to an email address that doesn't match a known account, the **grantedTo** property may not be set until the invitation is redeemed, which occurs the first time the user clicks the link and signs in.</span></span>

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

<span data-ttu-id="38ea2-184">Когда пользователь активирует приглашение к совместному использованию, в свойстве **grantedTo** появятся сведения об учетной записи, которая активировала разрешения:</span><span class="sxs-lookup"><span data-stu-id="38ea2-184">After the sharing invitation has been redeemed by a user, the **grantedTo** property will contain the information about the account that redeemed the permissions:</span></span>

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

## <a name="methods"></a><span data-ttu-id="38ea2-185">Методы</span><span class="sxs-lookup"><span data-stu-id="38ea2-185">Methods</span></span>

| <span data-ttu-id="38ea2-186">Метод</span><span class="sxs-lookup"><span data-stu-id="38ea2-186">Method</span></span>                                                   | <span data-ttu-id="38ea2-187">Путь REST</span><span class="sxs-lookup"><span data-stu-id="38ea2-187">REST Path</span></span>
|:---------------------------------------------------------|:-----------------------
| [<span data-ttu-id="38ea2-188">Получение списка разрешений</span><span class="sxs-lookup"><span data-stu-id="38ea2-188">List permissions</span></span>](../api/driveitem-list-permissions.md) | `GET /drive/items/{item-id}/permissions`
| [<span data-ttu-id="38ea2-189">Получение разрешения</span><span class="sxs-lookup"><span data-stu-id="38ea2-189">Get permission</span></span>](../api/permission-get.md)               | `GET /drive/items/{item-id}/permissions/{id}`
| <span data-ttu-id="38ea2-190">[Создать ссылку] [команду createLink]</span><span class="sxs-lookup"><span data-stu-id="38ea2-190">[Create link][createLink]</span></span>                                | `POST /drive/items/{item-id}/createLink`
| <span data-ttu-id="38ea2-191">[Приглашение пользователей] [приглашение]</span><span class="sxs-lookup"><span data-stu-id="38ea2-191">[Invite people][invite]</span></span>                                  | `POST /drive/items/{item-id}/invite`
| [<span data-ttu-id="38ea2-192">Обновление</span><span class="sxs-lookup"><span data-stu-id="38ea2-192">Update</span></span>](../api/permission-update.md)                    | `PATCH /drive/items/{item-id}/permissions/{id}`
| <span data-ttu-id="38ea2-193">[удаление](../api/permission-delete.md);</span><span class="sxs-lookup"><span data-stu-id="38ea2-193">[Delete](../api/permission-delete.md)</span></span>                    | `DELETE /drive/items/{item-id}/permissions/{id}`



[команду createLink]: ../api/driveitem-createlink.md
[createLink]: ../api/driveitem-createlink.md
[IdentitySet]: identityset.md
[приглашение]: ../api/driveitem-invite.md
[invite]: ../api/driveitem-invite.md
[ItemReference]: itemreference.md
[API общих папок]: ../api/shares-get.md
[shares API]: ../api/shares-get.md
[SharingInvitation]: sharinginvitation.md
[SharingLink]: sharinglink.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The permission object provides information about permissions and roles and sharing information.",
  "keywords": "sharing,permissions,read,write,acl",
  "section": "documentation",
  "tocPath": "Resources/Permission"
} -->
