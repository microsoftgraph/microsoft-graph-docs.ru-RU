---
title: Тип ресурса Маилбоксусажестораже
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 6f4ee4b29c82102db96cd4d71718f7da449776b5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009841"
---
# <a name="mailboxusagestorage-resource-type"></a><span data-ttu-id="3187a-103">Тип ресурса Маилбоксусажестораже</span><span class="sxs-lookup"><span data-stu-id="3187a-103">mailboxUsageStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="3187a-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="3187a-104">Properties</span></span>

| <span data-ttu-id="3187a-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="3187a-105">Property</span></span>           | <span data-ttu-id="3187a-106">Тип</span><span class="sxs-lookup"><span data-stu-id="3187a-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="3187a-107">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="3187a-107">reportRefreshDate</span></span>  | <span data-ttu-id="3187a-108">Дата</span><span class="sxs-lookup"><span data-stu-id="3187a-108">Date</span></span>   |
| <span data-ttu-id="3187a-109">Сторажеусединбитес</span><span class="sxs-lookup"><span data-stu-id="3187a-109">storageUsedInBytes</span></span> | <span data-ttu-id="3187a-110">Int64</span><span class="sxs-lookup"><span data-stu-id="3187a-110">Int64</span></span>  |
| <span data-ttu-id="3187a-111">reportDate</span><span class="sxs-lookup"><span data-stu-id="3187a-111">reportDate</span></span>         | <span data-ttu-id="3187a-112">Дата</span><span class="sxs-lookup"><span data-stu-id="3187a-112">Date</span></span>   |
| <span data-ttu-id="3187a-113">Репортпериод</span><span class="sxs-lookup"><span data-stu-id="3187a-113">reportPeriod</span></span>       | <span data-ttu-id="3187a-114">String</span><span class="sxs-lookup"><span data-stu-id="3187a-114">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3187a-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3187a-115">JSON representation</span></span>

<span data-ttu-id="3187a-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3187a-116">The following is a JSON representation of the resource.</span></span>

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
