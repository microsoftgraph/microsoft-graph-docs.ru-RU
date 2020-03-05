---
title: Тип ресурса Маилбоксусажестораже
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 40cc5f9b9cab7f17e185619d7fccdec028ae6250
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522836"
---
# <a name="mailboxusagestorage-resource-type"></a><span data-ttu-id="56409-103">Тип ресурса Маилбоксусажестораже</span><span class="sxs-lookup"><span data-stu-id="56409-103">mailboxUsageStorage resource type</span></span>

<span data-ttu-id="56409-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="56409-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="56409-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="56409-105">Properties</span></span>

| <span data-ttu-id="56409-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="56409-106">Property</span></span>           | <span data-ttu-id="56409-107">Тип</span><span class="sxs-lookup"><span data-stu-id="56409-107">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="56409-108">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="56409-108">reportRefreshDate</span></span>  | <span data-ttu-id="56409-109">Дата</span><span class="sxs-lookup"><span data-stu-id="56409-109">Date</span></span>   |
| <span data-ttu-id="56409-110">сторажеусединбитес</span><span class="sxs-lookup"><span data-stu-id="56409-110">storageUsedInBytes</span></span> | <span data-ttu-id="56409-111">Int64</span><span class="sxs-lookup"><span data-stu-id="56409-111">Int64</span></span>  |
| <span data-ttu-id="56409-112">reportDate</span><span class="sxs-lookup"><span data-stu-id="56409-112">reportDate</span></span>         | <span data-ttu-id="56409-113">Дата</span><span class="sxs-lookup"><span data-stu-id="56409-113">Date</span></span>   |
| <span data-ttu-id="56409-114">репортпериод</span><span class="sxs-lookup"><span data-stu-id="56409-114">reportPeriod</span></span>       | <span data-ttu-id="56409-115">String</span><span class="sxs-lookup"><span data-stu-id="56409-115">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="56409-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="56409-116">JSON representation</span></span>

<span data-ttu-id="56409-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="56409-117">The following is a JSON representation of the resource.</span></span>

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
