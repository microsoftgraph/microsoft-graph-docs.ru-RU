---
author: JeremyKelley
description: Этот ресурс предоставляет сведения о ходе выполнения асинхронного задания.
ms.date: 09/10/2017
title: AsyncJobStatus
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 81348ce59e060dadf4201222fca43bf96241dbc3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508173"
---
# <a name="asyncjobstatus-resource"></a><span data-ttu-id="7d36c-103">Ресурс AsyncJobStatus</span><span class="sxs-lookup"><span data-stu-id="7d36c-103">AsyncJobStatus resource</span></span>

<span data-ttu-id="7d36c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d36c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d36c-105">Этот ресурс предоставляет сведения о ходе выполнения асинхронного задания.</span><span class="sxs-lookup"><span data-stu-id="7d36c-105">This resource provides information on the status of a asynchronous job progress.</span></span>

<span data-ttu-id="7d36c-106">Указанные ниже вызовы API возвращают ресурсы **AsyncJobStatus**.</span><span class="sxs-lookup"><span data-stu-id="7d36c-106">The following API calls return **AsyncJobStatus** resources:</span></span>

* [<span data-ttu-id="7d36c-107">Копирование элемента</span><span class="sxs-lookup"><span data-stu-id="7d36c-107">Copy Item</span></span>](../api/driveitem-copy.md)

## <a name="json-representation"></a><span data-ttu-id="7d36c-108">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7d36c-108">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.asyncJobStatus", "@type.aka": "oneDrive.asyncOperationStatus" } -->

```json
{
  "percentageComplete": 100.0,
  "status": "notStarted | inProgress | completed | updating | failed | deletePending | deleteFailed | waiting"
}
```

## <a name="properties"></a><span data-ttu-id="7d36c-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="7d36c-109">Properties</span></span>

| <span data-ttu-id="7d36c-110">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="7d36c-110">Property name</span></span>          | <span data-ttu-id="7d36c-111">Тип</span><span class="sxs-lookup"><span data-stu-id="7d36c-111">Type</span></span>   | <span data-ttu-id="7d36c-112">Описание</span><span class="sxs-lookup"><span data-stu-id="7d36c-112">Description</span></span>                                                                                |
|:-----------------------|:-------|:-------------------------------------------------------------------------------------------|
| <span data-ttu-id="7d36c-113">**percentageComplete**</span><span class="sxs-lookup"><span data-stu-id="7d36c-113">**percentageComplete**</span></span> | <span data-ttu-id="7d36c-114">Double</span><span class="sxs-lookup"><span data-stu-id="7d36c-114">Double</span></span> | <span data-ttu-id="7d36c-115">Значение от 0 до 100, указывающее процент выполнения.</span><span class="sxs-lookup"><span data-stu-id="7d36c-115">A value between 0 and 100 that indicates the percentage complete.</span></span>                          |
| <span data-ttu-id="7d36c-116">**status**</span><span class="sxs-lookup"><span data-stu-id="7d36c-116">**status**</span></span>             | <span data-ttu-id="7d36c-117">Строка</span><span class="sxs-lookup"><span data-stu-id="7d36c-117">String</span></span> | <span data-ttu-id="7d36c-118">Строковое значение, сопоставляемое с перечислением возможных значений состояния задания.</span><span class="sxs-lookup"><span data-stu-id="7d36c-118">A string value that maps to an enumeration of possible values about the status of the job.</span></span> |

<!--
{
  "type": "#page.annotation",
  "description": "AsyncJobResource provides details about how to poll for an async completion.",
  "keywords": "async,job status,async status,copy,upload from url",
  "section": "documentation",
  "suppressions": []
}
-->
