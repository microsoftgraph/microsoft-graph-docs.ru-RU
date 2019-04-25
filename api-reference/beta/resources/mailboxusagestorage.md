---
title: Тип ресурса Маилбоксусажестораже
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 44b97c7b18264e01c86b34bfd8265246f80ab031
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32524547"
---
# <a name="mailboxusagestorage-resource-type"></a><span data-ttu-id="7a784-103">Тип ресурса Маилбоксусажестораже</span><span class="sxs-lookup"><span data-stu-id="7a784-103">mailboxUsageStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="7a784-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="7a784-104">Properties</span></span>

| <span data-ttu-id="7a784-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="7a784-105">Property</span></span>           | <span data-ttu-id="7a784-106">Тип</span><span class="sxs-lookup"><span data-stu-id="7a784-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="7a784-107">Репортрефрешдате</span><span class="sxs-lookup"><span data-stu-id="7a784-107">reportRefreshDate</span></span>  | <span data-ttu-id="7a784-108">Дата</span><span class="sxs-lookup"><span data-stu-id="7a784-108">Date</span></span>   |
| <span data-ttu-id="7a784-109">Сторажеусединбитес</span><span class="sxs-lookup"><span data-stu-id="7a784-109">storageUsedInBytes</span></span> | <span data-ttu-id="7a784-110">Int64</span><span class="sxs-lookup"><span data-stu-id="7a784-110">Int64</span></span>  |
| <span data-ttu-id="7a784-111">reportDate</span><span class="sxs-lookup"><span data-stu-id="7a784-111">reportDate</span></span>         | <span data-ttu-id="7a784-112">Дата</span><span class="sxs-lookup"><span data-stu-id="7a784-112">Date</span></span>   |
| <span data-ttu-id="7a784-113">Репортпериод</span><span class="sxs-lookup"><span data-stu-id="7a784-113">reportPeriod</span></span>       | <span data-ttu-id="7a784-114">String</span><span class="sxs-lookup"><span data-stu-id="7a784-114">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7a784-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7a784-115">JSON representation</span></span>

<span data-ttu-id="7a784-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7a784-116">The following is a JSON representation of the resource.</span></span>

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
