---
title: Тип ресурса oAuth2Permission
description: Представляет OAuth 2.0 делегировать область разрешений. Указанный OAuth 2.0, области делегированных разрешений может быть затребованы клиентских приложений (через коллекцию **requiredResourceAccess** для объекта application) при вызове ресурса приложения. Свойство **appRoles** servicePrincipal сущности и сущности приложения — это коллекция **oAuth2Permission**.
ms.openlocfilehash: 4a790c935dd84fb7bd4e1422ca59914d9a319ae9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080301"
---
# <a name="oauth2permission-resource-type"></a><span data-ttu-id="78f99-105">Тип ресурса oAuth2Permission</span><span class="sxs-lookup"><span data-stu-id="78f99-105">oAuth2Permission resource type</span></span>

> <span data-ttu-id="78f99-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="78f99-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="78f99-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="78f99-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="78f99-108">Представляет OAuth 2.0 делегировать область разрешений.</span><span class="sxs-lookup"><span data-stu-id="78f99-108">Represents an OAuth 2.0 delegated permission scope.</span></span> <span data-ttu-id="78f99-109">Указанный OAuth 2.0, области делегированных разрешений может быть затребованы клиентских приложений (через коллекцию **requiredResourceAccess** для объекта [application](application.md) ) при вызове ресурса приложения.</span><span class="sxs-lookup"><span data-stu-id="78f99-109">The specified OAuth 2.0 delegated permission scopes may be requested by client applications (through the **requiredResourceAccess** collection on the [application](application.md) object) when calling a resource application.</span></span> <span data-ttu-id="78f99-110">Свойство **appRoles** [servicePrincipal](serviceprincipal.md) сущности и сущности [приложения](application.md) — это коллекция **oAuth2Permission**.</span><span class="sxs-lookup"><span data-stu-id="78f99-110">The **appRoles** property of the [servicePrincipal](serviceprincipal.md) entity and of the [application](application.md) entity is a collection of **oAuth2Permission**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="78f99-111">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="78f99-111">JSON representation</span></span>

<span data-ttu-id="78f99-112">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="78f99-112">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="78f99-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="78f99-113">Properties</span></span>
| <span data-ttu-id="78f99-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="78f99-114">Property</span></span>     | <span data-ttu-id="78f99-115">Тип</span><span class="sxs-lookup"><span data-stu-id="78f99-115">Type</span></span>   |<span data-ttu-id="78f99-116">Description</span><span class="sxs-lookup"><span data-stu-id="78f99-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="78f99-117">adminConsentDescription</span><span class="sxs-lookup"><span data-stu-id="78f99-117">adminConsentDescription</span></span>|<span data-ttu-id="78f99-118">String</span><span class="sxs-lookup"><span data-stu-id="78f99-118">String</span></span>|<span data-ttu-id="78f99-119">Текст справки разрешение, которое отображается в admin согласия и приложение назначения приемы и способы работы.</span><span class="sxs-lookup"><span data-stu-id="78f99-119">Permission help text that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="78f99-120">adminConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="78f99-120">adminConsentDisplayName</span></span>|<span data-ttu-id="78f99-121">String</span><span class="sxs-lookup"><span data-stu-id="78f99-121">String</span></span>|<span data-ttu-id="78f99-122">Отображаемое имя для разрешения, которое отображается в admin согласия и приложение назначения приемы и способы работы.</span><span class="sxs-lookup"><span data-stu-id="78f99-122">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="78f99-123">id</span><span class="sxs-lookup"><span data-stu-id="78f99-123">id</span></span>|<span data-ttu-id="78f99-124">Guid</span><span class="sxs-lookup"><span data-stu-id="78f99-124">Guid</span></span>|<span data-ttu-id="78f99-125">Идентификатор уникальные области разрешений внутри семейства oauth2Permissions.</span><span class="sxs-lookup"><span data-stu-id="78f99-125">Unique scope permission identifier inside the oauth2Permissions collection.</span></span>|
|<span data-ttu-id="78f99-126">isEnabled</span><span class="sxs-lookup"><span data-stu-id="78f99-126">isEnabled</span></span>|<span data-ttu-id="78f99-127">Логический</span><span class="sxs-lookup"><span data-stu-id="78f99-127">Boolean</span></span>|<span data-ttu-id="78f99-128">При создании или обновлении разрешение, это свойство должно быть присвоено **значение true** (по умолчанию).</span><span class="sxs-lookup"><span data-stu-id="78f99-128">When creating or updating a permission, this property must be set to **true** (which is the default).</span></span> <span data-ttu-id="78f99-129">Чтобы удалить разрешение, это свойство необходимо сначала задать значение **false**.</span><span class="sxs-lookup"><span data-stu-id="78f99-129">To delete a permission, this property must first be set to **false**.</span></span>  <span data-ttu-id="78f99-130">На этом этапе в последующих вызовов, могут быть удалены разрешения.</span><span class="sxs-lookup"><span data-stu-id="78f99-130">At that point, in a subsequent call, the permission may be removed.</span></span>|
|<span data-ttu-id="78f99-131">type</span><span class="sxs-lookup"><span data-stu-id="78f99-131">type</span></span>|<span data-ttu-id="78f99-132">String</span><span class="sxs-lookup"><span data-stu-id="78f99-132">String</span></span>|<span data-ttu-id="78f99-133">Указывает, является ли это разрешение области можно consented конечным пользователем или, будет ли это разрешение всей клиента, в котором должен быть consented к администратором компании.</span><span class="sxs-lookup"><span data-stu-id="78f99-133">Specifies whether this scope permission can be consented to by an end user, or whether it is a tenant-wide permission that must be consented to by a Company Administrator.</span></span>  <span data-ttu-id="78f99-134">Возможные значения: «Пользователь» или «Администратор».</span><span class="sxs-lookup"><span data-stu-id="78f99-134">Possible values are "User" or "Admin".</span></span>|
|<span data-ttu-id="78f99-135">userConsentDescription</span><span class="sxs-lookup"><span data-stu-id="78f99-135">userConsentDescription</span></span>|<span data-ttu-id="78f99-136">String</span><span class="sxs-lookup"><span data-stu-id="78f99-136">String</span></span>|<span data-ttu-id="78f99-137">Текст справки разрешение, которое отображается в рабочую среду согласия пользователя.</span><span class="sxs-lookup"><span data-stu-id="78f99-137">Permission help text that appears in the end user consent experience.</span></span>|
|<span data-ttu-id="78f99-138">userConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="78f99-138">userConsentDisplayName</span></span>|<span data-ttu-id="78f99-139">String</span><span class="sxs-lookup"><span data-stu-id="78f99-139">String</span></span>|<span data-ttu-id="78f99-140">Отображаемое имя для разрешения, которое отображается в рабочую среду согласия пользователя.</span><span class="sxs-lookup"><span data-stu-id="78f99-140">Display name for the permission that appears in the end user consent experience.</span></span>|
|<span data-ttu-id="78f99-141">value</span><span class="sxs-lookup"><span data-stu-id="78f99-141">value</span></span>|<span data-ttu-id="78f99-142">String</span><span class="sxs-lookup"><span data-stu-id="78f99-142">String</span></span>|<span data-ttu-id="78f99-143">Значение утверждения область, должно привести к приложению ресурсов в маркер доступа OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="78f99-143">The value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "oAuth2Permission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
