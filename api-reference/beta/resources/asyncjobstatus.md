---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: AsyncJobStatus
localization_priority: Normal
ms.openlocfilehash: 74ead4ca8e45c5baebe3ea74377ce102d9e2ee88
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328652"
---
# <a name="asyncjobstatus-resource"></a><span data-ttu-id="d5f81-102">Ресурс AsyncJobStatus</span><span class="sxs-lookup"><span data-stu-id="d5f81-102">AsyncJobStatus resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5f81-103">Этот ресурс предоставляет сведения о ходе выполнения асинхронного задания.</span><span class="sxs-lookup"><span data-stu-id="d5f81-103">This resource provides information on the status of a asynchronous job progress.</span></span>

<span data-ttu-id="d5f81-104">Указанные ниже вызовы API возвращают ресурсы **AsyncJobStatus**.</span><span class="sxs-lookup"><span data-stu-id="d5f81-104">The following API calls return **AsyncJobStatus** resources:</span></span>

* [<span data-ttu-id="d5f81-105">Копирование элемента</span><span class="sxs-lookup"><span data-stu-id="d5f81-105">Copy Item</span></span>](../api/driveitem-copy.md)

## <a name="json-representation"></a><span data-ttu-id="d5f81-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d5f81-106">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.asyncJobStatus", "@type.aka": "oneDrive.asyncOperationStatus" } -->

```json
{
  "percentageComplete": 100.0,
  "status": "notStarted | inProgress | completed | updating | failed | deletePending | deleteFailed | waiting"
}
```

## <a name="properties"></a><span data-ttu-id="d5f81-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d5f81-107">Properties</span></span>

| <span data-ttu-id="d5f81-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="d5f81-108">Property name</span></span>          | <span data-ttu-id="d5f81-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d5f81-109">Type</span></span>   | <span data-ttu-id="d5f81-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d5f81-110">Description</span></span>                                                                                |
|:-----------------------|:-------|:-------------------------------------------------------------------------------------------|
| <span data-ttu-id="d5f81-111">**percentageComplete**</span><span class="sxs-lookup"><span data-stu-id="d5f81-111">**percentageComplete**</span></span> | <span data-ttu-id="d5f81-112">Double</span><span class="sxs-lookup"><span data-stu-id="d5f81-112">Double</span></span> | <span data-ttu-id="d5f81-113">Значение от 0 до 100, указывающее процент выполнения.</span><span class="sxs-lookup"><span data-stu-id="d5f81-113">A value between 0 and 100 that indicates the percentage complete.</span></span>                          |
| <span data-ttu-id="d5f81-114">**status**</span><span class="sxs-lookup"><span data-stu-id="d5f81-114">**status**</span></span>             | <span data-ttu-id="d5f81-115">Строка</span><span class="sxs-lookup"><span data-stu-id="d5f81-115">String</span></span> | <span data-ttu-id="d5f81-116">Строковое значение, сопоставляемое с перечислением возможных значений состояния задания.</span><span class="sxs-lookup"><span data-stu-id="d5f81-116">A string value that maps to an enumeration of possible values about the status of the job.</span></span> |

<!--
{
  "type": "#page.annotation",
  "description": "AsyncJobResource provides details about how to poll for an async completion.",
  "keywords": "async,job status,async status,copy,upload from url",
  "section": "documentation",
  "suppressions": []
}
-->
