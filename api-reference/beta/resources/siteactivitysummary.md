---
title: Тип ресурса siteActivitySummary
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: 2eb5bdb89924338d1d352ea80bd516b8fb948250
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817768"
---
# <a name="siteactivitysummary-resource-type"></a><span data-ttu-id="64818-103">Тип ресурса siteActivitySummary</span><span class="sxs-lookup"><span data-stu-id="64818-103">siteActivitySummary resource type</span></span>

## <a name="properties"></a><span data-ttu-id="64818-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="64818-104">Properties</span></span>

| <span data-ttu-id="64818-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="64818-105">Property</span></span>          | <span data-ttu-id="64818-106">Тип</span><span class="sxs-lookup"><span data-stu-id="64818-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="64818-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="64818-107">reportRefreshDate</span></span> | <span data-ttu-id="64818-108">Date</span><span class="sxs-lookup"><span data-stu-id="64818-108">Date</span></span>   |
| <span data-ttu-id="64818-109">viewedOrEdited</span><span class="sxs-lookup"><span data-stu-id="64818-109">viewedOrEdited</span></span>    | <span data-ttu-id="64818-110">Int64</span><span class="sxs-lookup"><span data-stu-id="64818-110">Int64</span></span>  |
| <span data-ttu-id="64818-111">синхронизирован</span><span class="sxs-lookup"><span data-stu-id="64818-111">synced</span></span>            | <span data-ttu-id="64818-112">Int64</span><span class="sxs-lookup"><span data-stu-id="64818-112">Int64</span></span>  |
| <span data-ttu-id="64818-113">sharedInternally</span><span class="sxs-lookup"><span data-stu-id="64818-113">sharedInternally</span></span>  | <span data-ttu-id="64818-114">Int64</span><span class="sxs-lookup"><span data-stu-id="64818-114">Int64</span></span>  |
| <span data-ttu-id="64818-115">sharedExternally</span><span class="sxs-lookup"><span data-stu-id="64818-115">sharedExternally</span></span>  | <span data-ttu-id="64818-116">Int64</span><span class="sxs-lookup"><span data-stu-id="64818-116">Int64</span></span>  |
| <span data-ttu-id="64818-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="64818-117">reportDate</span></span>        | <span data-ttu-id="64818-118">Date</span><span class="sxs-lookup"><span data-stu-id="64818-118">Date</span></span>   |
| <span data-ttu-id="64818-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="64818-119">reportPeriod</span></span>      | <span data-ttu-id="64818-120">String</span><span class="sxs-lookup"><span data-stu-id="64818-120">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="64818-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="64818-121">JSON representation</span></span>

<span data-ttu-id="64818-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="64818-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.siteActivitySummary"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "viewedOrEdited": 1024, 
  "synced": 1024, 
  "sharedInternally": 1024, 
  "sharedExternally": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
