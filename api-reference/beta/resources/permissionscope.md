---
title: Тип ресурса permissionScope
description: Представляет OAuth 2.0 делегировать область разрешений. Указанный OAuth 2.0, области делегированных разрешений может быть затребованы клиентских приложений (через коллекцию **requiredResourceAccess** для объекта Application) при вызове ресурса приложения. Свойство **oauth2Permissions** ServicePrincipal сущности и сущности приложения — это коллекция **OAuth2Permission**.
localization_priority: Normal
ms.openlocfilehash: 00629a6e123ef19290d3c1bd4797e4bab3ce95c0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517080"
---
# <a name="permissionscope-resource-type"></a><span data-ttu-id="f00cf-105">Тип ресурса permissionScope</span><span class="sxs-lookup"><span data-stu-id="f00cf-105">permissionScope resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f00cf-106">Представляет OAuth 2.0 делегировать область разрешений.</span><span class="sxs-lookup"><span data-stu-id="f00cf-106">Represents an OAuth 2.0 delegated permission scope.</span></span> <span data-ttu-id="f00cf-107">Указанный OAuth 2.0, области делегированных разрешений может быть затребованы клиентских приложений (через коллекцию **requiredResourceAccess** для объекта [Application](application.md) ) при вызове ресурса приложения.</span><span class="sxs-lookup"><span data-stu-id="f00cf-107">The specified OAuth 2.0 delegated permission scopes may be requested by client applications (through the **requiredResourceAccess** collection on the [Application](application.md) object) when calling a resource application.</span></span> <span data-ttu-id="f00cf-108">Свойство **oauth2Permissions** [ServicePrincipal](serviceprincipal.md) сущности и сущности [приложения](application.md) — это коллекция **OAuth2Permission**.</span><span class="sxs-lookup"><span data-stu-id="f00cf-108">The **oauth2Permissions** property of the [ServicePrincipal](serviceprincipal.md) entity and of the [Application](application.md) entity is a collection of **OAuth2Permission**.</span></span>

## <a name="properties"></a><span data-ttu-id="f00cf-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="f00cf-109">Properties</span></span>

| <span data-ttu-id="f00cf-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="f00cf-110">Property</span></span> | <span data-ttu-id="f00cf-111">Тип</span><span class="sxs-lookup"><span data-stu-id="f00cf-111">Type</span></span> | <span data-ttu-id="f00cf-112">Описание</span><span class="sxs-lookup"><span data-stu-id="f00cf-112">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="f00cf-113">adminConsentDescription</span><span class="sxs-lookup"><span data-stu-id="f00cf-113">adminConsentDescription</span></span>|<span data-ttu-id="f00cf-114">String</span><span class="sxs-lookup"><span data-stu-id="f00cf-114">String</span></span>| <span data-ttu-id="f00cf-115">Текст справки разрешение, которое отображается в admin согласия и приложение назначения приемы и способы работы.</span><span class="sxs-lookup"><span data-stu-id="f00cf-115">Permission help text that appears in the admin consent and app assignment experiences.</span></span> |
|<span data-ttu-id="f00cf-116">adminConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="f00cf-116">adminConsentDisplayName</span></span>|<span data-ttu-id="f00cf-117">String</span><span class="sxs-lookup"><span data-stu-id="f00cf-117">String</span></span>| <span data-ttu-id="f00cf-118">Отображаемое имя для разрешения, которое отображается в admin согласия и приложение назначения приемы и способы работы.</span><span class="sxs-lookup"><span data-stu-id="f00cf-118">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span> |
|<span data-ttu-id="f00cf-119">id</span><span class="sxs-lookup"><span data-stu-id="f00cf-119">id</span></span>|<span data-ttu-id="f00cf-120">Guid</span><span class="sxs-lookup"><span data-stu-id="f00cf-120">Guid</span></span>| <span data-ttu-id="f00cf-121">Идентификатор уникальные области разрешений внутри семейства oauth2Permissions.</span><span class="sxs-lookup"><span data-stu-id="f00cf-121">Unique scope permission identifier inside the oauth2Permissions collection.</span></span> |
|<span data-ttu-id="f00cf-122">isEnabled</span><span class="sxs-lookup"><span data-stu-id="f00cf-122">isEnabled</span></span>|<span data-ttu-id="f00cf-123">Логический</span><span class="sxs-lookup"><span data-stu-id="f00cf-123">Boolean</span></span>| <span data-ttu-id="f00cf-124">При создании или обновлении разрешение, это свойство должно быть присвоено **значение true** (по умолчанию).</span><span class="sxs-lookup"><span data-stu-id="f00cf-124">When creating or updating a permission, this property must be set to **true** (which is the default).</span></span> <span data-ttu-id="f00cf-125">Чтобы удалить разрешение, это свойство необходимо сначала задать значение **false**.</span><span class="sxs-lookup"><span data-stu-id="f00cf-125">To delete a permission, this property must first be set to **false**.</span></span> <span data-ttu-id="f00cf-126">На этом этапе в последующих вызовов, могут быть удалены разрешения.</span><span class="sxs-lookup"><span data-stu-id="f00cf-126">At that point, in a subsequent call, the permission may be removed.</span></span> |
|<span data-ttu-id="f00cf-127">Происхождение</span><span class="sxs-lookup"><span data-stu-id="f00cf-127">origin</span></span>|<span data-ttu-id="f00cf-128">String</span><span class="sxs-lookup"><span data-stu-id="f00cf-128">String</span></span>| <span data-ttu-id="f00cf-129">Для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="f00cf-129">For internal use.</span></span> |
|<span data-ttu-id="f00cf-130">type</span><span class="sxs-lookup"><span data-stu-id="f00cf-130">type</span></span>|<span data-ttu-id="f00cf-131">String</span><span class="sxs-lookup"><span data-stu-id="f00cf-131">String</span></span>| <span data-ttu-id="f00cf-132">Указывает, является ли это разрешение области можно consented конечным пользователем или, будет ли это разрешение всей клиента, в котором должен быть consented для администратором компании.</span><span class="sxs-lookup"><span data-stu-id="f00cf-132">Specifies whether this scope permission can be consented to by an end user, or whether it is a tenant-wide permission that must be consented to by a company administrator.</span></span> <span data-ttu-id="f00cf-133">Возможные значения: *пользователь* или *администратор*.</span><span class="sxs-lookup"><span data-stu-id="f00cf-133">Possible values are *User* or *Admin*.</span></span> |
|<span data-ttu-id="f00cf-134">userConsentDescription</span><span class="sxs-lookup"><span data-stu-id="f00cf-134">userConsentDescription</span></span>|<span data-ttu-id="f00cf-135">String</span><span class="sxs-lookup"><span data-stu-id="f00cf-135">String</span></span>| <span data-ttu-id="f00cf-136">Текст справки разрешение, которое отображается в разрешения для конечных пользователей.</span><span class="sxs-lookup"><span data-stu-id="f00cf-136">Permission help text that appears in the end-user consent experience.</span></span> |
|<span data-ttu-id="f00cf-137">userConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="f00cf-137">userConsentDisplayName</span></span>|<span data-ttu-id="f00cf-138">String</span><span class="sxs-lookup"><span data-stu-id="f00cf-138">String</span></span>| <span data-ttu-id="f00cf-139">Отображаемое имя для разрешения, которое отображается в разрешения для конечных пользователей.</span><span class="sxs-lookup"><span data-stu-id="f00cf-139">Display name for the permission that appears in the end-user consent experience.</span></span> |
|<span data-ttu-id="f00cf-140">value</span><span class="sxs-lookup"><span data-stu-id="f00cf-140">value</span></span>|<span data-ttu-id="f00cf-141">String</span><span class="sxs-lookup"><span data-stu-id="f00cf-141">String</span></span>| <span data-ttu-id="f00cf-142">Значение утверждения область, должно привести к приложению ресурсов в маркер доступа OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="f00cf-142">The value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f00cf-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f00cf-143">JSON representation</span></span>
<span data-ttu-id="f00cf-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f00cf-144">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.permissionScope"
}-->

```json
{
  "adminConsentDescription": "String",
  "adminConsentDisplayName": "String",
  "id": "Guid",
  "isEnabled": true,
  "origin": "String",
  "type": "String",
  "userConsentDescription": "String",
  "userConsentDisplayName": "String",
  "value": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "permissionScope resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/permissionscope.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
