---
title: Тип ресурса Плайпромптоператион
description: Операция Плайпромпт для получения результата действия Плайпромпт.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b79fa774c112433b09d75eb04f16823f2dad9b6c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008980"
---
# <a name="playpromptoperation-resource-type"></a><span data-ttu-id="35707-103">Тип ресурса Плайпромптоператион</span><span class="sxs-lookup"><span data-stu-id="35707-103">playPromptOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35707-104">Операция Плайпромпт для получения результата действия Плайпромпт.</span><span class="sxs-lookup"><span data-stu-id="35707-104">The playPrompt operation to obtain the result of the playPrompt action.</span></span>

## <a name="properties"></a><span data-ttu-id="35707-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="35707-105">Properties</span></span>

| <span data-ttu-id="35707-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="35707-106">Property</span></span>            | <span data-ttu-id="35707-107">Тип</span><span class="sxs-lookup"><span data-stu-id="35707-107">Type</span></span>                        | <span data-ttu-id="35707-108">Описание</span><span class="sxs-lookup"><span data-stu-id="35707-108">Description</span></span>|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| <span data-ttu-id="35707-109">Контекст</span><span class="sxs-lookup"><span data-stu-id="35707-109">clientContext</span></span>       | <span data-ttu-id="35707-110">String</span><span class="sxs-lookup"><span data-stu-id="35707-110">String</span></span>                      | <span data-ttu-id="35707-111">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="35707-111">The client context.</span></span>                                                                |
| <span data-ttu-id="35707-112">Комплетионреасон</span><span class="sxs-lookup"><span data-stu-id="35707-112">completionReason</span></span>    | <span data-ttu-id="35707-113">String</span><span class="sxs-lookup"><span data-stu-id="35707-113">String</span></span>                      | <span data-ttu-id="35707-114">Возможные значения: `unknown`, `completedSuccessfully`, `mediaOperationCanceled`.</span><span class="sxs-lookup"><span data-stu-id="35707-114">Possible values are: `unknown`, `completedSuccessfully`, `mediaOperationCanceled`.</span></span> |
| <span data-ttu-id="35707-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="35707-115">createdDateTime</span></span>     | <span data-ttu-id="35707-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35707-116">DateTimeOffset</span></span>              | <span data-ttu-id="35707-117">Время начала операции.</span><span class="sxs-lookup"><span data-stu-id="35707-117">The start time of the operation.</span></span>                                                   |
| <span data-ttu-id="35707-118">id</span><span class="sxs-lookup"><span data-stu-id="35707-118">id</span></span>                  | <span data-ttu-id="35707-119">Строка</span><span class="sxs-lookup"><span data-stu-id="35707-119">String</span></span>                      | <span data-ttu-id="35707-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="35707-120">Read-only.</span></span>                                                                         |
| <span data-ttu-id="35707-121">Ластактиондатетиме</span><span class="sxs-lookup"><span data-stu-id="35707-121">lastActionDateTime</span></span>  | <span data-ttu-id="35707-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35707-122">DateTimeOffset</span></span>              | <span data-ttu-id="35707-123">Время последнего действия операции.</span><span class="sxs-lookup"><span data-stu-id="35707-123">The time of the last action of the operation.</span></span>                                      |
| <span data-ttu-id="35707-124">resultInfo</span><span class="sxs-lookup"><span data-stu-id="35707-124">resultInfo</span></span>          | [<span data-ttu-id="35707-125">resultInfo</span><span class="sxs-lookup"><span data-stu-id="35707-125">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="35707-126">Сведения о результате.</span><span class="sxs-lookup"><span data-stu-id="35707-126">The result information.</span></span> <span data-ttu-id="35707-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="35707-127">Read-only.</span></span> <span data-ttu-id="35707-128">Создается сервером.</span><span class="sxs-lookup"><span data-stu-id="35707-128">Server generated.</span></span>                               |
| <span data-ttu-id="35707-129">status</span><span class="sxs-lookup"><span data-stu-id="35707-129">status</span></span>              | <span data-ttu-id="35707-130">String</span><span class="sxs-lookup"><span data-stu-id="35707-130">String</span></span>                      | <span data-ttu-id="35707-131">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="35707-131">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span>               |

## <a name="relationships"></a><span data-ttu-id="35707-132">Отношения</span><span class="sxs-lookup"><span data-stu-id="35707-132">Relationships</span></span>
<span data-ttu-id="35707-133">Нет</span><span class="sxs-lookup"><span data-stu-id="35707-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="35707-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="35707-134">JSON representation</span></span>

<span data-ttu-id="35707-135">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="35707-135">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
