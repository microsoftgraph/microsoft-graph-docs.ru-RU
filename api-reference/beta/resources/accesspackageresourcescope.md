---
title: Тип ресурса Акцесспаккажересаурцескопе
description: В управлении службой управления правами Azure AD областью ресурсов пакета Access является ссылка на область в пределах ресурса.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 355838fa9f93cef7d44972b98af317a74036e421
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48067526"
---
# <a name="accesspackageresourcescope-resource-type"></a><span data-ttu-id="0117a-103">Тип ресурса Акцесспаккажересаурцескопе</span><span class="sxs-lookup"><span data-stu-id="0117a-103">accessPackageResourceScope resource type</span></span>

<span data-ttu-id="0117a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0117a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0117a-105">В [управлении службой управления правами Azure AD](entitlementmanagement-root.md)область ресурсов пакета Access — это ссылка на область в ресурсе для этих ресурсов с несколькими областями.</span><span class="sxs-lookup"><span data-stu-id="0117a-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource scope is a reference to a scope within a resource, for those resources that have multiple scopes.</span></span>

<span data-ttu-id="0117a-106">Можно определить область ресурсов пакета доступа для ресурса, который уже был добавлен в пакет Access, с помощью [List акцесспаккажересаурцеролескопес](../api/accesspackage-list-accesspackageresourcerolescopes.md) , чтобы вернуть коллекцию объектов [акцесспаккажересаурцеролескопе](accesspackageresourcerolescope.md) .</span><span class="sxs-lookup"><span data-stu-id="0117a-106">You can determine the access package resource scope, for a resource that has already been added to an access package, by using [list accessPackageResourceRoleScopes](../api/accesspackage-list-accesspackageresourcerolescopes.md) to return a collection of [accessPackageResourceRoleScope](accesspackageresourcerolescope.md) objects.</span></span>

## <a name="properties"></a><span data-ttu-id="0117a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="0117a-107">Properties</span></span>

| <span data-ttu-id="0117a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="0117a-108">Property</span></span>     | <span data-ttu-id="0117a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="0117a-109">Type</span></span>        | <span data-ttu-id="0117a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0117a-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0117a-111">description</span><span class="sxs-lookup"><span data-stu-id="0117a-111">description</span></span>|<span data-ttu-id="0117a-112">String</span><span class="sxs-lookup"><span data-stu-id="0117a-112">String</span></span>|<span data-ttu-id="0117a-113">Описание области.</span><span class="sxs-lookup"><span data-stu-id="0117a-113">The description of the scope.</span></span>|
|<span data-ttu-id="0117a-114">displayName</span><span class="sxs-lookup"><span data-stu-id="0117a-114">displayName</span></span>|<span data-ttu-id="0117a-115">String</span><span class="sxs-lookup"><span data-stu-id="0117a-115">String</span></span>|<span data-ttu-id="0117a-116">Отображаемое имя области.</span><span class="sxs-lookup"><span data-stu-id="0117a-116">The display name of the scope.</span></span>|
|<span data-ttu-id="0117a-117">id</span><span class="sxs-lookup"><span data-stu-id="0117a-117">id</span></span>|<span data-ttu-id="0117a-118">String</span><span class="sxs-lookup"><span data-stu-id="0117a-118">String</span></span>| <span data-ttu-id="0117a-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0117a-119">Read-only.</span></span>|
|<span data-ttu-id="0117a-120">исрутскопе</span><span class="sxs-lookup"><span data-stu-id="0117a-120">isRootScope</span></span>|<span data-ttu-id="0117a-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="0117a-121">Boolean</span></span>|<span data-ttu-id="0117a-122">Значение true, если области упорядочены в иерархию, а это верхняя или корневая область ресурса.</span><span class="sxs-lookup"><span data-stu-id="0117a-122">True if the scopes are arranged in a hierarchy and this is the top or root scope of the resource.</span></span>|
|<span data-ttu-id="0117a-123">оригинид</span><span class="sxs-lookup"><span data-stu-id="0117a-123">originId</span></span>|<span data-ttu-id="0117a-124">String</span><span class="sxs-lookup"><span data-stu-id="0117a-124">String</span></span>|<span data-ttu-id="0117a-125">Уникальный идентификатор области ресурса в соответствии с определением в исходной системе.</span><span class="sxs-lookup"><span data-stu-id="0117a-125">The unique identifier for the scope in the resource as defined in the origin system.</span></span>|
|<span data-ttu-id="0117a-126">оригинсистем</span><span class="sxs-lookup"><span data-stu-id="0117a-126">originSystem</span></span>|<span data-ttu-id="0117a-127">String</span><span class="sxs-lookup"><span data-stu-id="0117a-127">String</span></span>|<span data-ttu-id="0117a-128">Исходная система для области.</span><span class="sxs-lookup"><span data-stu-id="0117a-128">The origin system for the scope.</span></span>|
|<span data-ttu-id="0117a-129">ролеоригинид</span><span class="sxs-lookup"><span data-stu-id="0117a-129">roleOriginId</span></span>|<span data-ttu-id="0117a-130">String</span><span class="sxs-lookup"><span data-stu-id="0117a-130">String</span></span>|<span data-ttu-id="0117a-131">Исходная система для роли, если она отличается.</span><span class="sxs-lookup"><span data-stu-id="0117a-131">The origin system for the role, if different.</span></span>|
|<span data-ttu-id="0117a-132">url</span><span class="sxs-lookup"><span data-stu-id="0117a-132">url</span></span>|<span data-ttu-id="0117a-133">String</span><span class="sxs-lookup"><span data-stu-id="0117a-133">String</span></span>|<span data-ttu-id="0117a-134">Указатель ресурсов для области.</span><span class="sxs-lookup"><span data-stu-id="0117a-134">A resource locator for the scope.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0117a-135">Отношения</span><span class="sxs-lookup"><span data-stu-id="0117a-135">Relationships</span></span>

| <span data-ttu-id="0117a-136">Связь</span><span class="sxs-lookup"><span data-stu-id="0117a-136">Relationship</span></span> | <span data-ttu-id="0117a-137">Тип</span><span class="sxs-lookup"><span data-stu-id="0117a-137">Type</span></span>        | <span data-ttu-id="0117a-138">Описание</span><span class="sxs-lookup"><span data-stu-id="0117a-138">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0117a-139">акцесспаккажересаурце</span><span class="sxs-lookup"><span data-stu-id="0117a-139">accessPackageResource</span></span>|[<span data-ttu-id="0117a-140">акцесспаккажересаурце</span><span class="sxs-lookup"><span data-stu-id="0117a-140">accessPackageResource</span></span>](accesspackageresource.md)| <span data-ttu-id="0117a-p101">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="0117a-p101">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0117a-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0117a-143">JSON representation</span></span>

<span data-ttu-id="0117a-144">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0117a-144">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageResourceScope",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isRootScope": true,
  "originId": "String",
  "originSystem": "String",
  "roleOriginId": "String",
  "url": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageResourceScope resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


