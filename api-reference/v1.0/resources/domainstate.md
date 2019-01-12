---
title: Тип ресурса domainState
description: Представляет состояние асинхронных операций, запланированных для домена.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6a7741448b9c91be32f67f89cbafa5a579320083
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938295"
---
# <a name="domainstate-resource-type"></a><span data-ttu-id="54b64-103">Тип ресурса domainState</span><span class="sxs-lookup"><span data-stu-id="54b64-103">domainState resource type</span></span>

<span data-ttu-id="54b64-104">Представляет состояние асинхронных операций, запланированных для домена.</span><span class="sxs-lookup"><span data-stu-id="54b64-104">Represents the status of asynchronous operations scheduled on a domain.</span></span>

## <a name="properties"></a><span data-ttu-id="54b64-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="54b64-105">Properties</span></span>

| <span data-ttu-id="54b64-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="54b64-106">Property</span></span>   | <span data-ttu-id="54b64-107">Тип</span><span class="sxs-lookup"><span data-stu-id="54b64-107">Type</span></span> | <span data-ttu-id="54b64-108">Описание</span><span class="sxs-lookup"><span data-stu-id="54b64-108">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="54b64-109">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="54b64-109">lastActionDateTime</span></span> | <span data-ttu-id="54b64-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54b64-110">DateTimeOffset</span></span> | <span data-ttu-id="54b64-p101">Метка времени возникновения последнего действия. Это значение обновляется при планировании операции, запуске асинхронной задачи и завершении операции.</span><span class="sxs-lookup"><span data-stu-id="54b64-p101">Timestamp for when the last activity occurred. The value is updated when an operation is scheduled, the asynchronous task starts, and when the operation completes.</span></span> |
| <span data-ttu-id="54b64-113">операция</span><span class="sxs-lookup"><span data-stu-id="54b64-113">operation</span></span> | <span data-ttu-id="54b64-114">String</span><span class="sxs-lookup"><span data-stu-id="54b64-114">String</span></span> | <span data-ttu-id="54b64-p102">Тип асинхронной операции. Возможные значения: *ForceDelete* или *Verification*.</span><span class="sxs-lookup"><span data-stu-id="54b64-p102">Type of asynchronous operation. The values can be *ForceDelete* or *Verification*</span></span> |
| <span data-ttu-id="54b64-117">status</span><span class="sxs-lookup"><span data-stu-id="54b64-117">status</span></span> | <span data-ttu-id="54b64-118">String</span><span class="sxs-lookup"><span data-stu-id="54b64-118">String</span></span> | <span data-ttu-id="54b64-119">Текущее состояние операции.</span><span class="sxs-lookup"><span data-stu-id="54b64-119">Current status of the operation.</span></span> <br> <span data-ttu-id="54b64-120">*Scheduled* — операция запланирована, но еще не запущена.</span><span class="sxs-lookup"><span data-stu-id="54b64-120">*Scheduled* - Operation has been scheduled but has not started.</span></span> <br> <span data-ttu-id="54b64-121">*InProgress* — операция запущена и в настоящее время выполняется.</span><span class="sxs-lookup"><span data-stu-id="54b64-121">*InProgress* - Task has started and is in progress.</span></span> <br> <span data-ttu-id="54b64-122">*Failed* — не удалось выполнить операцию.</span><span class="sxs-lookup"><span data-stu-id="54b64-122">*Failed* - Operation has failed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="54b64-123">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="54b64-123">JSON representation</span></span>
<span data-ttu-id="54b64-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="54b64-124">Here is a JSON representation of the resource.</span></span>

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
