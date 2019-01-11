---
title: Тип ресурса permissionScope
description: Представляет OAuth 2.0 делегировать область разрешений. Указанный OAuth 2.0, области делегированных разрешений может быть затребованы клиентских приложений (через коллекцию **requiredResourceAccess** для объекта Application) при вызове ресурса приложения. Свойство **oauth2Permissions** ServicePrincipal сущности и сущности приложения — это коллекция **OAuth2Permission**.
localization_priority: Normal
ms.openlocfilehash: a294316f5c6255d0873ce0dbe809c33dad89ae08
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818153"
---
# <a name="permissionscope-resource-type"></a><span data-ttu-id="70d4b-105">Тип ресурса permissionScope</span><span class="sxs-lookup"><span data-stu-id="70d4b-105">permissionScope resource type</span></span>

> <span data-ttu-id="70d4b-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="70d4b-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="70d4b-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70d4b-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="70d4b-108">Представляет OAuth 2.0 делегировать область разрешений.</span><span class="sxs-lookup"><span data-stu-id="70d4b-108">Represents an OAuth 2.0 delegated permission scope.</span></span> <span data-ttu-id="70d4b-109">Указанный OAuth 2.0, области делегированных разрешений может быть затребованы клиентских приложений (через коллекцию **requiredResourceAccess** для объекта [Application](application.md) ) при вызове ресурса приложения.</span><span class="sxs-lookup"><span data-stu-id="70d4b-109">The specified OAuth 2.0 delegated permission scopes may be requested by client applications (through the **requiredResourceAccess** collection on the [Application](application.md) object) when calling a resource application.</span></span> <span data-ttu-id="70d4b-110">Свойство **oauth2Permissions** [ServicePrincipal](serviceprincipal.md) сущности и сущности [приложения](application.md) — это коллекция **OAuth2Permission**.</span><span class="sxs-lookup"><span data-stu-id="70d4b-110">The **oauth2Permissions** property of the [ServicePrincipal](serviceprincipal.md) entity and of the [Application](application.md) entity is a collection of **OAuth2Permission**.</span></span>

## <a name="properties"></a><span data-ttu-id="70d4b-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="70d4b-111">Properties</span></span>

| <span data-ttu-id="70d4b-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="70d4b-112">Property</span></span> | <span data-ttu-id="70d4b-113">Тип</span><span class="sxs-lookup"><span data-stu-id="70d4b-113">Type</span></span> | <span data-ttu-id="70d4b-114">Описание</span><span class="sxs-lookup"><span data-stu-id="70d4b-114">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="70d4b-115">adminConsentDescription</span><span class="sxs-lookup"><span data-stu-id="70d4b-115">adminConsentDescription</span></span>|<span data-ttu-id="70d4b-116">Строка</span><span class="sxs-lookup"><span data-stu-id="70d4b-116">String</span></span>| <span data-ttu-id="70d4b-117">Текст справки разрешение, которое отображается в admin согласия и приложение назначения приемы и способы работы.</span><span class="sxs-lookup"><span data-stu-id="70d4b-117">Permission help text that appears in the admin consent and app assignment experiences.</span></span> |
|<span data-ttu-id="70d4b-118">adminConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="70d4b-118">adminConsentDisplayName</span></span>|<span data-ttu-id="70d4b-119">Строка</span><span class="sxs-lookup"><span data-stu-id="70d4b-119">String</span></span>| <span data-ttu-id="70d4b-120">Отображаемое имя для разрешения, которое отображается в admin согласия и приложение назначения приемы и способы работы.</span><span class="sxs-lookup"><span data-stu-id="70d4b-120">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span> |
|<span data-ttu-id="70d4b-121">id</span><span class="sxs-lookup"><span data-stu-id="70d4b-121">id</span></span>|<span data-ttu-id="70d4b-122">Guid</span><span class="sxs-lookup"><span data-stu-id="70d4b-122">Guid</span></span>| <span data-ttu-id="70d4b-123">Идентификатор уникальные области разрешений внутри семейства oauth2Permissions.</span><span class="sxs-lookup"><span data-stu-id="70d4b-123">Unique scope permission identifier inside the oauth2Permissions collection.</span></span> |
|<span data-ttu-id="70d4b-124">isEnabled</span><span class="sxs-lookup"><span data-stu-id="70d4b-124">isEnabled</span></span>|<span data-ttu-id="70d4b-125">Логический</span><span class="sxs-lookup"><span data-stu-id="70d4b-125">Boolean</span></span>| <span data-ttu-id="70d4b-126">При создании или обновлении разрешение, это свойство должно быть присвоено **значение true** (по умолчанию).</span><span class="sxs-lookup"><span data-stu-id="70d4b-126">When creating or updating a permission, this property must be set to **true** (which is the default).</span></span> <span data-ttu-id="70d4b-127">Чтобы удалить разрешение, это свойство необходимо сначала задать значение **false**.</span><span class="sxs-lookup"><span data-stu-id="70d4b-127">To delete a permission, this property must first be set to **false**.</span></span> <span data-ttu-id="70d4b-128">На этом этапе в последующих вызовов, могут быть удалены разрешения.</span><span class="sxs-lookup"><span data-stu-id="70d4b-128">At that point, in a subsequent call, the permission may be removed.</span></span> |
|<span data-ttu-id="70d4b-129">Происхождение</span><span class="sxs-lookup"><span data-stu-id="70d4b-129">origin</span></span>|<span data-ttu-id="70d4b-130">Строка</span><span class="sxs-lookup"><span data-stu-id="70d4b-130">String</span></span>| <span data-ttu-id="70d4b-131">Для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="70d4b-131">For internal use.</span></span> |
|<span data-ttu-id="70d4b-132">type</span><span class="sxs-lookup"><span data-stu-id="70d4b-132">type</span></span>|<span data-ttu-id="70d4b-133">Строка</span><span class="sxs-lookup"><span data-stu-id="70d4b-133">String</span></span>| <span data-ttu-id="70d4b-134">Указывает, является ли это разрешение области можно consented конечным пользователем или, будет ли это разрешение всей клиента, в котором должен быть consented для администратором компании.</span><span class="sxs-lookup"><span data-stu-id="70d4b-134">Specifies whether this scope permission can be consented to by an end user, or whether it is a tenant-wide permission that must be consented to by a company administrator.</span></span> <span data-ttu-id="70d4b-135">Возможные значения: *пользователь* или *администратор*.</span><span class="sxs-lookup"><span data-stu-id="70d4b-135">Possible values are *User* or *Admin*.</span></span> |
|<span data-ttu-id="70d4b-136">userConsentDescription</span><span class="sxs-lookup"><span data-stu-id="70d4b-136">userConsentDescription</span></span>|<span data-ttu-id="70d4b-137">Строка</span><span class="sxs-lookup"><span data-stu-id="70d4b-137">String</span></span>| <span data-ttu-id="70d4b-138">Текст справки разрешение, которое отображается в разрешения для конечных пользователей.</span><span class="sxs-lookup"><span data-stu-id="70d4b-138">Permission help text that appears in the end-user consent experience.</span></span> |
|<span data-ttu-id="70d4b-139">userConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="70d4b-139">userConsentDisplayName</span></span>|<span data-ttu-id="70d4b-140">Строка</span><span class="sxs-lookup"><span data-stu-id="70d4b-140">String</span></span>| <span data-ttu-id="70d4b-141">Отображаемое имя для разрешения, которое отображается в разрешения для конечных пользователей.</span><span class="sxs-lookup"><span data-stu-id="70d4b-141">Display name for the permission that appears in the end-user consent experience.</span></span> |
|<span data-ttu-id="70d4b-142">value</span><span class="sxs-lookup"><span data-stu-id="70d4b-142">value</span></span>|<span data-ttu-id="70d4b-143">Строка</span><span class="sxs-lookup"><span data-stu-id="70d4b-143">String</span></span>| <span data-ttu-id="70d4b-144">Значение утверждения область, должно привести к приложению ресурсов в маркер доступа OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="70d4b-144">The value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="70d4b-145">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="70d4b-145">JSON representation</span></span>
<span data-ttu-id="70d4b-146">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="70d4b-146">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "permissionScope resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
