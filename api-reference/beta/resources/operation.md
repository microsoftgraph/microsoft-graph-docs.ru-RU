---
title: Тип ресурса операции
description: Состояние выполнения длительной операции.
ms.openlocfilehash: 71e6a1c47e1f3b18f1481700320779714d716bec
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077502"
---
# <a name="operation-resource-type"></a><span data-ttu-id="2b88d-103">Тип ресурса операции</span><span class="sxs-lookup"><span data-stu-id="2b88d-103">operation resource type</span></span>

> <span data-ttu-id="2b88d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2b88d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2b88d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b88d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2b88d-106">Состояние выполнения длительной операции.</span><span class="sxs-lookup"><span data-stu-id="2b88d-106">The status of a long-running operation.</span></span>

## <a name="methods"></a><span data-ttu-id="2b88d-107">Методы</span><span class="sxs-lookup"><span data-stu-id="2b88d-107">Methods</span></span>

<span data-ttu-id="2b88d-108">Нет</span><span class="sxs-lookup"><span data-stu-id="2b88d-108">None</span></span>

## <a name="properties"></a><span data-ttu-id="2b88d-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="2b88d-109">Properties</span></span>

| <span data-ttu-id="2b88d-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="2b88d-110">Property</span></span>           | <span data-ttu-id="2b88d-111">Тип</span><span class="sxs-lookup"><span data-stu-id="2b88d-111">Type</span></span>            | <span data-ttu-id="2b88d-112">Описание</span><span class="sxs-lookup"><span data-stu-id="2b88d-112">Description</span></span>                                                                     |
| :----------------- | :-------------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="2b88d-113">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2b88d-113">createdDateTime</span></span>    | <span data-ttu-id="2b88d-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b88d-114">DateTimeOffset</span></span>  | <span data-ttu-id="2b88d-115">Время начала операции.</span><span class="sxs-lookup"><span data-stu-id="2b88d-115">The start time of the operation.</span></span>                                                |
| <span data-ttu-id="2b88d-116">id</span><span class="sxs-lookup"><span data-stu-id="2b88d-116">id</span></span>                 | <span data-ttu-id="2b88d-117">String</span><span class="sxs-lookup"><span data-stu-id="2b88d-117">String</span></span>          | <span data-ttu-id="2b88d-118">Идентификатор операции. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2b88d-118">The operation id. Read-only.</span></span> <span data-ttu-id="2b88d-119">Сервер, созданный.</span><span class="sxs-lookup"><span data-stu-id="2b88d-119">Server generated.</span></span>                                  |
| <span data-ttu-id="2b88d-120">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="2b88d-120">lastActionDateTime</span></span> | <span data-ttu-id="2b88d-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b88d-121">DateTimeOffset</span></span>  | <span data-ttu-id="2b88d-122">Время последнего действия операции.</span><span class="sxs-lookup"><span data-stu-id="2b88d-122">The time of the last action of the operation.</span></span>                                   |
| <span data-ttu-id="2b88d-123">status</span><span class="sxs-lookup"><span data-stu-id="2b88d-123">status</span></span>             | <span data-ttu-id="2b88d-124">String</span><span class="sxs-lookup"><span data-stu-id="2b88d-124">String</span></span>          | <span data-ttu-id="2b88d-125">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="2b88d-125">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="2b88d-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2b88d-126">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="2b88d-127">Связи</span><span class="sxs-lookup"><span data-stu-id="2b88d-127">Relationships</span></span>

<span data-ttu-id="2b88d-128">Нет</span><span class="sxs-lookup"><span data-stu-id="2b88d-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2b88d-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2b88d-129">JSON representation</span></span>

<span data-ttu-id="2b88d-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2b88d-130">The following is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.operation"
}-->
```json
{
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "status": "notStarted | running | completed | failed"
}
```

## <a name="example"></a><span data-ttu-id="2b88d-131">Пример</span><span class="sxs-lookup"><span data-stu-id="2b88d-131">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.operation"
}-->
```json
{
  "createdDateTime": "2018-09-06T15:58:41Z",
  "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "status": "completed"
}
```

<!-- uuid: 13fa92b1-3b41-498b-aab1-f943464a124f
2018-03-30 10:29:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->