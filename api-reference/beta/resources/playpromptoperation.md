---
title: Тип ресурса Плайпромптоператион
description: Операция Плайпромпт для получения результата действия Плайпромпт.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 663675bb895d452c9ad50c89f22f1a51efca20a9
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536997"
---
# <a name="playpromptoperation-resource-type"></a><span data-ttu-id="36f1e-103">Тип ресурса Плайпромптоператион</span><span class="sxs-lookup"><span data-stu-id="36f1e-103">playPromptOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36f1e-104">Операция Плайпромпт для получения результата действия Плайпромпт.</span><span class="sxs-lookup"><span data-stu-id="36f1e-104">The playPrompt operation to obtain the result of the playPrompt action.</span></span>

## <a name="properties"></a><span data-ttu-id="36f1e-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="36f1e-105">Properties</span></span>

| <span data-ttu-id="36f1e-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="36f1e-106">Property</span></span>            | <span data-ttu-id="36f1e-107">Тип</span><span class="sxs-lookup"><span data-stu-id="36f1e-107">Type</span></span>                        | <span data-ttu-id="36f1e-108">Описание</span><span class="sxs-lookup"><span data-stu-id="36f1e-108">Description</span></span>|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| <span data-ttu-id="36f1e-109">Контекст</span><span class="sxs-lookup"><span data-stu-id="36f1e-109">clientContext</span></span>       | <span data-ttu-id="36f1e-110">String</span><span class="sxs-lookup"><span data-stu-id="36f1e-110">String</span></span>                      | <span data-ttu-id="36f1e-111">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="36f1e-111">The client context.</span></span>                                                                |
| <span data-ttu-id="36f1e-112">Комплетионреасон</span><span class="sxs-lookup"><span data-stu-id="36f1e-112">completionReason</span></span>    | <span data-ttu-id="36f1e-113">String</span><span class="sxs-lookup"><span data-stu-id="36f1e-113">String</span></span>                      | <span data-ttu-id="36f1e-114">Возможные значения: `unknown`, `completedSuccessfully`, `mediaOperationCanceled`.</span><span class="sxs-lookup"><span data-stu-id="36f1e-114">Possible values are: `unknown`, `completedSuccessfully`, `mediaOperationCanceled`.</span></span> |
| <span data-ttu-id="36f1e-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="36f1e-115">createdDateTime</span></span>     | <span data-ttu-id="36f1e-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36f1e-116">DateTimeOffset</span></span>              | <span data-ttu-id="36f1e-117">Время начала операции.</span><span class="sxs-lookup"><span data-stu-id="36f1e-117">The start time of the operation.</span></span>                                                   |
| <span data-ttu-id="36f1e-118">id</span><span class="sxs-lookup"><span data-stu-id="36f1e-118">id</span></span>                  | <span data-ttu-id="36f1e-119">Строка</span><span class="sxs-lookup"><span data-stu-id="36f1e-119">String</span></span>                      | <span data-ttu-id="36f1e-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="36f1e-120">Read-only.</span></span>                                                                         |
| <span data-ttu-id="36f1e-121">Ластактиондатетиме</span><span class="sxs-lookup"><span data-stu-id="36f1e-121">lastActionDateTime</span></span>  | <span data-ttu-id="36f1e-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36f1e-122">DateTimeOffset</span></span>              | <span data-ttu-id="36f1e-123">Время последнего действия операции.</span><span class="sxs-lookup"><span data-stu-id="36f1e-123">The time of the last action of the operation.</span></span>                                      |
| <span data-ttu-id="36f1e-124">resultInfo</span><span class="sxs-lookup"><span data-stu-id="36f1e-124">resultInfo</span></span>          | [<span data-ttu-id="36f1e-125">resultInfo</span><span class="sxs-lookup"><span data-stu-id="36f1e-125">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="36f1e-126">Сведения о результате.</span><span class="sxs-lookup"><span data-stu-id="36f1e-126">The result information.</span></span> <span data-ttu-id="36f1e-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="36f1e-127">Read-only.</span></span> <span data-ttu-id="36f1e-128">Создается сервером.</span><span class="sxs-lookup"><span data-stu-id="36f1e-128">Server generated.</span></span>                               |
| <span data-ttu-id="36f1e-129">status</span><span class="sxs-lookup"><span data-stu-id="36f1e-129">status</span></span>              | <span data-ttu-id="36f1e-130">String</span><span class="sxs-lookup"><span data-stu-id="36f1e-130">String</span></span>                      | <span data-ttu-id="36f1e-131">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="36f1e-131">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span>               |

## <a name="relationships"></a><span data-ttu-id="36f1e-132">Отношения</span><span class="sxs-lookup"><span data-stu-id="36f1e-132">Relationships</span></span>
<span data-ttu-id="36f1e-133">Нет</span><span class="sxs-lookup"><span data-stu-id="36f1e-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="36f1e-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="36f1e-134">JSON representation</span></span>

<span data-ttu-id="36f1e-135">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="36f1e-135">The following is a JSON representation of the resource.</span></span>

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
