---
title: тип ресурса accessPackageAssignmentResourceRole
description: Роль ресурса назначения пакета доступа указывает на роль, определенную для ресурса, которую субъекту было назначено с помощью назначения пакета доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 4473c303a74cbf9e8e0c17d6c9060960590a3405
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433283"
---
# <a name="accesspackageassignmentresourcerole-resource-type"></a><span data-ttu-id="1f994-103">тип ресурса accessPackageAssignmentResourceRole</span><span class="sxs-lookup"><span data-stu-id="1f994-103">accessPackageAssignmentResourceRole resource type</span></span>

<span data-ttu-id="1f994-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f994-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f994-105">В управлении правами [Azure AD](entitlementmanagement-root.md)роль ресурса назначения пакета доступа указывает на роль, определенную для ресурса, которую субъекту было назначено с помощью назначения пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="1f994-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment resource role indicates the resource-specific role which a subject has been assigned through an access package assignment.</span></span>

## <a name="methods"></a><span data-ttu-id="1f994-106">Методы</span><span class="sxs-lookup"><span data-stu-id="1f994-106">Methods</span></span>

| <span data-ttu-id="1f994-107">Метод</span><span class="sxs-lookup"><span data-stu-id="1f994-107">Method</span></span>       | <span data-ttu-id="1f994-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1f994-108">Return Type</span></span> | <span data-ttu-id="1f994-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1f994-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="1f994-110">Получите accessPackageAssignmentResourceRole</span><span class="sxs-lookup"><span data-stu-id="1f994-110">Get accessPackageAssignmentResourceRole</span></span>](../api/accesspackageassignmentresourcerole-get.md) | [<span data-ttu-id="1f994-111">accessPackageAssignmentResourceRole</span><span class="sxs-lookup"><span data-stu-id="1f994-111">accessPackageAssignmentResourceRole</span></span>](accesspackageassignmentresourcerole.md)  | <span data-ttu-id="1f994-112">Извлечение объекта accessPackageAssignmentResourceRole.</span><span class="sxs-lookup"><span data-stu-id="1f994-112">Retrieve an accessPackageAssignmentResourceRole object.</span></span> |
| [<span data-ttu-id="1f994-113">Список accessPackageAssignmentResourceRoles</span><span class="sxs-lookup"><span data-stu-id="1f994-113">List accessPackageAssignmentResourceRoles</span></span>](../api/accesspackageassignmentresourcerole-list.md) | <span data-ttu-id="1f994-114">[коллекция accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="1f994-114">[accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) collection</span></span> | <span data-ttu-id="1f994-115">Извлечение списка объектов accessPackageAssignmentResourceRole.</span><span class="sxs-lookup"><span data-stu-id="1f994-115">Retrieve a list of accessPackageAssignmentResourceRole objects.</span></span> |

## <a name="properties"></a><span data-ttu-id="1f994-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="1f994-116">Properties</span></span>

| <span data-ttu-id="1f994-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="1f994-117">Property</span></span>     | <span data-ttu-id="1f994-118">Тип</span><span class="sxs-lookup"><span data-stu-id="1f994-118">Type</span></span>        | <span data-ttu-id="1f994-119">Описание</span><span class="sxs-lookup"><span data-stu-id="1f994-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1f994-120">id</span><span class="sxs-lookup"><span data-stu-id="1f994-120">id</span></span>|<span data-ttu-id="1f994-121">String</span><span class="sxs-lookup"><span data-stu-id="1f994-121">String</span></span>| <span data-ttu-id="1f994-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1f994-122">Read-only.</span></span>|
|<span data-ttu-id="1f994-123">OriginId</span><span class="sxs-lookup"><span data-stu-id="1f994-123">originId</span></span>|<span data-ttu-id="1f994-124">String</span><span class="sxs-lookup"><span data-stu-id="1f994-124">String</span></span>|<span data-ttu-id="1f994-125">Уникальный идентификатор относительно системы происхождения, соответствующий свойству originId [accessPackageResourceRole.](accesspackageresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="1f994-125">A unique identifier relative to the origin system, corresponding to the originId property of the [accessPackageResourceRole](accesspackageresourcerole.md).</span></span> |
|<span data-ttu-id="1f994-126">originSystem</span><span class="sxs-lookup"><span data-stu-id="1f994-126">originSystem</span></span>|<span data-ttu-id="1f994-127">String</span><span class="sxs-lookup"><span data-stu-id="1f994-127">String</span></span>|<span data-ttu-id="1f994-128">Система, в которой назначение ролей должно быть создано или создано для назначения пакета доступа, например, или , соответствующего свойству `SharePointOnline` `AadGroup` `AadApplication` [originSystem accessPackageResourceRole.](accesspackageresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="1f994-128">The system where the role assignment is to be created or has been created for an access package assignment, such as `SharePointOnline`, `AadGroup` or `AadApplication`, corresponding to the originSystem property of the [accessPackageResourceRole](accesspackageresourcerole.md).</span></span>|
|<span data-ttu-id="1f994-129">status</span><span class="sxs-lookup"><span data-stu-id="1f994-129">status</span></span>|<span data-ttu-id="1f994-130">String</span><span class="sxs-lookup"><span data-stu-id="1f994-130">String</span></span>|<span data-ttu-id="1f994-131">Значение — когда назначение пакета доступа еще не доставлено в систему происхождения и когда назначение пакета доступа было доставлено в `PendingFulfillment` `Fulfilled` систему происхождения.</span><span class="sxs-lookup"><span data-stu-id="1f994-131">The value is `PendingFulfillment` when the access package assignment has not yet been delivered to the origin system, and `Fulfilled` when the access package assignment has been delivered to the origin system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1f994-132">Связи</span><span class="sxs-lookup"><span data-stu-id="1f994-132">Relationships</span></span>

| <span data-ttu-id="1f994-133">Связь</span><span class="sxs-lookup"><span data-stu-id="1f994-133">Relationship</span></span> | <span data-ttu-id="1f994-134">Тип</span><span class="sxs-lookup"><span data-stu-id="1f994-134">Type</span></span>        | <span data-ttu-id="1f994-135">Описание</span><span class="sxs-lookup"><span data-stu-id="1f994-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1f994-136">accessPackageAssignments</span><span class="sxs-lookup"><span data-stu-id="1f994-136">accessPackageAssignments</span></span>|<span data-ttu-id="1f994-137">[коллекция accessPackageAssignment](accesspackageassignment.md)</span><span class="sxs-lookup"><span data-stu-id="1f994-137">[accessPackageAssignment](accesspackageassignment.md) collection</span></span>| <span data-ttu-id="1f994-138">Назначения пакета доступа, в результате чего это назначение роли.</span><span class="sxs-lookup"><span data-stu-id="1f994-138">The access package assignments resulting in this role assignment.</span></span> <span data-ttu-id="1f994-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1f994-139">Read-only.</span></span> <span data-ttu-id="1f994-140">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="1f994-140">Nullable.</span></span>|
|<span data-ttu-id="1f994-141">accessPackageResourceRole</span><span class="sxs-lookup"><span data-stu-id="1f994-141">accessPackageResourceRole</span></span>|[<span data-ttu-id="1f994-142">accessPackageResourceRole</span><span class="sxs-lookup"><span data-stu-id="1f994-142">accessPackageResourceRole</span></span>](accesspackageresourcerole.md)| <span data-ttu-id="1f994-143">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1f994-143">Read-only.</span></span> <span data-ttu-id="1f994-144">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="1f994-144">Nullable.</span></span>|
|<span data-ttu-id="1f994-145">accessPackageResourceScope</span><span class="sxs-lookup"><span data-stu-id="1f994-145">accessPackageResourceScope</span></span>|[<span data-ttu-id="1f994-146">accessPackageResourceScope</span><span class="sxs-lookup"><span data-stu-id="1f994-146">accessPackageResourceScope</span></span>](accesspackageresourcescope.md)| <span data-ttu-id="1f994-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1f994-147">Read-only.</span></span> <span data-ttu-id="1f994-148">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="1f994-148">Nullable.</span></span>|
|<span data-ttu-id="1f994-149">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="1f994-149">accessPackageSubject</span></span>|[<span data-ttu-id="1f994-150">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="1f994-150">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="1f994-p104">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="1f994-p104">Read-only. Nullable.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="1f994-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1f994-153">JSON representation</span></span>

<span data-ttu-id="1f994-154">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1f994-154">The following is a JSON representation of the resource.</span></span>

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


