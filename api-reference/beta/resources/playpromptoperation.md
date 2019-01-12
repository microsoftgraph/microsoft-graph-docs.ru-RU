---
title: Тип ресурса playPromptOperation
description: Операция playPrompt для получения результатов playPrompt действие.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d451418482d1adf1a4b7e16dc8a6eb8ca7febdb7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937819"
---
# <a name="playpromptoperation-resource-type"></a><span data-ttu-id="0e176-103">Тип ресурса playPromptOperation</span><span class="sxs-lookup"><span data-stu-id="0e176-103">playPromptOperation resource type</span></span>

> <span data-ttu-id="0e176-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0e176-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0e176-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e176-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0e176-106">Операция playPrompt для получения результатов playPrompt действие.</span><span class="sxs-lookup"><span data-stu-id="0e176-106">The playPrompt operation to obtain the result of the playPrompt action.</span></span>

## <a name="properties"></a><span data-ttu-id="0e176-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="0e176-107">Properties</span></span>

| <span data-ttu-id="0e176-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="0e176-108">Property</span></span>            | <span data-ttu-id="0e176-109">Тип</span><span class="sxs-lookup"><span data-stu-id="0e176-109">Type</span></span>                        | <span data-ttu-id="0e176-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0e176-110">Description</span></span>|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| <span data-ttu-id="0e176-111">clientContext</span><span class="sxs-lookup"><span data-stu-id="0e176-111">clientContext</span></span>       | <span data-ttu-id="0e176-112">Строка</span><span class="sxs-lookup"><span data-stu-id="0e176-112">String</span></span>                      | <span data-ttu-id="0e176-113">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="0e176-113">The client context.</span></span>                                                                |
| <span data-ttu-id="0e176-114">completionReason</span><span class="sxs-lookup"><span data-stu-id="0e176-114">completionReason</span></span>    | <span data-ttu-id="0e176-115">Строка</span><span class="sxs-lookup"><span data-stu-id="0e176-115">String</span></span>                      | <span data-ttu-id="0e176-116">Возможные значения: `unknown`, `completedSuccessfully`, `mediaOperationCanceled`.</span><span class="sxs-lookup"><span data-stu-id="0e176-116">Possible values are: `unknown`, `completedSuccessfully`, `mediaOperationCanceled`.</span></span> |
| <span data-ttu-id="0e176-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0e176-117">createdDateTime</span></span>     | <span data-ttu-id="0e176-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e176-118">DateTimeOffset</span></span>              | <span data-ttu-id="0e176-119">Время начала операции.</span><span class="sxs-lookup"><span data-stu-id="0e176-119">The start time of the operation.</span></span>                                                   |
| <span data-ttu-id="0e176-120">id</span><span class="sxs-lookup"><span data-stu-id="0e176-120">id</span></span>                  | <span data-ttu-id="0e176-121">Строка</span><span class="sxs-lookup"><span data-stu-id="0e176-121">String</span></span>                      | <span data-ttu-id="0e176-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0e176-122">Read-only.</span></span>                                                                         |
| <span data-ttu-id="0e176-123">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="0e176-123">lastActionDateTime</span></span>  | <span data-ttu-id="0e176-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e176-124">DateTimeOffset</span></span>              | <span data-ttu-id="0e176-125">Время последнего действия операции.</span><span class="sxs-lookup"><span data-stu-id="0e176-125">The time of the last action of the operation.</span></span>                                      |
| <span data-ttu-id="0e176-126">resultInfo</span><span class="sxs-lookup"><span data-stu-id="0e176-126">resultInfo</span></span>          | [<span data-ttu-id="0e176-127">resultInfo</span><span class="sxs-lookup"><span data-stu-id="0e176-127">resultInfo</span></span>](resultInfo.md) | <span data-ttu-id="0e176-128">Сведения о результатов.</span><span class="sxs-lookup"><span data-stu-id="0e176-128">The result information.</span></span> <span data-ttu-id="0e176-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0e176-129">Read-only.</span></span> <span data-ttu-id="0e176-130">Сервер, созданный.</span><span class="sxs-lookup"><span data-stu-id="0e176-130">Server generated.</span></span>                               |
| <span data-ttu-id="0e176-131">status</span><span class="sxs-lookup"><span data-stu-id="0e176-131">status</span></span>              | <span data-ttu-id="0e176-132">Строка</span><span class="sxs-lookup"><span data-stu-id="0e176-132">String</span></span>                      | <span data-ttu-id="0e176-133">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="0e176-133">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span>               |

## <a name="relationships"></a><span data-ttu-id="0e176-134">Связи</span><span class="sxs-lookup"><span data-stu-id="0e176-134">Relationships</span></span>
<span data-ttu-id="0e176-135">Нет</span><span class="sxs-lookup"><span data-stu-id="0e176-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0e176-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0e176-136">JSON representation</span></span>

<span data-ttu-id="0e176-137">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0e176-137">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "playPromptOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
