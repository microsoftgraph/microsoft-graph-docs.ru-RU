---
title: Тип ресурса Домаинстате
description: Представляет состояние асинхронных операций, запланированных в домене.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 66d5d5b57cb5ef30054a6187e34caf8713b6e63b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42505807"
---
# <a name="domainstate-resource-type"></a><span data-ttu-id="e2dfd-103">Тип ресурса Домаинстате</span><span class="sxs-lookup"><span data-stu-id="e2dfd-103">domainState resource type</span></span>

<span data-ttu-id="e2dfd-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e2dfd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2dfd-105">Представляет состояние асинхронных операций, запланированных в домене.</span><span class="sxs-lookup"><span data-stu-id="e2dfd-105">Represents the status of asynchronous operations scheduled on a domain.</span></span>

## <a name="properties"></a><span data-ttu-id="e2dfd-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e2dfd-106">Properties</span></span>

| <span data-ttu-id="e2dfd-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="e2dfd-107">Property</span></span>   | <span data-ttu-id="e2dfd-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e2dfd-108">Type</span></span> | <span data-ttu-id="e2dfd-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e2dfd-109">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="e2dfd-110">ластактиондатетиме</span><span class="sxs-lookup"><span data-stu-id="e2dfd-110">lastActionDateTime</span></span> | <span data-ttu-id="e2dfd-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2dfd-111">DateTimeOffset</span></span> | <span data-ttu-id="e2dfd-112">Временная метка времени последнего действия.</span><span class="sxs-lookup"><span data-stu-id="e2dfd-112">Timestamp for when the last activity occurred.</span></span> <span data-ttu-id="e2dfd-113">Значение обновляется при планировании операции асинхронная задача начинается и после завершения операции.</span><span class="sxs-lookup"><span data-stu-id="e2dfd-113">The value is updated when an operation is scheduled, the asynchronous task starts, and when the operation completes.</span></span> |
| <span data-ttu-id="e2dfd-114">восстановление</span><span class="sxs-lookup"><span data-stu-id="e2dfd-114">operation</span></span> | <span data-ttu-id="e2dfd-115">String</span><span class="sxs-lookup"><span data-stu-id="e2dfd-115">String</span></span> | <span data-ttu-id="e2dfd-116">Тип асинхронной операции.</span><span class="sxs-lookup"><span data-stu-id="e2dfd-116">Type of asynchronous operation.</span></span> <span data-ttu-id="e2dfd-117">Значения могут быть *форцеделете* или *верификацией*</span><span class="sxs-lookup"><span data-stu-id="e2dfd-117">The values can be *ForceDelete* or *Verification*</span></span> |
| <span data-ttu-id="e2dfd-118">status</span><span class="sxs-lookup"><span data-stu-id="e2dfd-118">status</span></span> | <span data-ttu-id="e2dfd-119">String</span><span class="sxs-lookup"><span data-stu-id="e2dfd-119">String</span></span> | <span data-ttu-id="e2dfd-120">Текущее состояние операции.</span><span class="sxs-lookup"><span data-stu-id="e2dfd-120">Current status of the operation.</span></span> <br> <span data-ttu-id="e2dfd-121">*Запланированная* операция запланирована, но еще не запущена.</span><span class="sxs-lookup"><span data-stu-id="e2dfd-121">*Scheduled* - Operation has been scheduled but has not started.</span></span> <br> <span data-ttu-id="e2dfd-122">*Выполнение* — задача запущена и выполняется.</span><span class="sxs-lookup"><span data-stu-id="e2dfd-122">*InProgress* - Task has started and is in progress.</span></span> <br> <span data-ttu-id="e2dfd-123">*Failed* — не удалось выполнить операцию.</span><span class="sxs-lookup"><span data-stu-id="e2dfd-123">*Failed* - Operation has failed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e2dfd-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e2dfd-124">JSON representation</span></span>
<span data-ttu-id="e2dfd-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e2dfd-125">Here is a JSON representation of the resource.</span></span>

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
