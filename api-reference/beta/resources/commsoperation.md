---
title: Тип ресурса Коммсоператион
description: Состояние определенных длительных операций.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a10b652179a8a3d369c07d34cb2681c4986b3abf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012900"
---
# <a name="commsoperation-resource-type"></a><span data-ttu-id="a5db1-103">Тип ресурса Коммсоператион</span><span class="sxs-lookup"><span data-stu-id="a5db1-103">commsOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5db1-104">Состояние определенных длительных операций.</span><span class="sxs-lookup"><span data-stu-id="a5db1-104">The status of certain long-running operations.</span></span>

## <a name="methods"></a><span data-ttu-id="a5db1-105">Методы</span><span class="sxs-lookup"><span data-stu-id="a5db1-105">Methods</span></span>
<span data-ttu-id="a5db1-106">Нет</span><span class="sxs-lookup"><span data-stu-id="a5db1-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="a5db1-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a5db1-107">Properties</span></span>

| <span data-ttu-id="a5db1-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a5db1-108">Property</span></span>           | <span data-ttu-id="a5db1-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a5db1-109">Type</span></span>                        | <span data-ttu-id="a5db1-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a5db1-110">Description</span></span>                                                                     |
| :----------------- | :-------------------------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="a5db1-111">Контекст</span><span class="sxs-lookup"><span data-stu-id="a5db1-111">clientContext</span></span>      | <span data-ttu-id="a5db1-112">String</span><span class="sxs-lookup"><span data-stu-id="a5db1-112">String</span></span>                      | <span data-ttu-id="a5db1-113">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="a5db1-113">The client context.</span></span>                                                             |
| <span data-ttu-id="a5db1-114">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a5db1-114">createdDateTime</span></span>    | <span data-ttu-id="a5db1-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a5db1-115">DateTimeOffset</span></span>              | <span data-ttu-id="a5db1-116">Время начала операции.</span><span class="sxs-lookup"><span data-stu-id="a5db1-116">The start time of the operation.</span></span>                                                |
| <span data-ttu-id="a5db1-117">id</span><span class="sxs-lookup"><span data-stu-id="a5db1-117">id</span></span>                 | <span data-ttu-id="a5db1-118">Строка</span><span class="sxs-lookup"><span data-stu-id="a5db1-118">String</span></span>                      | <span data-ttu-id="a5db1-119">Идентификатор операции. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a5db1-119">The operation id. Read-only.</span></span> <span data-ttu-id="a5db1-120">Создается сервером.</span><span class="sxs-lookup"><span data-stu-id="a5db1-120">Server generated.</span></span>                                  |
| <span data-ttu-id="a5db1-121">Ластактиондатетиме</span><span class="sxs-lookup"><span data-stu-id="a5db1-121">lastActionDateTime</span></span> | <span data-ttu-id="a5db1-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a5db1-122">DateTimeOffset</span></span>              | <span data-ttu-id="a5db1-123">Время последнего действия операции.</span><span class="sxs-lookup"><span data-stu-id="a5db1-123">The time of the last action of the operation.</span></span>                                   |
| <span data-ttu-id="a5db1-124">resultInfo</span><span class="sxs-lookup"><span data-stu-id="a5db1-124">resultInfo</span></span>         | [<span data-ttu-id="a5db1-125">resultInfo</span><span class="sxs-lookup"><span data-stu-id="a5db1-125">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="a5db1-126">Сведения о результате.</span><span class="sxs-lookup"><span data-stu-id="a5db1-126">The result information.</span></span> <span data-ttu-id="a5db1-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a5db1-127">Read-only.</span></span> <span data-ttu-id="a5db1-128">Создается сервером.</span><span class="sxs-lookup"><span data-stu-id="a5db1-128">Server generated.</span></span>                            |
| <span data-ttu-id="a5db1-129">status</span><span class="sxs-lookup"><span data-stu-id="a5db1-129">status</span></span>             | <span data-ttu-id="a5db1-130">String</span><span class="sxs-lookup"><span data-stu-id="a5db1-130">String</span></span>                      | <span data-ttu-id="a5db1-131">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="a5db1-131">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="a5db1-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a5db1-132">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="a5db1-133">Отношения</span><span class="sxs-lookup"><span data-stu-id="a5db1-133">Relationships</span></span>
<span data-ttu-id="a5db1-134">Нет</span><span class="sxs-lookup"><span data-stu-id="a5db1-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a5db1-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a5db1-135">JSON representation</span></span>

<span data-ttu-id="a5db1-136">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a5db1-136">The following is a JSON representation of the resource.</span></span>

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
  "resultInfo": { "@odata.type": "microsoft.graph.resultInfo" },
  "status": "notStarted | running | completed | failed"
}
```

## <a name="example"></a><span data-ttu-id="a5db1-137">Пример</span><span class="sxs-lookup"><span data-stu-id="a5db1-137">Example</span></span>

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
    "@odata.type": "microsoft.graph.resultInfo",
    "code": "200"
  },
  "status": "completed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "commsOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
