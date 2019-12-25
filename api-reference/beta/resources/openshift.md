---
title: Тип ресурса Опеншифт
description: Представляет неназначенный открытый сдвиг в расписании.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: fa87acd2065a3a56f15016bb7708e73cebe63a31
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870161"
---
# <a name="openshift-resource-type"></a><span data-ttu-id="ace2b-103">Тип ресурса Опеншифт</span><span class="sxs-lookup"><span data-stu-id="ace2b-103">openShift resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ace2b-104">Представляет Неназначенное, Открытый сдвиг по [расписанию](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="ace2b-104">Represents an unassigned, open shift in a [schedule](../resources/schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="ace2b-105">Методы</span><span class="sxs-lookup"><span data-stu-id="ace2b-105">Methods</span></span>

| <span data-ttu-id="ace2b-106">Метод</span><span class="sxs-lookup"><span data-stu-id="ace2b-106">Method</span></span>       | <span data-ttu-id="ace2b-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ace2b-107">Return Type</span></span> | <span data-ttu-id="ace2b-108">Описание</span><span class="sxs-lookup"><span data-stu-id="ace2b-108">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="ace2b-109">[получение](../api/openshift-get.md);</span><span class="sxs-lookup"><span data-stu-id="ace2b-109">[Get](../api/openshift-get.md)</span></span> | [<span data-ttu-id="ace2b-110">опеншифт</span><span class="sxs-lookup"><span data-stu-id="ace2b-110">openShift</span></span>](openshift.md) | <span data-ttu-id="ace2b-111">Чтение свойств и связей объекта **опеншифт** .</span><span class="sxs-lookup"><span data-stu-id="ace2b-111">Read the properties and relationships of an **openShift** object.</span></span> |
| <span data-ttu-id="ace2b-112">[обновление](../api/openshift-update.md).</span><span class="sxs-lookup"><span data-stu-id="ace2b-112">[Update](../api/openshift-update.md)</span></span> | [<span data-ttu-id="ace2b-113">опеншифт</span><span class="sxs-lookup"><span data-stu-id="ace2b-113">openShift</span></span>](openshift.md) | <span data-ttu-id="ace2b-114">Обновление объекта **опеншифт** .</span><span class="sxs-lookup"><span data-stu-id="ace2b-114">Update an **openShift** object.</span></span> |
| <span data-ttu-id="ace2b-115">[удаление](../api/openshift-delete.md);</span><span class="sxs-lookup"><span data-stu-id="ace2b-115">[Delete](../api/openshift-delete.md)</span></span> | <span data-ttu-id="ace2b-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="ace2b-116">None</span></span> | <span data-ttu-id="ace2b-117">Удаление объекта **опеншифт** .</span><span class="sxs-lookup"><span data-stu-id="ace2b-117">Delete an **openShift** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ace2b-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="ace2b-118">Properties</span></span>

| <span data-ttu-id="ace2b-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="ace2b-119">Property</span></span>     | <span data-ttu-id="ace2b-120">Тип</span><span class="sxs-lookup"><span data-stu-id="ace2b-120">Type</span></span>        | <span data-ttu-id="ace2b-121">Описание</span><span class="sxs-lookup"><span data-stu-id="ace2b-121">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ace2b-122">драфтопеншифт</span><span class="sxs-lookup"><span data-stu-id="ace2b-122">draftOpenShift</span></span>|[<span data-ttu-id="ace2b-123">опеншифтитем</span><span class="sxs-lookup"><span data-stu-id="ace2b-123">openShiftItem</span></span>](openshiftitem.md)|<span data-ttu-id="ace2b-124">Неопубликованная открытая смена.</span><span class="sxs-lookup"><span data-stu-id="ace2b-124">An unpublished open shift.</span></span>|
|<span data-ttu-id="ace2b-125">schedulingGroupId</span><span class="sxs-lookup"><span data-stu-id="ace2b-125">schedulingGroupId</span></span>|<span data-ttu-id="ace2b-126">String</span><span class="sxs-lookup"><span data-stu-id="ace2b-126">String</span></span>|<span data-ttu-id="ace2b-127">Идентификатор группы планирования, к которой относится открытая смена.</span><span class="sxs-lookup"><span data-stu-id="ace2b-127">ID for the scheduling group that the open shift belongs to.</span></span>|
|<span data-ttu-id="ace2b-128">шаредопеншифт</span><span class="sxs-lookup"><span data-stu-id="ace2b-128">sharedOpenShift</span></span>|[<span data-ttu-id="ace2b-129">опеншифтитем</span><span class="sxs-lookup"><span data-stu-id="ace2b-129">openShiftItem</span></span>](openshiftitem.md)|<span data-ttu-id="ace2b-130">Опубликованная открытая смена.</span><span class="sxs-lookup"><span data-stu-id="ace2b-130">A published open shift.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ace2b-131">Отношения</span><span class="sxs-lookup"><span data-stu-id="ace2b-131">Relationships</span></span>

<span data-ttu-id="ace2b-132">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ace2b-132">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ace2b-133">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="ace2b-133">JSON representation</span></span>

<span data-ttu-id="ace2b-134">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ace2b-134">The following is a JSON representation of the resource.</span></span>

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
