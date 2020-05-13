---
title: Тип ресурса permissionScope
description: Представляет область делегированного разрешения OAuth 2,0.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 725fe0c65fd05752cd6f862291efcffbcf3d22c5
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2020
ms.locfileid: "43469068"
---
# <a name="permissionscope-resource-type"></a><span data-ttu-id="3e948-103">Тип ресурса permissionScope</span><span class="sxs-lookup"><span data-stu-id="3e948-103">permissionScope resource type</span></span>

<span data-ttu-id="3e948-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e948-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e948-105">Представляет область делегированного разрешения OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="3e948-105">Represents an OAuth 2.0 delegated permission scope.</span></span> <span data-ttu-id="3e948-106">Указанные делегированные области разрешений OAuth 2,0 могут запрашиваться клиентскими приложениями (через коллекцию **рекуиредресаурцеакцесс** для объекта [Application](application.md) ) при вызове приложения-ресурса.</span><span class="sxs-lookup"><span data-stu-id="3e948-106">The specified OAuth 2.0 delegated permission scopes may be requested by client applications (through the **requiredResourceAccess** collection on the [application](application.md) object) when calling a resource application.</span></span> <span data-ttu-id="3e948-107">Свойство **oauth2Permissions** объекта [ServicePrincipal](serviceprincipal.md) и сущности [приложения](application.md) является коллекцией **permissionScope**.</span><span class="sxs-lookup"><span data-stu-id="3e948-107">The **oauth2Permissions** property of the [servicePrincipal](serviceprincipal.md) entity and of the [Application](application.md) entity is a collection of **permissionScope**.</span></span>

## <a name="properties"></a><span data-ttu-id="3e948-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3e948-108">Properties</span></span>

| <span data-ttu-id="3e948-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="3e948-109">Property</span></span> | <span data-ttu-id="3e948-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3e948-110">Type</span></span> | <span data-ttu-id="3e948-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3e948-111">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="3e948-112">админконсентдескриптион</span><span class="sxs-lookup"><span data-stu-id="3e948-112">adminConsentDescription</span></span>|<span data-ttu-id="3e948-113">String</span><span class="sxs-lookup"><span data-stu-id="3e948-113">String</span></span>| <span data-ttu-id="3e948-114">Текст справки по разрешениям, который отображается в качестве согласия администратора и взаимодействия с назначением приложений.</span><span class="sxs-lookup"><span data-stu-id="3e948-114">Permission help text that appears in the admin consent and app assignment experiences.</span></span> |
|<span data-ttu-id="3e948-115">админконсентдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="3e948-115">adminConsentDisplayName</span></span>|<span data-ttu-id="3e948-116">String</span><span class="sxs-lookup"><span data-stu-id="3e948-116">String</span></span>| <span data-ttu-id="3e948-117">Отображаемое имя разрешения, которое отображается в качестве согласия администратора и взаимодействия с назначением приложений.</span><span class="sxs-lookup"><span data-stu-id="3e948-117">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span> |
|<span data-ttu-id="3e948-118">id</span><span class="sxs-lookup"><span data-stu-id="3e948-118">id</span></span>|<span data-ttu-id="3e948-119">GUID</span><span class="sxs-lookup"><span data-stu-id="3e948-119">Guid</span></span>| <span data-ttu-id="3e948-120">Уникальный идентификатор разрешения области в коллекции oauth2Permissions.</span><span class="sxs-lookup"><span data-stu-id="3e948-120">Unique scope permission identifier inside the oauth2Permissions collection.</span></span> |
|<span data-ttu-id="3e948-121">isEnabled</span><span class="sxs-lookup"><span data-stu-id="3e948-121">isEnabled</span></span>|<span data-ttu-id="3e948-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="3e948-122">Boolean</span></span>| <span data-ttu-id="3e948-123">При создании или обновлении разрешения для этого свойства должно быть задано **значение true** (значение по умолчанию).</span><span class="sxs-lookup"><span data-stu-id="3e948-123">When creating or updating a permission, this property must be set to **true** (which is the default).</span></span> <span data-ttu-id="3e948-124">Чтобы удалить разрешение, необходимо сначала задать для этого свойства значение **false**.</span><span class="sxs-lookup"><span data-stu-id="3e948-124">To delete a permission, this property must first be set to **false**.</span></span> <span data-ttu-id="3e948-125">В этот момент разрешение может быть удалено из последующего вызова.</span><span class="sxs-lookup"><span data-stu-id="3e948-125">At that point, in a subsequent call, the permission may be removed.</span></span> |
|<span data-ttu-id="3e948-126">основания</span><span class="sxs-lookup"><span data-stu-id="3e948-126">origin</span></span>|<span data-ttu-id="3e948-127">String</span><span class="sxs-lookup"><span data-stu-id="3e948-127">String</span></span>| <span data-ttu-id="3e948-128">Для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="3e948-128">For internal use.</span></span> |
|<span data-ttu-id="3e948-129">type</span><span class="sxs-lookup"><span data-stu-id="3e948-129">type</span></span>|<span data-ttu-id="3e948-130">String</span><span class="sxs-lookup"><span data-stu-id="3e948-130">String</span></span>| <span data-ttu-id="3e948-131">Указывает, может ли пользователь иметь разрешение на доступ к области, а также о том, является ли оно разрешением, которое должно быть отослано администратором компании.</span><span class="sxs-lookup"><span data-stu-id="3e948-131">Specifies whether this scope permission can be consented to by an end user, or whether it is a tenant-wide permission that must be consented to by a company administrator.</span></span> <span data-ttu-id="3e948-132">Возможные значения: *User* или *Admin*.</span><span class="sxs-lookup"><span data-stu-id="3e948-132">Possible values are *User* or *Admin*.</span></span> |
|<span data-ttu-id="3e948-133">усерконсентдескриптион</span><span class="sxs-lookup"><span data-stu-id="3e948-133">userConsentDescription</span></span>|<span data-ttu-id="3e948-134">String</span><span class="sxs-lookup"><span data-stu-id="3e948-134">String</span></span>| <span data-ttu-id="3e948-135">Текст справки по разрешениям, который отображается в диалоговом окне согласия конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="3e948-135">Permission help text that appears in the end-user consent experience.</span></span> |
|<span data-ttu-id="3e948-136">усерконсентдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="3e948-136">userConsentDisplayName</span></span>|<span data-ttu-id="3e948-137">String</span><span class="sxs-lookup"><span data-stu-id="3e948-137">String</span></span>| <span data-ttu-id="3e948-138">Отображаемое имя разрешения, которое отображается в диалоговом окне согласия конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="3e948-138">Display name for the permission that appears in the end-user consent experience.</span></span> |
|<span data-ttu-id="3e948-139">value</span><span class="sxs-lookup"><span data-stu-id="3e948-139">value</span></span>|<span data-ttu-id="3e948-140">String</span><span class="sxs-lookup"><span data-stu-id="3e948-140">String</span></span>| <span data-ttu-id="3e948-141">Значение утверждения области, которое должно ожидать приложение ресурсов в маркере доступа OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="3e948-141">The value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3e948-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3e948-142">JSON representation</span></span>
<span data-ttu-id="3e948-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3e948-143">Here is a JSON representation of the resource.</span></span>

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
