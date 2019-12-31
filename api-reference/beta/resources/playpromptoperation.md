---
title: Тип ресурса Плайпромптоператион
description: Операция Плайпромпт для получения результата действия Плайпромпт.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 3aff109b152be328e6923f6fdb36f116e63a9c16
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913312"
---
# <a name="playpromptoperation-resource-type"></a><span data-ttu-id="98001-103">Тип ресурса Плайпромптоператион</span><span class="sxs-lookup"><span data-stu-id="98001-103">playPromptOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98001-104">Операция Плайпромпт для получения результата действия Плайпромпт.</span><span class="sxs-lookup"><span data-stu-id="98001-104">The playPrompt operation to obtain the result of the playPrompt action.</span></span>

## <a name="properties"></a><span data-ttu-id="98001-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="98001-105">Properties</span></span>

| <span data-ttu-id="98001-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="98001-106">Property</span></span>            | <span data-ttu-id="98001-107">Тип</span><span class="sxs-lookup"><span data-stu-id="98001-107">Type</span></span>                        | <span data-ttu-id="98001-108">Описание</span><span class="sxs-lookup"><span data-stu-id="98001-108">Description</span></span>|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| <span data-ttu-id="98001-109">Контекст</span><span class="sxs-lookup"><span data-stu-id="98001-109">clientContext</span></span>       | <span data-ttu-id="98001-110">String</span><span class="sxs-lookup"><span data-stu-id="98001-110">String</span></span>                      | <span data-ttu-id="98001-111">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="98001-111">Unique Client Context string.</span></span> <span data-ttu-id="98001-112">Максимальный лимит — 256 символов.</span><span class="sxs-lookup"><span data-stu-id="98001-112">Max limit is 256 chars.</span></span>                              |
| <span data-ttu-id="98001-113">комплетионреасон</span><span class="sxs-lookup"><span data-stu-id="98001-113">completionReason</span></span>    | <span data-ttu-id="98001-114">String</span><span class="sxs-lookup"><span data-stu-id="98001-114">String</span></span>                      | <span data-ttu-id="98001-115">Возможные значения: `unknown`, `completedSuccessfully`, `mediaOperationCanceled`.</span><span class="sxs-lookup"><span data-stu-id="98001-115">Possible values are: `unknown`, `completedSuccessfully`, `mediaOperationCanceled`.</span></span> |
| <span data-ttu-id="98001-116">id</span><span class="sxs-lookup"><span data-stu-id="98001-116">id</span></span>                  | <span data-ttu-id="98001-117">Строка</span><span class="sxs-lookup"><span data-stu-id="98001-117">String</span></span>                      | <span data-ttu-id="98001-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="98001-118">Read-only.</span></span>                                                                         |
| <span data-ttu-id="98001-119">resultInfo</span><span class="sxs-lookup"><span data-stu-id="98001-119">resultInfo</span></span>          | [<span data-ttu-id="98001-120">resultInfo</span><span class="sxs-lookup"><span data-stu-id="98001-120">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="98001-121">Сведения о результате.</span><span class="sxs-lookup"><span data-stu-id="98001-121">The result information.</span></span> <span data-ttu-id="98001-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="98001-122">Read-only.</span></span>                                |
| <span data-ttu-id="98001-123">status</span><span class="sxs-lookup"><span data-stu-id="98001-123">status</span></span>              | <span data-ttu-id="98001-124">String</span><span class="sxs-lookup"><span data-stu-id="98001-124">String</span></span>                      | <span data-ttu-id="98001-125">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="98001-125">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span>               |

## <a name="relationships"></a><span data-ttu-id="98001-126">Отношения</span><span class="sxs-lookup"><span data-stu-id="98001-126">Relationships</span></span>
<span data-ttu-id="98001-127">Нет</span><span class="sxs-lookup"><span data-stu-id="98001-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="98001-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="98001-128">JSON representation</span></span>

<span data-ttu-id="98001-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="98001-129">The following is a JSON representation of the resource.</span></span>

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
