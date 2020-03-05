---
title: Тип ресурса Плайпромптоператион
description: Операция Плайпромпт для получения результата действия Плайпромпт.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 5adc385c5764371c1e2cab516bc33fd8504aecf5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447089"
---
# <a name="playpromptoperation-resource-type"></a><span data-ttu-id="bc56a-103">Тип ресурса Плайпромптоператион</span><span class="sxs-lookup"><span data-stu-id="bc56a-103">playPromptOperation resource type</span></span>

<span data-ttu-id="bc56a-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="bc56a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bc56a-105">Операция Плайпромпт для получения результата действия Плайпромпт.</span><span class="sxs-lookup"><span data-stu-id="bc56a-105">The playPrompt operation to obtain the result of the playPrompt action.</span></span>

## <a name="properties"></a><span data-ttu-id="bc56a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="bc56a-106">Properties</span></span>

| <span data-ttu-id="bc56a-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="bc56a-107">Property</span></span>            | <span data-ttu-id="bc56a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="bc56a-108">Type</span></span>                        | <span data-ttu-id="bc56a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="bc56a-109">Description</span></span>|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| <span data-ttu-id="bc56a-110">Контекст</span><span class="sxs-lookup"><span data-stu-id="bc56a-110">clientContext</span></span>       | <span data-ttu-id="bc56a-111">String</span><span class="sxs-lookup"><span data-stu-id="bc56a-111">String</span></span>                      | <span data-ttu-id="bc56a-112">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="bc56a-112">Unique Client Context string.</span></span> <span data-ttu-id="bc56a-113">Максимальный лимит — 256 символов.</span><span class="sxs-lookup"><span data-stu-id="bc56a-113">Max limit is 256 chars.</span></span>                              |
| <span data-ttu-id="bc56a-114">id</span><span class="sxs-lookup"><span data-stu-id="bc56a-114">id</span></span>                  | <span data-ttu-id="bc56a-115">Строка</span><span class="sxs-lookup"><span data-stu-id="bc56a-115">String</span></span>                      | <span data-ttu-id="bc56a-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bc56a-116">Read-only.</span></span>                                                                         |
| <span data-ttu-id="bc56a-117">resultInfo</span><span class="sxs-lookup"><span data-stu-id="bc56a-117">resultInfo</span></span>          | [<span data-ttu-id="bc56a-118">resultInfo</span><span class="sxs-lookup"><span data-stu-id="bc56a-118">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="bc56a-119">Сведения о результате.</span><span class="sxs-lookup"><span data-stu-id="bc56a-119">The result information.</span></span> <span data-ttu-id="bc56a-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bc56a-120">Read-only.</span></span>                                |
| <span data-ttu-id="bc56a-121">status</span><span class="sxs-lookup"><span data-stu-id="bc56a-121">status</span></span>              | <span data-ttu-id="bc56a-122">String</span><span class="sxs-lookup"><span data-stu-id="bc56a-122">String</span></span>                      | <span data-ttu-id="bc56a-123">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="bc56a-123">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span>               |

## <a name="relationships"></a><span data-ttu-id="bc56a-124">Связи</span><span class="sxs-lookup"><span data-stu-id="bc56a-124">Relationships</span></span>
<span data-ttu-id="bc56a-125">Нет</span><span class="sxs-lookup"><span data-stu-id="bc56a-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bc56a-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bc56a-126">JSON representation</span></span>

<span data-ttu-id="bc56a-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bc56a-127">The following is a JSON representation of the resource.</span></span>

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
