---
title: тип ресурса threatAssessmentResult
description: Представляет элемент результатов оценки угроз.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0657cef555cd982c6649f6a8a4f40b7e5e15eaab
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722103"
---
# <a name="threatassessmentresult-resource-type"></a><span data-ttu-id="19f00-103">тип ресурса threatAssessmentResult</span><span class="sxs-lookup"><span data-stu-id="19f00-103">threatAssessmentResult resource type</span></span>

<span data-ttu-id="19f00-104">Представляет элемент результатов оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="19f00-104">Represents a threat assessment result item.</span></span>

## <a name="properties"></a><span data-ttu-id="19f00-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="19f00-105">Properties</span></span>

| <span data-ttu-id="19f00-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="19f00-106">Property</span></span>     | <span data-ttu-id="19f00-107">Тип</span><span class="sxs-lookup"><span data-stu-id="19f00-107">Type</span></span>        | <span data-ttu-id="19f00-108">Описание</span><span class="sxs-lookup"><span data-stu-id="19f00-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="19f00-109">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="19f00-109">createdDateTime</span></span>|<span data-ttu-id="19f00-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19f00-110">DateTimeOffset</span></span>|<span data-ttu-id="19f00-111">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="19f00-111">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="19f00-112">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="19f00-112">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="19f00-113">id</span><span class="sxs-lookup"><span data-stu-id="19f00-113">id</span></span>|<span data-ttu-id="19f00-114">String</span><span class="sxs-lookup"><span data-stu-id="19f00-114">String</span></span>|<span data-ttu-id="19f00-115">Идентификатор результатов оценки угроз — это уникальный идентификатор глобального идентификатора (GUID).</span><span class="sxs-lookup"><span data-stu-id="19f00-115">The threat assessment result ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="19f00-116">message</span><span class="sxs-lookup"><span data-stu-id="19f00-116">message</span></span>|<span data-ttu-id="19f00-117">String</span><span class="sxs-lookup"><span data-stu-id="19f00-117">String</span></span>|<span data-ttu-id="19f00-118">Сообщение результата для каждой оценки угрозы.</span><span class="sxs-lookup"><span data-stu-id="19f00-118">The result message for each threat assessment.</span></span>|
|<span data-ttu-id="19f00-119">resultType</span><span class="sxs-lookup"><span data-stu-id="19f00-119">resultType</span></span>|[<span data-ttu-id="19f00-120">threatAssessmentResultType</span><span class="sxs-lookup"><span data-stu-id="19f00-120">threatAssessmentResultType</span></span>](enums.md#threatassessmentresulttype-values)|<span data-ttu-id="19f00-121">Тип результатов оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="19f00-121">The threat assessment result type.</span></span> <span data-ttu-id="19f00-122">Возможные значения: `checkPolicy`, `rescan`.</span><span class="sxs-lookup"><span data-stu-id="19f00-122">Possible values are: `checkPolicy`, `rescan`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="19f00-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="19f00-123">JSON representation</span></span>

<span data-ttu-id="19f00-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="19f00-124">The following is a JSON representation of the resource.</span></span>

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

