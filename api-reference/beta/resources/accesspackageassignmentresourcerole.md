---
title: Тип ресурса Акцесспаккажеассигнментресаурцероле
description: Роль ресурса назначения пакета Access указывает на роль, связанную с определенным ресурсом, которой назначена тема с помощью назначения пакета Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 403b97dc335e57dfd2d4f2fe2aa75c4f6fd07682
ms.sourcegitcommit: 2c6e16dd8381945de6adf1eea020c142969b7801
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/01/2020
ms.locfileid: "47319521"
---
# <a name="accesspackageassignmentresourcerole-resource-type"></a><span data-ttu-id="429c6-103">Тип ресурса Акцесспаккажеассигнментресаурцероле</span><span class="sxs-lookup"><span data-stu-id="429c6-103">accessPackageAssignmentResourceRole resource type</span></span>

<span data-ttu-id="429c6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="429c6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="429c6-105">В разделе [Управление обслуживанием в Azure AD](entitlementmanagement-root.md)роль ресурса назначения пакета Access указывает роль, связанную с определенным ресурсом, которой назначена тема с помощью назначения пакета Access.</span><span class="sxs-lookup"><span data-stu-id="429c6-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment resource role indicates the resource-specific role which a subject has been assigned through an access package assignment.</span></span>

## <a name="methods"></a><span data-ttu-id="429c6-106">Методы</span><span class="sxs-lookup"><span data-stu-id="429c6-106">Methods</span></span>

| <span data-ttu-id="429c6-107">Метод</span><span class="sxs-lookup"><span data-stu-id="429c6-107">Method</span></span>       | <span data-ttu-id="429c6-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="429c6-108">Return Type</span></span> | <span data-ttu-id="429c6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="429c6-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="429c6-110">Получение Акцесспаккажеассигнментресаурцероле</span><span class="sxs-lookup"><span data-stu-id="429c6-110">Get accessPackageAssignmentResourceRole</span></span>](../api/accesspackageassignmentresourcerole-get.md) | [<span data-ttu-id="429c6-111">акцесспаккажеассигнментресаурцероле</span><span class="sxs-lookup"><span data-stu-id="429c6-111">accessPackageAssignmentResourceRole</span></span>](accesspackageassignmentresourcerole.md)  | <span data-ttu-id="429c6-112">Получение объекта Акцесспаккажеассигнментресаурцероле.</span><span class="sxs-lookup"><span data-stu-id="429c6-112">Retrieve an accessPackageAssignmentResourceRole object.</span></span> |
| [<span data-ttu-id="429c6-113">Список Акцесспаккажеассигнментресаурцеролес</span><span class="sxs-lookup"><span data-stu-id="429c6-113">List accessPackageAssignmentResourceRoles</span></span>](../api/accesspackageassignmentresourcerole-list.md) | <span data-ttu-id="429c6-114">Коллекция [акцесспаккажеассигнментресаурцероле](accesspackageassignmentresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="429c6-114">[accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) collection</span></span> | <span data-ttu-id="429c6-115">Получение списка объектов Акцесспаккажеассигнментресаурцероле.</span><span class="sxs-lookup"><span data-stu-id="429c6-115">Retrieve a list of accessPackageAssignmentResourceRole objects.</span></span> |

## <a name="properties"></a><span data-ttu-id="429c6-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="429c6-116">Properties</span></span>

| <span data-ttu-id="429c6-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="429c6-117">Property</span></span>     | <span data-ttu-id="429c6-118">Тип</span><span class="sxs-lookup"><span data-stu-id="429c6-118">Type</span></span>        | <span data-ttu-id="429c6-119">Описание</span><span class="sxs-lookup"><span data-stu-id="429c6-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="429c6-120">id</span><span class="sxs-lookup"><span data-stu-id="429c6-120">id</span></span>|<span data-ttu-id="429c6-121">String</span><span class="sxs-lookup"><span data-stu-id="429c6-121">String</span></span>| <span data-ttu-id="429c6-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="429c6-122">Read-only.</span></span>|
|<span data-ttu-id="429c6-123">оригинид</span><span class="sxs-lookup"><span data-stu-id="429c6-123">originId</span></span>|<span data-ttu-id="429c6-124">String</span><span class="sxs-lookup"><span data-stu-id="429c6-124">String</span></span>|<span data-ttu-id="429c6-125">Уникальный идентификатор, относящийся к исходной системе, соответствующий свойству Оригинид объекта [акцесспаккажересаурцероле](accesspackageresourcerole.md).</span><span class="sxs-lookup"><span data-stu-id="429c6-125">A unique identifier relative to the origin system, corresponding to the originId property of the [accessPackageResourceRole](accesspackageresourcerole.md).</span></span> |
|<span data-ttu-id="429c6-126">оригинсистем</span><span class="sxs-lookup"><span data-stu-id="429c6-126">originSystem</span></span>|<span data-ttu-id="429c6-127">String</span><span class="sxs-lookup"><span data-stu-id="429c6-127">String</span></span>|<span data-ttu-id="429c6-128">Система, в которой необходимо создать назначение роли или она была создана для назначения пакета Access, например `SharePointOnline` , `AadGroup` или `AadApplication` соответствующего свойству оригинсистем объекта [акцесспаккажересаурцероле](accesspackageresourcerole.md).</span><span class="sxs-lookup"><span data-stu-id="429c6-128">The system where the role assignment is to be created or has been created for an access package assignment, such as `SharePointOnline`, `AadGroup` or `AadApplication`, corresponding to the originSystem property of the [accessPackageResourceRole](accesspackageresourcerole.md).</span></span>|
|<span data-ttu-id="429c6-129">status</span><span class="sxs-lookup"><span data-stu-id="429c6-129">status</span></span>|<span data-ttu-id="429c6-130">String</span><span class="sxs-lookup"><span data-stu-id="429c6-130">String</span></span>|<span data-ttu-id="429c6-131">Это значение используется, `PendingFulfillment` когда назначение пакета Access еще не было доставлено в исходную систему, и `Fulfilled` когда назначение пакета Access было доставлено в исходную систему.</span><span class="sxs-lookup"><span data-stu-id="429c6-131">The value is `PendingFulfillment` when the access package assignment has not yet been delivered to the origin system, and `Fulfilled` when the access package assignment has been delivered to the origin system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="429c6-132">Отношения</span><span class="sxs-lookup"><span data-stu-id="429c6-132">Relationships</span></span>

| <span data-ttu-id="429c6-133">Связь</span><span class="sxs-lookup"><span data-stu-id="429c6-133">Relationship</span></span> | <span data-ttu-id="429c6-134">Тип</span><span class="sxs-lookup"><span data-stu-id="429c6-134">Type</span></span>        | <span data-ttu-id="429c6-135">Описание</span><span class="sxs-lookup"><span data-stu-id="429c6-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="429c6-136">акцесспаккажеассигнментс</span><span class="sxs-lookup"><span data-stu-id="429c6-136">accessPackageAssignments</span></span>|<span data-ttu-id="429c6-137">Коллекция [акцесспаккажеассигнмент](accesspackageassignment.md)</span><span class="sxs-lookup"><span data-stu-id="429c6-137">[accessPackageAssignment](accesspackageassignment.md) collection</span></span>| <span data-ttu-id="429c6-138">Назначения для пакетов Access, которые применяют это назначение роли.</span><span class="sxs-lookup"><span data-stu-id="429c6-138">The access package assignments resulting in this role assignment.</span></span> <span data-ttu-id="429c6-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="429c6-139">Read-only.</span></span> <span data-ttu-id="429c6-140">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="429c6-140">Nullable.</span></span>|
|<span data-ttu-id="429c6-141">акцесспаккажересаурцероле</span><span class="sxs-lookup"><span data-stu-id="429c6-141">accessPackageResourceRole</span></span>|[<span data-ttu-id="429c6-142">акцесспаккажересаурцероле</span><span class="sxs-lookup"><span data-stu-id="429c6-142">accessPackageResourceRole</span></span>](accesspackageresourcerole.md)| <span data-ttu-id="429c6-143">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="429c6-143">Read-only.</span></span> <span data-ttu-id="429c6-144">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="429c6-144">Nullable.</span></span>|
|<span data-ttu-id="429c6-145">акцесспаккажересаурцескопе</span><span class="sxs-lookup"><span data-stu-id="429c6-145">accessPackageResourceScope</span></span>|[<span data-ttu-id="429c6-146">акцесспаккажересаурцескопе</span><span class="sxs-lookup"><span data-stu-id="429c6-146">accessPackageResourceScope</span></span>](accesspackageresourcescope.md)| <span data-ttu-id="429c6-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="429c6-147">Read-only.</span></span> <span data-ttu-id="429c6-148">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="429c6-148">Nullable.</span></span>|
|<span data-ttu-id="429c6-149">акцесспаккажесубжект</span><span class="sxs-lookup"><span data-stu-id="429c6-149">accessPackageSubject</span></span>|[<span data-ttu-id="429c6-150">акцесспаккажесубжект</span><span class="sxs-lookup"><span data-stu-id="429c6-150">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="429c6-p104">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="429c6-p104">Read-only. Nullable.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="429c6-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="429c6-153">JSON representation</span></span>

<span data-ttu-id="429c6-154">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="429c6-154">The following is a JSON representation of the resource.</span></span>

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
