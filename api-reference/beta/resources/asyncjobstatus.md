---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: AsyncJobStatus
ms.openlocfilehash: 9e0f95802f9f75930384ab1534bf4c519fd9cfeb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075142"
---
# <a name="asyncjobstatus-resource"></a><span data-ttu-id="e9432-102">Ресурс AsyncJobStatus</span><span class="sxs-lookup"><span data-stu-id="e9432-102">AsyncJobStatus resource</span></span>

> <span data-ttu-id="e9432-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e9432-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e9432-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9432-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e9432-105">Этот ресурс предоставляет сведения о ходе выполнения асинхронного задания.</span><span class="sxs-lookup"><span data-stu-id="e9432-105">This resource provides information on the status of a asynchronous job progress.</span></span>

<span data-ttu-id="e9432-106">Указанные ниже вызовы API возвращают ресурсы **AsyncJobStatus**.</span><span class="sxs-lookup"><span data-stu-id="e9432-106">The following API calls return **AsyncJobStatus** resources:</span></span>

* [<span data-ttu-id="e9432-107">Копирование элемента</span><span class="sxs-lookup"><span data-stu-id="e9432-107">Copy Item</span></span>](../api/driveitem-copy.md)

## <a name="json-representation"></a><span data-ttu-id="e9432-108">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e9432-108">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.asyncJobStatus", "@type.aka": "oneDrive.asyncOperationStatus" } -->

```json
{
  "percentageComplete": 100.0,
  "status": "notStarted | inProgress | completed | updating | failed | deletePending | deleteFailed | waiting"
}
```

## <a name="properties"></a><span data-ttu-id="e9432-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="e9432-109">Properties</span></span>

| <span data-ttu-id="e9432-110">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="e9432-110">Property name</span></span>          | <span data-ttu-id="e9432-111">Тип</span><span class="sxs-lookup"><span data-stu-id="e9432-111">Type</span></span>   | <span data-ttu-id="e9432-112">Описание</span><span class="sxs-lookup"><span data-stu-id="e9432-112">Description</span></span>                                                                                |
|:-----------------------|:-------|:-------------------------------------------------------------------------------------------|
| <span data-ttu-id="e9432-113">**percentageComplete**</span><span class="sxs-lookup"><span data-stu-id="e9432-113">**percentageComplete**</span></span> | <span data-ttu-id="e9432-114">Double</span><span class="sxs-lookup"><span data-stu-id="e9432-114">Double</span></span> | <span data-ttu-id="e9432-115">Значение от 0 до 100, указывающее процент выполнения.</span><span class="sxs-lookup"><span data-stu-id="e9432-115">A value between 0 and 100 that indicates the percentage complete.</span></span>                          |
| <span data-ttu-id="e9432-116">**status**</span><span class="sxs-lookup"><span data-stu-id="e9432-116">**status**</span></span>             | <span data-ttu-id="e9432-117">Строка</span><span class="sxs-lookup"><span data-stu-id="e9432-117">String</span></span> | <span data-ttu-id="e9432-118">Строковое значение, сопоставляемое с перечислением возможных значений состояния задания.</span><span class="sxs-lookup"><span data-stu-id="e9432-118">A string value that maps to an enumeration of possible values about the status of the job.</span></span> |

<!-- {
  "type": "#page.annotation",
  "description": "AsyncJobResource provides details about how to poll for an async completion.",
  "keywords": "async,job status,async status,copy,upload from url",
  "section": "documentation"
} -->
