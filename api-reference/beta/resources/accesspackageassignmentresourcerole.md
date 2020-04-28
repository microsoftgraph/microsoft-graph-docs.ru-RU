---
title: Тип ресурса Акцесспаккажеассигнментресаурцероле
description: Роль ресурса назначения пакета Access указывает на роль, связанную с определенным ресурсом, которой назначена тема с помощью назначения пакета Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c9eddff042af5b2cd724e87e3438f398e8d68c19
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508543"
---
# <a name="accesspackageassignmentresourcerole-resource-type"></a><span data-ttu-id="5eaf7-103">Тип ресурса Акцесспаккажеассигнментресаурцероле</span><span class="sxs-lookup"><span data-stu-id="5eaf7-103">accessPackageAssignmentResourceRole resource type</span></span>

<span data-ttu-id="5eaf7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5eaf7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5eaf7-105">В разделе [Управление обслуживанием в Azure AD](entitlementmanagement-root.md)роль ресурса назначения пакета Access указывает роль, связанную с определенным ресурсом, которой назначена тема с помощью назначения пакета Access.</span><span class="sxs-lookup"><span data-stu-id="5eaf7-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment resource role indicates the resource-specific role which a subject has been assigned through an access package assignment.</span></span>

## <a name="methods"></a><span data-ttu-id="5eaf7-106">Методы</span><span class="sxs-lookup"><span data-stu-id="5eaf7-106">Methods</span></span>

| <span data-ttu-id="5eaf7-107">Метод</span><span class="sxs-lookup"><span data-stu-id="5eaf7-107">Method</span></span>       | <span data-ttu-id="5eaf7-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5eaf7-108">Return Type</span></span> | <span data-ttu-id="5eaf7-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5eaf7-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="5eaf7-110">Список Акцесспаккажеассигнментресаурцеролес</span><span class="sxs-lookup"><span data-stu-id="5eaf7-110">List accessPackageAssignmentResourceRoles</span></span>](../api/accesspackageassignmentresourcerole-list.md) | <span data-ttu-id="5eaf7-111">Коллекция [акцесспаккажеассигнментресаурцероле](accesspackageassignmentresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="5eaf7-111">[accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) collection</span></span> | <span data-ttu-id="5eaf7-112">Получение списка объектов Акцесспаккажеассигнментресаурцероле.</span><span class="sxs-lookup"><span data-stu-id="5eaf7-112">Retrieve a list of accessPackageAssignmentResourceRole objects.</span></span> |

## <a name="properties"></a><span data-ttu-id="5eaf7-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="5eaf7-113">Properties</span></span>

| <span data-ttu-id="5eaf7-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="5eaf7-114">Property</span></span>     | <span data-ttu-id="5eaf7-115">Тип</span><span class="sxs-lookup"><span data-stu-id="5eaf7-115">Type</span></span>        | <span data-ttu-id="5eaf7-116">Описание</span><span class="sxs-lookup"><span data-stu-id="5eaf7-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5eaf7-117">id</span><span class="sxs-lookup"><span data-stu-id="5eaf7-117">id</span></span>|<span data-ttu-id="5eaf7-118">String</span><span class="sxs-lookup"><span data-stu-id="5eaf7-118">String</span></span>| <span data-ttu-id="5eaf7-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5eaf7-119">Read-only.</span></span>|
|<span data-ttu-id="5eaf7-120">оригинид</span><span class="sxs-lookup"><span data-stu-id="5eaf7-120">originId</span></span>|<span data-ttu-id="5eaf7-121">String</span><span class="sxs-lookup"><span data-stu-id="5eaf7-121">String</span></span>|<span data-ttu-id="5eaf7-122">Уникальный идентификатор, связанный с исходной системой.</span><span class="sxs-lookup"><span data-stu-id="5eaf7-122">A unique identifier relative to the origin system.</span></span> |
|<span data-ttu-id="5eaf7-123">оригинсистем</span><span class="sxs-lookup"><span data-stu-id="5eaf7-123">originSystem</span></span>|<span data-ttu-id="5eaf7-124">String</span><span class="sxs-lookup"><span data-stu-id="5eaf7-124">String</span></span>|<span data-ttu-id="5eaf7-125">Система, в которой необходимо создать назначение ролей для назначения пакета Access.</span><span class="sxs-lookup"><span data-stu-id="5eaf7-125">The system where the role assignment is to be created for an access package assignment.</span></span>|
|<span data-ttu-id="5eaf7-126">status</span><span class="sxs-lookup"><span data-stu-id="5eaf7-126">status</span></span>|<span data-ttu-id="5eaf7-127">String</span><span class="sxs-lookup"><span data-stu-id="5eaf7-127">String</span></span>|<span data-ttu-id="5eaf7-128">Значение задается, `Fulfilled` когда назначение пакета Access было доставлено в исходную систему.</span><span class="sxs-lookup"><span data-stu-id="5eaf7-128">The value is `Fulfilled` when the access package assignment has been delivered to the origin system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5eaf7-129">Связи</span><span class="sxs-lookup"><span data-stu-id="5eaf7-129">Relationships</span></span>

| <span data-ttu-id="5eaf7-130">Связь</span><span class="sxs-lookup"><span data-stu-id="5eaf7-130">Relationship</span></span> | <span data-ttu-id="5eaf7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5eaf7-131">Type</span></span>        | <span data-ttu-id="5eaf7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5eaf7-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5eaf7-133">акцесспаккажеассигнментс</span><span class="sxs-lookup"><span data-stu-id="5eaf7-133">accessPackageAssignments</span></span>|<span data-ttu-id="5eaf7-134">Коллекция [акцесспаккажеассигнмент](accesspackageassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5eaf7-134">[accessPackageAssignment](accesspackageassignment.md) collection</span></span>| <span data-ttu-id="5eaf7-135">Назначения для пакетов Access, которые применяют это назначение роли.</span><span class="sxs-lookup"><span data-stu-id="5eaf7-135">The access package assignments resulting in this role assignment.</span></span> <span data-ttu-id="5eaf7-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5eaf7-136">Read-only.</span></span> <span data-ttu-id="5eaf7-137">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="5eaf7-137">Nullable.</span></span>|
|<span data-ttu-id="5eaf7-138">акцесспаккажересаурцероле</span><span class="sxs-lookup"><span data-stu-id="5eaf7-138">accessPackageResourceRole</span></span>|[<span data-ttu-id="5eaf7-139">акцесспаккажересаурцероле</span><span class="sxs-lookup"><span data-stu-id="5eaf7-139">accessPackageResourceRole</span></span>](accesspackageresourcerole.md)| <span data-ttu-id="5eaf7-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5eaf7-140">Read-only.</span></span> <span data-ttu-id="5eaf7-141">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="5eaf7-141">Nullable.</span></span>|
|<span data-ttu-id="5eaf7-142">акцесспаккажересаурцескопе</span><span class="sxs-lookup"><span data-stu-id="5eaf7-142">accessPackageResourceScope</span></span>|[<span data-ttu-id="5eaf7-143">акцесспаккажересаурцескопе</span><span class="sxs-lookup"><span data-stu-id="5eaf7-143">accessPackageResourceScope</span></span>](accesspackageresourcescope.md)| <span data-ttu-id="5eaf7-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5eaf7-144">Read-only.</span></span> <span data-ttu-id="5eaf7-145">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="5eaf7-145">Nullable.</span></span>|
|<span data-ttu-id="5eaf7-146">акцесспаккажесубжект</span><span class="sxs-lookup"><span data-stu-id="5eaf7-146">accessPackageSubject</span></span>|[<span data-ttu-id="5eaf7-147">акцесспаккажесубжект</span><span class="sxs-lookup"><span data-stu-id="5eaf7-147">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="5eaf7-p104">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="5eaf7-p104">Read-only. Nullable.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="5eaf7-150">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5eaf7-150">JSON representation</span></span>

<span data-ttu-id="5eaf7-151">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5eaf7-151">The following is a JSON representation of the resource.</span></span>

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
