---
title: Тип ресурса Емаилактивитисуммари
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 78853954ef7c6fe4a191cbccefca350e628db210
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47989593"
---
# <a name="emailactivitysummary-resource-type"></a><span data-ttu-id="1e9fd-103">Тип ресурса Емаилактивитисуммари</span><span class="sxs-lookup"><span data-stu-id="1e9fd-103">emailActivitySummary resource type</span></span>

<span data-ttu-id="1e9fd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e9fd-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="1e9fd-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="1e9fd-105">Properties</span></span>

| <span data-ttu-id="1e9fd-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="1e9fd-106">Property</span></span>          | <span data-ttu-id="1e9fd-107">Тип</span><span class="sxs-lookup"><span data-stu-id="1e9fd-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="1e9fd-108">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="1e9fd-108">reportRefreshDate</span></span> | <span data-ttu-id="1e9fd-109">Дата</span><span class="sxs-lookup"><span data-stu-id="1e9fd-109">Date</span></span>   |
| <span data-ttu-id="1e9fd-110">send</span><span class="sxs-lookup"><span data-stu-id="1e9fd-110">send</span></span>              | <span data-ttu-id="1e9fd-111">Int64</span><span class="sxs-lookup"><span data-stu-id="1e9fd-111">Int64</span></span>  |
| <span data-ttu-id="1e9fd-112">получил</span><span class="sxs-lookup"><span data-stu-id="1e9fd-112">receive</span></span>           | <span data-ttu-id="1e9fd-113">Int64</span><span class="sxs-lookup"><span data-stu-id="1e9fd-113">Int64</span></span>  |
| <span data-ttu-id="1e9fd-114">read</span><span class="sxs-lookup"><span data-stu-id="1e9fd-114">read</span></span>              | <span data-ttu-id="1e9fd-115">Int64</span><span class="sxs-lookup"><span data-stu-id="1e9fd-115">Int64</span></span>  |
| <span data-ttu-id="1e9fd-116">reportDate</span><span class="sxs-lookup"><span data-stu-id="1e9fd-116">reportDate</span></span>        | <span data-ttu-id="1e9fd-117">Дата</span><span class="sxs-lookup"><span data-stu-id="1e9fd-117">Date</span></span>   |
| <span data-ttu-id="1e9fd-118">репортпериод</span><span class="sxs-lookup"><span data-stu-id="1e9fd-118">reportPeriod</span></span>      | <span data-ttu-id="1e9fd-119">String</span><span class="sxs-lookup"><span data-stu-id="1e9fd-119">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1e9fd-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1e9fd-120">JSON representation</span></span>

<span data-ttu-id="1e9fd-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1e9fd-121">The following is a JSON representation of the resource.</span></span>

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


