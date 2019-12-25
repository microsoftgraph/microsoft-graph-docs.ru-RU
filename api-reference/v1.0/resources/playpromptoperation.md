---
title: Тип ресурса Плайпромптоператион
description: Операция Плайпромпт для получения результата действия Плайпромпт.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: ae7b1f33216d2d9ae9d867fca57fe2dd27e2e4df
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866259"
---
# <a name="playpromptoperation-resource-type"></a><span data-ttu-id="9099f-103">Тип ресурса Плайпромптоператион</span><span class="sxs-lookup"><span data-stu-id="9099f-103">playPromptOperation resource type</span></span>

<span data-ttu-id="9099f-104">Операция Плайпромпт для получения результата действия Плайпромпт.</span><span class="sxs-lookup"><span data-stu-id="9099f-104">The playPrompt operation to obtain the result of the playPrompt action.</span></span>

## <a name="properties"></a><span data-ttu-id="9099f-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="9099f-105">Properties</span></span>

| <span data-ttu-id="9099f-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="9099f-106">Property</span></span>            | <span data-ttu-id="9099f-107">Тип</span><span class="sxs-lookup"><span data-stu-id="9099f-107">Type</span></span>                        | <span data-ttu-id="9099f-108">Описание</span><span class="sxs-lookup"><span data-stu-id="9099f-108">Description</span></span>|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| <span data-ttu-id="9099f-109">Контекст</span><span class="sxs-lookup"><span data-stu-id="9099f-109">clientContext</span></span>       | <span data-ttu-id="9099f-110">String</span><span class="sxs-lookup"><span data-stu-id="9099f-110">String</span></span>                      | <span data-ttu-id="9099f-111">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="9099f-111">Unique Client Context string.</span></span> <span data-ttu-id="9099f-112">Максимальный лимит — 256 символов.</span><span class="sxs-lookup"><span data-stu-id="9099f-112">Max limit is 256 chars.</span></span>                              |
| <span data-ttu-id="9099f-113">id</span><span class="sxs-lookup"><span data-stu-id="9099f-113">id</span></span>                  | <span data-ttu-id="9099f-114">Строка</span><span class="sxs-lookup"><span data-stu-id="9099f-114">String</span></span>                      | <span data-ttu-id="9099f-115">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9099f-115">Read-only.</span></span>                                                                         |
| <span data-ttu-id="9099f-116">resultInfo</span><span class="sxs-lookup"><span data-stu-id="9099f-116">resultInfo</span></span>          | [<span data-ttu-id="9099f-117">resultInfo</span><span class="sxs-lookup"><span data-stu-id="9099f-117">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="9099f-118">Сведения о результате.</span><span class="sxs-lookup"><span data-stu-id="9099f-118">The result information.</span></span> <span data-ttu-id="9099f-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9099f-119">Read-only.</span></span>                                |
| <span data-ttu-id="9099f-120">status</span><span class="sxs-lookup"><span data-stu-id="9099f-120">status</span></span>              | <span data-ttu-id="9099f-121">String</span><span class="sxs-lookup"><span data-stu-id="9099f-121">String</span></span>                      | <span data-ttu-id="9099f-122">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="9099f-122">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span>               |

## <a name="relationships"></a><span data-ttu-id="9099f-123">Отношения</span><span class="sxs-lookup"><span data-stu-id="9099f-123">Relationships</span></span>
<span data-ttu-id="9099f-124">Нет</span><span class="sxs-lookup"><span data-stu-id="9099f-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9099f-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9099f-125">JSON representation</span></span>

<span data-ttu-id="9099f-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9099f-126">The following is a JSON representation of the resource.</span></span>

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
