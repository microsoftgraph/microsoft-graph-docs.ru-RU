---
title: Тип ресурса domainState
description: Представляет состояние асинхронных операций, запланированных для домена.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: cee5ef9e0d0f4a5ada0d9117f755c407d081461d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27963103"
---
# <a name="domainstate-resource-type"></a><span data-ttu-id="7fcdc-103">Тип ресурса domainState</span><span class="sxs-lookup"><span data-stu-id="7fcdc-103">domainState resource type</span></span>

> <span data-ttu-id="7fcdc-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7fcdc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7fcdc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7fcdc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7fcdc-106">Представляет состояние асинхронных операций, запланированных для домена.</span><span class="sxs-lookup"><span data-stu-id="7fcdc-106">Represents the status of asynchronous operations scheduled on a domain.</span></span>

## <a name="properties"></a><span data-ttu-id="7fcdc-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="7fcdc-107">Properties</span></span>

| <span data-ttu-id="7fcdc-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="7fcdc-108">Property</span></span>   | <span data-ttu-id="7fcdc-109">Тип</span><span class="sxs-lookup"><span data-stu-id="7fcdc-109">Type</span></span> | <span data-ttu-id="7fcdc-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7fcdc-110">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="7fcdc-111">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="7fcdc-111">lastActionDateTime</span></span> | <span data-ttu-id="7fcdc-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7fcdc-112">DateTimeOffset</span></span> | <span data-ttu-id="7fcdc-p102">Метка времени возникновения последнего действия. Это значение обновляется при планировании операции, запуске асинхронной задачи и завершении операции.</span><span class="sxs-lookup"><span data-stu-id="7fcdc-p102">Timestamp for when the last activity occurred. The value is updated when an operation is scheduled, the asynchronous task starts, and when the operation completes.</span></span> |
| <span data-ttu-id="7fcdc-115">операция</span><span class="sxs-lookup"><span data-stu-id="7fcdc-115">operation</span></span> | <span data-ttu-id="7fcdc-116">String</span><span class="sxs-lookup"><span data-stu-id="7fcdc-116">String</span></span> | <span data-ttu-id="7fcdc-p103">Тип асинхронной операции. Возможные значения: *ForceDelete* или *Verification*.</span><span class="sxs-lookup"><span data-stu-id="7fcdc-p103">Type of asynchronous operation. The values can be *ForceDelete* or *Verification*</span></span> |
| <span data-ttu-id="7fcdc-119">status</span><span class="sxs-lookup"><span data-stu-id="7fcdc-119">status</span></span> | <span data-ttu-id="7fcdc-120">String</span><span class="sxs-lookup"><span data-stu-id="7fcdc-120">String</span></span> | <span data-ttu-id="7fcdc-121">Текущее состояние операции.</span><span class="sxs-lookup"><span data-stu-id="7fcdc-121">Current status of the operation.</span></span> <br> <span data-ttu-id="7fcdc-122">*Scheduled* — операция запланирована, но еще не запущена.</span><span class="sxs-lookup"><span data-stu-id="7fcdc-122">*Scheduled* - Operation has been scheduled but has not started.</span></span> <br> <span data-ttu-id="7fcdc-123">*InProgress* — операция запущена и в настоящее время выполняется.</span><span class="sxs-lookup"><span data-stu-id="7fcdc-123">*InProgress* - Task has started and is in progress.</span></span> <br> <span data-ttu-id="7fcdc-124">*Failed* — не удалось выполнить операцию.</span><span class="sxs-lookup"><span data-stu-id="7fcdc-124">*Failed* - Operation has failed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7fcdc-125">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="7fcdc-125">JSON representation</span></span>
<span data-ttu-id="7fcdc-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7fcdc-126">Here is a JSON representation of the resource.</span></span>

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
