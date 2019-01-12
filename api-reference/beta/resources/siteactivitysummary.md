---
title: Тип ресурса siteActivitySummary
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: a49b8e47ca2a6efcc5c5c87702fdea0122b208e1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957139"
---
# <a name="siteactivitysummary-resource-type"></a><span data-ttu-id="6b71e-103">Тип ресурса siteActivitySummary</span><span class="sxs-lookup"><span data-stu-id="6b71e-103">siteActivitySummary resource type</span></span>

## <a name="properties"></a><span data-ttu-id="6b71e-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="6b71e-104">Properties</span></span>

| <span data-ttu-id="6b71e-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="6b71e-105">Property</span></span>          | <span data-ttu-id="6b71e-106">Тип</span><span class="sxs-lookup"><span data-stu-id="6b71e-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="6b71e-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="6b71e-107">reportRefreshDate</span></span> | <span data-ttu-id="6b71e-108">Date</span><span class="sxs-lookup"><span data-stu-id="6b71e-108">Date</span></span>   |
| <span data-ttu-id="6b71e-109">viewedOrEdited</span><span class="sxs-lookup"><span data-stu-id="6b71e-109">viewedOrEdited</span></span>    | <span data-ttu-id="6b71e-110">Int64</span><span class="sxs-lookup"><span data-stu-id="6b71e-110">Int64</span></span>  |
| <span data-ttu-id="6b71e-111">синхронизирован</span><span class="sxs-lookup"><span data-stu-id="6b71e-111">synced</span></span>            | <span data-ttu-id="6b71e-112">Int64</span><span class="sxs-lookup"><span data-stu-id="6b71e-112">Int64</span></span>  |
| <span data-ttu-id="6b71e-113">sharedInternally</span><span class="sxs-lookup"><span data-stu-id="6b71e-113">sharedInternally</span></span>  | <span data-ttu-id="6b71e-114">Int64</span><span class="sxs-lookup"><span data-stu-id="6b71e-114">Int64</span></span>  |
| <span data-ttu-id="6b71e-115">sharedExternally</span><span class="sxs-lookup"><span data-stu-id="6b71e-115">sharedExternally</span></span>  | <span data-ttu-id="6b71e-116">Int64</span><span class="sxs-lookup"><span data-stu-id="6b71e-116">Int64</span></span>  |
| <span data-ttu-id="6b71e-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="6b71e-117">reportDate</span></span>        | <span data-ttu-id="6b71e-118">Date</span><span class="sxs-lookup"><span data-stu-id="6b71e-118">Date</span></span>   |
| <span data-ttu-id="6b71e-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="6b71e-119">reportPeriod</span></span>      | <span data-ttu-id="6b71e-120">String</span><span class="sxs-lookup"><span data-stu-id="6b71e-120">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6b71e-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6b71e-121">JSON representation</span></span>

<span data-ttu-id="6b71e-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6b71e-122">The following is a JSON representation of the resource.</span></span>

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
