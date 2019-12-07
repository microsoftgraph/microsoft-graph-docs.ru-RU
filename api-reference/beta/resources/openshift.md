---
title: Тип ресурса Опеншифт
description: Представляет неназначенный открытый сдвиг в расписании.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3eff83475c4a36ec1c294c62b9e1b87673926d8d
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895850"
---
# <a name="openshift-resource-type"></a><span data-ttu-id="68a0d-103">Тип ресурса Опеншифт</span><span class="sxs-lookup"><span data-stu-id="68a0d-103">openShift resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68a0d-104">Представляет Неназначенное, Открытый сдвиг по [расписанию](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="68a0d-104">Represents an unassigned, open shift in a [schedule](../resources/schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="68a0d-105">Методы</span><span class="sxs-lookup"><span data-stu-id="68a0d-105">Methods</span></span>

| <span data-ttu-id="68a0d-106">Метод</span><span class="sxs-lookup"><span data-stu-id="68a0d-106">Method</span></span>       | <span data-ttu-id="68a0d-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="68a0d-107">Return Type</span></span> | <span data-ttu-id="68a0d-108">Описание</span><span class="sxs-lookup"><span data-stu-id="68a0d-108">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="68a0d-109">[получение](../api/openshift-get.md);</span><span class="sxs-lookup"><span data-stu-id="68a0d-109">[Get](../api/openshift-get.md)</span></span> | [<span data-ttu-id="68a0d-110">опеншифт</span><span class="sxs-lookup"><span data-stu-id="68a0d-110">openShift</span></span>](openshift.md) | <span data-ttu-id="68a0d-111">Чтение свойств и связей объекта Опеншифт.</span><span class="sxs-lookup"><span data-stu-id="68a0d-111">Read properties and relationships of openShift object.</span></span> |
| <span data-ttu-id="68a0d-112">[обновление](../api/openshift-update.md).</span><span class="sxs-lookup"><span data-stu-id="68a0d-112">[Update](../api/openshift-update.md)</span></span> | [<span data-ttu-id="68a0d-113">опеншифт</span><span class="sxs-lookup"><span data-stu-id="68a0d-113">openShift</span></span>](openshift.md) | <span data-ttu-id="68a0d-114">Обновление объекта Опеншифт.</span><span class="sxs-lookup"><span data-stu-id="68a0d-114">Update openShift object.</span></span> |
| <span data-ttu-id="68a0d-115">[удаление](../api/openshift-delete.md);</span><span class="sxs-lookup"><span data-stu-id="68a0d-115">[Delete](../api/openshift-delete.md)</span></span> | <span data-ttu-id="68a0d-116">Нет</span><span class="sxs-lookup"><span data-stu-id="68a0d-116">None</span></span> | <span data-ttu-id="68a0d-117">Удаление объекта Опеншифт.</span><span class="sxs-lookup"><span data-stu-id="68a0d-117">Delete openShift object.</span></span> |

## <a name="properties"></a><span data-ttu-id="68a0d-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="68a0d-118">Properties</span></span>

| <span data-ttu-id="68a0d-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="68a0d-119">Property</span></span>     | <span data-ttu-id="68a0d-120">Тип</span><span class="sxs-lookup"><span data-stu-id="68a0d-120">Type</span></span>        | <span data-ttu-id="68a0d-121">Описание</span><span class="sxs-lookup"><span data-stu-id="68a0d-121">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="68a0d-122">драфтопеншифт</span><span class="sxs-lookup"><span data-stu-id="68a0d-122">draftOpenShift</span></span>|[<span data-ttu-id="68a0d-123">опеншифтитем</span><span class="sxs-lookup"><span data-stu-id="68a0d-123">openShiftItem</span></span>](openshiftitem.md)|<span data-ttu-id="68a0d-124">Неопубликованная открытая смена.</span><span class="sxs-lookup"><span data-stu-id="68a0d-124">An unpublished open shift.</span></span>|
|<span data-ttu-id="68a0d-125">schedulingGroupId</span><span class="sxs-lookup"><span data-stu-id="68a0d-125">schedulingGroupId</span></span>|<span data-ttu-id="68a0d-126">String</span><span class="sxs-lookup"><span data-stu-id="68a0d-126">String</span></span>|<span data-ttu-id="68a0d-127">Идентификатор группы планирования, к которой относится открытая смена.</span><span class="sxs-lookup"><span data-stu-id="68a0d-127">ID for the scheduling group that the open shift belongs to.</span></span>|
|<span data-ttu-id="68a0d-128">шаредопеншифт</span><span class="sxs-lookup"><span data-stu-id="68a0d-128">sharedOpenShift</span></span>|[<span data-ttu-id="68a0d-129">опеншифтитем</span><span class="sxs-lookup"><span data-stu-id="68a0d-129">openShiftItem</span></span>](openshiftitem.md)|<span data-ttu-id="68a0d-130">Опубликованная открытая смена.</span><span class="sxs-lookup"><span data-stu-id="68a0d-130">A published open shift.</span></span>|

## <a name="relationships"></a><span data-ttu-id="68a0d-131">Связи</span><span class="sxs-lookup"><span data-stu-id="68a0d-131">Relationships</span></span>

<span data-ttu-id="68a0d-132">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="68a0d-132">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="68a0d-133">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="68a0d-133">JSON representation</span></span>

<span data-ttu-id="68a0d-134">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="68a0d-134">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.openShift",
  "baseType": ""
}-->

```json
{
  "draftOpenShift": {"@odata.type": "microsoft.graph.openShiftItem"},
  "schedulingGroupId": "String",
  "sharedOpenShift": {"@odata.type": "microsoft.graph.openShiftItem"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "openShift resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
