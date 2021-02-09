---
title: Тип ресурса accessPackageResourceScope
description: В управлении правами Azure AD область ресурсов пакета доступа является ссылкой на область в ресурсе.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: cd6641b93517f2eadb15e19ef24b35f9f98626fc
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158551"
---
# <a name="accesspackageresourcescope-resource-type"></a><span data-ttu-id="e3016-103">Тип ресурса accessPackageResourceScope</span><span class="sxs-lookup"><span data-stu-id="e3016-103">accessPackageResourceScope resource type</span></span>

<span data-ttu-id="e3016-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3016-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3016-105">В [управлении правами Azure AD](entitlementmanagement-root.md)область ресурсов пакета доступа — это ссылка на область в ресурсе для ресурсов с несколькими уровнями.</span><span class="sxs-lookup"><span data-stu-id="e3016-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource scope is a reference to a scope within a resource, for those resources that have multiple scopes.</span></span>

<span data-ttu-id="e3016-106">Область ресурсов пакета доступа для ресурса, который уже был добавлен в пакет доступа, можно определить с помощью списка [accessPackageResourceRoleScopes](../api/accesspackage-list-accesspackageresourcerolescopes.md) для возврата коллекции объектов [accessPackageResourceRoleScope.](accesspackageresourcerolescope.md)</span><span class="sxs-lookup"><span data-stu-id="e3016-106">You can determine the access package resource scope, for a resource that has already been added to an access package, by using [list accessPackageResourceRoleScopes](../api/accesspackage-list-accesspackageresourcerolescopes.md) to return a collection of [accessPackageResourceRoleScope](accesspackageresourcerolescope.md) objects.</span></span>

## <a name="properties"></a><span data-ttu-id="e3016-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e3016-107">Properties</span></span>

| <span data-ttu-id="e3016-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e3016-108">Property</span></span>     | <span data-ttu-id="e3016-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e3016-109">Type</span></span>        | <span data-ttu-id="e3016-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e3016-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e3016-111">description</span><span class="sxs-lookup"><span data-stu-id="e3016-111">description</span></span>|<span data-ttu-id="e3016-112">String</span><span class="sxs-lookup"><span data-stu-id="e3016-112">String</span></span>|<span data-ttu-id="e3016-113">Описание области.</span><span class="sxs-lookup"><span data-stu-id="e3016-113">The description of the scope.</span></span>|
|<span data-ttu-id="e3016-114">displayName</span><span class="sxs-lookup"><span data-stu-id="e3016-114">displayName</span></span>|<span data-ttu-id="e3016-115">String</span><span class="sxs-lookup"><span data-stu-id="e3016-115">String</span></span>|<span data-ttu-id="e3016-116">Отображаемого имени области.</span><span class="sxs-lookup"><span data-stu-id="e3016-116">The display name of the scope.</span></span>|
|<span data-ttu-id="e3016-117">id</span><span class="sxs-lookup"><span data-stu-id="e3016-117">id</span></span>|<span data-ttu-id="e3016-118">String</span><span class="sxs-lookup"><span data-stu-id="e3016-118">String</span></span>| <span data-ttu-id="e3016-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e3016-119">Read-only.</span></span>|
|<span data-ttu-id="e3016-120">isRootScope</span><span class="sxs-lookup"><span data-stu-id="e3016-120">isRootScope</span></span>|<span data-ttu-id="e3016-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="e3016-121">Boolean</span></span>|<span data-ttu-id="e3016-122">Имеет true, если области расположены в иерархии и это верхняя или корневая область ресурса.</span><span class="sxs-lookup"><span data-stu-id="e3016-122">True if the scopes are arranged in a hierarchy and this is the top or root scope of the resource.</span></span>|
|<span data-ttu-id="e3016-123">originId</span><span class="sxs-lookup"><span data-stu-id="e3016-123">originId</span></span>|<span data-ttu-id="e3016-124">String</span><span class="sxs-lookup"><span data-stu-id="e3016-124">String</span></span>|<span data-ttu-id="e3016-125">Уникальный идентификатор области в ресурсе, определенный в системе источника.</span><span class="sxs-lookup"><span data-stu-id="e3016-125">The unique identifier for the scope in the resource as defined in the origin system.</span></span>|
|<span data-ttu-id="e3016-126">originSystem</span><span class="sxs-lookup"><span data-stu-id="e3016-126">originSystem</span></span>|<span data-ttu-id="e3016-127">String</span><span class="sxs-lookup"><span data-stu-id="e3016-127">String</span></span>|<span data-ttu-id="e3016-128">Система источника для области.</span><span class="sxs-lookup"><span data-stu-id="e3016-128">The origin system for the scope.</span></span>|
|<span data-ttu-id="e3016-129">roleOriginId</span><span class="sxs-lookup"><span data-stu-id="e3016-129">roleOriginId</span></span>|<span data-ttu-id="e3016-130">String</span><span class="sxs-lookup"><span data-stu-id="e3016-130">String</span></span>|<span data-ttu-id="e3016-131">Система источника для роли, если она отличается.</span><span class="sxs-lookup"><span data-stu-id="e3016-131">The origin system for the role, if different.</span></span>|
|<span data-ttu-id="e3016-132">url</span><span class="sxs-lookup"><span data-stu-id="e3016-132">url</span></span>|<span data-ttu-id="e3016-133">String</span><span class="sxs-lookup"><span data-stu-id="e3016-133">String</span></span>|<span data-ttu-id="e3016-134">Локатор ресурсов для области.</span><span class="sxs-lookup"><span data-stu-id="e3016-134">A resource locator for the scope.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e3016-135">Связи</span><span class="sxs-lookup"><span data-stu-id="e3016-135">Relationships</span></span>

| <span data-ttu-id="e3016-136">Связь</span><span class="sxs-lookup"><span data-stu-id="e3016-136">Relationship</span></span> | <span data-ttu-id="e3016-137">Тип</span><span class="sxs-lookup"><span data-stu-id="e3016-137">Type</span></span>        | <span data-ttu-id="e3016-138">Описание</span><span class="sxs-lookup"><span data-stu-id="e3016-138">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e3016-139">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="e3016-139">accessPackageResource</span></span>|[<span data-ttu-id="e3016-140">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="e3016-140">accessPackageResource</span></span>](accesspackageresource.md)| <span data-ttu-id="e3016-p101">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="e3016-p101">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e3016-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e3016-143">JSON representation</span></span>

<span data-ttu-id="e3016-144">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e3016-144">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageResourceScope",
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


