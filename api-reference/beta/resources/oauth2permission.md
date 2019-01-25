---
title: Тип ресурса oAuth2Permission
description: Представляет OAuth 2.0 делегировать область разрешений. Указанный OAuth 2.0, области делегированных разрешений может быть затребованы клиентских приложений (через коллекцию **requiredResourceAccess** для объекта application) при вызове ресурса приложения. Свойство **appRoles** servicePrincipal сущности и сущности приложения — это коллекция **oAuth2Permission**.
localization_priority: Normal
ms.openlocfilehash: 8d8bb0bb5af17b7322bd6be37ac48ae9edbeba42
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510815"
---
# <a name="oauth2permission-resource-type"></a><span data-ttu-id="14e2f-105">Тип ресурса oAuth2Permission</span><span class="sxs-lookup"><span data-stu-id="14e2f-105">oAuth2Permission resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14e2f-106">Представляет OAuth 2.0 делегировать область разрешений.</span><span class="sxs-lookup"><span data-stu-id="14e2f-106">Represents an OAuth 2.0 delegated permission scope.</span></span> <span data-ttu-id="14e2f-107">Указанный OAuth 2.0, области делегированных разрешений может быть затребованы клиентских приложений (через коллекцию **requiredResourceAccess** для объекта [application](application.md) ) при вызове ресурса приложения.</span><span class="sxs-lookup"><span data-stu-id="14e2f-107">The specified OAuth 2.0 delegated permission scopes may be requested by client applications (through the **requiredResourceAccess** collection on the [application](application.md) object) when calling a resource application.</span></span> <span data-ttu-id="14e2f-108">Свойство **appRoles** [servicePrincipal](serviceprincipal.md) сущности и сущности [приложения](application.md) — это коллекция **oAuth2Permission**.</span><span class="sxs-lookup"><span data-stu-id="14e2f-108">The **appRoles** property of the [servicePrincipal](serviceprincipal.md) entity and of the [application](application.md) entity is a collection of **oAuth2Permission**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="14e2f-109">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="14e2f-109">JSON representation</span></span>

<span data-ttu-id="14e2f-110">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="14e2f-110">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.oAuth2Permission"
}-->

```json
{
  "adminConsentDescription": "string",
  "adminConsentDisplayName": "string",
  "id": "guid",
  "isEnabled": true,
  "origin": "string",
  "type": "string",
  "userConsentDescription": "string",
  "userConsentDisplayName": "string",
  "value": "string"
}

```
## <a name="properties"></a><span data-ttu-id="14e2f-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="14e2f-111">Properties</span></span>
| <span data-ttu-id="14e2f-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="14e2f-112">Property</span></span>     | <span data-ttu-id="14e2f-113">Тип</span><span class="sxs-lookup"><span data-stu-id="14e2f-113">Type</span></span>   |<span data-ttu-id="14e2f-114">Описание</span><span class="sxs-lookup"><span data-stu-id="14e2f-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="14e2f-115">adminConsentDescription</span><span class="sxs-lookup"><span data-stu-id="14e2f-115">adminConsentDescription</span></span>|<span data-ttu-id="14e2f-116">String</span><span class="sxs-lookup"><span data-stu-id="14e2f-116">String</span></span>|<span data-ttu-id="14e2f-117">Текст справки разрешение, которое отображается в admin согласия и приложение назначения приемы и способы работы.</span><span class="sxs-lookup"><span data-stu-id="14e2f-117">Permission help text that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="14e2f-118">adminConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="14e2f-118">adminConsentDisplayName</span></span>|<span data-ttu-id="14e2f-119">String</span><span class="sxs-lookup"><span data-stu-id="14e2f-119">String</span></span>|<span data-ttu-id="14e2f-120">Отображаемое имя для разрешения, которое отображается в admin согласия и приложение назначения приемы и способы работы.</span><span class="sxs-lookup"><span data-stu-id="14e2f-120">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="14e2f-121">id</span><span class="sxs-lookup"><span data-stu-id="14e2f-121">id</span></span>|<span data-ttu-id="14e2f-122">Guid</span><span class="sxs-lookup"><span data-stu-id="14e2f-122">Guid</span></span>|<span data-ttu-id="14e2f-123">Идентификатор уникальные области разрешений внутри семейства oauth2Permissions.</span><span class="sxs-lookup"><span data-stu-id="14e2f-123">Unique scope permission identifier inside the oauth2Permissions collection.</span></span>|
|<span data-ttu-id="14e2f-124">isEnabled</span><span class="sxs-lookup"><span data-stu-id="14e2f-124">isEnabled</span></span>|<span data-ttu-id="14e2f-125">Логический</span><span class="sxs-lookup"><span data-stu-id="14e2f-125">Boolean</span></span>|<span data-ttu-id="14e2f-126">При создании или обновлении разрешение, это свойство должно быть присвоено **значение true** (по умолчанию).</span><span class="sxs-lookup"><span data-stu-id="14e2f-126">When creating or updating a permission, this property must be set to **true** (which is the default).</span></span> <span data-ttu-id="14e2f-127">Чтобы удалить разрешение, это свойство необходимо сначала задать значение **false**.</span><span class="sxs-lookup"><span data-stu-id="14e2f-127">To delete a permission, this property must first be set to **false**.</span></span>  <span data-ttu-id="14e2f-128">На этом этапе в последующих вызовов, могут быть удалены разрешения.</span><span class="sxs-lookup"><span data-stu-id="14e2f-128">At that point, in a subsequent call, the permission may be removed.</span></span>|
|<span data-ttu-id="14e2f-129">type</span><span class="sxs-lookup"><span data-stu-id="14e2f-129">type</span></span>|<span data-ttu-id="14e2f-130">String</span><span class="sxs-lookup"><span data-stu-id="14e2f-130">String</span></span>|<span data-ttu-id="14e2f-131">Указывает, является ли это разрешение области можно consented конечным пользователем или, будет ли это разрешение всей клиента, в котором должен быть consented к администратором компании.</span><span class="sxs-lookup"><span data-stu-id="14e2f-131">Specifies whether this scope permission can be consented to by an end user, or whether it is a tenant-wide permission that must be consented to by a Company Administrator.</span></span>  <span data-ttu-id="14e2f-132">Возможные значения: «Пользователь» или «Администратор».</span><span class="sxs-lookup"><span data-stu-id="14e2f-132">Possible values are "User" or "Admin".</span></span>|
|<span data-ttu-id="14e2f-133">userConsentDescription</span><span class="sxs-lookup"><span data-stu-id="14e2f-133">userConsentDescription</span></span>|<span data-ttu-id="14e2f-134">String</span><span class="sxs-lookup"><span data-stu-id="14e2f-134">String</span></span>|<span data-ttu-id="14e2f-135">Текст справки разрешение, которое отображается в рабочую среду согласия пользователя.</span><span class="sxs-lookup"><span data-stu-id="14e2f-135">Permission help text that appears in the end user consent experience.</span></span>|
|<span data-ttu-id="14e2f-136">userConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="14e2f-136">userConsentDisplayName</span></span>|<span data-ttu-id="14e2f-137">String</span><span class="sxs-lookup"><span data-stu-id="14e2f-137">String</span></span>|<span data-ttu-id="14e2f-138">Отображаемое имя для разрешения, которое отображается в рабочую среду согласия пользователя.</span><span class="sxs-lookup"><span data-stu-id="14e2f-138">Display name for the permission that appears in the end user consent experience.</span></span>|
|<span data-ttu-id="14e2f-139">value</span><span class="sxs-lookup"><span data-stu-id="14e2f-139">value</span></span>|<span data-ttu-id="14e2f-140">String</span><span class="sxs-lookup"><span data-stu-id="14e2f-140">String</span></span>|<span data-ttu-id="14e2f-141">Значение утверждения область, должно привести к приложению ресурсов в маркер доступа OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="14e2f-141">The value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oAuth2Permission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/oauth2permission.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
