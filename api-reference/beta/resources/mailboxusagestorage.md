---
title: Тип ресурса mailboxUsageStorage
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 44b97c7b18264e01c86b34bfd8265246f80ab031
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917869"
---
# <a name="mailboxusagestorage-resource-type"></a><span data-ttu-id="b9ff1-103">Тип ресурса mailboxUsageStorage</span><span class="sxs-lookup"><span data-stu-id="b9ff1-103">mailboxUsageStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="b9ff1-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="b9ff1-104">Properties</span></span>

| <span data-ttu-id="b9ff1-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="b9ff1-105">Property</span></span>           | <span data-ttu-id="b9ff1-106">Тип</span><span class="sxs-lookup"><span data-stu-id="b9ff1-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="b9ff1-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="b9ff1-107">reportRefreshDate</span></span>  | <span data-ttu-id="b9ff1-108">Date</span><span class="sxs-lookup"><span data-stu-id="b9ff1-108">Date</span></span>   |
| <span data-ttu-id="b9ff1-109">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="b9ff1-109">storageUsedInBytes</span></span> | <span data-ttu-id="b9ff1-110">Int64</span><span class="sxs-lookup"><span data-stu-id="b9ff1-110">Int64</span></span>  |
| <span data-ttu-id="b9ff1-111">reportDate</span><span class="sxs-lookup"><span data-stu-id="b9ff1-111">reportDate</span></span>         | <span data-ttu-id="b9ff1-112">Date</span><span class="sxs-lookup"><span data-stu-id="b9ff1-112">Date</span></span>   |
| <span data-ttu-id="b9ff1-113">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="b9ff1-113">reportPeriod</span></span>       | <span data-ttu-id="b9ff1-114">String</span><span class="sxs-lookup"><span data-stu-id="b9ff1-114">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b9ff1-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b9ff1-115">JSON representation</span></span>

<span data-ttu-id="b9ff1-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b9ff1-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailboxUsageStorage"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "storageUsedInBytes": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
