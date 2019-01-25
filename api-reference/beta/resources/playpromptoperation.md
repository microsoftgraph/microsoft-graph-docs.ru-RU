---
title: Тип ресурса playPromptOperation
description: Операция playPrompt для получения результатов playPrompt действие.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a6ecdb06c910923d35f9d36590ad09fd7835fccb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515204"
---
# <a name="playpromptoperation-resource-type"></a><span data-ttu-id="0b9ad-103">Тип ресурса playPromptOperation</span><span class="sxs-lookup"><span data-stu-id="0b9ad-103">playPromptOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b9ad-104">Операция playPrompt для получения результатов playPrompt действие.</span><span class="sxs-lookup"><span data-stu-id="0b9ad-104">The playPrompt operation to obtain the result of the playPrompt action.</span></span>

## <a name="properties"></a><span data-ttu-id="0b9ad-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="0b9ad-105">Properties</span></span>

| <span data-ttu-id="0b9ad-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="0b9ad-106">Property</span></span>            | <span data-ttu-id="0b9ad-107">Тип</span><span class="sxs-lookup"><span data-stu-id="0b9ad-107">Type</span></span>                        | <span data-ttu-id="0b9ad-108">Описание</span><span class="sxs-lookup"><span data-stu-id="0b9ad-108">Description</span></span>|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| <span data-ttu-id="0b9ad-109">ClientContext</span><span class="sxs-lookup"><span data-stu-id="0b9ad-109">clientContext</span></span>       | <span data-ttu-id="0b9ad-110">String</span><span class="sxs-lookup"><span data-stu-id="0b9ad-110">String</span></span>                      | <span data-ttu-id="0b9ad-111">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="0b9ad-111">The client context.</span></span>                                                                |
| <span data-ttu-id="0b9ad-112">completionReason</span><span class="sxs-lookup"><span data-stu-id="0b9ad-112">completionReason</span></span>    | <span data-ttu-id="0b9ad-113">String</span><span class="sxs-lookup"><span data-stu-id="0b9ad-113">String</span></span>                      | <span data-ttu-id="0b9ad-114">Возможные значения: `unknown`, `completedSuccessfully`, `mediaOperationCanceled`.</span><span class="sxs-lookup"><span data-stu-id="0b9ad-114">Possible values are: `unknown`, `completedSuccessfully`, `mediaOperationCanceled`.</span></span> |
| <span data-ttu-id="0b9ad-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0b9ad-115">createdDateTime</span></span>     | <span data-ttu-id="0b9ad-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b9ad-116">DateTimeOffset</span></span>              | <span data-ttu-id="0b9ad-117">Время начала операции.</span><span class="sxs-lookup"><span data-stu-id="0b9ad-117">The start time of the operation.</span></span>                                                   |
| <span data-ttu-id="0b9ad-118">id</span><span class="sxs-lookup"><span data-stu-id="0b9ad-118">id</span></span>                  | <span data-ttu-id="0b9ad-119">String</span><span class="sxs-lookup"><span data-stu-id="0b9ad-119">String</span></span>                      | <span data-ttu-id="0b9ad-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0b9ad-120">Read-only.</span></span>                                                                         |
| <span data-ttu-id="0b9ad-121">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="0b9ad-121">lastActionDateTime</span></span>  | <span data-ttu-id="0b9ad-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b9ad-122">DateTimeOffset</span></span>              | <span data-ttu-id="0b9ad-123">Время последнего действия операции.</span><span class="sxs-lookup"><span data-stu-id="0b9ad-123">The time of the last action of the operation.</span></span>                                      |
| <span data-ttu-id="0b9ad-124">resultInfo</span><span class="sxs-lookup"><span data-stu-id="0b9ad-124">resultInfo</span></span>          | [<span data-ttu-id="0b9ad-125">resultInfo</span><span class="sxs-lookup"><span data-stu-id="0b9ad-125">resultInfo</span></span>](resultInfo.md) | <span data-ttu-id="0b9ad-126">Сведения о результатов.</span><span class="sxs-lookup"><span data-stu-id="0b9ad-126">The result information.</span></span> <span data-ttu-id="0b9ad-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0b9ad-127">Read-only.</span></span> <span data-ttu-id="0b9ad-128">Сервер, созданный.</span><span class="sxs-lookup"><span data-stu-id="0b9ad-128">Server generated.</span></span>                               |
| <span data-ttu-id="0b9ad-129">status</span><span class="sxs-lookup"><span data-stu-id="0b9ad-129">status</span></span>              | <span data-ttu-id="0b9ad-130">String</span><span class="sxs-lookup"><span data-stu-id="0b9ad-130">String</span></span>                      | <span data-ttu-id="0b9ad-131">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="0b9ad-131">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span>               |

## <a name="relationships"></a><span data-ttu-id="0b9ad-132">Связи</span><span class="sxs-lookup"><span data-stu-id="0b9ad-132">Relationships</span></span>
<span data-ttu-id="0b9ad-133">Нет</span><span class="sxs-lookup"><span data-stu-id="0b9ad-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0b9ad-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0b9ad-134">JSON representation</span></span>

<span data-ttu-id="0b9ad-135">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0b9ad-135">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.playPromptOperation"
}-->
```json
{
  "clientContext": "String",
  "completionReason": "unknown | completedSuccessfully | mediaOperationCanceled",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "status": "notStarted | running | completed | failed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "playPromptOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/playpromptoperation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
