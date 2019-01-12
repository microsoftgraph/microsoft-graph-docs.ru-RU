---
title: Тип ресурса oneDriveUsageFileCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: a7e3a52d082d1acdd2e685008d60e6594615f57a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941025"
---
# <a name="onedriveusagefilecounts-resource-type"></a><span data-ttu-id="691fa-103">Тип ресурса oneDriveUsageFileCounts</span><span class="sxs-lookup"><span data-stu-id="691fa-103">oneDriveUsageFileCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="691fa-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="691fa-104">Properties</span></span>

| <span data-ttu-id="691fa-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="691fa-105">Property</span></span>          | <span data-ttu-id="691fa-106">Тип</span><span class="sxs-lookup"><span data-stu-id="691fa-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="691fa-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="691fa-107">reportRefreshDate</span></span> | <span data-ttu-id="691fa-108">Date</span><span class="sxs-lookup"><span data-stu-id="691fa-108">Date</span></span>   |
| <span data-ttu-id="691fa-109">siteType</span><span class="sxs-lookup"><span data-stu-id="691fa-109">siteType</span></span>          | <span data-ttu-id="691fa-110">Строка</span><span class="sxs-lookup"><span data-stu-id="691fa-110">String</span></span> |
| <span data-ttu-id="691fa-111">total</span><span class="sxs-lookup"><span data-stu-id="691fa-111">total</span></span>             | <span data-ttu-id="691fa-112">Int64</span><span class="sxs-lookup"><span data-stu-id="691fa-112">Int64</span></span>  |
| <span data-ttu-id="691fa-113">активных</span><span class="sxs-lookup"><span data-stu-id="691fa-113">active</span></span>            | <span data-ttu-id="691fa-114">Int64</span><span class="sxs-lookup"><span data-stu-id="691fa-114">Int64</span></span>  |
| <span data-ttu-id="691fa-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="691fa-115">reportDate</span></span>        | <span data-ttu-id="691fa-116">Date</span><span class="sxs-lookup"><span data-stu-id="691fa-116">Date</span></span>   |
| <span data-ttu-id="691fa-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="691fa-117">reportPeriod</span></span>      | <span data-ttu-id="691fa-118">String</span><span class="sxs-lookup"><span data-stu-id="691fa-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="691fa-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="691fa-119">JSON representation</span></span>

<span data-ttu-id="691fa-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="691fa-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.oneDriveUsageFileCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "siteType": "String", 
  "total": 1024, 
  "active": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
