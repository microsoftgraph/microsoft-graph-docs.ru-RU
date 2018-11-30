---
title: Тип ресурса mailboxUsageStorage
description: Ниже указано представление ресурса в формате JSON.
ms.openlocfilehash: 8cc26c5d3cc30529857ed3273f8ee66c7373327a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076505"
---
# <a name="mailboxusagestorage-resource-type"></a><span data-ttu-id="ee786-103">Тип ресурса mailboxUsageStorage</span><span class="sxs-lookup"><span data-stu-id="ee786-103">mailboxUsageStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="ee786-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="ee786-104">Properties</span></span>

| <span data-ttu-id="ee786-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="ee786-105">Property</span></span>           | <span data-ttu-id="ee786-106">Тип</span><span class="sxs-lookup"><span data-stu-id="ee786-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="ee786-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="ee786-107">reportRefreshDate</span></span>  | <span data-ttu-id="ee786-108">Date</span><span class="sxs-lookup"><span data-stu-id="ee786-108">Date</span></span>   |
| <span data-ttu-id="ee786-109">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="ee786-109">storageUsedInBytes</span></span> | <span data-ttu-id="ee786-110">Int64</span><span class="sxs-lookup"><span data-stu-id="ee786-110">Int64</span></span>  |
| <span data-ttu-id="ee786-111">reportDate</span><span class="sxs-lookup"><span data-stu-id="ee786-111">reportDate</span></span>         | <span data-ttu-id="ee786-112">Date</span><span class="sxs-lookup"><span data-stu-id="ee786-112">Date</span></span>   |
| <span data-ttu-id="ee786-113">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="ee786-113">reportPeriod</span></span>       | <span data-ttu-id="ee786-114">String</span><span class="sxs-lookup"><span data-stu-id="ee786-114">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ee786-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ee786-115">JSON representation</span></span>

<span data-ttu-id="ee786-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ee786-116">The following is a JSON representation of the resource.</span></span>

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
