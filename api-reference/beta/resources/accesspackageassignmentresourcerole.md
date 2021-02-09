---
title: Тип ресурса accessPackageAssignmentResourceRole
description: Роль ресурса назначения пакета доступа указывает роль, относяющуюся к ресурсу, которая была назначена субъекту посредством назначения пакета доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2b4893d40db8b5ac70a2ac3093d8dfbdf55c3175
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155603"
---
# <a name="accesspackageassignmentresourcerole-resource-type"></a><span data-ttu-id="9139f-103">Тип ресурса accessPackageAssignmentResourceRole</span><span class="sxs-lookup"><span data-stu-id="9139f-103">accessPackageAssignmentResourceRole resource type</span></span>

<span data-ttu-id="9139f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9139f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9139f-105">В [управлении правами Azure AD](entitlementmanagement-root.md)роль ресурса назначения пакета доступа указывает роль, относяющуюся к ресурсу, которой субъект был назначен посредством назначения пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="9139f-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment resource role indicates the resource-specific role which a subject has been assigned through an access package assignment.</span></span>

## <a name="methods"></a><span data-ttu-id="9139f-106">Методы</span><span class="sxs-lookup"><span data-stu-id="9139f-106">Methods</span></span>

| <span data-ttu-id="9139f-107">Метод</span><span class="sxs-lookup"><span data-stu-id="9139f-107">Method</span></span>       | <span data-ttu-id="9139f-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9139f-108">Return Type</span></span> | <span data-ttu-id="9139f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9139f-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="9139f-110">Get accessPackageAssignmentResourceRole</span><span class="sxs-lookup"><span data-stu-id="9139f-110">Get accessPackageAssignmentResourceRole</span></span>](../api/accesspackageassignmentresourcerole-get.md) | [<span data-ttu-id="9139f-111">accessPackageAssignmentResourceRole</span><span class="sxs-lookup"><span data-stu-id="9139f-111">accessPackageAssignmentResourceRole</span></span>](accesspackageassignmentresourcerole.md)  | <span data-ttu-id="9139f-112">Извлечение объекта accessPackageAssignmentResourceRole.</span><span class="sxs-lookup"><span data-stu-id="9139f-112">Retrieve an accessPackageAssignmentResourceRole object.</span></span> |
| [<span data-ttu-id="9139f-113">Список accessPackageAssignmentResourceRoles</span><span class="sxs-lookup"><span data-stu-id="9139f-113">List accessPackageAssignmentResourceRoles</span></span>](../api/accesspackageassignmentresourcerole-list.md) | <span data-ttu-id="9139f-114">[Коллекция accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="9139f-114">[accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) collection</span></span> | <span data-ttu-id="9139f-115">Получить список объектов accessPackageAssignmentResourceRole.</span><span class="sxs-lookup"><span data-stu-id="9139f-115">Retrieve a list of accessPackageAssignmentResourceRole objects.</span></span> |

## <a name="properties"></a><span data-ttu-id="9139f-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="9139f-116">Properties</span></span>

| <span data-ttu-id="9139f-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="9139f-117">Property</span></span>     | <span data-ttu-id="9139f-118">Тип</span><span class="sxs-lookup"><span data-stu-id="9139f-118">Type</span></span>        | <span data-ttu-id="9139f-119">Описание</span><span class="sxs-lookup"><span data-stu-id="9139f-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9139f-120">id</span><span class="sxs-lookup"><span data-stu-id="9139f-120">id</span></span>|<span data-ttu-id="9139f-121">String</span><span class="sxs-lookup"><span data-stu-id="9139f-121">String</span></span>| <span data-ttu-id="9139f-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9139f-122">Read-only.</span></span>|
|<span data-ttu-id="9139f-123">originId</span><span class="sxs-lookup"><span data-stu-id="9139f-123">originId</span></span>|<span data-ttu-id="9139f-124">String</span><span class="sxs-lookup"><span data-stu-id="9139f-124">String</span></span>|<span data-ttu-id="9139f-125">Уникальный идентификатор относительно системы источника, соответствующий свойству originId [объекта accessPackageResourceRole.](accesspackageresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="9139f-125">A unique identifier relative to the origin system, corresponding to the originId property of the [accessPackageResourceRole](accesspackageresourcerole.md).</span></span> |
|<span data-ttu-id="9139f-126">originSystem</span><span class="sxs-lookup"><span data-stu-id="9139f-126">originSystem</span></span>|<span data-ttu-id="9139f-127">String</span><span class="sxs-lookup"><span data-stu-id="9139f-127">String</span></span>|<span data-ttu-id="9139f-128">Система, в которой должно быть создано назначение роли или создано для назначения пакета доступа, например , или ,, соответствующие свойству `SharePointOnline` `AadGroup` `AadApplication` originSystem [accessPackageResourceRole](accesspackageresourcerole.md).</span><span class="sxs-lookup"><span data-stu-id="9139f-128">The system where the role assignment is to be created or has been created for an access package assignment, such as `SharePointOnline`, `AadGroup` or `AadApplication`, corresponding to the originSystem property of the [accessPackageResourceRole](accesspackageresourcerole.md).</span></span>|
|<span data-ttu-id="9139f-129">status</span><span class="sxs-lookup"><span data-stu-id="9139f-129">status</span></span>|<span data-ttu-id="9139f-130">String</span><span class="sxs-lookup"><span data-stu-id="9139f-130">String</span></span>|<span data-ttu-id="9139f-131">Значением является то, когда назначение пакета доступа еще не было доставлено в систему источника и когда назначение пакета доступа было доставлено в систему `PendingFulfillment` `Fulfilled` источника.</span><span class="sxs-lookup"><span data-stu-id="9139f-131">The value is `PendingFulfillment` when the access package assignment has not yet been delivered to the origin system, and `Fulfilled` when the access package assignment has been delivered to the origin system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9139f-132">Связи</span><span class="sxs-lookup"><span data-stu-id="9139f-132">Relationships</span></span>

| <span data-ttu-id="9139f-133">Связь</span><span class="sxs-lookup"><span data-stu-id="9139f-133">Relationship</span></span> | <span data-ttu-id="9139f-134">Тип</span><span class="sxs-lookup"><span data-stu-id="9139f-134">Type</span></span>        | <span data-ttu-id="9139f-135">Описание</span><span class="sxs-lookup"><span data-stu-id="9139f-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9139f-136">accessPackageAssignments</span><span class="sxs-lookup"><span data-stu-id="9139f-136">accessPackageAssignments</span></span>|<span data-ttu-id="9139f-137">[Коллекция accessPackageAssignment](accesspackageassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9139f-137">[accessPackageAssignment](accesspackageassignment.md) collection</span></span>| <span data-ttu-id="9139f-138">Назначения пакета доступа, в результате чего это назначение роли.</span><span class="sxs-lookup"><span data-stu-id="9139f-138">The access package assignments resulting in this role assignment.</span></span> <span data-ttu-id="9139f-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9139f-139">Read-only.</span></span> <span data-ttu-id="9139f-140">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="9139f-140">Nullable.</span></span>|
|<span data-ttu-id="9139f-141">accessPackageResourceRole</span><span class="sxs-lookup"><span data-stu-id="9139f-141">accessPackageResourceRole</span></span>|[<span data-ttu-id="9139f-142">accessPackageResourceRole</span><span class="sxs-lookup"><span data-stu-id="9139f-142">accessPackageResourceRole</span></span>](accesspackageresourcerole.md)| <span data-ttu-id="9139f-143">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9139f-143">Read-only.</span></span> <span data-ttu-id="9139f-144">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="9139f-144">Nullable.</span></span>|
|<span data-ttu-id="9139f-145">accessPackageResourceScope</span><span class="sxs-lookup"><span data-stu-id="9139f-145">accessPackageResourceScope</span></span>|[<span data-ttu-id="9139f-146">accessPackageResourceScope</span><span class="sxs-lookup"><span data-stu-id="9139f-146">accessPackageResourceScope</span></span>](accesspackageresourcescope.md)| <span data-ttu-id="9139f-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9139f-147">Read-only.</span></span> <span data-ttu-id="9139f-148">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="9139f-148">Nullable.</span></span>|
|<span data-ttu-id="9139f-149">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="9139f-149">accessPackageSubject</span></span>|[<span data-ttu-id="9139f-150">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="9139f-150">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="9139f-p104">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="9139f-p104">Read-only. Nullable.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="9139f-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9139f-153">JSON representation</span></span>

<span data-ttu-id="9139f-154">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9139f-154">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageAssignmentResourceRole",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "originId": "String",
  "originSystem": "String",
  "status": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageAssignmentResourceRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


