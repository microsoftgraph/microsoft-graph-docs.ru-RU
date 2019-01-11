---
title: Тип ресурса commsOperation
description: Состояние определенных длительных операций.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: d70ad6535d5ae829de4b9bac3c5b9fea9b53188b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821450"
---
# <a name="commsoperation-resource-type"></a><span data-ttu-id="8899d-103">Тип ресурса commsOperation</span><span class="sxs-lookup"><span data-stu-id="8899d-103">commsOperation resource type</span></span>

> <span data-ttu-id="8899d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8899d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8899d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8899d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8899d-106">Состояние определенных длительных операций.</span><span class="sxs-lookup"><span data-stu-id="8899d-106">The status of certain long-running operations.</span></span>

## <a name="methods"></a><span data-ttu-id="8899d-107">Методы</span><span class="sxs-lookup"><span data-stu-id="8899d-107">Methods</span></span>
<span data-ttu-id="8899d-108">Нет</span><span class="sxs-lookup"><span data-stu-id="8899d-108">None</span></span>

## <a name="properties"></a><span data-ttu-id="8899d-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="8899d-109">Properties</span></span>

| <span data-ttu-id="8899d-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="8899d-110">Property</span></span>           | <span data-ttu-id="8899d-111">Тип</span><span class="sxs-lookup"><span data-stu-id="8899d-111">Type</span></span>                        | <span data-ttu-id="8899d-112">Описание</span><span class="sxs-lookup"><span data-stu-id="8899d-112">Description</span></span>                                                                     |
| :----------------- | :-------------------------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="8899d-113">clientContext</span><span class="sxs-lookup"><span data-stu-id="8899d-113">clientContext</span></span>      | <span data-ttu-id="8899d-114">Строка</span><span class="sxs-lookup"><span data-stu-id="8899d-114">String</span></span>                      | <span data-ttu-id="8899d-115">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="8899d-115">The client context.</span></span>                                                             |
| <span data-ttu-id="8899d-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8899d-116">createdDateTime</span></span>    | <span data-ttu-id="8899d-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8899d-117">DateTimeOffset</span></span>              | <span data-ttu-id="8899d-118">Время начала операции.</span><span class="sxs-lookup"><span data-stu-id="8899d-118">The start time of the operation.</span></span>                                                |
| <span data-ttu-id="8899d-119">id</span><span class="sxs-lookup"><span data-stu-id="8899d-119">id</span></span>                 | <span data-ttu-id="8899d-120">Строка</span><span class="sxs-lookup"><span data-stu-id="8899d-120">String</span></span>                      | <span data-ttu-id="8899d-121">Идентификатор операции. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8899d-121">The operation id. Read-only.</span></span> <span data-ttu-id="8899d-122">Сервер, созданный.</span><span class="sxs-lookup"><span data-stu-id="8899d-122">Server generated.</span></span>                                  |
| <span data-ttu-id="8899d-123">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="8899d-123">lastActionDateTime</span></span> | <span data-ttu-id="8899d-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8899d-124">DateTimeOffset</span></span>              | <span data-ttu-id="8899d-125">Время последнего действия операции.</span><span class="sxs-lookup"><span data-stu-id="8899d-125">The time of the last action of the operation.</span></span>                                   |
| <span data-ttu-id="8899d-126">resultInfo</span><span class="sxs-lookup"><span data-stu-id="8899d-126">resultInfo</span></span>         | [<span data-ttu-id="8899d-127">resultInfo</span><span class="sxs-lookup"><span data-stu-id="8899d-127">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="8899d-128">Сведения о результатов.</span><span class="sxs-lookup"><span data-stu-id="8899d-128">The result information.</span></span> <span data-ttu-id="8899d-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8899d-129">Read-only.</span></span> <span data-ttu-id="8899d-130">Сервер, созданный.</span><span class="sxs-lookup"><span data-stu-id="8899d-130">Server generated.</span></span>                            |
| <span data-ttu-id="8899d-131">status</span><span class="sxs-lookup"><span data-stu-id="8899d-131">status</span></span>             | <span data-ttu-id="8899d-132">Строка</span><span class="sxs-lookup"><span data-stu-id="8899d-132">String</span></span>                      | <span data-ttu-id="8899d-133">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="8899d-133">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="8899d-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8899d-134">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="8899d-135">Связи</span><span class="sxs-lookup"><span data-stu-id="8899d-135">Relationships</span></span>
<span data-ttu-id="8899d-136">Нет</span><span class="sxs-lookup"><span data-stu-id="8899d-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8899d-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8899d-137">JSON representation</span></span>

<span data-ttu-id="8899d-138">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8899d-138">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.commsOperation"
}-->
```json
{
  "clientContext": "String",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "resultInfo": { "@odata.type": "#microsoft.graph.resultInfo" },
  "status": "notStarted | running | completed | failed"
}
```

## <a name="example"></a><span data-ttu-id="8899d-139">Пример</span><span class="sxs-lookup"><span data-stu-id="8899d-139">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsOperation"
}-->
```json
{
  "clientContext": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "createdDateTime": "2018-09-06T15:58:41Z",
  "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "resultInfo": {
    "@odata.type": "#microsoft.graph.resultInfo",
    "code": "200"
  },
  "status": "completed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "commsOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
