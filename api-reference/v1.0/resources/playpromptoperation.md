---
title: Тип ресурса Плайпромптоператион
description: Операция Плайпромпт для получения результата действия Плайпромпт.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 731e8597fba4347659a3cddea8fb2934258255c7
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913221"
---
# <a name="playpromptoperation-resource-type"></a><span data-ttu-id="5a171-103">Тип ресурса Плайпромптоператион</span><span class="sxs-lookup"><span data-stu-id="5a171-103">playPromptOperation resource type</span></span>

<span data-ttu-id="5a171-104">Операция Плайпромпт для получения результата действия Плайпромпт.</span><span class="sxs-lookup"><span data-stu-id="5a171-104">The playPrompt operation to obtain the result of the playPrompt action.</span></span>

## <a name="properties"></a><span data-ttu-id="5a171-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="5a171-105">Properties</span></span>

| <span data-ttu-id="5a171-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="5a171-106">Property</span></span>            | <span data-ttu-id="5a171-107">Тип</span><span class="sxs-lookup"><span data-stu-id="5a171-107">Type</span></span>                        | <span data-ttu-id="5a171-108">Описание</span><span class="sxs-lookup"><span data-stu-id="5a171-108">Description</span></span>|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| <span data-ttu-id="5a171-109">Контекст</span><span class="sxs-lookup"><span data-stu-id="5a171-109">clientContext</span></span>       | <span data-ttu-id="5a171-110">String</span><span class="sxs-lookup"><span data-stu-id="5a171-110">String</span></span>                      | <span data-ttu-id="5a171-111">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="5a171-111">Unique Client Context string.</span></span> <span data-ttu-id="5a171-112">Максимальный лимит — 256 символов.</span><span class="sxs-lookup"><span data-stu-id="5a171-112">Max limit is 256 chars.</span></span>                              |
| <span data-ttu-id="5a171-113">id</span><span class="sxs-lookup"><span data-stu-id="5a171-113">id</span></span>                  | <span data-ttu-id="5a171-114">Строка</span><span class="sxs-lookup"><span data-stu-id="5a171-114">String</span></span>                      | <span data-ttu-id="5a171-115">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5a171-115">Read-only.</span></span>                                                                         |
| <span data-ttu-id="5a171-116">resultInfo</span><span class="sxs-lookup"><span data-stu-id="5a171-116">resultInfo</span></span>          | [<span data-ttu-id="5a171-117">resultInfo</span><span class="sxs-lookup"><span data-stu-id="5a171-117">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="5a171-118">Сведения о результате.</span><span class="sxs-lookup"><span data-stu-id="5a171-118">The result information.</span></span> <span data-ttu-id="5a171-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5a171-119">Read-only.</span></span>                                |
| <span data-ttu-id="5a171-120">status</span><span class="sxs-lookup"><span data-stu-id="5a171-120">status</span></span>              | <span data-ttu-id="5a171-121">String</span><span class="sxs-lookup"><span data-stu-id="5a171-121">String</span></span>                      | <span data-ttu-id="5a171-122">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="5a171-122">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span>               |

## <a name="relationships"></a><span data-ttu-id="5a171-123">Отношения</span><span class="sxs-lookup"><span data-stu-id="5a171-123">Relationships</span></span>
<span data-ttu-id="5a171-124">Нет</span><span class="sxs-lookup"><span data-stu-id="5a171-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5a171-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5a171-125">JSON representation</span></span>

<span data-ttu-id="5a171-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5a171-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.playPromptOperation"
}-->
```json
{
  "clientContext": "String",
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
