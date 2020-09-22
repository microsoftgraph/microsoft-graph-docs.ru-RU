---
title: Тип ресурса Плайпромптоператион
description: Операция Плайпромпт для получения результата действия Плайпромпт.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 43f36c1843a8f9e92081015dd349ee48a1f768ef
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037348"
---
# <a name="playpromptoperation-resource-type"></a><span data-ttu-id="d8266-103">Тип ресурса Плайпромптоператион</span><span class="sxs-lookup"><span data-stu-id="d8266-103">playPromptOperation resource type</span></span>

<span data-ttu-id="d8266-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8266-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d8266-105">Операция Плайпромпт для получения результата действия Плайпромпт.</span><span class="sxs-lookup"><span data-stu-id="d8266-105">The playPrompt operation to obtain the result of the playPrompt action.</span></span>

## <a name="properties"></a><span data-ttu-id="d8266-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="d8266-106">Properties</span></span>

| <span data-ttu-id="d8266-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="d8266-107">Property</span></span>            | <span data-ttu-id="d8266-108">Тип</span><span class="sxs-lookup"><span data-stu-id="d8266-108">Type</span></span>                        | <span data-ttu-id="d8266-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d8266-109">Description</span></span>|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| <span data-ttu-id="d8266-110">Контекст</span><span class="sxs-lookup"><span data-stu-id="d8266-110">clientContext</span></span>       | <span data-ttu-id="d8266-111">String</span><span class="sxs-lookup"><span data-stu-id="d8266-111">String</span></span>                      | <span data-ttu-id="d8266-112">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="d8266-112">Unique Client Context string.</span></span> <span data-ttu-id="d8266-113">Максимальный лимит — 256 символов.</span><span class="sxs-lookup"><span data-stu-id="d8266-113">Max limit is 256 chars.</span></span>                              |
| <span data-ttu-id="d8266-114">id</span><span class="sxs-lookup"><span data-stu-id="d8266-114">id</span></span>                  | <span data-ttu-id="d8266-115">String</span><span class="sxs-lookup"><span data-stu-id="d8266-115">String</span></span>                      | <span data-ttu-id="d8266-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d8266-116">Read-only.</span></span>                                                                         |
| <span data-ttu-id="d8266-117">resultInfo</span><span class="sxs-lookup"><span data-stu-id="d8266-117">resultInfo</span></span>          | [<span data-ttu-id="d8266-118">resultInfo</span><span class="sxs-lookup"><span data-stu-id="d8266-118">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="d8266-119">Сведения о результате.</span><span class="sxs-lookup"><span data-stu-id="d8266-119">The result information.</span></span> <span data-ttu-id="d8266-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d8266-120">Read-only.</span></span>                                |
| <span data-ttu-id="d8266-121">status</span><span class="sxs-lookup"><span data-stu-id="d8266-121">status</span></span>              | <span data-ttu-id="d8266-122">String</span><span class="sxs-lookup"><span data-stu-id="d8266-122">String</span></span>                      | <span data-ttu-id="d8266-123">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="d8266-123">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span>               |

## <a name="relationships"></a><span data-ttu-id="d8266-124">Связи</span><span class="sxs-lookup"><span data-stu-id="d8266-124">Relationships</span></span>
<span data-ttu-id="d8266-125">Нет</span><span class="sxs-lookup"><span data-stu-id="d8266-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d8266-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d8266-126">JSON representation</span></span>

<span data-ttu-id="d8266-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d8266-127">The following is a JSON representation of the resource.</span></span>

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

