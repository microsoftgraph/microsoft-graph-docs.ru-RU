---
title: Тип ресурса Принтусажесуммарибюсер
description: Описывает действия печати для пользователя в указанный период времени (Усажедате).
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 30769d9bd7ee76494b1582a3d7afc8a7f75bb07a
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895984"
---
# <a name="printusagesummarybyuser-resource-type"></a><span data-ttu-id="d4ffd-103">Тип ресурса Принтусажесуммарибюсер</span><span class="sxs-lookup"><span data-stu-id="d4ffd-103">printUsageSummaryByUser resource type</span></span>

<span data-ttu-id="d4ffd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4ffd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4ffd-105">Описывает действия печати для пользователя в указанный период времени (Усажедате).</span><span class="sxs-lookup"><span data-stu-id="d4ffd-105">Describes print activity for a user during a specified time period (usageDate).</span></span>

## <a name="methods"></a><span data-ttu-id="d4ffd-106">Методы</span><span class="sxs-lookup"><span data-stu-id="d4ffd-106">Methods</span></span>

| <span data-ttu-id="d4ffd-107">Метод</span><span class="sxs-lookup"><span data-stu-id="d4ffd-107">Method</span></span>       | <span data-ttu-id="d4ffd-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d4ffd-108">Return Type</span></span> | <span data-ttu-id="d4ffd-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d4ffd-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="d4ffd-110">Список (ежедневно)</span><span class="sxs-lookup"><span data-stu-id="d4ffd-110">List (daily)</span></span>](../api/reportroot-list-dailyprintusagesummariesbyuser.md) | [<span data-ttu-id="d4ffd-111">принтусажесуммарибюсер</span><span class="sxs-lookup"><span data-stu-id="d4ffd-111">printUsageSummaryByUser</span></span>](printusagesummarybyuser.md) | <span data-ttu-id="d4ffd-112">Получение списка сводных сведений об использовании печати, сгруппированных по пользователям.</span><span class="sxs-lookup"><span data-stu-id="d4ffd-112">Get a list of daily print usage summaries, grouped by user.</span></span> |
| [<span data-ttu-id="d4ffd-113">Список (ежемесячно)</span><span class="sxs-lookup"><span data-stu-id="d4ffd-113">List (monthly)</span></span>](../api/reportroot-list-monthlyprintusagesummariesbyuser.md) | [<span data-ttu-id="d4ffd-114">принтусажесуммарибюсер</span><span class="sxs-lookup"><span data-stu-id="d4ffd-114">printUsageSummaryByUser</span></span>](printusagesummarybyuser.md) | <span data-ttu-id="d4ffd-115">Получение списка ежемесячных сводок использования печати, сгруппированных по пользователям.</span><span class="sxs-lookup"><span data-stu-id="d4ffd-115">Get a list of monthly print usage summaries, grouped by user.</span></span> |
| <span data-ttu-id="d4ffd-116">[получение](../api/printusagesummarybyuser-get.md);</span><span class="sxs-lookup"><span data-stu-id="d4ffd-116">[Get](../api/printusagesummarybyuser-get.md)</span></span> | [<span data-ttu-id="d4ffd-117">принтусажесуммарибюсер</span><span class="sxs-lookup"><span data-stu-id="d4ffd-117">printUsageSummaryByUser</span></span>](printusagesummarybyuser.md) | <span data-ttu-id="d4ffd-118">Чтение свойств и связей объекта Принтусажесуммарибюсер.</span><span class="sxs-lookup"><span data-stu-id="d4ffd-118">Read properties and relationships of a printUsageSummaryByUser object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d4ffd-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="d4ffd-119">Properties</span></span>
| <span data-ttu-id="d4ffd-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="d4ffd-120">Property</span></span>     | <span data-ttu-id="d4ffd-121">Тип</span><span class="sxs-lookup"><span data-stu-id="d4ffd-121">Type</span></span>        | <span data-ttu-id="d4ffd-122">Описание</span><span class="sxs-lookup"><span data-stu-id="d4ffd-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d4ffd-123">id</span><span class="sxs-lookup"><span data-stu-id="d4ffd-123">id</span></span>|<span data-ttu-id="d4ffd-124">Строка</span><span class="sxs-lookup"><span data-stu-id="d4ffd-124">String</span></span>|<span data-ttu-id="d4ffd-125">Идентификатор этой сводки использования.</span><span class="sxs-lookup"><span data-stu-id="d4ffd-125">The ID of this usage summary.</span></span>|
|<span data-ttu-id="d4ffd-126">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d4ffd-126">userPrincipalName</span></span>|<span data-ttu-id="d4ffd-127">String</span><span class="sxs-lookup"><span data-stu-id="d4ffd-127">String</span></span>|<span data-ttu-id="d4ffd-128">Имя участника-пользователя, представленное этой статистикой.</span><span class="sxs-lookup"><span data-stu-id="d4ffd-128">The UPN of the user represented by these statistics.</span></span>|
|<span data-ttu-id="d4ffd-129">усажедате</span><span class="sxs-lookup"><span data-stu-id="d4ffd-129">usageDate</span></span>|<span data-ttu-id="d4ffd-130">Дата</span><span class="sxs-lookup"><span data-stu-id="d4ffd-130">Date</span></span>|<span data-ttu-id="d4ffd-131">Дата, связанная с этими статистикой.</span><span class="sxs-lookup"><span data-stu-id="d4ffd-131">The date associated with these statistics.</span></span>|
|<span data-ttu-id="d4ffd-132">комплетедблаккандвхитежобкаунт</span><span class="sxs-lookup"><span data-stu-id="d4ffd-132">completedBlackAndWhiteJobCount</span></span>|<span data-ttu-id="d4ffd-133">Int64</span><span class="sxs-lookup"><span data-stu-id="d4ffd-133">Int64</span></span>|<span data-ttu-id="d4ffd-134">Количество черно-белых заданий печати, выполненных от имени пользователя на соответствующую дату.</span><span class="sxs-lookup"><span data-stu-id="d4ffd-134">The number of black and white print jobs completed on behalf of the user on the associated date.</span></span>|
|<span data-ttu-id="d4ffd-135">комплетедколоржобкаунт</span><span class="sxs-lookup"><span data-stu-id="d4ffd-135">completedColorJobCount</span></span>|<span data-ttu-id="d4ffd-136">Int64</span><span class="sxs-lookup"><span data-stu-id="d4ffd-136">Int64</span></span>|<span data-ttu-id="d4ffd-137">Число заданий цветной печати, выполненных от имени пользователя на соответствующую дату.</span><span class="sxs-lookup"><span data-stu-id="d4ffd-137">The number of color print jobs completed on behalf of the user on the associated date.</span></span>|
|<span data-ttu-id="d4ffd-138">инкомплетежобкаунт</span><span class="sxs-lookup"><span data-stu-id="d4ffd-138">incompleteJobCount</span></span>|<span data-ttu-id="d4ffd-139">Int64</span><span class="sxs-lookup"><span data-stu-id="d4ffd-139">Int64</span></span>|<span data-ttu-id="d4ffd-140">Количество заданий печати, которые были поставлены в очередь от имени пользователя, но не завершены, на соответствующую дату.</span><span class="sxs-lookup"><span data-stu-id="d4ffd-140">The number of print jobs that were queued on behalf of the user, but not completed, on the associated date.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d4ffd-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d4ffd-141">JSON representation</span></span>

<span data-ttu-id="d4ffd-142">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d4ffd-142">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printUsageSummaryByUser"
}-->

```json
{
    "id": "String (identifier)",
    "userPrincipalName": "String (identifier)",
    "usageDate": "String (timestamp)",
    "completedBlackAndWhiteJobCount": 123456,
    "completedColorJobCount": 123456,
    "incompleteJobCount": 123456
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printUsageSummaryByUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->