---
title: Тип ресурса Емаилактивитисуммари
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 6a8b6fd714b506404e7788a067fc655197f22ccc
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43440578"
---
# <a name="emailactivitysummary-resource-type"></a><span data-ttu-id="88dc3-103">Тип ресурса Емаилактивитисуммари</span><span class="sxs-lookup"><span data-stu-id="88dc3-103">emailActivitySummary resource type</span></span>

<span data-ttu-id="88dc3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88dc3-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="88dc3-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="88dc3-105">Properties</span></span>

| <span data-ttu-id="88dc3-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="88dc3-106">Property</span></span>          | <span data-ttu-id="88dc3-107">Тип</span><span class="sxs-lookup"><span data-stu-id="88dc3-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="88dc3-108">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="88dc3-108">reportRefreshDate</span></span> | <span data-ttu-id="88dc3-109">Дата</span><span class="sxs-lookup"><span data-stu-id="88dc3-109">Date</span></span>   |
| <span data-ttu-id="88dc3-110">send</span><span class="sxs-lookup"><span data-stu-id="88dc3-110">send</span></span>              | <span data-ttu-id="88dc3-111">Int64</span><span class="sxs-lookup"><span data-stu-id="88dc3-111">Int64</span></span>  |
| <span data-ttu-id="88dc3-112">получил</span><span class="sxs-lookup"><span data-stu-id="88dc3-112">receive</span></span>           | <span data-ttu-id="88dc3-113">Int64</span><span class="sxs-lookup"><span data-stu-id="88dc3-113">Int64</span></span>  |
| <span data-ttu-id="88dc3-114">прочитан</span><span class="sxs-lookup"><span data-stu-id="88dc3-114">read</span></span>              | <span data-ttu-id="88dc3-115">Int64</span><span class="sxs-lookup"><span data-stu-id="88dc3-115">Int64</span></span>  |
| <span data-ttu-id="88dc3-116">reportDate</span><span class="sxs-lookup"><span data-stu-id="88dc3-116">reportDate</span></span>        | <span data-ttu-id="88dc3-117">Дата</span><span class="sxs-lookup"><span data-stu-id="88dc3-117">Date</span></span>   |
| <span data-ttu-id="88dc3-118">репортпериод</span><span class="sxs-lookup"><span data-stu-id="88dc3-118">reportPeriod</span></span>      | <span data-ttu-id="88dc3-119">String</span><span class="sxs-lookup"><span data-stu-id="88dc3-119">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="88dc3-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="88dc3-120">JSON representation</span></span>

<span data-ttu-id="88dc3-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="88dc3-121">The following is a JSON representation of the resource.</span></span>

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
