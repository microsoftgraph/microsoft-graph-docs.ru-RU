---
title: Тип ресурса Акцесспаккажеассигнментресаурцероле
description: Роль ресурса назначения пакета Access указывает на роль, связанную с определенным ресурсом, которой назначена тема с помощью назначения пакета Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1dbf73623ddd51cc1172e5610e84cc7861657489
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939196"
---
# <a name="accesspackageassignmentresourcerole-resource-type"></a><span data-ttu-id="50d17-103">Тип ресурса Акцесспаккажеассигнментресаурцероле</span><span class="sxs-lookup"><span data-stu-id="50d17-103">accessPackageAssignmentResourceRole resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50d17-104">В разделе [Управление обслуживанием в Azure AD](entitlementmanagement-root.md)роль ресурса назначения пакета Access указывает роль, связанную с определенным ресурсом, которой назначена тема с помощью назначения пакета Access.</span><span class="sxs-lookup"><span data-stu-id="50d17-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment resource role indicates the resource-specific role which a subject has been assigned through an access package assignment.</span></span>

## <a name="methods"></a><span data-ttu-id="50d17-105">Методы</span><span class="sxs-lookup"><span data-stu-id="50d17-105">Methods</span></span>

| <span data-ttu-id="50d17-106">Метод</span><span class="sxs-lookup"><span data-stu-id="50d17-106">Method</span></span>       | <span data-ttu-id="50d17-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="50d17-107">Return Type</span></span> | <span data-ttu-id="50d17-108">Описание</span><span class="sxs-lookup"><span data-stu-id="50d17-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="50d17-109">Список Акцесспаккажеассигнментресаурцеролес</span><span class="sxs-lookup"><span data-stu-id="50d17-109">List accessPackageAssignmentResourceRoles</span></span>](../api/accesspackageassignmentresourcerole-list.md) | <span data-ttu-id="50d17-110">Коллекция [акцесспаккажеассигнментресаурцероле](accesspackageassignmentresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="50d17-110">[accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) collection</span></span> | <span data-ttu-id="50d17-111">Получение списка объектов Акцесспаккажеассигнментресаурцероле.</span><span class="sxs-lookup"><span data-stu-id="50d17-111">Retrieve a list of accessPackageAssignmentResourceRole objects.</span></span> |

## <a name="properties"></a><span data-ttu-id="50d17-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="50d17-112">Properties</span></span>

| <span data-ttu-id="50d17-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="50d17-113">Property</span></span>     | <span data-ttu-id="50d17-114">Тип</span><span class="sxs-lookup"><span data-stu-id="50d17-114">Type</span></span>        | <span data-ttu-id="50d17-115">Описание</span><span class="sxs-lookup"><span data-stu-id="50d17-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="50d17-116">id</span><span class="sxs-lookup"><span data-stu-id="50d17-116">id</span></span>|<span data-ttu-id="50d17-117">Строка</span><span class="sxs-lookup"><span data-stu-id="50d17-117">String</span></span>| <span data-ttu-id="50d17-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="50d17-118">Read-only.</span></span>|
|<span data-ttu-id="50d17-119">оригинид</span><span class="sxs-lookup"><span data-stu-id="50d17-119">originId</span></span>|<span data-ttu-id="50d17-120">Строка</span><span class="sxs-lookup"><span data-stu-id="50d17-120">String</span></span>|<span data-ttu-id="50d17-121">Уникальный идентификатор, связанный с исходной системой.</span><span class="sxs-lookup"><span data-stu-id="50d17-121">A unique identifier relative to the origin system.</span></span> |
|<span data-ttu-id="50d17-122">оригинсистем</span><span class="sxs-lookup"><span data-stu-id="50d17-122">originSystem</span></span>|<span data-ttu-id="50d17-123">Строка</span><span class="sxs-lookup"><span data-stu-id="50d17-123">String</span></span>|<span data-ttu-id="50d17-124">Система, в которой необходимо создать назначение ролей для назначения пакета Access.</span><span class="sxs-lookup"><span data-stu-id="50d17-124">The system where the role assignment is to be created for an access package assignment.</span></span>|
|<span data-ttu-id="50d17-125">status</span><span class="sxs-lookup"><span data-stu-id="50d17-125">status</span></span>|<span data-ttu-id="50d17-126">String</span><span class="sxs-lookup"><span data-stu-id="50d17-126">String</span></span>|<span data-ttu-id="50d17-127">Значение задается, `Fulfilled` когда назначение пакета Access было доставлено в исходную систему.</span><span class="sxs-lookup"><span data-stu-id="50d17-127">The value is `Fulfilled` when the access package assignment has been delivered to the origin system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="50d17-128">Связи</span><span class="sxs-lookup"><span data-stu-id="50d17-128">Relationships</span></span>

| <span data-ttu-id="50d17-129">Связь</span><span class="sxs-lookup"><span data-stu-id="50d17-129">Relationship</span></span> | <span data-ttu-id="50d17-130">Тип</span><span class="sxs-lookup"><span data-stu-id="50d17-130">Type</span></span>        | <span data-ttu-id="50d17-131">Описание</span><span class="sxs-lookup"><span data-stu-id="50d17-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="50d17-132">акцесспаккажеассигнментс</span><span class="sxs-lookup"><span data-stu-id="50d17-132">accessPackageAssignments</span></span>|<span data-ttu-id="50d17-133">Коллекция [акцесспаккажеассигнмент](accesspackageassignment.md)</span><span class="sxs-lookup"><span data-stu-id="50d17-133">[accessPackageAssignment](accesspackageassignment.md) collection</span></span>| <span data-ttu-id="50d17-134">Назначения для пакетов Access, которые применяют это назначение роли.</span><span class="sxs-lookup"><span data-stu-id="50d17-134">The access package assignments resulting in this role assignment.</span></span> <span data-ttu-id="50d17-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="50d17-135">Read-only.</span></span> <span data-ttu-id="50d17-136">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="50d17-136">Nullable.</span></span>|
|<span data-ttu-id="50d17-137">акцесспаккажересаурцероле</span><span class="sxs-lookup"><span data-stu-id="50d17-137">accessPackageResourceRole</span></span>|[<span data-ttu-id="50d17-138">акцесспаккажересаурцероле</span><span class="sxs-lookup"><span data-stu-id="50d17-138">accessPackageResourceRole</span></span>](accesspackageresourcerole.md)| <span data-ttu-id="50d17-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="50d17-139">Read-only.</span></span> <span data-ttu-id="50d17-140">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="50d17-140">Nullable.</span></span>|
|<span data-ttu-id="50d17-141">акцесспаккажересаурцескопе</span><span class="sxs-lookup"><span data-stu-id="50d17-141">accessPackageResourceScope</span></span>|[<span data-ttu-id="50d17-142">акцесспаккажересаурцескопе</span><span class="sxs-lookup"><span data-stu-id="50d17-142">accessPackageResourceScope</span></span>](accesspackageresourcescope.md)| <span data-ttu-id="50d17-143">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="50d17-143">Read-only.</span></span> <span data-ttu-id="50d17-144">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="50d17-144">Nullable.</span></span>|
|<span data-ttu-id="50d17-145">акцесспаккажесубжект</span><span class="sxs-lookup"><span data-stu-id="50d17-145">accessPackageSubject</span></span>|[<span data-ttu-id="50d17-146">акцесспаккажесубжект</span><span class="sxs-lookup"><span data-stu-id="50d17-146">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="50d17-p104">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="50d17-p104">Read-only. Nullable.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="50d17-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="50d17-149">JSON representation</span></span>

<span data-ttu-id="50d17-150">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="50d17-150">The following is a JSON representation of the resource.</span></span>

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
