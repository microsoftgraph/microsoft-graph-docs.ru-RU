---
title: Тип ресурса commsOperation
description: Состояние определенных длительных операций.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b7914bd9692b4d9a94294f9a09659467e10550a6
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642207"
---
# <a name="commsoperation-resource-type"></a><span data-ttu-id="9d4f6-103">Тип ресурса commsOperation</span><span class="sxs-lookup"><span data-stu-id="9d4f6-103">commsOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d4f6-104">Состояние определенных длительных операций.</span><span class="sxs-lookup"><span data-stu-id="9d4f6-104">The status of certain long-running operations.</span></span>

## <a name="methods"></a><span data-ttu-id="9d4f6-105">Методы</span><span class="sxs-lookup"><span data-stu-id="9d4f6-105">Methods</span></span>
<span data-ttu-id="9d4f6-106">Нет</span><span class="sxs-lookup"><span data-stu-id="9d4f6-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="9d4f6-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="9d4f6-107">Properties</span></span>

| <span data-ttu-id="9d4f6-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="9d4f6-108">Property</span></span>           | <span data-ttu-id="9d4f6-109">Тип</span><span class="sxs-lookup"><span data-stu-id="9d4f6-109">Type</span></span>                        | <span data-ttu-id="9d4f6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9d4f6-110">Description</span></span>                                                                     |
| :----------------- | :-------------------------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="9d4f6-111">clientContext</span><span class="sxs-lookup"><span data-stu-id="9d4f6-111">clientContext</span></span>      | <span data-ttu-id="9d4f6-112">String</span><span class="sxs-lookup"><span data-stu-id="9d4f6-112">String</span></span>                      | <span data-ttu-id="9d4f6-113">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="9d4f6-113">The client context.</span></span>                                                             |
| <span data-ttu-id="9d4f6-114">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9d4f6-114">createdDateTime</span></span>    | <span data-ttu-id="9d4f6-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d4f6-115">DateTimeOffset</span></span>              | <span data-ttu-id="9d4f6-116">Время начала операции.</span><span class="sxs-lookup"><span data-stu-id="9d4f6-116">The start time of the operation.</span></span>                                                |
| <span data-ttu-id="9d4f6-117">id</span><span class="sxs-lookup"><span data-stu-id="9d4f6-117">id</span></span>                 | <span data-ttu-id="9d4f6-118">String</span><span class="sxs-lookup"><span data-stu-id="9d4f6-118">String</span></span>                      | <span data-ttu-id="9d4f6-119">Идентификатор операции. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9d4f6-119">The operation id. Read-only.</span></span> <span data-ttu-id="9d4f6-120">Создается сервером.</span><span class="sxs-lookup"><span data-stu-id="9d4f6-120">Server generated.</span></span>                                  |
| <span data-ttu-id="9d4f6-121">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="9d4f6-121">lastActionDateTime</span></span> | <span data-ttu-id="9d4f6-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d4f6-122">DateTimeOffset</span></span>              | <span data-ttu-id="9d4f6-123">Время последнего действия операции.</span><span class="sxs-lookup"><span data-stu-id="9d4f6-123">The time of the last action of the operation.</span></span>                                   |
| <span data-ttu-id="9d4f6-124">resultInfo</span><span class="sxs-lookup"><span data-stu-id="9d4f6-124">resultInfo</span></span>         | [<span data-ttu-id="9d4f6-125">resultInfo</span><span class="sxs-lookup"><span data-stu-id="9d4f6-125">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="9d4f6-126">Сведения о результате.</span><span class="sxs-lookup"><span data-stu-id="9d4f6-126">The result information.</span></span> <span data-ttu-id="9d4f6-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9d4f6-127">Read-only.</span></span> <span data-ttu-id="9d4f6-128">Создается сервером.</span><span class="sxs-lookup"><span data-stu-id="9d4f6-128">Server generated.</span></span>                            |
| <span data-ttu-id="9d4f6-129">status</span><span class="sxs-lookup"><span data-stu-id="9d4f6-129">status</span></span>             | <span data-ttu-id="9d4f6-130">String</span><span class="sxs-lookup"><span data-stu-id="9d4f6-130">String</span></span>                      | <span data-ttu-id="9d4f6-131">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="9d4f6-131">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="9d4f6-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9d4f6-132">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="9d4f6-133">Связи</span><span class="sxs-lookup"><span data-stu-id="9d4f6-133">Relationships</span></span>
<span data-ttu-id="9d4f6-134">Нет</span><span class="sxs-lookup"><span data-stu-id="9d4f6-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9d4f6-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9d4f6-135">JSON representation</span></span>

<span data-ttu-id="9d4f6-136">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9d4f6-136">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="9d4f6-137">Пример</span><span class="sxs-lookup"><span data-stu-id="9d4f6-137">Example</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "commsOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/commsoperation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
