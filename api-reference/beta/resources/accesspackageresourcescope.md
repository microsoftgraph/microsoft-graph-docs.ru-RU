---
title: Тип ресурса Акцесспаккажересаурцескопе
description: В управлении службой управления правами Azure AD областью ресурсов пакета Access является ссылка на область в пределах ресурса.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7bfa2f617e746aee17a62a7550c41e3de54f47cd
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939518"
---
# <a name="accesspackageresourcescope-resource-type"></a><span data-ttu-id="d20da-103">Тип ресурса Акцесспаккажересаурцескопе</span><span class="sxs-lookup"><span data-stu-id="d20da-103">accessPackageResourceScope resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d20da-104">В [управлении службой управления правами Azure AD](entitlementmanagement-root.md)область ресурсов пакета Access — это ссылка на область в ресурсе для этих ресурсов с несколькими областями.</span><span class="sxs-lookup"><span data-stu-id="d20da-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource scope is a reference to a scope within a resource, for those resources that have multiple scopes.</span></span>

## <a name="properties"></a><span data-ttu-id="d20da-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="d20da-105">Properties</span></span>

| <span data-ttu-id="d20da-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="d20da-106">Property</span></span>     | <span data-ttu-id="d20da-107">Тип</span><span class="sxs-lookup"><span data-stu-id="d20da-107">Type</span></span>        | <span data-ttu-id="d20da-108">Описание</span><span class="sxs-lookup"><span data-stu-id="d20da-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d20da-109">description</span><span class="sxs-lookup"><span data-stu-id="d20da-109">description</span></span>|<span data-ttu-id="d20da-110">String</span><span class="sxs-lookup"><span data-stu-id="d20da-110">String</span></span>|<span data-ttu-id="d20da-111">Описание области.</span><span class="sxs-lookup"><span data-stu-id="d20da-111">The description of the scope.</span></span>|
|<span data-ttu-id="d20da-112">displayName</span><span class="sxs-lookup"><span data-stu-id="d20da-112">displayName</span></span>|<span data-ttu-id="d20da-113">Строка</span><span class="sxs-lookup"><span data-stu-id="d20da-113">String</span></span>|<span data-ttu-id="d20da-114">Отображаемое имя области.</span><span class="sxs-lookup"><span data-stu-id="d20da-114">The display name of the scope.</span></span>|
|<span data-ttu-id="d20da-115">id</span><span class="sxs-lookup"><span data-stu-id="d20da-115">id</span></span>|<span data-ttu-id="d20da-116">String</span><span class="sxs-lookup"><span data-stu-id="d20da-116">String</span></span>| <span data-ttu-id="d20da-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d20da-117">Read-only.</span></span>|
|<span data-ttu-id="d20da-118">исрутскопе</span><span class="sxs-lookup"><span data-stu-id="d20da-118">isRootScope</span></span>|<span data-ttu-id="d20da-119">Логический</span><span class="sxs-lookup"><span data-stu-id="d20da-119">Boolean</span></span>|<span data-ttu-id="d20da-120">Значение true, если области упорядочены в иерархию, а это верхняя или корневая область ресурса.</span><span class="sxs-lookup"><span data-stu-id="d20da-120">True if the scopes are arranged in a hierarchy and this is the top or root scope of the resource.</span></span>|
|<span data-ttu-id="d20da-121">оригинид</span><span class="sxs-lookup"><span data-stu-id="d20da-121">originId</span></span>|<span data-ttu-id="d20da-122">Строка</span><span class="sxs-lookup"><span data-stu-id="d20da-122">String</span></span>|<span data-ttu-id="d20da-123">Уникальный идентификатор области ресурса в соответствии с определением в исходной системе.</span><span class="sxs-lookup"><span data-stu-id="d20da-123">The unique identifier for the scope in the resource as defined in the origin system.</span></span>|
|<span data-ttu-id="d20da-124">оригинсистем</span><span class="sxs-lookup"><span data-stu-id="d20da-124">originSystem</span></span>|<span data-ttu-id="d20da-125">Строка</span><span class="sxs-lookup"><span data-stu-id="d20da-125">String</span></span>|<span data-ttu-id="d20da-126">Исходная система для области.</span><span class="sxs-lookup"><span data-stu-id="d20da-126">The origin system for the scope.</span></span>|
|<span data-ttu-id="d20da-127">ролеоригинид</span><span class="sxs-lookup"><span data-stu-id="d20da-127">roleOriginId</span></span>|<span data-ttu-id="d20da-128">Строка</span><span class="sxs-lookup"><span data-stu-id="d20da-128">String</span></span>|<span data-ttu-id="d20da-129">Исходная система для роли, если она отличается.</span><span class="sxs-lookup"><span data-stu-id="d20da-129">The origin system for the role, if different.</span></span>|
|<span data-ttu-id="d20da-130">url</span><span class="sxs-lookup"><span data-stu-id="d20da-130">url</span></span>|<span data-ttu-id="d20da-131">String</span><span class="sxs-lookup"><span data-stu-id="d20da-131">String</span></span>|<span data-ttu-id="d20da-132">Указатель ресурсов для области.</span><span class="sxs-lookup"><span data-stu-id="d20da-132">A resource locator for the scope.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d20da-133">Связи</span><span class="sxs-lookup"><span data-stu-id="d20da-133">Relationships</span></span>

| <span data-ttu-id="d20da-134">Связь</span><span class="sxs-lookup"><span data-stu-id="d20da-134">Relationship</span></span> | <span data-ttu-id="d20da-135">Тип</span><span class="sxs-lookup"><span data-stu-id="d20da-135">Type</span></span>        | <span data-ttu-id="d20da-136">Описание</span><span class="sxs-lookup"><span data-stu-id="d20da-136">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d20da-137">акцесспаккажересаурце</span><span class="sxs-lookup"><span data-stu-id="d20da-137">accessPackageResource</span></span>|[<span data-ttu-id="d20da-138">акцесспаккажересаурце</span><span class="sxs-lookup"><span data-stu-id="d20da-138">accessPackageResource</span></span>](accesspackageresource.md)| <span data-ttu-id="d20da-p101">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="d20da-p101">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d20da-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d20da-141">JSON representation</span></span>

<span data-ttu-id="d20da-142">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d20da-142">The following is a JSON representation of the resource.</span></span>

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
