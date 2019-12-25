---
title: Тип ресурса Акцесспаккажересаурцескопе
description: В управлении службой управления правами Azure AD областью ресурсов пакета Access является ссылка на область в пределах ресурса.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1418e2cb21a1023e864d842b760006e05f3afb03
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870969"
---
# <a name="accesspackageresourcescope-resource-type"></a><span data-ttu-id="bb6bc-103">Тип ресурса Акцесспаккажересаурцескопе</span><span class="sxs-lookup"><span data-stu-id="bb6bc-103">accessPackageResourceScope resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb6bc-104">В [управлении службой управления правами Azure AD](entitlementmanagement-root.md)область ресурсов пакета Access — это ссылка на область в ресурсе для этих ресурсов с несколькими областями.</span><span class="sxs-lookup"><span data-stu-id="bb6bc-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource scope is a reference to a scope within a resource, for those resources that have multiple scopes.</span></span>

<span data-ttu-id="bb6bc-105">Можно определить область ресурсов пакета доступа для ресурса, который уже был добавлен в пакет Access, с помощью [List акцесспаккажересаурцеролескопес](../api/accesspackage-list-accesspackageresourcerolescopes.md) , чтобы вернуть коллекцию объектов [акцесспаккажересаурцеролескопе](accesspackageresourcerolescope.md) .</span><span class="sxs-lookup"><span data-stu-id="bb6bc-105">You can determine the access package resource scope, for a resource that has already been added to an access package, by using [list accessPackageResourceRoleScopes](../api/accesspackage-list-accesspackageresourcerolescopes.md) to return a collection of [accessPackageResourceRoleScope](accesspackageresourcerolescope.md) objects.</span></span>

## <a name="properties"></a><span data-ttu-id="bb6bc-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="bb6bc-106">Properties</span></span>

| <span data-ttu-id="bb6bc-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="bb6bc-107">Property</span></span>     | <span data-ttu-id="bb6bc-108">Тип</span><span class="sxs-lookup"><span data-stu-id="bb6bc-108">Type</span></span>        | <span data-ttu-id="bb6bc-109">Описание</span><span class="sxs-lookup"><span data-stu-id="bb6bc-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bb6bc-110">description</span><span class="sxs-lookup"><span data-stu-id="bb6bc-110">description</span></span>|<span data-ttu-id="bb6bc-111">String</span><span class="sxs-lookup"><span data-stu-id="bb6bc-111">String</span></span>|<span data-ttu-id="bb6bc-112">Описание области.</span><span class="sxs-lookup"><span data-stu-id="bb6bc-112">The description of the scope.</span></span>|
|<span data-ttu-id="bb6bc-113">displayName</span><span class="sxs-lookup"><span data-stu-id="bb6bc-113">displayName</span></span>|<span data-ttu-id="bb6bc-114">Строка</span><span class="sxs-lookup"><span data-stu-id="bb6bc-114">String</span></span>|<span data-ttu-id="bb6bc-115">Отображаемое имя области.</span><span class="sxs-lookup"><span data-stu-id="bb6bc-115">The display name of the scope.</span></span>|
|<span data-ttu-id="bb6bc-116">id</span><span class="sxs-lookup"><span data-stu-id="bb6bc-116">id</span></span>|<span data-ttu-id="bb6bc-117">String</span><span class="sxs-lookup"><span data-stu-id="bb6bc-117">String</span></span>| <span data-ttu-id="bb6bc-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bb6bc-118">Read-only.</span></span>|
|<span data-ttu-id="bb6bc-119">исрутскопе</span><span class="sxs-lookup"><span data-stu-id="bb6bc-119">isRootScope</span></span>|<span data-ttu-id="bb6bc-120">Логический</span><span class="sxs-lookup"><span data-stu-id="bb6bc-120">Boolean</span></span>|<span data-ttu-id="bb6bc-121">Значение true, если области упорядочены в иерархию, а это верхняя или корневая область ресурса.</span><span class="sxs-lookup"><span data-stu-id="bb6bc-121">True if the scopes are arranged in a hierarchy and this is the top or root scope of the resource.</span></span>|
|<span data-ttu-id="bb6bc-122">оригинид</span><span class="sxs-lookup"><span data-stu-id="bb6bc-122">originId</span></span>|<span data-ttu-id="bb6bc-123">String</span><span class="sxs-lookup"><span data-stu-id="bb6bc-123">String</span></span>|<span data-ttu-id="bb6bc-124">Уникальный идентификатор области ресурса в соответствии с определением в исходной системе.</span><span class="sxs-lookup"><span data-stu-id="bb6bc-124">The unique identifier for the scope in the resource as defined in the origin system.</span></span>|
|<span data-ttu-id="bb6bc-125">оригинсистем</span><span class="sxs-lookup"><span data-stu-id="bb6bc-125">originSystem</span></span>|<span data-ttu-id="bb6bc-126">String</span><span class="sxs-lookup"><span data-stu-id="bb6bc-126">String</span></span>|<span data-ttu-id="bb6bc-127">Исходная система для области.</span><span class="sxs-lookup"><span data-stu-id="bb6bc-127">The origin system for the scope.</span></span>|
|<span data-ttu-id="bb6bc-128">ролеоригинид</span><span class="sxs-lookup"><span data-stu-id="bb6bc-128">roleOriginId</span></span>|<span data-ttu-id="bb6bc-129">String</span><span class="sxs-lookup"><span data-stu-id="bb6bc-129">String</span></span>|<span data-ttu-id="bb6bc-130">Исходная система для роли, если она отличается.</span><span class="sxs-lookup"><span data-stu-id="bb6bc-130">The origin system for the role, if different.</span></span>|
|<span data-ttu-id="bb6bc-131">url</span><span class="sxs-lookup"><span data-stu-id="bb6bc-131">url</span></span>|<span data-ttu-id="bb6bc-132">String</span><span class="sxs-lookup"><span data-stu-id="bb6bc-132">String</span></span>|<span data-ttu-id="bb6bc-133">Указатель ресурсов для области.</span><span class="sxs-lookup"><span data-stu-id="bb6bc-133">A resource locator for the scope.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb6bc-134">Отношения</span><span class="sxs-lookup"><span data-stu-id="bb6bc-134">Relationships</span></span>

| <span data-ttu-id="bb6bc-135">Связь</span><span class="sxs-lookup"><span data-stu-id="bb6bc-135">Relationship</span></span> | <span data-ttu-id="bb6bc-136">Тип</span><span class="sxs-lookup"><span data-stu-id="bb6bc-136">Type</span></span>        | <span data-ttu-id="bb6bc-137">Описание</span><span class="sxs-lookup"><span data-stu-id="bb6bc-137">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bb6bc-138">акцесспаккажересаурце</span><span class="sxs-lookup"><span data-stu-id="bb6bc-138">accessPackageResource</span></span>|[<span data-ttu-id="bb6bc-139">акцесспаккажересаурце</span><span class="sxs-lookup"><span data-stu-id="bb6bc-139">accessPackageResource</span></span>](accesspackageresource.md)| <span data-ttu-id="bb6bc-p101">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="bb6bc-p101">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bb6bc-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bb6bc-142">JSON representation</span></span>

<span data-ttu-id="bb6bc-143">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bb6bc-143">The following is a JSON representation of the resource.</span></span>

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
