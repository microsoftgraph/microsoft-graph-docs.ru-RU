---
title: Тип ресурса permissionScope
description: Представляет область делегированного разрешения OAuth 2,0. Указанные делегированные области разрешений OAuth 2,0 могут запрашиваться клиентскими приложениями (через коллекцию **рекуиредресаурцеакцесс** для объекта Application) при вызове приложения-ресурса. Свойство **oauth2Permissions** объекта ServicePrincipal и сущности приложения является коллекцией **OAuth2Permission**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 59770460b8fbc3c0a8946eeed94adfbe027f20cc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966169"
---
# <a name="permissionscope-resource-type"></a><span data-ttu-id="b5c5e-105">Тип ресурса permissionScope</span><span class="sxs-lookup"><span data-stu-id="b5c5e-105">permissionScope resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5c5e-106">Представляет область делегированного разрешения OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="b5c5e-106">Represents an OAuth 2.0 delegated permission scope.</span></span> <span data-ttu-id="b5c5e-107">Указанные делегированные области разрешений OAuth 2,0 могут запрашиваться клиентскими приложениями (через коллекцию **рекуиредресаурцеакцесс** для объекта [Application](application.md) ) при вызове приложения-ресурса.</span><span class="sxs-lookup"><span data-stu-id="b5c5e-107">The specified OAuth 2.0 delegated permission scopes may be requested by client applications (through the **requiredResourceAccess** collection on the [application](application.md) object) when calling a resource application.</span></span> <span data-ttu-id="b5c5e-108">Свойство **oauth2Permissions** объекта [ServicePrincipal](serviceprincipal.md) и сущности [приложения](application.md) является коллекцией **OAuth2Permission**.</span><span class="sxs-lookup"><span data-stu-id="b5c5e-108">The **oauth2Permissions** property of the [servicePrincipal](serviceprincipal.md) entity and of the [Application](application.md) entity is a collection of **OAuth2Permission**.</span></span>

## <a name="properties"></a><span data-ttu-id="b5c5e-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="b5c5e-109">Properties</span></span>

| <span data-ttu-id="b5c5e-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="b5c5e-110">Property</span></span> | <span data-ttu-id="b5c5e-111">Тип</span><span class="sxs-lookup"><span data-stu-id="b5c5e-111">Type</span></span> | <span data-ttu-id="b5c5e-112">Описание</span><span class="sxs-lookup"><span data-stu-id="b5c5e-112">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="b5c5e-113">Админконсентдескриптион</span><span class="sxs-lookup"><span data-stu-id="b5c5e-113">adminConsentDescription</span></span>|<span data-ttu-id="b5c5e-114">String</span><span class="sxs-lookup"><span data-stu-id="b5c5e-114">String</span></span>| <span data-ttu-id="b5c5e-115">Текст справки по разрешениям, который отображается в качестве согласия администратора и взаимодействия с назначением приложений.</span><span class="sxs-lookup"><span data-stu-id="b5c5e-115">Permission help text that appears in the admin consent and app assignment experiences.</span></span> |
|<span data-ttu-id="b5c5e-116">Админконсентдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="b5c5e-116">adminConsentDisplayName</span></span>|<span data-ttu-id="b5c5e-117">String</span><span class="sxs-lookup"><span data-stu-id="b5c5e-117">String</span></span>| <span data-ttu-id="b5c5e-118">Отображаемое имя разрешения, которое отображается в качестве согласия администратора и взаимодействия с назначением приложений.</span><span class="sxs-lookup"><span data-stu-id="b5c5e-118">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span> |
|<span data-ttu-id="b5c5e-119">id</span><span class="sxs-lookup"><span data-stu-id="b5c5e-119">id</span></span>|<span data-ttu-id="b5c5e-120">GUID</span><span class="sxs-lookup"><span data-stu-id="b5c5e-120">Guid</span></span>| <span data-ttu-id="b5c5e-121">Уникальный идентификатор разрешения области в коллекции oauth2Permissions.</span><span class="sxs-lookup"><span data-stu-id="b5c5e-121">Unique scope permission identifier inside the oauth2Permissions collection.</span></span> |
|<span data-ttu-id="b5c5e-122">isEnabled</span><span class="sxs-lookup"><span data-stu-id="b5c5e-122">isEnabled</span></span>|<span data-ttu-id="b5c5e-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5c5e-123">Boolean</span></span>| <span data-ttu-id="b5c5e-124">При создании или обновлении разрешения для этого свойства должно быть задано **значение true** (значение по умолчанию).</span><span class="sxs-lookup"><span data-stu-id="b5c5e-124">When creating or updating a permission, this property must be set to **true** (which is the default).</span></span> <span data-ttu-id="b5c5e-125">Чтобы удалить разрешение, необходимо сначала задать для этого свойства значение **false**.</span><span class="sxs-lookup"><span data-stu-id="b5c5e-125">To delete a permission, this property must first be set to **false**.</span></span> <span data-ttu-id="b5c5e-126">В этот момент разрешение может быть удалено из последующего вызова.</span><span class="sxs-lookup"><span data-stu-id="b5c5e-126">At that point, in a subsequent call, the permission may be removed.</span></span> |
|<span data-ttu-id="b5c5e-127">основания</span><span class="sxs-lookup"><span data-stu-id="b5c5e-127">origin</span></span>|<span data-ttu-id="b5c5e-128">String</span><span class="sxs-lookup"><span data-stu-id="b5c5e-128">String</span></span>| <span data-ttu-id="b5c5e-129">Для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="b5c5e-129">For internal use.</span></span> |
|<span data-ttu-id="b5c5e-130">type</span><span class="sxs-lookup"><span data-stu-id="b5c5e-130">type</span></span>|<span data-ttu-id="b5c5e-131">String</span><span class="sxs-lookup"><span data-stu-id="b5c5e-131">String</span></span>| <span data-ttu-id="b5c5e-132">Указывает, может ли пользователь иметь разрешение на доступ к области, а также о том, является ли оно разрешением, которое должно быть отослано администратором компании.</span><span class="sxs-lookup"><span data-stu-id="b5c5e-132">Specifies whether this scope permission can be consented to by an end user, or whether it is a tenant-wide permission that must be consented to by a company administrator.</span></span> <span data-ttu-id="b5c5e-133">Возможные значения: *User* или *Admin*.</span><span class="sxs-lookup"><span data-stu-id="b5c5e-133">Possible values are *User* or *Admin*.</span></span> |
|<span data-ttu-id="b5c5e-134">Усерконсентдескриптион</span><span class="sxs-lookup"><span data-stu-id="b5c5e-134">userConsentDescription</span></span>|<span data-ttu-id="b5c5e-135">String</span><span class="sxs-lookup"><span data-stu-id="b5c5e-135">String</span></span>| <span data-ttu-id="b5c5e-136">Текст справки по разрешениям, который отображается в диалоговом окне согласия конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="b5c5e-136">Permission help text that appears in the end-user consent experience.</span></span> |
|<span data-ttu-id="b5c5e-137">Усерконсентдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="b5c5e-137">userConsentDisplayName</span></span>|<span data-ttu-id="b5c5e-138">String</span><span class="sxs-lookup"><span data-stu-id="b5c5e-138">String</span></span>| <span data-ttu-id="b5c5e-139">Отображаемое имя разрешения, которое отображается в диалоговом окне согласия конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="b5c5e-139">Display name for the permission that appears in the end-user consent experience.</span></span> |
|<span data-ttu-id="b5c5e-140">value</span><span class="sxs-lookup"><span data-stu-id="b5c5e-140">value</span></span>|<span data-ttu-id="b5c5e-141">String</span><span class="sxs-lookup"><span data-stu-id="b5c5e-141">String</span></span>| <span data-ttu-id="b5c5e-142">Значение утверждения области, которое должно ожидать приложение ресурсов в маркере доступа OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="b5c5e-142">The value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b5c5e-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b5c5e-143">JSON representation</span></span>
<span data-ttu-id="b5c5e-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b5c5e-144">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
