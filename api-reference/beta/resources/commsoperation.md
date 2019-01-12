---
title: Тип ресурса commsOperation
description: Состояние определенных длительных операций.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 79fc6801e95854b2530f8a28c13f7180ed02203f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957727"
---
# <a name="commsoperation-resource-type"></a><span data-ttu-id="54614-103">Тип ресурса commsOperation</span><span class="sxs-lookup"><span data-stu-id="54614-103">commsOperation resource type</span></span>

> <span data-ttu-id="54614-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="54614-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="54614-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54614-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="54614-106">Состояние определенных длительных операций.</span><span class="sxs-lookup"><span data-stu-id="54614-106">The status of certain long-running operations.</span></span>

## <a name="methods"></a><span data-ttu-id="54614-107">Методы</span><span class="sxs-lookup"><span data-stu-id="54614-107">Methods</span></span>
<span data-ttu-id="54614-108">Нет</span><span class="sxs-lookup"><span data-stu-id="54614-108">None</span></span>

## <a name="properties"></a><span data-ttu-id="54614-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="54614-109">Properties</span></span>

| <span data-ttu-id="54614-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="54614-110">Property</span></span>           | <span data-ttu-id="54614-111">Тип</span><span class="sxs-lookup"><span data-stu-id="54614-111">Type</span></span>                        | <span data-ttu-id="54614-112">Описание</span><span class="sxs-lookup"><span data-stu-id="54614-112">Description</span></span>                                                                     |
| :----------------- | :-------------------------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="54614-113">clientContext</span><span class="sxs-lookup"><span data-stu-id="54614-113">clientContext</span></span>      | <span data-ttu-id="54614-114">String</span><span class="sxs-lookup"><span data-stu-id="54614-114">String</span></span>                      | <span data-ttu-id="54614-115">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="54614-115">The client context.</span></span>                                                             |
| <span data-ttu-id="54614-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="54614-116">createdDateTime</span></span>    | <span data-ttu-id="54614-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54614-117">DateTimeOffset</span></span>              | <span data-ttu-id="54614-118">Время начала операции.</span><span class="sxs-lookup"><span data-stu-id="54614-118">The start time of the operation.</span></span>                                                |
| <span data-ttu-id="54614-119">id</span><span class="sxs-lookup"><span data-stu-id="54614-119">id</span></span>                 | <span data-ttu-id="54614-120">String</span><span class="sxs-lookup"><span data-stu-id="54614-120">String</span></span>                      | <span data-ttu-id="54614-121">Идентификатор операции. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="54614-121">The operation id. Read-only.</span></span> <span data-ttu-id="54614-122">Сервер, созданный.</span><span class="sxs-lookup"><span data-stu-id="54614-122">Server generated.</span></span>                                  |
| <span data-ttu-id="54614-123">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="54614-123">lastActionDateTime</span></span> | <span data-ttu-id="54614-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54614-124">DateTimeOffset</span></span>              | <span data-ttu-id="54614-125">Время последнего действия операции.</span><span class="sxs-lookup"><span data-stu-id="54614-125">The time of the last action of the operation.</span></span>                                   |
| <span data-ttu-id="54614-126">resultInfo</span><span class="sxs-lookup"><span data-stu-id="54614-126">resultInfo</span></span>         | [<span data-ttu-id="54614-127">resultInfo</span><span class="sxs-lookup"><span data-stu-id="54614-127">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="54614-128">Сведения о результатов.</span><span class="sxs-lookup"><span data-stu-id="54614-128">The result information.</span></span> <span data-ttu-id="54614-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="54614-129">Read-only.</span></span> <span data-ttu-id="54614-130">Сервер, созданный.</span><span class="sxs-lookup"><span data-stu-id="54614-130">Server generated.</span></span>                            |
| <span data-ttu-id="54614-131">status</span><span class="sxs-lookup"><span data-stu-id="54614-131">status</span></span>             | <span data-ttu-id="54614-132">String</span><span class="sxs-lookup"><span data-stu-id="54614-132">String</span></span>                      | <span data-ttu-id="54614-133">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="54614-133">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="54614-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="54614-134">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="54614-135">Связи</span><span class="sxs-lookup"><span data-stu-id="54614-135">Relationships</span></span>
<span data-ttu-id="54614-136">Нет</span><span class="sxs-lookup"><span data-stu-id="54614-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="54614-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="54614-137">JSON representation</span></span>

<span data-ttu-id="54614-138">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="54614-138">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="54614-139">Пример</span><span class="sxs-lookup"><span data-stu-id="54614-139">Example</span></span>

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
