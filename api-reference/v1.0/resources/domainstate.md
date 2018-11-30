---
title: Тип ресурса domainState
description: Представляет состояние асинхронных операций, запланированных для домена.
ms.openlocfilehash: 73a83eddb46b9305a6d74e283bae1c009361195d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026918"
---
# <a name="domainstate-resource-type"></a><span data-ttu-id="b2569-103">Тип ресурса domainState</span><span class="sxs-lookup"><span data-stu-id="b2569-103">domainState resource type</span></span>

<span data-ttu-id="b2569-104">Представляет состояние асинхронных операций, запланированных для домена.</span><span class="sxs-lookup"><span data-stu-id="b2569-104">Represents the status of asynchronous operations scheduled on a domain.</span></span>

## <a name="properties"></a><span data-ttu-id="b2569-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="b2569-105">Properties</span></span>

| <span data-ttu-id="b2569-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="b2569-106">Property</span></span>   | <span data-ttu-id="b2569-107">Тип</span><span class="sxs-lookup"><span data-stu-id="b2569-107">Type</span></span> | <span data-ttu-id="b2569-108">Описание</span><span class="sxs-lookup"><span data-stu-id="b2569-108">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="b2569-109">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="b2569-109">lastActionDateTime</span></span> | <span data-ttu-id="b2569-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2569-110">DateTimeOffset</span></span> | <span data-ttu-id="b2569-p101">Метка времени возникновения последнего действия. Это значение обновляется при планировании операции, запуске асинхронной задачи и завершении операции.</span><span class="sxs-lookup"><span data-stu-id="b2569-p101">Timestamp for when the last activity occurred. The value is updated when an operation is scheduled, the asynchronous task starts, and when the operation completes.</span></span> |
| <span data-ttu-id="b2569-113">операция</span><span class="sxs-lookup"><span data-stu-id="b2569-113">operation</span></span> | <span data-ttu-id="b2569-114">String</span><span class="sxs-lookup"><span data-stu-id="b2569-114">String</span></span> | <span data-ttu-id="b2569-p102">Тип асинхронной операции. Возможные значения: *ForceDelete* или *Verification*.</span><span class="sxs-lookup"><span data-stu-id="b2569-p102">Type of asynchronous operation. The values can be *ForceDelete* or *Verification*</span></span> |
| <span data-ttu-id="b2569-117">status</span><span class="sxs-lookup"><span data-stu-id="b2569-117">status</span></span> | <span data-ttu-id="b2569-118">String</span><span class="sxs-lookup"><span data-stu-id="b2569-118">String</span></span> | <span data-ttu-id="b2569-119">Текущее состояние операции.</span><span class="sxs-lookup"><span data-stu-id="b2569-119">Current status of the operation.</span></span> <br> <span data-ttu-id="b2569-120">*Scheduled* — операция запланирована, но еще не запущена.</span><span class="sxs-lookup"><span data-stu-id="b2569-120">*Scheduled* - Operation has been scheduled but has not started.</span></span> <br> <span data-ttu-id="b2569-121">*InProgress* — операция запущена и в настоящее время выполняется.</span><span class="sxs-lookup"><span data-stu-id="b2569-121">*InProgress* - Task has started and is in progress.</span></span> <br> <span data-ttu-id="b2569-122">*Failed* — не удалось выполнить операцию.</span><span class="sxs-lookup"><span data-stu-id="b2569-122">*Failed* - Operation has failed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b2569-123">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b2569-123">JSON representation</span></span>
<span data-ttu-id="b2569-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b2569-124">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "domainState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->