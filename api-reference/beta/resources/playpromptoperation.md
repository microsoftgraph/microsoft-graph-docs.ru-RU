---
title: Тип ресурса Плайпромптоператион
description: Операция Плайпромпт для получения результата действия Плайпромпт.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 84b54fbce830f5b505decee7e2d25618700728b3
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006580"
---
# <a name="playpromptoperation-resource-type"></a><span data-ttu-id="7c3c3-103">Тип ресурса Плайпромптоператион</span><span class="sxs-lookup"><span data-stu-id="7c3c3-103">playPromptOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c3c3-104">Операция Плайпромпт для получения результата действия Плайпромпт.</span><span class="sxs-lookup"><span data-stu-id="7c3c3-104">The playPrompt operation to obtain the result of the playPrompt action.</span></span>

## <a name="properties"></a><span data-ttu-id="7c3c3-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="7c3c3-105">Properties</span></span>

| <span data-ttu-id="7c3c3-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="7c3c3-106">Property</span></span>            | <span data-ttu-id="7c3c3-107">Тип</span><span class="sxs-lookup"><span data-stu-id="7c3c3-107">Type</span></span>                        | <span data-ttu-id="7c3c3-108">Описание</span><span class="sxs-lookup"><span data-stu-id="7c3c3-108">Description</span></span>|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| <span data-ttu-id="7c3c3-109">Контекст</span><span class="sxs-lookup"><span data-stu-id="7c3c3-109">clientContext</span></span>       | <span data-ttu-id="7c3c3-110">String</span><span class="sxs-lookup"><span data-stu-id="7c3c3-110">String</span></span>                      | <span data-ttu-id="7c3c3-111">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="7c3c3-111">Unique Client Context string.</span></span> <span data-ttu-id="7c3c3-112">Максимальный лимит — 256 символов.</span><span class="sxs-lookup"><span data-stu-id="7c3c3-112">Max limit is 256 chars.</span></span>                              |
| <span data-ttu-id="7c3c3-113">комплетионреасон</span><span class="sxs-lookup"><span data-stu-id="7c3c3-113">completionReason</span></span>    | <span data-ttu-id="7c3c3-114">String</span><span class="sxs-lookup"><span data-stu-id="7c3c3-114">String</span></span>                      | <span data-ttu-id="7c3c3-115">Возможные значения: `unknown`, `completedSuccessfully`, `mediaOperationCanceled`.</span><span class="sxs-lookup"><span data-stu-id="7c3c3-115">Possible values are: `unknown`, `completedSuccessfully`, `mediaOperationCanceled`.</span></span> |
| <span data-ttu-id="7c3c3-116">id</span><span class="sxs-lookup"><span data-stu-id="7c3c3-116">id</span></span>                  | <span data-ttu-id="7c3c3-117">Строка</span><span class="sxs-lookup"><span data-stu-id="7c3c3-117">String</span></span>                      | <span data-ttu-id="7c3c3-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7c3c3-118">Read-only.</span></span>                                                                         |
| <span data-ttu-id="7c3c3-119">resultInfo</span><span class="sxs-lookup"><span data-stu-id="7c3c3-119">resultInfo</span></span>          | [<span data-ttu-id="7c3c3-120">resultInfo</span><span class="sxs-lookup"><span data-stu-id="7c3c3-120">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="7c3c3-121">Сведения о результате.</span><span class="sxs-lookup"><span data-stu-id="7c3c3-121">The result information.</span></span> <span data-ttu-id="7c3c3-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7c3c3-122">Read-only.</span></span>                                |
| <span data-ttu-id="7c3c3-123">status</span><span class="sxs-lookup"><span data-stu-id="7c3c3-123">status</span></span>              | <span data-ttu-id="7c3c3-124">String</span><span class="sxs-lookup"><span data-stu-id="7c3c3-124">String</span></span>                      | <span data-ttu-id="7c3c3-125">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="7c3c3-125">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span>               |

## <a name="relationships"></a><span data-ttu-id="7c3c3-126">Связи</span><span class="sxs-lookup"><span data-stu-id="7c3c3-126">Relationships</span></span>
<span data-ttu-id="7c3c3-127">Нет</span><span class="sxs-lookup"><span data-stu-id="7c3c3-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7c3c3-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7c3c3-128">JSON representation</span></span>

<span data-ttu-id="7c3c3-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7c3c3-129">The following is a JSON representation of the resource.</span></span>

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
  "id": "String (identifier)",
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
