---
title: Тип ресурса Маилбоксусажестораже
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 080b1e5eafb23e40df1307fc6ab3e9a4ef9c87f0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075534"
---
# <a name="mailboxusagestorage-resource-type"></a><span data-ttu-id="5339d-103">Тип ресурса Маилбоксусажестораже</span><span class="sxs-lookup"><span data-stu-id="5339d-103">mailboxUsageStorage resource type</span></span>

<span data-ttu-id="5339d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5339d-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="5339d-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="5339d-105">Properties</span></span>

| <span data-ttu-id="5339d-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="5339d-106">Property</span></span>           | <span data-ttu-id="5339d-107">Тип</span><span class="sxs-lookup"><span data-stu-id="5339d-107">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="5339d-108">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="5339d-108">reportRefreshDate</span></span>  | <span data-ttu-id="5339d-109">Дата</span><span class="sxs-lookup"><span data-stu-id="5339d-109">Date</span></span>   |
| <span data-ttu-id="5339d-110">сторажеусединбитес</span><span class="sxs-lookup"><span data-stu-id="5339d-110">storageUsedInBytes</span></span> | <span data-ttu-id="5339d-111">Int64</span><span class="sxs-lookup"><span data-stu-id="5339d-111">Int64</span></span>  |
| <span data-ttu-id="5339d-112">reportDate</span><span class="sxs-lookup"><span data-stu-id="5339d-112">reportDate</span></span>         | <span data-ttu-id="5339d-113">Дата</span><span class="sxs-lookup"><span data-stu-id="5339d-113">Date</span></span>   |
| <span data-ttu-id="5339d-114">репортпериод</span><span class="sxs-lookup"><span data-stu-id="5339d-114">reportPeriod</span></span>       | <span data-ttu-id="5339d-115">String</span><span class="sxs-lookup"><span data-stu-id="5339d-115">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5339d-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5339d-116">JSON representation</span></span>

<span data-ttu-id="5339d-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5339d-117">The following is a JSON representation of the resource.</span></span>

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


