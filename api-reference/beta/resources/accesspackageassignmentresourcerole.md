---
title: Тип ресурса Акцесспаккажеассигнментресаурцероле
description: Роль ресурса назначения пакета Access указывает на роль, связанную с определенным ресурсом, которой назначена тема с помощью назначения пакета Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6ef0827736d16f1dbf3aedfb664467011e75e7b2
ms.sourcegitcommit: 7a6231aeb570ff45d01b3db3df07a411f9f60fd1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2020
ms.locfileid: "44383779"
---
# <a name="accesspackageassignmentresourcerole-resource-type"></a><span data-ttu-id="f18ca-103">Тип ресурса Акцесспаккажеассигнментресаурцероле</span><span class="sxs-lookup"><span data-stu-id="f18ca-103">accessPackageAssignmentResourceRole resource type</span></span>

<span data-ttu-id="f18ca-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f18ca-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f18ca-105">В разделе [Управление обслуживанием в Azure AD](entitlementmanagement-root.md)роль ресурса назначения пакета Access указывает роль, связанную с определенным ресурсом, которой назначена тема с помощью назначения пакета Access.</span><span class="sxs-lookup"><span data-stu-id="f18ca-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment resource role indicates the resource-specific role which a subject has been assigned through an access package assignment.</span></span>

## <a name="methods"></a><span data-ttu-id="f18ca-106">Методы</span><span class="sxs-lookup"><span data-stu-id="f18ca-106">Methods</span></span>

| <span data-ttu-id="f18ca-107">Метод</span><span class="sxs-lookup"><span data-stu-id="f18ca-107">Method</span></span>       | <span data-ttu-id="f18ca-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f18ca-108">Return Type</span></span> | <span data-ttu-id="f18ca-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f18ca-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="f18ca-110">Получение Акцесспаккажеассигнментресаурцероле</span><span class="sxs-lookup"><span data-stu-id="f18ca-110">Get accessPackageAssignmentResourceRole</span></span>](../api/accesspackageassignmentresourcerole-get.md) | [<span data-ttu-id="f18ca-111">акцесспаккажеассигнментресаурцероле</span><span class="sxs-lookup"><span data-stu-id="f18ca-111">accessPackageAssignmentResourceRole</span></span>](accesspackageassignmentresourcerole.md)  | <span data-ttu-id="f18ca-112">Получение объекта Акцесспаккажеассигнментресаурцероле.</span><span class="sxs-lookup"><span data-stu-id="f18ca-112">Retrieve an accessPackageAssignmentResourceRole object.</span></span> |
| [<span data-ttu-id="f18ca-113">Список Акцесспаккажеассигнментресаурцеролес</span><span class="sxs-lookup"><span data-stu-id="f18ca-113">List accessPackageAssignmentResourceRoles</span></span>](../api/accesspackageassignmentresourcerole-list.md) | <span data-ttu-id="f18ca-114">Коллекция [акцесспаккажеассигнментресаурцероле](accesspackageassignmentresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="f18ca-114">[accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) collection</span></span> | <span data-ttu-id="f18ca-115">Получение списка объектов Акцесспаккажеассигнментресаурцероле.</span><span class="sxs-lookup"><span data-stu-id="f18ca-115">Retrieve a list of accessPackageAssignmentResourceRole objects.</span></span> |

## <a name="properties"></a><span data-ttu-id="f18ca-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="f18ca-116">Properties</span></span>

| <span data-ttu-id="f18ca-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="f18ca-117">Property</span></span>     | <span data-ttu-id="f18ca-118">Тип</span><span class="sxs-lookup"><span data-stu-id="f18ca-118">Type</span></span>        | <span data-ttu-id="f18ca-119">Описание</span><span class="sxs-lookup"><span data-stu-id="f18ca-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f18ca-120">id</span><span class="sxs-lookup"><span data-stu-id="f18ca-120">id</span></span>|<span data-ttu-id="f18ca-121">String</span><span class="sxs-lookup"><span data-stu-id="f18ca-121">String</span></span>| <span data-ttu-id="f18ca-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f18ca-122">Read-only.</span></span>|
|<span data-ttu-id="f18ca-123">оригинид</span><span class="sxs-lookup"><span data-stu-id="f18ca-123">originId</span></span>|<span data-ttu-id="f18ca-124">String</span><span class="sxs-lookup"><span data-stu-id="f18ca-124">String</span></span>|<span data-ttu-id="f18ca-125">Уникальный идентификатор, связанный с исходной системой.</span><span class="sxs-lookup"><span data-stu-id="f18ca-125">A unique identifier relative to the origin system.</span></span> |
|<span data-ttu-id="f18ca-126">оригинсистем</span><span class="sxs-lookup"><span data-stu-id="f18ca-126">originSystem</span></span>|<span data-ttu-id="f18ca-127">String</span><span class="sxs-lookup"><span data-stu-id="f18ca-127">String</span></span>|<span data-ttu-id="f18ca-128">Система, в которой необходимо создать назначение роли или она была создана для назначения пакета Access, например `SharePointOnline` .</span><span class="sxs-lookup"><span data-stu-id="f18ca-128">The system where the role assignment is to be created or has been created for an access package assignment, such as `SharePointOnline`.</span></span>|
|<span data-ttu-id="f18ca-129">status</span><span class="sxs-lookup"><span data-stu-id="f18ca-129">status</span></span>|<span data-ttu-id="f18ca-130">String</span><span class="sxs-lookup"><span data-stu-id="f18ca-130">String</span></span>|<span data-ttu-id="f18ca-131">Значение задается, `Fulfilled` когда назначение пакета Access было доставлено в исходную систему.</span><span class="sxs-lookup"><span data-stu-id="f18ca-131">The value is `Fulfilled` when the access package assignment has been delivered to the origin system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f18ca-132">Связи</span><span class="sxs-lookup"><span data-stu-id="f18ca-132">Relationships</span></span>

| <span data-ttu-id="f18ca-133">Связь</span><span class="sxs-lookup"><span data-stu-id="f18ca-133">Relationship</span></span> | <span data-ttu-id="f18ca-134">Тип</span><span class="sxs-lookup"><span data-stu-id="f18ca-134">Type</span></span>        | <span data-ttu-id="f18ca-135">Описание</span><span class="sxs-lookup"><span data-stu-id="f18ca-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f18ca-136">акцесспаккажеассигнментс</span><span class="sxs-lookup"><span data-stu-id="f18ca-136">accessPackageAssignments</span></span>|<span data-ttu-id="f18ca-137">Коллекция [акцесспаккажеассигнмент](accesspackageassignment.md)</span><span class="sxs-lookup"><span data-stu-id="f18ca-137">[accessPackageAssignment](accesspackageassignment.md) collection</span></span>| <span data-ttu-id="f18ca-138">Назначения для пакетов Access, которые применяют это назначение роли.</span><span class="sxs-lookup"><span data-stu-id="f18ca-138">The access package assignments resulting in this role assignment.</span></span> <span data-ttu-id="f18ca-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f18ca-139">Read-only.</span></span> <span data-ttu-id="f18ca-140">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="f18ca-140">Nullable.</span></span>|
|<span data-ttu-id="f18ca-141">акцесспаккажересаурцероле</span><span class="sxs-lookup"><span data-stu-id="f18ca-141">accessPackageResourceRole</span></span>|[<span data-ttu-id="f18ca-142">акцесспаккажересаурцероле</span><span class="sxs-lookup"><span data-stu-id="f18ca-142">accessPackageResourceRole</span></span>](accesspackageresourcerole.md)| <span data-ttu-id="f18ca-143">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f18ca-143">Read-only.</span></span> <span data-ttu-id="f18ca-144">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="f18ca-144">Nullable.</span></span>|
|<span data-ttu-id="f18ca-145">акцесспаккажересаурцескопе</span><span class="sxs-lookup"><span data-stu-id="f18ca-145">accessPackageResourceScope</span></span>|[<span data-ttu-id="f18ca-146">акцесспаккажересаурцескопе</span><span class="sxs-lookup"><span data-stu-id="f18ca-146">accessPackageResourceScope</span></span>](accesspackageresourcescope.md)| <span data-ttu-id="f18ca-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f18ca-147">Read-only.</span></span> <span data-ttu-id="f18ca-148">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="f18ca-148">Nullable.</span></span>|
|<span data-ttu-id="f18ca-149">акцесспаккажесубжект</span><span class="sxs-lookup"><span data-stu-id="f18ca-149">accessPackageSubject</span></span>|[<span data-ttu-id="f18ca-150">акцесспаккажесубжект</span><span class="sxs-lookup"><span data-stu-id="f18ca-150">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="f18ca-p104">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="f18ca-p104">Read-only. Nullable.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="f18ca-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f18ca-153">JSON representation</span></span>

<span data-ttu-id="f18ca-154">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f18ca-154">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageAssignmentResourceRole",
  "baseType": "",
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
