---
title: тип ресурса accessPackageResourceRoleScope
description: Область роли ресурсов пакета доступа — это ссылка как на область в ресурсе, так и на роль в этом ресурсе.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8fa3e0a20646f2acf72d26d31c20bac674e751cd
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720951"
---
# <a name="accesspackageresourcerolescope-resource-type"></a><span data-ttu-id="bddae-103">тип ресурса accessPackageResourceRoleScope</span><span class="sxs-lookup"><span data-stu-id="bddae-103">accessPackageResourceRoleScope resource type</span></span>

<span data-ttu-id="bddae-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bddae-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bddae-105">В управлении правами [Azure AD](entitlementmanagement-root.md)область ролей пакета доступа является ссылкой как на область в ресурсе, так и на роль в этом ресурсе для этой области.</span><span class="sxs-lookup"><span data-stu-id="bddae-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource role scope is a reference to both a scope within a resource, and a role in that resource for that scope.</span></span>  <span data-ttu-id="bddae-106">Пакет доступа будет иметь области ролей ресурсов пакета доступа для ресурсов в его каталоге, которые имеют отношение к этому пакету доступа.</span><span class="sxs-lookup"><span data-stu-id="bddae-106">An access package will have access package resource role scopes for the resources in its catalog which are relevant to that access package.</span></span>  <span data-ttu-id="bddae-107">Когда субъект получает назначение пакета доступа, субъекту будет присвоена роль в этой области для каждого области ролей ресурсов пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="bddae-107">When a subject receives an access package assignment, the subject will be provisioned with the role in that scope of each access package resource role scope.</span></span>

## <a name="methods"></a><span data-ttu-id="bddae-108">Методы</span><span class="sxs-lookup"><span data-stu-id="bddae-108">Methods</span></span>

| <span data-ttu-id="bddae-109">Метод</span><span class="sxs-lookup"><span data-stu-id="bddae-109">Method</span></span>       | <span data-ttu-id="bddae-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bddae-110">Return Type</span></span> | <span data-ttu-id="bddae-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bddae-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="bddae-112">Список accessPackageResourceRoleScopes</span><span class="sxs-lookup"><span data-stu-id="bddae-112">List accessPackageResourceRoleScopes</span></span>](../api/accesspackage-list-accesspackageresourcerolescopes.md) | <span data-ttu-id="bddae-113">[коллекция accessPackageResourceRoleScope](accesspackageresourcerolescope.md)</span><span class="sxs-lookup"><span data-stu-id="bddae-113">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md) collection</span></span> | <span data-ttu-id="bddae-114">Извлечение списка **объектов accessPackageResourceRoleScope** для пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="bddae-114">Retrieve a list of **accessPackageResourceRoleScope** objects for an access package.</span></span> |
| [<span data-ttu-id="bddae-115">Создание accessPackageResourceRoleScope</span><span class="sxs-lookup"><span data-stu-id="bddae-115">Create accessPackageResourceRoleScope</span></span>](../api/accesspackage-post-accesspackageresourcerolescopes.md) | | <span data-ttu-id="bddae-116">Создайте новый **объект accessPackageResourceRoleScope** для пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="bddae-116">Create a new **accessPackageResourceRoleScope** object for an access package.</span></span> |

## <a name="properties"></a><span data-ttu-id="bddae-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="bddae-117">Properties</span></span>

| <span data-ttu-id="bddae-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="bddae-118">Property</span></span>     | <span data-ttu-id="bddae-119">Тип</span><span class="sxs-lookup"><span data-stu-id="bddae-119">Type</span></span>        | <span data-ttu-id="bddae-120">Описание</span><span class="sxs-lookup"><span data-stu-id="bddae-120">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bddae-121">createdBy</span><span class="sxs-lookup"><span data-stu-id="bddae-121">createdBy</span></span>|<span data-ttu-id="bddae-122">String</span><span class="sxs-lookup"><span data-stu-id="bddae-122">String</span></span>|<span data-ttu-id="bddae-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bddae-123">Read-only.</span></span>|
|<span data-ttu-id="bddae-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bddae-124">createdDateTime</span></span>|<span data-ttu-id="bddae-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bddae-125">DateTimeOffset</span></span>|<span data-ttu-id="bddae-126">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="bddae-126">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="bddae-127">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="bddae-127">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="bddae-128">id</span><span class="sxs-lookup"><span data-stu-id="bddae-128">id</span></span>|<span data-ttu-id="bddae-129">String</span><span class="sxs-lookup"><span data-stu-id="bddae-129">String</span></span>| <span data-ttu-id="bddae-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bddae-130">Read-only.</span></span>|
|<span data-ttu-id="bddae-131">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="bddae-131">modifiedBy</span></span>|<span data-ttu-id="bddae-132">String</span><span class="sxs-lookup"><span data-stu-id="bddae-132">String</span></span>|<span data-ttu-id="bddae-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bddae-133">Read-only.</span></span>|
|<span data-ttu-id="bddae-134">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bddae-134">modifiedDateTime</span></span>|<span data-ttu-id="bddae-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bddae-135">DateTimeOffset</span></span>|<span data-ttu-id="bddae-136">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="bddae-136">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="bddae-137">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="bddae-137">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|

## <a name="relationships"></a><span data-ttu-id="bddae-138">Связи</span><span class="sxs-lookup"><span data-stu-id="bddae-138">Relationships</span></span>

| <span data-ttu-id="bddae-139">Связь</span><span class="sxs-lookup"><span data-stu-id="bddae-139">Relationship</span></span> | <span data-ttu-id="bddae-140">Тип</span><span class="sxs-lookup"><span data-stu-id="bddae-140">Type</span></span>        | <span data-ttu-id="bddae-141">Описание</span><span class="sxs-lookup"><span data-stu-id="bddae-141">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bddae-142">accessPackageResourceRole</span><span class="sxs-lookup"><span data-stu-id="bddae-142">accessPackageResourceRole</span></span>|[<span data-ttu-id="bddae-143">accessPackageResourceRole</span><span class="sxs-lookup"><span data-stu-id="bddae-143">accessPackageResourceRole</span></span>](accesspackageresourcerole.md)| <span data-ttu-id="bddae-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bddae-144">Read-only.</span></span> <span data-ttu-id="bddae-145">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="bddae-145">Nullable.</span></span>|
|<span data-ttu-id="bddae-146">accessPackageResourceScope</span><span class="sxs-lookup"><span data-stu-id="bddae-146">accessPackageResourceScope</span></span>|[<span data-ttu-id="bddae-147">accessPackageResourceScope</span><span class="sxs-lookup"><span data-stu-id="bddae-147">accessPackageResourceScope</span></span>](accesspackageresourcescope.md)| <span data-ttu-id="bddae-p105">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="bddae-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bddae-150">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bddae-150">JSON representation</span></span>

<span data-ttu-id="bddae-151">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bddae-151">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageResourceRoleScope",
  "keyProperty": "id"
}-->

```json
{
   "createdBy":"String",
   "createdDateTime":"String (timestamp)",
   "id":"String (identifier)",
   "modifiedBy":"String",
   "modifiedDateTime":"String (timestamp)",
   "accessPackageResourceRole":{
      "id":"String (identifier)",
      "displayName":"String",
      "originSystem":"String",
      "originId":"String"
   },
   "accessPackageResourceScope":{
      "id":"String (identifier)",
      "displayName":"String",
      "description":"String",
      "originId":"String (identifier)",
      "originSystem":"String"
   }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageResourceRoleScope resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


