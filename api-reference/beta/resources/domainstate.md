---
title: Тип ресурса Домаинстате
description: Представляет состояние асинхронных операций, запланированных в домене.
author: adimitui
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 86c5bc7fa987b137b7e11fe9ff825939e95d4426
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181752"
---
# <a name="domainstate-resource-type"></a><span data-ttu-id="a2caf-103">Тип ресурса Домаинстате</span><span class="sxs-lookup"><span data-stu-id="a2caf-103">domainState resource type</span></span>

<span data-ttu-id="a2caf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2caf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2caf-105">Представляет состояние асинхронных операций, запланированных в домене.</span><span class="sxs-lookup"><span data-stu-id="a2caf-105">Represents the status of asynchronous operations scheduled on a domain.</span></span>

## <a name="properties"></a><span data-ttu-id="a2caf-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a2caf-106">Properties</span></span>

| <span data-ttu-id="a2caf-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="a2caf-107">Property</span></span>   | <span data-ttu-id="a2caf-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a2caf-108">Type</span></span> | <span data-ttu-id="a2caf-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a2caf-109">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="a2caf-110">ластактиондатетиме</span><span class="sxs-lookup"><span data-stu-id="a2caf-110">lastActionDateTime</span></span> | <span data-ttu-id="a2caf-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2caf-111">DateTimeOffset</span></span> | <span data-ttu-id="a2caf-112">Временная метка времени последнего действия.</span><span class="sxs-lookup"><span data-stu-id="a2caf-112">Timestamp for when the last activity occurred.</span></span> <span data-ttu-id="a2caf-113">Значение обновляется при планировании операции асинхронная задача начинается и после завершения операции.</span><span class="sxs-lookup"><span data-stu-id="a2caf-113">The value is updated when an operation is scheduled, the asynchronous task starts, and when the operation completes.</span></span> |
| <span data-ttu-id="a2caf-114">восстановление</span><span class="sxs-lookup"><span data-stu-id="a2caf-114">operation</span></span> | <span data-ttu-id="a2caf-115">String</span><span class="sxs-lookup"><span data-stu-id="a2caf-115">String</span></span> | <span data-ttu-id="a2caf-116">Тип асинхронной операции.</span><span class="sxs-lookup"><span data-stu-id="a2caf-116">Type of asynchronous operation.</span></span> <span data-ttu-id="a2caf-117">Значения могут быть *форцеделете* или *верификацией*</span><span class="sxs-lookup"><span data-stu-id="a2caf-117">The values can be *ForceDelete* or *Verification*</span></span> |
| <span data-ttu-id="a2caf-118">status</span><span class="sxs-lookup"><span data-stu-id="a2caf-118">status</span></span> | <span data-ttu-id="a2caf-119">String</span><span class="sxs-lookup"><span data-stu-id="a2caf-119">String</span></span> | <span data-ttu-id="a2caf-120">Текущее состояние операции.</span><span class="sxs-lookup"><span data-stu-id="a2caf-120">Current status of the operation.</span></span> <br> <span data-ttu-id="a2caf-121">*Запланированная* операция запланирована, но еще не запущена.</span><span class="sxs-lookup"><span data-stu-id="a2caf-121">*Scheduled* - Operation has been scheduled but has not started.</span></span> <br> <span data-ttu-id="a2caf-122">*Выполнение* — задача запущена и выполняется.</span><span class="sxs-lookup"><span data-stu-id="a2caf-122">*InProgress* - Task has started and is in progress.</span></span> <br> <span data-ttu-id="a2caf-123">*Failed* — не удалось выполнить операцию.</span><span class="sxs-lookup"><span data-stu-id="a2caf-123">*Failed* - Operation has failed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a2caf-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a2caf-124">JSON representation</span></span>
<span data-ttu-id="a2caf-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a2caf-125">Here is a JSON representation of the resource.</span></span>

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
