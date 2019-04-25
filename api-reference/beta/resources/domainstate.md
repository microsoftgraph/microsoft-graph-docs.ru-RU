---
title: Тип ресурса Домаинстате
description: Представляет состояние асинхронных операций, запланированных в домене.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 39ded8e4ff3458ebaceea09b3003d0bd14be36cf
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543184"
---
# <a name="domainstate-resource-type"></a><span data-ttu-id="9ac44-103">Тип ресурса Домаинстате</span><span class="sxs-lookup"><span data-stu-id="9ac44-103">domainState resource type</span></span>

<span data-ttu-id="9ac44-104">Представляет состояние асинхронных операций, запланированных в домене.</span><span class="sxs-lookup"><span data-stu-id="9ac44-104">Represents the status of asynchronous operations scheduled on a domain.</span></span>

## <a name="properties"></a><span data-ttu-id="9ac44-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="9ac44-105">Properties</span></span>

| <span data-ttu-id="9ac44-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="9ac44-106">Property</span></span>   | <span data-ttu-id="9ac44-107">Тип</span><span class="sxs-lookup"><span data-stu-id="9ac44-107">Type</span></span> | <span data-ttu-id="9ac44-108">Описание</span><span class="sxs-lookup"><span data-stu-id="9ac44-108">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="9ac44-109">Ластактиондатетиме</span><span class="sxs-lookup"><span data-stu-id="9ac44-109">lastActionDateTime</span></span> | <span data-ttu-id="9ac44-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ac44-110">DateTimeOffset</span></span> | <span data-ttu-id="9ac44-111">Временная метка времени последнего действия.</span><span class="sxs-lookup"><span data-stu-id="9ac44-111">Timestamp for when the last activity occurred.</span></span> <span data-ttu-id="9ac44-112">Значение обновляется при планировании операции асинхронная задача начинается и после завершения операции.</span><span class="sxs-lookup"><span data-stu-id="9ac44-112">The value is updated when an operation is scheduled, the asynchronous task starts, and when the operation completes.</span></span> |
| <span data-ttu-id="9ac44-113">восстановление</span><span class="sxs-lookup"><span data-stu-id="9ac44-113">operation</span></span> | <span data-ttu-id="9ac44-114">String</span><span class="sxs-lookup"><span data-stu-id="9ac44-114">String</span></span> | <span data-ttu-id="9ac44-115">Тип асинхронной операции.</span><span class="sxs-lookup"><span data-stu-id="9ac44-115">Type of asynchronous operation.</span></span> <span data-ttu-id="9ac44-116">Значения могут быть *форцеделете* или *верификацией*</span><span class="sxs-lookup"><span data-stu-id="9ac44-116">The values can be *ForceDelete* or *Verification*</span></span> |
| <span data-ttu-id="9ac44-117">status</span><span class="sxs-lookup"><span data-stu-id="9ac44-117">status</span></span> | <span data-ttu-id="9ac44-118">String</span><span class="sxs-lookup"><span data-stu-id="9ac44-118">String</span></span> | <span data-ttu-id="9ac44-119">Текущее состояние операции.</span><span class="sxs-lookup"><span data-stu-id="9ac44-119">Current status of the operation.</span></span> <br> <span data-ttu-id="9ac44-120">*Запланированная* операция запланирована, но еще не запущена.</span><span class="sxs-lookup"><span data-stu-id="9ac44-120">*Scheduled* - Operation has been scheduled but has not started.</span></span> <br> <span data-ttu-id="9ac44-121">*Выполнение* — задача запущена и выполняется.</span><span class="sxs-lookup"><span data-stu-id="9ac44-121">*InProgress* - Task has started and is in progress.</span></span> <br> <span data-ttu-id="9ac44-122">*Failed* — не удалось выполнить операцию.</span><span class="sxs-lookup"><span data-stu-id="9ac44-122">*Failed* - Operation has failed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9ac44-123">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="9ac44-123">JSON representation</span></span>
<span data-ttu-id="9ac44-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9ac44-124">Here is a JSON representation of the resource.</span></span>

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
