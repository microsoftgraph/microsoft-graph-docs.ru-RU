---
title: тип ресурса domainState
description: Представляет состояние асинхронных операций, запланированных в домене.
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 15189beb4441d606becc470f4fb3fbe14f4370c4
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761116"
---
# <a name="domainstate-resource-type"></a><span data-ttu-id="5ffcd-103">тип ресурса domainState</span><span class="sxs-lookup"><span data-stu-id="5ffcd-103">domainState resource type</span></span>

<span data-ttu-id="5ffcd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ffcd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ffcd-105">Представляет состояние асинхронных операций, запланированных в домене.</span><span class="sxs-lookup"><span data-stu-id="5ffcd-105">Represents the status of asynchronous operations scheduled on a domain.</span></span>

## <a name="properties"></a><span data-ttu-id="5ffcd-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="5ffcd-106">Properties</span></span>

| <span data-ttu-id="5ffcd-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="5ffcd-107">Property</span></span>   | <span data-ttu-id="5ffcd-108">Тип</span><span class="sxs-lookup"><span data-stu-id="5ffcd-108">Type</span></span> | <span data-ttu-id="5ffcd-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5ffcd-109">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="5ffcd-110">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="5ffcd-110">lastActionDateTime</span></span> | <span data-ttu-id="5ffcd-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ffcd-111">DateTimeOffset</span></span> | <span data-ttu-id="5ffcd-112">Timestamp для последнего действия.</span><span class="sxs-lookup"><span data-stu-id="5ffcd-112">Timestamp for when the last activity occurred.</span></span> <span data-ttu-id="5ffcd-113">Значение обновляется, когда запланирована операция, начинается асинхронная задача и когда операция завершается.</span><span class="sxs-lookup"><span data-stu-id="5ffcd-113">The value is updated when an operation is scheduled, the asynchronous task starts, and when the operation completes.</span></span> |
| <span data-ttu-id="5ffcd-114">операция</span><span class="sxs-lookup"><span data-stu-id="5ffcd-114">operation</span></span> | <span data-ttu-id="5ffcd-115">String</span><span class="sxs-lookup"><span data-stu-id="5ffcd-115">String</span></span> | <span data-ttu-id="5ffcd-116">Тип асинхронной операции.</span><span class="sxs-lookup"><span data-stu-id="5ffcd-116">Type of asynchronous operation.</span></span> <span data-ttu-id="5ffcd-117">Значения могут быть *ForceDelete или* *Проверка*</span><span class="sxs-lookup"><span data-stu-id="5ffcd-117">The values can be *ForceDelete* or *Verification*</span></span> |
| <span data-ttu-id="5ffcd-118">status</span><span class="sxs-lookup"><span data-stu-id="5ffcd-118">status</span></span> | <span data-ttu-id="5ffcd-119">String</span><span class="sxs-lookup"><span data-stu-id="5ffcd-119">String</span></span> | <span data-ttu-id="5ffcd-120">Текущее состояние операции.</span><span class="sxs-lookup"><span data-stu-id="5ffcd-120">Current status of the operation.</span></span> <br> <span data-ttu-id="5ffcd-121">*Запланированный* . Операция была запланирована, но не началась.</span><span class="sxs-lookup"><span data-stu-id="5ffcd-121">*Scheduled* - Operation has been scheduled but has not started.</span></span> <br> <span data-ttu-id="5ffcd-122">*InProgress* — задача запущена и находится в процессе выполнения.</span><span class="sxs-lookup"><span data-stu-id="5ffcd-122">*InProgress* - Task has started and is in progress.</span></span> <br> <span data-ttu-id="5ffcd-123">*Failed* - Operation has failed.</span><span class="sxs-lookup"><span data-stu-id="5ffcd-123">*Failed* - Operation has failed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5ffcd-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5ffcd-124">JSON representation</span></span>
<span data-ttu-id="5ffcd-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5ffcd-125">Here is a JSON representation of the resource.</span></span>

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


