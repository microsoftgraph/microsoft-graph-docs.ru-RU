---
title: тип ресурса threatAssessmentResult
description: Представляет элемент результатов оценки угроз.
localization_priority: Normal
author: hafen-ms
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 307b3bbebd9059ffee057781b5f647e407657684
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950285"
---
# <a name="threatassessmentresult-resource-type"></a><span data-ttu-id="6e970-103">тип ресурса threatAssessmentResult</span><span class="sxs-lookup"><span data-stu-id="6e970-103">threatAssessmentResult resource type</span></span>

<span data-ttu-id="6e970-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e970-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e970-105">Представляет элемент результатов оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="6e970-105">Represents a threat assessment result item.</span></span>

## <a name="properties"></a><span data-ttu-id="6e970-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="6e970-106">Properties</span></span>

| <span data-ttu-id="6e970-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="6e970-107">Property</span></span>     | <span data-ttu-id="6e970-108">Тип</span><span class="sxs-lookup"><span data-stu-id="6e970-108">Type</span></span>        | <span data-ttu-id="6e970-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6e970-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6e970-110">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6e970-110">createdDateTime</span></span>|<span data-ttu-id="6e970-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e970-111">DateTimeOffset</span></span>|<span data-ttu-id="6e970-112">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="6e970-112">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6e970-113">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="6e970-113">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="6e970-114">id</span><span class="sxs-lookup"><span data-stu-id="6e970-114">id</span></span>|<span data-ttu-id="6e970-115">Строка</span><span class="sxs-lookup"><span data-stu-id="6e970-115">String</span></span>|<span data-ttu-id="6e970-116">Идентификатор результатов оценки угроз — это уникальный идентификатор глобального идентификатора (GUID).</span><span class="sxs-lookup"><span data-stu-id="6e970-116">The threat assessment result ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="6e970-117">message</span><span class="sxs-lookup"><span data-stu-id="6e970-117">message</span></span>|<span data-ttu-id="6e970-118">String</span><span class="sxs-lookup"><span data-stu-id="6e970-118">String</span></span>|<span data-ttu-id="6e970-119">Сообщение результата для каждой оценки угрозы.</span><span class="sxs-lookup"><span data-stu-id="6e970-119">The result message for each threat assessment.</span></span>|
|<span data-ttu-id="6e970-120">resultType</span><span class="sxs-lookup"><span data-stu-id="6e970-120">resultType</span></span>|<span data-ttu-id="6e970-121">threatAssessmentResultType</span><span class="sxs-lookup"><span data-stu-id="6e970-121">threatAssessmentResultType</span></span>|<span data-ttu-id="6e970-122">Тип результатов оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="6e970-122">The threat assessment result type.</span></span> <span data-ttu-id="6e970-123">Возможные значения: `checkPolicy` (только для оценки почты) `rescan` .</span><span class="sxs-lookup"><span data-stu-id="6e970-123">Possible values are: `checkPolicy` (only for mail assessment), `rescan`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6e970-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6e970-124">JSON representation</span></span>

<span data-ttu-id="6e970-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6e970-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.threatAssessmentResult",
  "keyProperty": "id"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "message": "String",
  "resultType": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "threatAssessmentResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


