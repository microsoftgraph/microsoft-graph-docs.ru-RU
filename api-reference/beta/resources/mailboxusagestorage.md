---
title: Тип ресурса mailboxUsageStorage
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: sarahwxy
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 4fedb101fbab2b14ec2d1ada1e02faa4bc729e0d
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982203"
---
# <a name="mailboxusagestorage-resource-type"></a><span data-ttu-id="d663c-103">Тип ресурса mailboxUsageStorage</span><span class="sxs-lookup"><span data-stu-id="d663c-103">mailboxUsageStorage resource type</span></span>

<span data-ttu-id="d663c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d663c-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="d663c-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="d663c-105">Properties</span></span>

| <span data-ttu-id="d663c-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="d663c-106">Property</span></span>           | <span data-ttu-id="d663c-107">Тип</span><span class="sxs-lookup"><span data-stu-id="d663c-107">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="d663c-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="d663c-108">reportRefreshDate</span></span>  | <span data-ttu-id="d663c-109">Дата</span><span class="sxs-lookup"><span data-stu-id="d663c-109">Date</span></span>   |
| <span data-ttu-id="d663c-110">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="d663c-110">storageUsedInBytes</span></span> | <span data-ttu-id="d663c-111">Int64</span><span class="sxs-lookup"><span data-stu-id="d663c-111">Int64</span></span>  |
| <span data-ttu-id="d663c-112">reportDate</span><span class="sxs-lookup"><span data-stu-id="d663c-112">reportDate</span></span>         | <span data-ttu-id="d663c-113">Дата</span><span class="sxs-lookup"><span data-stu-id="d663c-113">Date</span></span>   |
| <span data-ttu-id="d663c-114">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="d663c-114">reportPeriod</span></span>       | <span data-ttu-id="d663c-115">String</span><span class="sxs-lookup"><span data-stu-id="d663c-115">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d663c-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d663c-116">JSON representation</span></span>

<span data-ttu-id="d663c-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d663c-117">The following is a JSON representation of the resource.</span></span>

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


