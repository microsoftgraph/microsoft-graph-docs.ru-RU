---
title: Тип ресурса Коммсоператион
description: Состояние определенных длительных операций.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b7914bd9692b4d9a94294f9a09659467e10550a6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32460599"
---
# <a name="commsoperation-resource-type"></a><span data-ttu-id="d59a2-103">Тип ресурса Коммсоператион</span><span class="sxs-lookup"><span data-stu-id="d59a2-103">commsOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d59a2-104">Состояние определенных длительных операций.</span><span class="sxs-lookup"><span data-stu-id="d59a2-104">The status of certain long-running operations.</span></span>

## <a name="methods"></a><span data-ttu-id="d59a2-105">Методы</span><span class="sxs-lookup"><span data-stu-id="d59a2-105">Methods</span></span>
<span data-ttu-id="d59a2-106">Нет</span><span class="sxs-lookup"><span data-stu-id="d59a2-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="d59a2-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d59a2-107">Properties</span></span>

| <span data-ttu-id="d59a2-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d59a2-108">Property</span></span>           | <span data-ttu-id="d59a2-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d59a2-109">Type</span></span>                        | <span data-ttu-id="d59a2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d59a2-110">Description</span></span>                                                                     |
| :----------------- | :-------------------------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="d59a2-111">Контекст</span><span class="sxs-lookup"><span data-stu-id="d59a2-111">clientContext</span></span>      | <span data-ttu-id="d59a2-112">String</span><span class="sxs-lookup"><span data-stu-id="d59a2-112">String</span></span>                      | <span data-ttu-id="d59a2-113">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="d59a2-113">The client context.</span></span>                                                             |
| <span data-ttu-id="d59a2-114">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d59a2-114">createdDateTime</span></span>    | <span data-ttu-id="d59a2-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d59a2-115">DateTimeOffset</span></span>              | <span data-ttu-id="d59a2-116">Время начала операции.</span><span class="sxs-lookup"><span data-stu-id="d59a2-116">The start time of the operation.</span></span>                                                |
| <span data-ttu-id="d59a2-117">id</span><span class="sxs-lookup"><span data-stu-id="d59a2-117">id</span></span>                 | <span data-ttu-id="d59a2-118">String</span><span class="sxs-lookup"><span data-stu-id="d59a2-118">String</span></span>                      | <span data-ttu-id="d59a2-119">Идентификатор операции. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d59a2-119">The operation id. Read-only.</span></span> <span data-ttu-id="d59a2-120">Создается сервером.</span><span class="sxs-lookup"><span data-stu-id="d59a2-120">Server generated.</span></span>                                  |
| <span data-ttu-id="d59a2-121">Ластактиондатетиме</span><span class="sxs-lookup"><span data-stu-id="d59a2-121">lastActionDateTime</span></span> | <span data-ttu-id="d59a2-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d59a2-122">DateTimeOffset</span></span>              | <span data-ttu-id="d59a2-123">Время последнего действия операции.</span><span class="sxs-lookup"><span data-stu-id="d59a2-123">The time of the last action of the operation.</span></span>                                   |
| <span data-ttu-id="d59a2-124">resultInfo</span><span class="sxs-lookup"><span data-stu-id="d59a2-124">resultInfo</span></span>         | [<span data-ttu-id="d59a2-125">resultInfo</span><span class="sxs-lookup"><span data-stu-id="d59a2-125">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="d59a2-126">Сведения о результате.</span><span class="sxs-lookup"><span data-stu-id="d59a2-126">The result information.</span></span> <span data-ttu-id="d59a2-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d59a2-127">Read-only.</span></span> <span data-ttu-id="d59a2-128">Создается сервером.</span><span class="sxs-lookup"><span data-stu-id="d59a2-128">Server generated.</span></span>                            |
| <span data-ttu-id="d59a2-129">status</span><span class="sxs-lookup"><span data-stu-id="d59a2-129">status</span></span>             | <span data-ttu-id="d59a2-130">String</span><span class="sxs-lookup"><span data-stu-id="d59a2-130">String</span></span>                      | <span data-ttu-id="d59a2-131">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="d59a2-131">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="d59a2-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d59a2-132">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="d59a2-133">Отношения</span><span class="sxs-lookup"><span data-stu-id="d59a2-133">Relationships</span></span>
<span data-ttu-id="d59a2-134">Нет</span><span class="sxs-lookup"><span data-stu-id="d59a2-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d59a2-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d59a2-135">JSON representation</span></span>

<span data-ttu-id="d59a2-136">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d59a2-136">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="d59a2-137">Пример</span><span class="sxs-lookup"><span data-stu-id="d59a2-137">Example</span></span>

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
