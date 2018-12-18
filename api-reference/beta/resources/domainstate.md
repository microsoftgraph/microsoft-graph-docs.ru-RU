---
title: Тип ресурса domainState
description: Представляет состояние асинхронных операций, запланированных для домена.
author: lleonard-msft
ms.openlocfilehash: 683390998254cbf3f7146d1fe89a0a2f109be320
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27355890"
---
# <a name="domainstate-resource-type"></a><span data-ttu-id="4b67e-103">Тип ресурса domainState</span><span class="sxs-lookup"><span data-stu-id="4b67e-103">domainState resource type</span></span>

> <span data-ttu-id="4b67e-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4b67e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4b67e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b67e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4b67e-106">Представляет состояние асинхронных операций, запланированных для домена.</span><span class="sxs-lookup"><span data-stu-id="4b67e-106">Represents the status of asynchronous operations scheduled on a domain.</span></span>

## <a name="properties"></a><span data-ttu-id="4b67e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4b67e-107">Properties</span></span>

| <span data-ttu-id="4b67e-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="4b67e-108">Property</span></span>   | <span data-ttu-id="4b67e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4b67e-109">Type</span></span> | <span data-ttu-id="4b67e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4b67e-110">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="4b67e-111">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="4b67e-111">lastActionDateTime</span></span> | <span data-ttu-id="4b67e-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b67e-112">DateTimeOffset</span></span> | <span data-ttu-id="4b67e-p102">Метка времени возникновения последнего действия. Это значение обновляется при планировании операции, запуске асинхронной задачи и завершении операции.</span><span class="sxs-lookup"><span data-stu-id="4b67e-p102">Timestamp for when the last activity occurred. The value is updated when an operation is scheduled, the asynchronous task starts, and when the operation completes.</span></span> |
| <span data-ttu-id="4b67e-115">операция</span><span class="sxs-lookup"><span data-stu-id="4b67e-115">operation</span></span> | <span data-ttu-id="4b67e-116">String</span><span class="sxs-lookup"><span data-stu-id="4b67e-116">String</span></span> | <span data-ttu-id="4b67e-p103">Тип асинхронной операции. Возможные значения: *ForceDelete* или *Verification*.</span><span class="sxs-lookup"><span data-stu-id="4b67e-p103">Type of asynchronous operation. The values can be *ForceDelete* or *Verification*</span></span> |
| <span data-ttu-id="4b67e-119">status</span><span class="sxs-lookup"><span data-stu-id="4b67e-119">status</span></span> | <span data-ttu-id="4b67e-120">String</span><span class="sxs-lookup"><span data-stu-id="4b67e-120">String</span></span> | <span data-ttu-id="4b67e-121">Текущее состояние операции.</span><span class="sxs-lookup"><span data-stu-id="4b67e-121">Current status of the operation.</span></span> <br> <span data-ttu-id="4b67e-122">*Scheduled* — операция запланирована, но еще не запущена.</span><span class="sxs-lookup"><span data-stu-id="4b67e-122">*Scheduled* - Operation has been scheduled but has not started.</span></span> <br> <span data-ttu-id="4b67e-123">*InProgress* — операция запущена и в настоящее время выполняется.</span><span class="sxs-lookup"><span data-stu-id="4b67e-123">*InProgress* - Task has started and is in progress.</span></span> <br> <span data-ttu-id="4b67e-124">*Failed* — не удалось выполнить операцию.</span><span class="sxs-lookup"><span data-stu-id="4b67e-124">*Failed* - Operation has failed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4b67e-125">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4b67e-125">JSON representation</span></span>
<span data-ttu-id="4b67e-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4b67e-126">Here is a JSON representation of the resource.</span></span>

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