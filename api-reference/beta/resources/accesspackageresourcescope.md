---
title: Тип ресурса Акцесспаккажересаурцескопе
description: В управлении службой управления правами Azure AD областью ресурсов пакета Access является ссылка на область в пределах ресурса.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 242c90e9d0e506dbeb6576975305d0a0f8397f86
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508501"
---
# <a name="accesspackageresourcescope-resource-type"></a><span data-ttu-id="d9ef7-103">Тип ресурса Акцесспаккажересаурцескопе</span><span class="sxs-lookup"><span data-stu-id="d9ef7-103">accessPackageResourceScope resource type</span></span>

<span data-ttu-id="d9ef7-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d9ef7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9ef7-105">В [управлении службой управления правами Azure AD](entitlementmanagement-root.md)область ресурсов пакета Access — это ссылка на область в ресурсе для этих ресурсов с несколькими областями.</span><span class="sxs-lookup"><span data-stu-id="d9ef7-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource scope is a reference to a scope within a resource, for those resources that have multiple scopes.</span></span>

<span data-ttu-id="d9ef7-106">Можно определить область ресурсов пакета доступа для ресурса, который уже был добавлен в пакет Access, с помощью [List акцесспаккажересаурцеролескопес](../api/accesspackage-list-accesspackageresourcerolescopes.md) , чтобы вернуть коллекцию объектов [акцесспаккажересаурцеролескопе](accesspackageresourcerolescope.md) .</span><span class="sxs-lookup"><span data-stu-id="d9ef7-106">You can determine the access package resource scope, for a resource that has already been added to an access package, by using [list accessPackageResourceRoleScopes](../api/accesspackage-list-accesspackageresourcerolescopes.md) to return a collection of [accessPackageResourceRoleScope](accesspackageresourcerolescope.md) objects.</span></span>

## <a name="properties"></a><span data-ttu-id="d9ef7-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d9ef7-107">Properties</span></span>

| <span data-ttu-id="d9ef7-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d9ef7-108">Property</span></span>     | <span data-ttu-id="d9ef7-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d9ef7-109">Type</span></span>        | <span data-ttu-id="d9ef7-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d9ef7-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d9ef7-111">description</span><span class="sxs-lookup"><span data-stu-id="d9ef7-111">description</span></span>|<span data-ttu-id="d9ef7-112">String</span><span class="sxs-lookup"><span data-stu-id="d9ef7-112">String</span></span>|<span data-ttu-id="d9ef7-113">Описание области.</span><span class="sxs-lookup"><span data-stu-id="d9ef7-113">The description of the scope.</span></span>|
|<span data-ttu-id="d9ef7-114">displayName</span><span class="sxs-lookup"><span data-stu-id="d9ef7-114">displayName</span></span>|<span data-ttu-id="d9ef7-115">Строка</span><span class="sxs-lookup"><span data-stu-id="d9ef7-115">String</span></span>|<span data-ttu-id="d9ef7-116">Отображаемое имя области.</span><span class="sxs-lookup"><span data-stu-id="d9ef7-116">The display name of the scope.</span></span>|
|<span data-ttu-id="d9ef7-117">id</span><span class="sxs-lookup"><span data-stu-id="d9ef7-117">id</span></span>|<span data-ttu-id="d9ef7-118">String</span><span class="sxs-lookup"><span data-stu-id="d9ef7-118">String</span></span>| <span data-ttu-id="d9ef7-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d9ef7-119">Read-only.</span></span>|
|<span data-ttu-id="d9ef7-120">исрутскопе</span><span class="sxs-lookup"><span data-stu-id="d9ef7-120">isRootScope</span></span>|<span data-ttu-id="d9ef7-121">Логический</span><span class="sxs-lookup"><span data-stu-id="d9ef7-121">Boolean</span></span>|<span data-ttu-id="d9ef7-122">Значение true, если области упорядочены в иерархию, а это верхняя или корневая область ресурса.</span><span class="sxs-lookup"><span data-stu-id="d9ef7-122">True if the scopes are arranged in a hierarchy and this is the top or root scope of the resource.</span></span>|
|<span data-ttu-id="d9ef7-123">оригинид</span><span class="sxs-lookup"><span data-stu-id="d9ef7-123">originId</span></span>|<span data-ttu-id="d9ef7-124">String</span><span class="sxs-lookup"><span data-stu-id="d9ef7-124">String</span></span>|<span data-ttu-id="d9ef7-125">Уникальный идентификатор области ресурса в соответствии с определением в исходной системе.</span><span class="sxs-lookup"><span data-stu-id="d9ef7-125">The unique identifier for the scope in the resource as defined in the origin system.</span></span>|
|<span data-ttu-id="d9ef7-126">оригинсистем</span><span class="sxs-lookup"><span data-stu-id="d9ef7-126">originSystem</span></span>|<span data-ttu-id="d9ef7-127">String</span><span class="sxs-lookup"><span data-stu-id="d9ef7-127">String</span></span>|<span data-ttu-id="d9ef7-128">Исходная система для области.</span><span class="sxs-lookup"><span data-stu-id="d9ef7-128">The origin system for the scope.</span></span>|
|<span data-ttu-id="d9ef7-129">ролеоригинид</span><span class="sxs-lookup"><span data-stu-id="d9ef7-129">roleOriginId</span></span>|<span data-ttu-id="d9ef7-130">String</span><span class="sxs-lookup"><span data-stu-id="d9ef7-130">String</span></span>|<span data-ttu-id="d9ef7-131">Исходная система для роли, если она отличается.</span><span class="sxs-lookup"><span data-stu-id="d9ef7-131">The origin system for the role, if different.</span></span>|
|<span data-ttu-id="d9ef7-132">url</span><span class="sxs-lookup"><span data-stu-id="d9ef7-132">url</span></span>|<span data-ttu-id="d9ef7-133">String</span><span class="sxs-lookup"><span data-stu-id="d9ef7-133">String</span></span>|<span data-ttu-id="d9ef7-134">Указатель ресурсов для области.</span><span class="sxs-lookup"><span data-stu-id="d9ef7-134">A resource locator for the scope.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d9ef7-135">Связи</span><span class="sxs-lookup"><span data-stu-id="d9ef7-135">Relationships</span></span>

| <span data-ttu-id="d9ef7-136">Связь</span><span class="sxs-lookup"><span data-stu-id="d9ef7-136">Relationship</span></span> | <span data-ttu-id="d9ef7-137">Тип</span><span class="sxs-lookup"><span data-stu-id="d9ef7-137">Type</span></span>        | <span data-ttu-id="d9ef7-138">Описание</span><span class="sxs-lookup"><span data-stu-id="d9ef7-138">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d9ef7-139">акцесспаккажересаурце</span><span class="sxs-lookup"><span data-stu-id="d9ef7-139">accessPackageResource</span></span>|[<span data-ttu-id="d9ef7-140">акцесспаккажересаурце</span><span class="sxs-lookup"><span data-stu-id="d9ef7-140">accessPackageResource</span></span>](accesspackageresource.md)| <span data-ttu-id="d9ef7-p101">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="d9ef7-p101">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d9ef7-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d9ef7-143">JSON representation</span></span>

<span data-ttu-id="d9ef7-144">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d9ef7-144">The following is a JSON representation of the resource.</span></span>

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
