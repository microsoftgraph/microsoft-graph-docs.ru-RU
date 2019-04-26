---
title: Тип ресурса Operation
description: Состояние длительной операции.
localization_priority: Normal
ms.openlocfilehash: 3ad9848387dab2de928f7ace2fa4b905720be615
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568912"
---
# <a name="operation-resource-type"></a><span data-ttu-id="0f8fe-103">Тип ресурса Operation</span><span class="sxs-lookup"><span data-stu-id="0f8fe-103">operation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f8fe-104">Состояние длительной операции.</span><span class="sxs-lookup"><span data-stu-id="0f8fe-104">The status of a long-running operation.</span></span>

## <a name="methods"></a><span data-ttu-id="0f8fe-105">Методы</span><span class="sxs-lookup"><span data-stu-id="0f8fe-105">Methods</span></span>

<span data-ttu-id="0f8fe-106">Нет</span><span class="sxs-lookup"><span data-stu-id="0f8fe-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="0f8fe-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="0f8fe-107">Properties</span></span>

| <span data-ttu-id="0f8fe-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="0f8fe-108">Property</span></span>           | <span data-ttu-id="0f8fe-109">Тип</span><span class="sxs-lookup"><span data-stu-id="0f8fe-109">Type</span></span>            | <span data-ttu-id="0f8fe-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0f8fe-110">Description</span></span>                                                                     |
| :----------------- | :-------------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="0f8fe-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0f8fe-111">createdDateTime</span></span>    | <span data-ttu-id="0f8fe-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f8fe-112">DateTimeOffset</span></span>  | <span data-ttu-id="0f8fe-113">Время начала операции.</span><span class="sxs-lookup"><span data-stu-id="0f8fe-113">The start time of the operation.</span></span>                                                |
| <span data-ttu-id="0f8fe-114">id</span><span class="sxs-lookup"><span data-stu-id="0f8fe-114">id</span></span>                 | <span data-ttu-id="0f8fe-115">Строка</span><span class="sxs-lookup"><span data-stu-id="0f8fe-115">String</span></span>          | <span data-ttu-id="0f8fe-116">Идентификатор операции. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0f8fe-116">The operation id. Read-only.</span></span> <span data-ttu-id="0f8fe-117">Создается сервером.</span><span class="sxs-lookup"><span data-stu-id="0f8fe-117">Server generated.</span></span>                                  |
| <span data-ttu-id="0f8fe-118">Ластактиондатетиме</span><span class="sxs-lookup"><span data-stu-id="0f8fe-118">lastActionDateTime</span></span> | <span data-ttu-id="0f8fe-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f8fe-119">DateTimeOffset</span></span>  | <span data-ttu-id="0f8fe-120">Время последнего действия операции.</span><span class="sxs-lookup"><span data-stu-id="0f8fe-120">The time of the last action of the operation.</span></span>                                   |
| <span data-ttu-id="0f8fe-121">status</span><span class="sxs-lookup"><span data-stu-id="0f8fe-121">status</span></span>             | <span data-ttu-id="0f8fe-122">String</span><span class="sxs-lookup"><span data-stu-id="0f8fe-122">String</span></span>          | <span data-ttu-id="0f8fe-123">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="0f8fe-123">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="0f8fe-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0f8fe-124">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="0f8fe-125">Отношения</span><span class="sxs-lookup"><span data-stu-id="0f8fe-125">Relationships</span></span>

<span data-ttu-id="0f8fe-126">Нет</span><span class="sxs-lookup"><span data-stu-id="0f8fe-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0f8fe-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0f8fe-127">JSON representation</span></span>

<span data-ttu-id="0f8fe-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0f8fe-128">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="0f8fe-129">Пример</span><span class="sxs-lookup"><span data-stu-id="0f8fe-129">Example</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/operation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
