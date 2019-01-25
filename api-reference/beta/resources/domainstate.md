---
title: Тип ресурса domainState
description: Представляет состояние асинхронных операций, запланированных для домена.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 39ded8e4ff3458ebaceea09b3003d0bd14be36cf
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512978"
---
# <a name="domainstate-resource-type"></a><span data-ttu-id="c3dea-103">Тип ресурса domainState</span><span class="sxs-lookup"><span data-stu-id="c3dea-103">domainState resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3dea-104">Представляет состояние асинхронных операций, запланированных для домена.</span><span class="sxs-lookup"><span data-stu-id="c3dea-104">Represents the status of asynchronous operations scheduled on a domain.</span></span>

## <a name="properties"></a><span data-ttu-id="c3dea-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="c3dea-105">Properties</span></span>

| <span data-ttu-id="c3dea-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="c3dea-106">Property</span></span>   | <span data-ttu-id="c3dea-107">Тип</span><span class="sxs-lookup"><span data-stu-id="c3dea-107">Type</span></span> | <span data-ttu-id="c3dea-108">Описание</span><span class="sxs-lookup"><span data-stu-id="c3dea-108">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="c3dea-109">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="c3dea-109">lastActionDateTime</span></span> | <span data-ttu-id="c3dea-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3dea-110">DateTimeOffset</span></span> | <span data-ttu-id="c3dea-p101">Метка времени возникновения последнего действия. Это значение обновляется при планировании операции, запуске асинхронной задачи и завершении операции.</span><span class="sxs-lookup"><span data-stu-id="c3dea-p101">Timestamp for when the last activity occurred. The value is updated when an operation is scheduled, the asynchronous task starts, and when the operation completes.</span></span> |
| <span data-ttu-id="c3dea-113">операция</span><span class="sxs-lookup"><span data-stu-id="c3dea-113">operation</span></span> | <span data-ttu-id="c3dea-114">String</span><span class="sxs-lookup"><span data-stu-id="c3dea-114">String</span></span> | <span data-ttu-id="c3dea-p102">Тип асинхронной операции. Возможные значения: *ForceDelete* или *Verification*.</span><span class="sxs-lookup"><span data-stu-id="c3dea-p102">Type of asynchronous operation. The values can be *ForceDelete* or *Verification*</span></span> |
| <span data-ttu-id="c3dea-117">status</span><span class="sxs-lookup"><span data-stu-id="c3dea-117">status</span></span> | <span data-ttu-id="c3dea-118">String</span><span class="sxs-lookup"><span data-stu-id="c3dea-118">String</span></span> | <span data-ttu-id="c3dea-119">Текущее состояние операции.</span><span class="sxs-lookup"><span data-stu-id="c3dea-119">Current status of the operation.</span></span> <br> <span data-ttu-id="c3dea-120">*Scheduled* — операция запланирована, но еще не запущена.</span><span class="sxs-lookup"><span data-stu-id="c3dea-120">*Scheduled* - Operation has been scheduled but has not started.</span></span> <br> <span data-ttu-id="c3dea-121">*InProgress* — операция запущена и в настоящее время выполняется.</span><span class="sxs-lookup"><span data-stu-id="c3dea-121">*InProgress* - Task has started and is in progress.</span></span> <br> <span data-ttu-id="c3dea-122">*Failed* — не удалось выполнить операцию.</span><span class="sxs-lookup"><span data-stu-id="c3dea-122">*Failed* - Operation has failed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c3dea-123">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c3dea-123">JSON representation</span></span>
<span data-ttu-id="c3dea-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c3dea-124">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainState"
}-->

```json
{
  "lastActionDateTime": "String (timestamp)",
  "operation": "String",
  "status": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "domainState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/domainstate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
