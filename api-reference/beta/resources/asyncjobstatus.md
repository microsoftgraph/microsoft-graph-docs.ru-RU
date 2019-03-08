---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: AsyncJobStatus
localization_priority: Normal
ms.openlocfilehash: c951aa05b2b0f6f2b036bdf145e161a8d5b52ba7
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482233"
---
# <a name="asyncjobstatus-resource"></a><span data-ttu-id="6aca8-102">Ресурс AsyncJobStatus</span><span class="sxs-lookup"><span data-stu-id="6aca8-102">AsyncJobStatus resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6aca8-103">Этот ресурс предоставляет сведения о ходе выполнения асинхронного задания.</span><span class="sxs-lookup"><span data-stu-id="6aca8-103">This resource provides information on the status of a asynchronous job progress.</span></span>

<span data-ttu-id="6aca8-104">Указанные ниже вызовы API возвращают ресурсы **AsyncJobStatus**.</span><span class="sxs-lookup"><span data-stu-id="6aca8-104">The following API calls return **AsyncJobStatus** resources:</span></span>

* [<span data-ttu-id="6aca8-105">Копирование элемента</span><span class="sxs-lookup"><span data-stu-id="6aca8-105">Copy Item</span></span>](../api/driveitem-copy.md)

## <a name="json-representation"></a><span data-ttu-id="6aca8-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6aca8-106">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.asyncJobStatus", "@type.aka": "oneDrive.asyncOperationStatus" } -->

```json
{
  "percentageComplete": 100.0,
  "status": "notStarted | inProgress | completed | updating | failed | deletePending | deleteFailed | waiting"
}
```

## <a name="properties"></a><span data-ttu-id="6aca8-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6aca8-107">Properties</span></span>

| <span data-ttu-id="6aca8-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="6aca8-108">Property name</span></span>          | <span data-ttu-id="6aca8-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6aca8-109">Type</span></span>   | <span data-ttu-id="6aca8-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6aca8-110">Description</span></span>                                                                                |
|:-----------------------|:-------|:-------------------------------------------------------------------------------------------|
| <span data-ttu-id="6aca8-111">**percentageComplete**</span><span class="sxs-lookup"><span data-stu-id="6aca8-111">**percentageComplete**</span></span> | <span data-ttu-id="6aca8-112">Double</span><span class="sxs-lookup"><span data-stu-id="6aca8-112">Double</span></span> | <span data-ttu-id="6aca8-113">Значение от 0 до 100, указывающее процент выполнения.</span><span class="sxs-lookup"><span data-stu-id="6aca8-113">A value between 0 and 100 that indicates the percentage complete.</span></span>                          |
| <span data-ttu-id="6aca8-114">**status**</span><span class="sxs-lookup"><span data-stu-id="6aca8-114">**status**</span></span>             | <span data-ttu-id="6aca8-115">Строка</span><span class="sxs-lookup"><span data-stu-id="6aca8-115">String</span></span> | <span data-ttu-id="6aca8-116">Строковое значение, сопоставляемое с перечислением возможных значений состояния задания.</span><span class="sxs-lookup"><span data-stu-id="6aca8-116">A string value that maps to an enumeration of possible values about the status of the job.</span></span> |

<!--
{
  "type": "#page.annotation",
  "description": "AsyncJobResource provides details about how to poll for an async completion.",
  "keywords": "async,job status,async status,copy,upload from url",
  "section": "documentation",
  "suppressions": [
    "Error: /api-reference/beta/resources/asyncjobstatus.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
