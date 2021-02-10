---
title: Тип ресурса threatAssessmentResult
description: Представляет элемент результата оценки угрозы.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 014ef33859afc933f5d3f5e065b4b33b1788b721
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158956"
---
# <a name="threatassessmentresult-resource-type"></a><span data-ttu-id="9a8f6-103">Тип ресурса threatAssessmentResult</span><span class="sxs-lookup"><span data-stu-id="9a8f6-103">threatAssessmentResult resource type</span></span>

<span data-ttu-id="9a8f6-104">Представляет элемент результата оценки угрозы.</span><span class="sxs-lookup"><span data-stu-id="9a8f6-104">Represents a threat assessment result item.</span></span>

## <a name="properties"></a><span data-ttu-id="9a8f6-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="9a8f6-105">Properties</span></span>

| <span data-ttu-id="9a8f6-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="9a8f6-106">Property</span></span>     | <span data-ttu-id="9a8f6-107">Тип</span><span class="sxs-lookup"><span data-stu-id="9a8f6-107">Type</span></span>        | <span data-ttu-id="9a8f6-108">Описание</span><span class="sxs-lookup"><span data-stu-id="9a8f6-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9a8f6-109">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9a8f6-109">createdDateTime</span></span>|<span data-ttu-id="9a8f6-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a8f6-110">DateTimeOffset</span></span>|<span data-ttu-id="9a8f6-111">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="9a8f6-111">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9a8f6-112">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="9a8f6-112">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="9a8f6-113">id</span><span class="sxs-lookup"><span data-stu-id="9a8f6-113">id</span></span>|<span data-ttu-id="9a8f6-114">String</span><span class="sxs-lookup"><span data-stu-id="9a8f6-114">String</span></span>|<span data-ttu-id="9a8f6-115">Идентификатор результата оценки угроз — это глобальный уникальный идентификатор (GUID).</span><span class="sxs-lookup"><span data-stu-id="9a8f6-115">The threat assessment result ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="9a8f6-116">message</span><span class="sxs-lookup"><span data-stu-id="9a8f6-116">message</span></span>|<span data-ttu-id="9a8f6-117">String</span><span class="sxs-lookup"><span data-stu-id="9a8f6-117">String</span></span>|<span data-ttu-id="9a8f6-118">Сообщение результата для каждой оценки угрозы.</span><span class="sxs-lookup"><span data-stu-id="9a8f6-118">The result message for each threat assessment.</span></span>|
|<span data-ttu-id="9a8f6-119">resultType</span><span class="sxs-lookup"><span data-stu-id="9a8f6-119">resultType</span></span>|[<span data-ttu-id="9a8f6-120">threatAssessmentResultType</span><span class="sxs-lookup"><span data-stu-id="9a8f6-120">threatAssessmentResultType</span></span>](enums.md#threatassessmentresulttype-values)|<span data-ttu-id="9a8f6-121">Тип результата оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="9a8f6-121">The threat assessment result type.</span></span> <span data-ttu-id="9a8f6-122">Возможные значения: `checkPolicy`, `rescan`.</span><span class="sxs-lookup"><span data-stu-id="9a8f6-122">Possible values are: `checkPolicy`, `rescan`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9a8f6-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9a8f6-123">JSON representation</span></span>

<span data-ttu-id="9a8f6-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9a8f6-124">The following is a JSON representation of the resource.</span></span>

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

