---
title: Тип ресурса Плайпромптоператион
description: Операция Плайпромпт для получения результата действия Плайпромпт.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: a1f5c72ed315714039d964c99437af28425bb064
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033652"
---
# <a name="playpromptoperation-resource-type"></a><span data-ttu-id="cc4f9-103">Тип ресурса Плайпромптоператион</span><span class="sxs-lookup"><span data-stu-id="cc4f9-103">playPromptOperation resource type</span></span>

<span data-ttu-id="cc4f9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc4f9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc4f9-105">Операция Плайпромпт для получения результата действия Плайпромпт.</span><span class="sxs-lookup"><span data-stu-id="cc4f9-105">The playPrompt operation to obtain the result of the playPrompt action.</span></span>

## <a name="properties"></a><span data-ttu-id="cc4f9-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="cc4f9-106">Properties</span></span>

| <span data-ttu-id="cc4f9-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="cc4f9-107">Property</span></span>            | <span data-ttu-id="cc4f9-108">Тип</span><span class="sxs-lookup"><span data-stu-id="cc4f9-108">Type</span></span>                        | <span data-ttu-id="cc4f9-109">Описание</span><span class="sxs-lookup"><span data-stu-id="cc4f9-109">Description</span></span>|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| <span data-ttu-id="cc4f9-110">Контекст</span><span class="sxs-lookup"><span data-stu-id="cc4f9-110">clientContext</span></span>       | <span data-ttu-id="cc4f9-111">String</span><span class="sxs-lookup"><span data-stu-id="cc4f9-111">String</span></span>                      | <span data-ttu-id="cc4f9-112">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="cc4f9-112">Unique Client Context string.</span></span> <span data-ttu-id="cc4f9-113">Максимальный лимит — 256 символов.</span><span class="sxs-lookup"><span data-stu-id="cc4f9-113">Max limit is 256 chars.</span></span>                              |
| <span data-ttu-id="cc4f9-114">комплетионреасон</span><span class="sxs-lookup"><span data-stu-id="cc4f9-114">completionReason</span></span>    | <span data-ttu-id="cc4f9-115">String</span><span class="sxs-lookup"><span data-stu-id="cc4f9-115">String</span></span>                      | <span data-ttu-id="cc4f9-116">Возможные значения: `unknown`, `completedSuccessfully`, `mediaOperationCanceled`.</span><span class="sxs-lookup"><span data-stu-id="cc4f9-116">Possible values are: `unknown`, `completedSuccessfully`, `mediaOperationCanceled`.</span></span> |
| <span data-ttu-id="cc4f9-117">id</span><span class="sxs-lookup"><span data-stu-id="cc4f9-117">id</span></span>                  | <span data-ttu-id="cc4f9-118">String</span><span class="sxs-lookup"><span data-stu-id="cc4f9-118">String</span></span>                      | <span data-ttu-id="cc4f9-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cc4f9-119">Read-only.</span></span>                                                                         |
| <span data-ttu-id="cc4f9-120">resultInfo</span><span class="sxs-lookup"><span data-stu-id="cc4f9-120">resultInfo</span></span>          | [<span data-ttu-id="cc4f9-121">resultInfo</span><span class="sxs-lookup"><span data-stu-id="cc4f9-121">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="cc4f9-122">Сведения о результате.</span><span class="sxs-lookup"><span data-stu-id="cc4f9-122">The result information.</span></span> <span data-ttu-id="cc4f9-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cc4f9-123">Read-only.</span></span>                                |
| <span data-ttu-id="cc4f9-124">status</span><span class="sxs-lookup"><span data-stu-id="cc4f9-124">status</span></span>              | <span data-ttu-id="cc4f9-125">String</span><span class="sxs-lookup"><span data-stu-id="cc4f9-125">String</span></span>                      | <span data-ttu-id="cc4f9-126">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="cc4f9-126">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span>               |

## <a name="relationships"></a><span data-ttu-id="cc4f9-127">Отношения</span><span class="sxs-lookup"><span data-stu-id="cc4f9-127">Relationships</span></span>
<span data-ttu-id="cc4f9-128">Нет</span><span class="sxs-lookup"><span data-stu-id="cc4f9-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cc4f9-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cc4f9-129">JSON representation</span></span>

<span data-ttu-id="cc4f9-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cc4f9-130">The following is a JSON representation of the resource.</span></span>

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


