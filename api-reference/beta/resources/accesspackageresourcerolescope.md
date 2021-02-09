---
title: Тип ресурса accessPackageResourceRoleScope
description: Область роли ресурса пакета доступа — это ссылка как на область в ресурсе, так и на роль в этом ресурсе.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6f6b68ad23505458a40be54ed073e0c01a81f06e
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158557"
---
# <a name="accesspackageresourcerolescope-resource-type"></a><span data-ttu-id="e37ef-103">Тип ресурса accessPackageResourceRoleScope</span><span class="sxs-lookup"><span data-stu-id="e37ef-103">accessPackageResourceRoleScope resource type</span></span>

<span data-ttu-id="e37ef-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e37ef-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e37ef-105">В управлении правами [Azure AD](entitlementmanagement-root.md)область роли пакета доступа — это ссылка как на область ресурса, так и на роль в этом ресурсе для этой области.</span><span class="sxs-lookup"><span data-stu-id="e37ef-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource role scope is a reference to both a scope within a resource, and a role in that resource for that scope.</span></span>  <span data-ttu-id="e37ef-106">Пакет доступа будет иметь области ролей ресурсов пакета доступа для ресурсов в каталоге, которые имеют отношение к этому пакету доступа.</span><span class="sxs-lookup"><span data-stu-id="e37ef-106">An access package will have access package resource role scopes for the resources in its catalog which are relevant to that access package.</span></span>  <span data-ttu-id="e37ef-107">Когда субъект получает назначение пакета доступа, субъекту будет присвоена роль в этой области каждой области роли ресурса пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="e37ef-107">When a subject receives an access package assignment, the subject will be provisioned with the role in that scope of each access package resource role scope.</span></span>

## <a name="methods"></a><span data-ttu-id="e37ef-108">Методы</span><span class="sxs-lookup"><span data-stu-id="e37ef-108">Methods</span></span>

| <span data-ttu-id="e37ef-109">Метод</span><span class="sxs-lookup"><span data-stu-id="e37ef-109">Method</span></span>       | <span data-ttu-id="e37ef-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e37ef-110">Return Type</span></span> | <span data-ttu-id="e37ef-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e37ef-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e37ef-112">Список accessPackageResourceRoleScopes</span><span class="sxs-lookup"><span data-stu-id="e37ef-112">List accessPackageResourceRoleScopes</span></span>](../api/accesspackage-list-accesspackageresourcerolescopes.md) | <span data-ttu-id="e37ef-113">[Коллекция accessPackageResourceRoleScope](accesspackageresourcerolescope.md)</span><span class="sxs-lookup"><span data-stu-id="e37ef-113">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md) collection</span></span> | <span data-ttu-id="e37ef-114">Получить список объектов **accessPackageResourceRoleScope** для пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="e37ef-114">Retrieve a list of **accessPackageResourceRoleScope** objects for an access package.</span></span> |
| [<span data-ttu-id="e37ef-115">Создание accessPackageResourceRoleScope</span><span class="sxs-lookup"><span data-stu-id="e37ef-115">Create accessPackageResourceRoleScope</span></span>](../api/accesspackage-post-accesspackageresourcerolescopes.md) | | <span data-ttu-id="e37ef-116">Создайте новый **объект accessPackageResourceRoleScope** для пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="e37ef-116">Create a new **accessPackageResourceRoleScope** object for an access package.</span></span> |

## <a name="properties"></a><span data-ttu-id="e37ef-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="e37ef-117">Properties</span></span>

| <span data-ttu-id="e37ef-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="e37ef-118">Property</span></span>     | <span data-ttu-id="e37ef-119">Тип</span><span class="sxs-lookup"><span data-stu-id="e37ef-119">Type</span></span>        | <span data-ttu-id="e37ef-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e37ef-120">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e37ef-121">createdBy</span><span class="sxs-lookup"><span data-stu-id="e37ef-121">createdBy</span></span>|<span data-ttu-id="e37ef-122">String</span><span class="sxs-lookup"><span data-stu-id="e37ef-122">String</span></span>|<span data-ttu-id="e37ef-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e37ef-123">Read-only.</span></span>|
|<span data-ttu-id="e37ef-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e37ef-124">createdDateTime</span></span>|<span data-ttu-id="e37ef-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e37ef-125">DateTimeOffset</span></span>|<span data-ttu-id="e37ef-p102">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="e37ef-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="e37ef-128">id</span><span class="sxs-lookup"><span data-stu-id="e37ef-128">id</span></span>|<span data-ttu-id="e37ef-129">String</span><span class="sxs-lookup"><span data-stu-id="e37ef-129">String</span></span>| <span data-ttu-id="e37ef-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e37ef-130">Read-only.</span></span>|
|<span data-ttu-id="e37ef-131">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="e37ef-131">modifiedBy</span></span>|<span data-ttu-id="e37ef-132">String</span><span class="sxs-lookup"><span data-stu-id="e37ef-132">String</span></span>|<span data-ttu-id="e37ef-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e37ef-133">Read-only.</span></span>|
|<span data-ttu-id="e37ef-134">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e37ef-134">modifiedDateTime</span></span>|<span data-ttu-id="e37ef-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e37ef-135">DateTimeOffset</span></span>|<span data-ttu-id="e37ef-p103">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="e37ef-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="e37ef-138">Связи</span><span class="sxs-lookup"><span data-stu-id="e37ef-138">Relationships</span></span>

| <span data-ttu-id="e37ef-139">Связь</span><span class="sxs-lookup"><span data-stu-id="e37ef-139">Relationship</span></span> | <span data-ttu-id="e37ef-140">Тип</span><span class="sxs-lookup"><span data-stu-id="e37ef-140">Type</span></span>        | <span data-ttu-id="e37ef-141">Описание</span><span class="sxs-lookup"><span data-stu-id="e37ef-141">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e37ef-142">accessPackageResourceRole</span><span class="sxs-lookup"><span data-stu-id="e37ef-142">accessPackageResourceRole</span></span>|[<span data-ttu-id="e37ef-143">accessPackageResourceRole</span><span class="sxs-lookup"><span data-stu-id="e37ef-143">accessPackageResourceRole</span></span>](accesspackageresourcerole.md)| <span data-ttu-id="e37ef-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e37ef-144">Read-only.</span></span> <span data-ttu-id="e37ef-145">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="e37ef-145">Nullable.</span></span>|
|<span data-ttu-id="e37ef-146">accessPackageResourceScope</span><span class="sxs-lookup"><span data-stu-id="e37ef-146">accessPackageResourceScope</span></span>|[<span data-ttu-id="e37ef-147">accessPackageResourceScope</span><span class="sxs-lookup"><span data-stu-id="e37ef-147">accessPackageResourceScope</span></span>](accesspackageresourcescope.md)| <span data-ttu-id="e37ef-p105">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="e37ef-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e37ef-150">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e37ef-150">JSON representation</span></span>

<span data-ttu-id="e37ef-151">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e37ef-151">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageResourceRoleScope",
  "keyProperty": "id"
}-->

```json
{
  "createdBy": "String",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "modifiedBy": "String",
  "modifiedDateTime": "String (timestamp)",
  "accessPackageResourceRole": {
    "id": "String (identifier)",
     "displayName": "String",
     "originSystem": "String",
     "originId": "String"
  },
  "accessPackageResourceScope": {
     "id": "String (identifier)",
     "displayName": "String",
     "description": "String",
     "originId": "String (identifier)",
     "originSystem": "String"
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


