---
author: JeremyKelley
description: Этот ресурс предоставляет сведения о ходе выполнения асинхронного задания.
ms.date: 09/10/2017
title: AsyncJobStatus
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: e8a745a6ab03728eb879767c6af45a423f151d63
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974306"
---
# <a name="asyncjobstatus-resource"></a><span data-ttu-id="7b1a4-103">Ресурс AsyncJobStatus</span><span class="sxs-lookup"><span data-stu-id="7b1a4-103">AsyncJobStatus resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b1a4-104">Этот ресурс предоставляет сведения о ходе выполнения асинхронного задания.</span><span class="sxs-lookup"><span data-stu-id="7b1a4-104">This resource provides information on the status of a asynchronous job progress.</span></span>

<span data-ttu-id="7b1a4-105">Указанные ниже вызовы API возвращают ресурсы **AsyncJobStatus**.</span><span class="sxs-lookup"><span data-stu-id="7b1a4-105">The following API calls return **AsyncJobStatus** resources:</span></span>

* [<span data-ttu-id="7b1a4-106">Копирование элемента</span><span class="sxs-lookup"><span data-stu-id="7b1a4-106">Copy Item</span></span>](../api/driveitem-copy.md)

## <a name="json-representation"></a><span data-ttu-id="7b1a4-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7b1a4-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.asyncJobStatus", "@type.aka": "oneDrive.asyncOperationStatus" } -->

```json
{
  "percentageComplete": 100.0,
  "status": "notStarted | inProgress | completed | updating | failed | deletePending | deleteFailed | waiting"
}
```

## <a name="properties"></a><span data-ttu-id="7b1a4-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="7b1a4-108">Properties</span></span>

| <span data-ttu-id="7b1a4-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="7b1a4-109">Property name</span></span>          | <span data-ttu-id="7b1a4-110">Тип</span><span class="sxs-lookup"><span data-stu-id="7b1a4-110">Type</span></span>   | <span data-ttu-id="7b1a4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7b1a4-111">Description</span></span>                                                                                |
|:-----------------------|:-------|:-------------------------------------------------------------------------------------------|
| <span data-ttu-id="7b1a4-112">**percentageComplete**</span><span class="sxs-lookup"><span data-stu-id="7b1a4-112">**percentageComplete**</span></span> | <span data-ttu-id="7b1a4-113">Double</span><span class="sxs-lookup"><span data-stu-id="7b1a4-113">Double</span></span> | <span data-ttu-id="7b1a4-114">Значение от 0 до 100, указывающее процент выполнения.</span><span class="sxs-lookup"><span data-stu-id="7b1a4-114">A value between 0 and 100 that indicates the percentage complete.</span></span>                          |
| <span data-ttu-id="7b1a4-115">**status**</span><span class="sxs-lookup"><span data-stu-id="7b1a4-115">**status**</span></span>             | <span data-ttu-id="7b1a4-116">Строка</span><span class="sxs-lookup"><span data-stu-id="7b1a4-116">String</span></span> | <span data-ttu-id="7b1a4-117">Строковое значение, сопоставляемое с перечислением возможных значений состояния задания.</span><span class="sxs-lookup"><span data-stu-id="7b1a4-117">A string value that maps to an enumeration of possible values about the status of the job.</span></span> |

<!--
{
  "type": "#page.annotation",
  "description": "AsyncJobResource provides details about how to poll for an async completion.",
  "keywords": "async,job status,async status,copy,upload from url",
  "section": "documentation",
  "suppressions": []
}
-->
