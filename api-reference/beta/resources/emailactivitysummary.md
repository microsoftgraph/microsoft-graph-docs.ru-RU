---
title: Тип ресурса emailActivitySummary
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: 82fbdc2621b9c8746ed3028fe44414edeb7e56db
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871346"
---
# <a name="emailactivitysummary-resource-type"></a><span data-ttu-id="be6d6-103">Тип ресурса emailActivitySummary</span><span class="sxs-lookup"><span data-stu-id="be6d6-103">emailActivitySummary resource type</span></span>

## <a name="properties"></a><span data-ttu-id="be6d6-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="be6d6-104">Properties</span></span>

| <span data-ttu-id="be6d6-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="be6d6-105">Property</span></span>          | <span data-ttu-id="be6d6-106">Тип</span><span class="sxs-lookup"><span data-stu-id="be6d6-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="be6d6-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="be6d6-107">reportRefreshDate</span></span> | <span data-ttu-id="be6d6-108">Date</span><span class="sxs-lookup"><span data-stu-id="be6d6-108">Date</span></span>   |
| <span data-ttu-id="be6d6-109">отправить</span><span class="sxs-lookup"><span data-stu-id="be6d6-109">send</span></span>              | <span data-ttu-id="be6d6-110">Int64</span><span class="sxs-lookup"><span data-stu-id="be6d6-110">Int64</span></span>  |
| <span data-ttu-id="be6d6-111">Получение</span><span class="sxs-lookup"><span data-stu-id="be6d6-111">receive</span></span>           | <span data-ttu-id="be6d6-112">Int64</span><span class="sxs-lookup"><span data-stu-id="be6d6-112">Int64</span></span>  |
| <span data-ttu-id="be6d6-113">чтение</span><span class="sxs-lookup"><span data-stu-id="be6d6-113">read</span></span>              | <span data-ttu-id="be6d6-114">Int64</span><span class="sxs-lookup"><span data-stu-id="be6d6-114">Int64</span></span>  |
| <span data-ttu-id="be6d6-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="be6d6-115">reportDate</span></span>        | <span data-ttu-id="be6d6-116">Date</span><span class="sxs-lookup"><span data-stu-id="be6d6-116">Date</span></span>   |
| <span data-ttu-id="be6d6-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="be6d6-117">reportPeriod</span></span>      | <span data-ttu-id="be6d6-118">String</span><span class="sxs-lookup"><span data-stu-id="be6d6-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="be6d6-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="be6d6-119">JSON representation</span></span>

<span data-ttu-id="be6d6-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="be6d6-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailActivitySummary"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "send": 1024, 
  "receive": 1024, 
  "read": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
