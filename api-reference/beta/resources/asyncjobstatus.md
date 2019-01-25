---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: AsyncJobStatus
localization_priority: Normal
ms.openlocfilehash: ee7cc92bff47edc3a1a15b5f27cb2f5afe061d4e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510213"
---
# <a name="asyncjobstatus-resource"></a><span data-ttu-id="4ae28-102">Ресурс AsyncJobStatus</span><span class="sxs-lookup"><span data-stu-id="4ae28-102">AsyncJobStatus resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ae28-103">Этот ресурс предоставляет сведения о ходе выполнения асинхронного задания.</span><span class="sxs-lookup"><span data-stu-id="4ae28-103">This resource provides information on the status of a asynchronous job progress.</span></span>

<span data-ttu-id="4ae28-104">Указанные ниже вызовы API возвращают ресурсы **AsyncJobStatus**.</span><span class="sxs-lookup"><span data-stu-id="4ae28-104">The following API calls return **AsyncJobStatus** resources:</span></span>

* [<span data-ttu-id="4ae28-105">Копирование элемента</span><span class="sxs-lookup"><span data-stu-id="4ae28-105">Copy Item</span></span>](../api/driveitem-copy.md)

## <a name="json-representation"></a><span data-ttu-id="4ae28-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4ae28-106">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.asyncJobStatus", "@type.aka": "oneDrive.asyncOperationStatus" } -->

```json
{
  "percentageComplete": 100.0,
  "status": "notStarted | inProgress | completed | updating | failed | deletePending | deleteFailed | waiting"
}
```

## <a name="properties"></a><span data-ttu-id="4ae28-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4ae28-107">Properties</span></span>

| <span data-ttu-id="4ae28-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="4ae28-108">Property name</span></span>          | <span data-ttu-id="4ae28-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4ae28-109">Type</span></span>   | <span data-ttu-id="4ae28-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4ae28-110">Description</span></span>                                                                                |
|:-----------------------|:-------|:-------------------------------------------------------------------------------------------|
| <span data-ttu-id="4ae28-111">**percentageComplete**</span><span class="sxs-lookup"><span data-stu-id="4ae28-111">**percentageComplete**</span></span> | <span data-ttu-id="4ae28-112">Double</span><span class="sxs-lookup"><span data-stu-id="4ae28-112">Double</span></span> | <span data-ttu-id="4ae28-113">Значение от 0 до 100, указывающее процент выполнения.</span><span class="sxs-lookup"><span data-stu-id="4ae28-113">A value between 0 and 100 that indicates the percentage complete.</span></span>                          |
| <span data-ttu-id="4ae28-114">**status**</span><span class="sxs-lookup"><span data-stu-id="4ae28-114">**status**</span></span>             | <span data-ttu-id="4ae28-115">Строка</span><span class="sxs-lookup"><span data-stu-id="4ae28-115">String</span></span> | <span data-ttu-id="4ae28-116">Строковое значение, сопоставляемое с перечислением возможных значений состояния задания.</span><span class="sxs-lookup"><span data-stu-id="4ae28-116">A string value that maps to an enumeration of possible values about the status of the job.</span></span> |

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
