---
title: тип ресурса accessPackageResourceScope
description: В управлении правами Azure AD область ресурсов пакета доступа является ссылкой на область в ресурсе.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 6da0211cad6dcca225f4c9848216eda2deaf7b0a
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467178"
---
# <a name="accesspackageresourcescope-resource-type"></a><span data-ttu-id="96241-103">тип ресурса accessPackageResourceScope</span><span class="sxs-lookup"><span data-stu-id="96241-103">accessPackageResourceScope resource type</span></span>

<span data-ttu-id="96241-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96241-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96241-105">В управлении правами [Azure AD](entitlementmanagement-root.md)область ресурсов пакета доступа является ссылкой на область в ресурсе для тех ресурсов, которые имеют несколько областей.</span><span class="sxs-lookup"><span data-stu-id="96241-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource scope is a reference to a scope within a resource, for those resources that have multiple scopes.</span></span>

<span data-ttu-id="96241-106">Область ресурсов пакета доступа для ресурса, который уже добавлен в пакет доступа, можно определить с помощью списка [accessPackageResourceRoleScopes](../api/accesspackage-list-accesspackageresourcerolescopes.md) для возврата коллекции объектов [accessPackageResourceRoleScope.](accesspackageresourcerolescope.md)</span><span class="sxs-lookup"><span data-stu-id="96241-106">You can determine the access package resource scope, for a resource which has roles already added to an access package, by using [list accessPackageResourceRoleScopes](../api/accesspackage-list-accesspackageresourcerolescopes.md) to return a collection of [accessPackageResourceRoleScope](accesspackageresourcerolescope.md) objects.</span></span>

<span data-ttu-id="96241-107">Если ресурс находится в каталоге пакетов доступа, но его роли еще не добавлены в пакет доступа, можно определить область ресурсов пакета доступа с помощью списка [accessPackageResources](../api/accesspackagecatalog-list-accesspackageresources.md) и в том числе в `$expand=accessPackageResourceScopes,accessPackageResourceEnvironment` запросе.</span><span class="sxs-lookup"><span data-stu-id="96241-107">If the resource is in an access package catalog but has not yet had its roles added to an access package, you can determine the access package resource scope by using [list accessPackageResources](../api/accesspackagecatalog-list-accesspackageresources.md) and including `$expand=accessPackageResourceScopes,accessPackageResourceEnvironment` in the query.</span></span>

## <a name="properties"></a><span data-ttu-id="96241-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="96241-108">Properties</span></span>

| <span data-ttu-id="96241-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="96241-109">Property</span></span>     | <span data-ttu-id="96241-110">Тип</span><span class="sxs-lookup"><span data-stu-id="96241-110">Type</span></span>        | <span data-ttu-id="96241-111">Описание</span><span class="sxs-lookup"><span data-stu-id="96241-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="96241-112">description</span><span class="sxs-lookup"><span data-stu-id="96241-112">description</span></span>|<span data-ttu-id="96241-113">String</span><span class="sxs-lookup"><span data-stu-id="96241-113">String</span></span>|<span data-ttu-id="96241-114">Описание области.</span><span class="sxs-lookup"><span data-stu-id="96241-114">The description of the scope.</span></span>|
|<span data-ttu-id="96241-115">displayName</span><span class="sxs-lookup"><span data-stu-id="96241-115">displayName</span></span>|<span data-ttu-id="96241-116">String</span><span class="sxs-lookup"><span data-stu-id="96241-116">String</span></span>|<span data-ttu-id="96241-117">Имя отображения области.</span><span class="sxs-lookup"><span data-stu-id="96241-117">The display name of the scope.</span></span>|
|<span data-ttu-id="96241-118">id</span><span class="sxs-lookup"><span data-stu-id="96241-118">id</span></span>|<span data-ttu-id="96241-119">String</span><span class="sxs-lookup"><span data-stu-id="96241-119">String</span></span>| <span data-ttu-id="96241-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="96241-120">Read-only.</span></span>|
|<span data-ttu-id="96241-121">isRootScope</span><span class="sxs-lookup"><span data-stu-id="96241-121">isRootScope</span></span>|<span data-ttu-id="96241-122">Логический</span><span class="sxs-lookup"><span data-stu-id="96241-122">Boolean</span></span>|<span data-ttu-id="96241-123">Верно, если области расположены в иерархии и это верхняя или корневая область ресурса.</span><span class="sxs-lookup"><span data-stu-id="96241-123">True if the scopes are arranged in a hierarchy and this is the top or root scope of the resource.</span></span>|
|<span data-ttu-id="96241-124">OriginId</span><span class="sxs-lookup"><span data-stu-id="96241-124">originId</span></span>|<span data-ttu-id="96241-125">String</span><span class="sxs-lookup"><span data-stu-id="96241-125">String</span></span>|<span data-ttu-id="96241-126">Уникальный идентификатор области в ресурсе, как определено в системе происхождения.</span><span class="sxs-lookup"><span data-stu-id="96241-126">The unique identifier for the scope in the resource as defined in the origin system.</span></span>|
|<span data-ttu-id="96241-127">originSystem</span><span class="sxs-lookup"><span data-stu-id="96241-127">originSystem</span></span>|<span data-ttu-id="96241-128">String</span><span class="sxs-lookup"><span data-stu-id="96241-128">String</span></span>|<span data-ttu-id="96241-129">Система происхождения для области.</span><span class="sxs-lookup"><span data-stu-id="96241-129">The origin system for the scope.</span></span>|
|<span data-ttu-id="96241-130">roleOriginId</span><span class="sxs-lookup"><span data-stu-id="96241-130">roleOriginId</span></span>|<span data-ttu-id="96241-131">String</span><span class="sxs-lookup"><span data-stu-id="96241-131">String</span></span>|<span data-ttu-id="96241-132">Система происхождения для роли, если отличается.</span><span class="sxs-lookup"><span data-stu-id="96241-132">The origin system for the role, if different.</span></span>|
|<span data-ttu-id="96241-133">url</span><span class="sxs-lookup"><span data-stu-id="96241-133">url</span></span>|<span data-ttu-id="96241-134">String</span><span class="sxs-lookup"><span data-stu-id="96241-134">String</span></span>|<span data-ttu-id="96241-135">Локатор ресурсов для области.</span><span class="sxs-lookup"><span data-stu-id="96241-135">A resource locator for the scope.</span></span>|

## <a name="relationships"></a><span data-ttu-id="96241-136">Связи</span><span class="sxs-lookup"><span data-stu-id="96241-136">Relationships</span></span>

| <span data-ttu-id="96241-137">Связь</span><span class="sxs-lookup"><span data-stu-id="96241-137">Relationship</span></span> | <span data-ttu-id="96241-138">Тип</span><span class="sxs-lookup"><span data-stu-id="96241-138">Type</span></span>        | <span data-ttu-id="96241-139">Описание</span><span class="sxs-lookup"><span data-stu-id="96241-139">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="96241-140">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="96241-140">accessPackageResource</span></span>|[<span data-ttu-id="96241-141">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="96241-141">accessPackageResource</span></span>](accesspackageresource.md)| <span data-ttu-id="96241-p101">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="96241-p101">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="96241-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="96241-144">JSON representation</span></span>

<span data-ttu-id="96241-145">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="96241-145">The following is a JSON representation of the resource.</span></span>

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


