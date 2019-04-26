---
title: Тип ресурса Плайпромптоператион
description: Операция Плайпромпт для получения результата действия Плайпромпт.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a6ecdb06c910923d35f9d36590ad09fd7835fccb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563688"
---
# <a name="playpromptoperation-resource-type"></a><span data-ttu-id="2e579-103">Тип ресурса Плайпромптоператион</span><span class="sxs-lookup"><span data-stu-id="2e579-103">playPromptOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e579-104">Операция Плайпромпт для получения результата действия Плайпромпт.</span><span class="sxs-lookup"><span data-stu-id="2e579-104">The playPrompt operation to obtain the result of the playPrompt action.</span></span>

## <a name="properties"></a><span data-ttu-id="2e579-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="2e579-105">Properties</span></span>

| <span data-ttu-id="2e579-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="2e579-106">Property</span></span>            | <span data-ttu-id="2e579-107">Тип</span><span class="sxs-lookup"><span data-stu-id="2e579-107">Type</span></span>                        | <span data-ttu-id="2e579-108">Описание</span><span class="sxs-lookup"><span data-stu-id="2e579-108">Description</span></span>|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| <span data-ttu-id="2e579-109">Контекст</span><span class="sxs-lookup"><span data-stu-id="2e579-109">clientContext</span></span>       | <span data-ttu-id="2e579-110">String</span><span class="sxs-lookup"><span data-stu-id="2e579-110">String</span></span>                      | <span data-ttu-id="2e579-111">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="2e579-111">The client context.</span></span>                                                                |
| <span data-ttu-id="2e579-112">Комплетионреасон</span><span class="sxs-lookup"><span data-stu-id="2e579-112">completionReason</span></span>    | <span data-ttu-id="2e579-113">String</span><span class="sxs-lookup"><span data-stu-id="2e579-113">String</span></span>                      | <span data-ttu-id="2e579-114">Возможные значения: `unknown`, `completedSuccessfully`, `mediaOperationCanceled`.</span><span class="sxs-lookup"><span data-stu-id="2e579-114">Possible values are: `unknown`, `completedSuccessfully`, `mediaOperationCanceled`.</span></span> |
| <span data-ttu-id="2e579-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2e579-115">createdDateTime</span></span>     | <span data-ttu-id="2e579-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e579-116">DateTimeOffset</span></span>              | <span data-ttu-id="2e579-117">Время начала операции.</span><span class="sxs-lookup"><span data-stu-id="2e579-117">The start time of the operation.</span></span>                                                   |
| <span data-ttu-id="2e579-118">id</span><span class="sxs-lookup"><span data-stu-id="2e579-118">id</span></span>                  | <span data-ttu-id="2e579-119">Строка</span><span class="sxs-lookup"><span data-stu-id="2e579-119">String</span></span>                      | <span data-ttu-id="2e579-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2e579-120">Read-only.</span></span>                                                                         |
| <span data-ttu-id="2e579-121">Ластактиондатетиме</span><span class="sxs-lookup"><span data-stu-id="2e579-121">lastActionDateTime</span></span>  | <span data-ttu-id="2e579-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e579-122">DateTimeOffset</span></span>              | <span data-ttu-id="2e579-123">Время последнего действия операции.</span><span class="sxs-lookup"><span data-stu-id="2e579-123">The time of the last action of the operation.</span></span>                                      |
| <span data-ttu-id="2e579-124">resultInfo</span><span class="sxs-lookup"><span data-stu-id="2e579-124">resultInfo</span></span>          | [<span data-ttu-id="2e579-125">resultInfo</span><span class="sxs-lookup"><span data-stu-id="2e579-125">resultInfo</span></span>](resultInfo.md) | <span data-ttu-id="2e579-126">Сведения о результате.</span><span class="sxs-lookup"><span data-stu-id="2e579-126">The result information.</span></span> <span data-ttu-id="2e579-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2e579-127">Read-only.</span></span> <span data-ttu-id="2e579-128">Создается сервером.</span><span class="sxs-lookup"><span data-stu-id="2e579-128">Server generated.</span></span>                               |
| <span data-ttu-id="2e579-129">status</span><span class="sxs-lookup"><span data-stu-id="2e579-129">status</span></span>              | <span data-ttu-id="2e579-130">String</span><span class="sxs-lookup"><span data-stu-id="2e579-130">String</span></span>                      | <span data-ttu-id="2e579-131">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="2e579-131">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span>               |

## <a name="relationships"></a><span data-ttu-id="2e579-132">Отношения</span><span class="sxs-lookup"><span data-stu-id="2e579-132">Relationships</span></span>
<span data-ttu-id="2e579-133">Нет</span><span class="sxs-lookup"><span data-stu-id="2e579-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2e579-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2e579-134">JSON representation</span></span>

<span data-ttu-id="2e579-135">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2e579-135">The following is a JSON representation of the resource.</span></span>

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
