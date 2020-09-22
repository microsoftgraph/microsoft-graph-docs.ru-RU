---
title: Тип ресурса Акцесспаккажеассигнментресаурцероле
description: Роль ресурса назначения пакета Access указывает на роль, связанную с определенным ресурсом, которой назначена тема с помощью назначения пакета Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8bf839d68db3f54df5a27601a4a05463e013fbef
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48089863"
---
# <a name="accesspackageassignmentresourcerole-resource-type"></a><span data-ttu-id="0744c-103">Тип ресурса Акцесспаккажеассигнментресаурцероле</span><span class="sxs-lookup"><span data-stu-id="0744c-103">accessPackageAssignmentResourceRole resource type</span></span>

<span data-ttu-id="0744c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0744c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0744c-105">В разделе [Управление обслуживанием в Azure AD](entitlementmanagement-root.md)роль ресурса назначения пакета Access указывает роль, связанную с определенным ресурсом, которой назначена тема с помощью назначения пакета Access.</span><span class="sxs-lookup"><span data-stu-id="0744c-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment resource role indicates the resource-specific role which a subject has been assigned through an access package assignment.</span></span>

## <a name="methods"></a><span data-ttu-id="0744c-106">Методы</span><span class="sxs-lookup"><span data-stu-id="0744c-106">Methods</span></span>

| <span data-ttu-id="0744c-107">Метод</span><span class="sxs-lookup"><span data-stu-id="0744c-107">Method</span></span>       | <span data-ttu-id="0744c-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0744c-108">Return Type</span></span> | <span data-ttu-id="0744c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0744c-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="0744c-110">Получение Акцесспаккажеассигнментресаурцероле</span><span class="sxs-lookup"><span data-stu-id="0744c-110">Get accessPackageAssignmentResourceRole</span></span>](../api/accesspackageassignmentresourcerole-get.md) | [<span data-ttu-id="0744c-111">акцесспаккажеассигнментресаурцероле</span><span class="sxs-lookup"><span data-stu-id="0744c-111">accessPackageAssignmentResourceRole</span></span>](accesspackageassignmentresourcerole.md)  | <span data-ttu-id="0744c-112">Получение объекта Акцесспаккажеассигнментресаурцероле.</span><span class="sxs-lookup"><span data-stu-id="0744c-112">Retrieve an accessPackageAssignmentResourceRole object.</span></span> |
| [<span data-ttu-id="0744c-113">Список Акцесспаккажеассигнментресаурцеролес</span><span class="sxs-lookup"><span data-stu-id="0744c-113">List accessPackageAssignmentResourceRoles</span></span>](../api/accesspackageassignmentresourcerole-list.md) | <span data-ttu-id="0744c-114">Коллекция [акцесспаккажеассигнментресаурцероле](accesspackageassignmentresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="0744c-114">[accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) collection</span></span> | <span data-ttu-id="0744c-115">Получение списка объектов Акцесспаккажеассигнментресаурцероле.</span><span class="sxs-lookup"><span data-stu-id="0744c-115">Retrieve a list of accessPackageAssignmentResourceRole objects.</span></span> |

## <a name="properties"></a><span data-ttu-id="0744c-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="0744c-116">Properties</span></span>

| <span data-ttu-id="0744c-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="0744c-117">Property</span></span>     | <span data-ttu-id="0744c-118">Тип</span><span class="sxs-lookup"><span data-stu-id="0744c-118">Type</span></span>        | <span data-ttu-id="0744c-119">Описание</span><span class="sxs-lookup"><span data-stu-id="0744c-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0744c-120">id</span><span class="sxs-lookup"><span data-stu-id="0744c-120">id</span></span>|<span data-ttu-id="0744c-121">String</span><span class="sxs-lookup"><span data-stu-id="0744c-121">String</span></span>| <span data-ttu-id="0744c-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0744c-122">Read-only.</span></span>|
|<span data-ttu-id="0744c-123">оригинид</span><span class="sxs-lookup"><span data-stu-id="0744c-123">originId</span></span>|<span data-ttu-id="0744c-124">Строка</span><span class="sxs-lookup"><span data-stu-id="0744c-124">String</span></span>|<span data-ttu-id="0744c-125">Уникальный идентификатор, относящийся к исходной системе, соответствующий свойству Оригинид объекта [акцесспаккажересаурцероле](accesspackageresourcerole.md).</span><span class="sxs-lookup"><span data-stu-id="0744c-125">A unique identifier relative to the origin system, corresponding to the originId property of the [accessPackageResourceRole](accesspackageresourcerole.md).</span></span> |
|<span data-ttu-id="0744c-126">оригинсистем</span><span class="sxs-lookup"><span data-stu-id="0744c-126">originSystem</span></span>|<span data-ttu-id="0744c-127">Строка</span><span class="sxs-lookup"><span data-stu-id="0744c-127">String</span></span>|<span data-ttu-id="0744c-128">Система, в которой необходимо создать назначение роли или она была создана для назначения пакета Access, например `SharePointOnline` , `AadGroup` или `AadApplication` соответствующего свойству оригинсистем объекта [акцесспаккажересаурцероле](accesspackageresourcerole.md).</span><span class="sxs-lookup"><span data-stu-id="0744c-128">The system where the role assignment is to be created or has been created for an access package assignment, such as `SharePointOnline`, `AadGroup` or `AadApplication`, corresponding to the originSystem property of the [accessPackageResourceRole](accesspackageresourcerole.md).</span></span>|
|<span data-ttu-id="0744c-129">status</span><span class="sxs-lookup"><span data-stu-id="0744c-129">status</span></span>|<span data-ttu-id="0744c-130">String</span><span class="sxs-lookup"><span data-stu-id="0744c-130">String</span></span>|<span data-ttu-id="0744c-131">Это значение используется, `PendingFulfillment` когда назначение пакета Access еще не было доставлено в исходную систему, и `Fulfilled` когда назначение пакета Access было доставлено в исходную систему.</span><span class="sxs-lookup"><span data-stu-id="0744c-131">The value is `PendingFulfillment` when the access package assignment has not yet been delivered to the origin system, and `Fulfilled` when the access package assignment has been delivered to the origin system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0744c-132">Связи</span><span class="sxs-lookup"><span data-stu-id="0744c-132">Relationships</span></span>

| <span data-ttu-id="0744c-133">Связь</span><span class="sxs-lookup"><span data-stu-id="0744c-133">Relationship</span></span> | <span data-ttu-id="0744c-134">Тип</span><span class="sxs-lookup"><span data-stu-id="0744c-134">Type</span></span>        | <span data-ttu-id="0744c-135">Описание</span><span class="sxs-lookup"><span data-stu-id="0744c-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0744c-136">акцесспаккажеассигнментс</span><span class="sxs-lookup"><span data-stu-id="0744c-136">accessPackageAssignments</span></span>|<span data-ttu-id="0744c-137">Коллекция [акцесспаккажеассигнмент](accesspackageassignment.md)</span><span class="sxs-lookup"><span data-stu-id="0744c-137">[accessPackageAssignment](accesspackageassignment.md) collection</span></span>| <span data-ttu-id="0744c-138">Назначения для пакетов Access, которые применяют это назначение роли.</span><span class="sxs-lookup"><span data-stu-id="0744c-138">The access package assignments resulting in this role assignment.</span></span> <span data-ttu-id="0744c-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0744c-139">Read-only.</span></span> <span data-ttu-id="0744c-140">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="0744c-140">Nullable.</span></span>|
|<span data-ttu-id="0744c-141">акцесспаккажересаурцероле</span><span class="sxs-lookup"><span data-stu-id="0744c-141">accessPackageResourceRole</span></span>|[<span data-ttu-id="0744c-142">акцесспаккажересаурцероле</span><span class="sxs-lookup"><span data-stu-id="0744c-142">accessPackageResourceRole</span></span>](accesspackageresourcerole.md)| <span data-ttu-id="0744c-143">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0744c-143">Read-only.</span></span> <span data-ttu-id="0744c-144">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="0744c-144">Nullable.</span></span>|
|<span data-ttu-id="0744c-145">акцесспаккажересаурцескопе</span><span class="sxs-lookup"><span data-stu-id="0744c-145">accessPackageResourceScope</span></span>|[<span data-ttu-id="0744c-146">акцесспаккажересаурцескопе</span><span class="sxs-lookup"><span data-stu-id="0744c-146">accessPackageResourceScope</span></span>](accesspackageresourcescope.md)| <span data-ttu-id="0744c-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0744c-147">Read-only.</span></span> <span data-ttu-id="0744c-148">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="0744c-148">Nullable.</span></span>|
|<span data-ttu-id="0744c-149">акцесспаккажесубжект</span><span class="sxs-lookup"><span data-stu-id="0744c-149">accessPackageSubject</span></span>|[<span data-ttu-id="0744c-150">акцесспаккажесубжект</span><span class="sxs-lookup"><span data-stu-id="0744c-150">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="0744c-p104">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="0744c-p104">Read-only. Nullable.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="0744c-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0744c-153">JSON representation</span></span>

<span data-ttu-id="0744c-154">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0744c-154">The following is a JSON representation of the resource.</span></span>

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


