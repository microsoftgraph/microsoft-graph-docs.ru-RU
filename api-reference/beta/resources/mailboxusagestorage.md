---
title: Тип ресурса Маилбоксусажестораже
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 636417b5ec299bb11f82c406abecdebe72ee45de
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43473417"
---
# <a name="mailboxusagestorage-resource-type"></a><span data-ttu-id="29a98-103">Тип ресурса Маилбоксусажестораже</span><span class="sxs-lookup"><span data-stu-id="29a98-103">mailboxUsageStorage resource type</span></span>

<span data-ttu-id="29a98-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29a98-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="29a98-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="29a98-105">Properties</span></span>

| <span data-ttu-id="29a98-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="29a98-106">Property</span></span>           | <span data-ttu-id="29a98-107">Тип</span><span class="sxs-lookup"><span data-stu-id="29a98-107">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="29a98-108">репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="29a98-108">reportRefreshDate</span></span>  | <span data-ttu-id="29a98-109">Дата</span><span class="sxs-lookup"><span data-stu-id="29a98-109">Date</span></span>   |
| <span data-ttu-id="29a98-110">сторажеусединбитес</span><span class="sxs-lookup"><span data-stu-id="29a98-110">storageUsedInBytes</span></span> | <span data-ttu-id="29a98-111">Int64</span><span class="sxs-lookup"><span data-stu-id="29a98-111">Int64</span></span>  |
| <span data-ttu-id="29a98-112">reportDate</span><span class="sxs-lookup"><span data-stu-id="29a98-112">reportDate</span></span>         | <span data-ttu-id="29a98-113">Дата</span><span class="sxs-lookup"><span data-stu-id="29a98-113">Date</span></span>   |
| <span data-ttu-id="29a98-114">репортпериод</span><span class="sxs-lookup"><span data-stu-id="29a98-114">reportPeriod</span></span>       | <span data-ttu-id="29a98-115">String</span><span class="sxs-lookup"><span data-stu-id="29a98-115">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="29a98-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="29a98-116">JSON representation</span></span>

<span data-ttu-id="29a98-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="29a98-117">The following is a JSON representation of the resource.</span></span>

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
