---
title: Тип ресурса Домаинстате
description: Представляет состояние асинхронных операций, запланированных в домене.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c1afe3402d20c534a3e976d21a4f00de969f20ee
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657121"
---
# <a name="domainstate-resource-type"></a><span data-ttu-id="f39aa-103">Тип ресурса Домаинстате</span><span class="sxs-lookup"><span data-stu-id="f39aa-103">domainState resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f39aa-104">Представляет состояние асинхронных операций, запланированных в домене.</span><span class="sxs-lookup"><span data-stu-id="f39aa-104">Represents the status of asynchronous operations scheduled on a domain.</span></span>

## <a name="properties"></a><span data-ttu-id="f39aa-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="f39aa-105">Properties</span></span>

| <span data-ttu-id="f39aa-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="f39aa-106">Property</span></span>   | <span data-ttu-id="f39aa-107">Тип</span><span class="sxs-lookup"><span data-stu-id="f39aa-107">Type</span></span> | <span data-ttu-id="f39aa-108">Описание</span><span class="sxs-lookup"><span data-stu-id="f39aa-108">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="f39aa-109">Ластактиондатетиме</span><span class="sxs-lookup"><span data-stu-id="f39aa-109">lastActionDateTime</span></span> | <span data-ttu-id="f39aa-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f39aa-110">DateTimeOffset</span></span> | <span data-ttu-id="f39aa-111">Временная метка времени последнего действия.</span><span class="sxs-lookup"><span data-stu-id="f39aa-111">Timestamp for when the last activity occurred.</span></span> <span data-ttu-id="f39aa-112">Значение обновляется при планировании операции асинхронная задача начинается и после завершения операции.</span><span class="sxs-lookup"><span data-stu-id="f39aa-112">The value is updated when an operation is scheduled, the asynchronous task starts, and when the operation completes.</span></span> |
| <span data-ttu-id="f39aa-113">восстановление</span><span class="sxs-lookup"><span data-stu-id="f39aa-113">operation</span></span> | <span data-ttu-id="f39aa-114">String</span><span class="sxs-lookup"><span data-stu-id="f39aa-114">String</span></span> | <span data-ttu-id="f39aa-115">Тип асинхронной операции.</span><span class="sxs-lookup"><span data-stu-id="f39aa-115">Type of asynchronous operation.</span></span> <span data-ttu-id="f39aa-116">Значения могут быть *форцеделете* или *верификацией*</span><span class="sxs-lookup"><span data-stu-id="f39aa-116">The values can be *ForceDelete* or *Verification*</span></span> |
| <span data-ttu-id="f39aa-117">status</span><span class="sxs-lookup"><span data-stu-id="f39aa-117">status</span></span> | <span data-ttu-id="f39aa-118">String</span><span class="sxs-lookup"><span data-stu-id="f39aa-118">String</span></span> | <span data-ttu-id="f39aa-119">Текущее состояние операции.</span><span class="sxs-lookup"><span data-stu-id="f39aa-119">Current status of the operation.</span></span> <br> <span data-ttu-id="f39aa-120">*Запланированная* операция запланирована, но еще не запущена.</span><span class="sxs-lookup"><span data-stu-id="f39aa-120">*Scheduled* - Operation has been scheduled but has not started.</span></span> <br> <span data-ttu-id="f39aa-121">*Выполнение* — задача запущена и выполняется.</span><span class="sxs-lookup"><span data-stu-id="f39aa-121">*InProgress* - Task has started and is in progress.</span></span> <br> <span data-ttu-id="f39aa-122">*Failed* — не удалось выполнить операцию.</span><span class="sxs-lookup"><span data-stu-id="f39aa-122">*Failed* - Operation has failed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f39aa-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f39aa-123">JSON representation</span></span>
<span data-ttu-id="f39aa-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f39aa-124">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
