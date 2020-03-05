---
title: Тип ресурса Яммерактивитисуммари
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: fc7fc9679de3a655e76b6182f218010de7e39997
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519038"
---
# <a name="yammeractivitysummary-resource-type"></a><span data-ttu-id="cb3bb-103">Тип ресурса Яммерактивитисуммари</span><span class="sxs-lookup"><span data-stu-id="cb3bb-103">yammerActivitySummary resource type</span></span>

<span data-ttu-id="cb3bb-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="cb3bb-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="cb3bb-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="cb3bb-105">Properties</span></span>

| <span data-ttu-id="cb3bb-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="cb3bb-106">Property</span></span>          | <span data-ttu-id="cb3bb-107">Тип</span><span class="sxs-lookup"><span data-stu-id="cb3bb-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="cb3bb-108">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="cb3bb-108">reportRefreshDate</span></span> | <span data-ttu-id="cb3bb-109">Дата</span><span class="sxs-lookup"><span data-stu-id="cb3bb-109">Date</span></span>   |
| <span data-ttu-id="cb3bb-110">метк</span><span class="sxs-lookup"><span data-stu-id="cb3bb-110">liked</span></span>             | <span data-ttu-id="cb3bb-111">Int64</span><span class="sxs-lookup"><span data-stu-id="cb3bb-111">Int64</span></span>  |
| <span data-ttu-id="cb3bb-112">размещен</span><span class="sxs-lookup"><span data-stu-id="cb3bb-112">posted</span></span>            | <span data-ttu-id="cb3bb-113">Int64</span><span class="sxs-lookup"><span data-stu-id="cb3bb-113">Int64</span></span>  |
| <span data-ttu-id="cb3bb-114">прочитан</span><span class="sxs-lookup"><span data-stu-id="cb3bb-114">read</span></span>              | <span data-ttu-id="cb3bb-115">Int64</span><span class="sxs-lookup"><span data-stu-id="cb3bb-115">Int64</span></span>  |
| <span data-ttu-id="cb3bb-116">reportDate</span><span class="sxs-lookup"><span data-stu-id="cb3bb-116">reportDate</span></span>        | <span data-ttu-id="cb3bb-117">Дата</span><span class="sxs-lookup"><span data-stu-id="cb3bb-117">Date</span></span>   |
| <span data-ttu-id="cb3bb-118">репортпериод</span><span class="sxs-lookup"><span data-stu-id="cb3bb-118">reportPeriod</span></span>      | <span data-ttu-id="cb3bb-119">String</span><span class="sxs-lookup"><span data-stu-id="cb3bb-119">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="cb3bb-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cb3bb-120">JSON representation</span></span>

<span data-ttu-id="cb3bb-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cb3bb-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerActivitySummary"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "liked": 1024, 
  "posted": 1024, 
  "read": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
