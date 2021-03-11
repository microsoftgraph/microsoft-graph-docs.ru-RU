---
title: тип ресурса threatAssessmentResult
description: Представляет элемент результатов оценки угроз.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9120ad0afe3efb2a559e913c7b6357a76e9ac49b
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722078"
---
# <a name="threatassessmentresult-resource-type"></a><span data-ttu-id="033a3-103">тип ресурса threatAssessmentResult</span><span class="sxs-lookup"><span data-stu-id="033a3-103">threatAssessmentResult resource type</span></span>

<span data-ttu-id="033a3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="033a3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="033a3-105">Представляет элемент результатов оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="033a3-105">Represents a threat assessment result item.</span></span>

## <a name="properties"></a><span data-ttu-id="033a3-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="033a3-106">Properties</span></span>

| <span data-ttu-id="033a3-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="033a3-107">Property</span></span>     | <span data-ttu-id="033a3-108">Тип</span><span class="sxs-lookup"><span data-stu-id="033a3-108">Type</span></span>        | <span data-ttu-id="033a3-109">Описание</span><span class="sxs-lookup"><span data-stu-id="033a3-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="033a3-110">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="033a3-110">createdDateTime</span></span>|<span data-ttu-id="033a3-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="033a3-111">DateTimeOffset</span></span>|<span data-ttu-id="033a3-112">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="033a3-112">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="033a3-113">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="033a3-113">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="033a3-114">id</span><span class="sxs-lookup"><span data-stu-id="033a3-114">id</span></span>|<span data-ttu-id="033a3-115">String</span><span class="sxs-lookup"><span data-stu-id="033a3-115">String</span></span>|<span data-ttu-id="033a3-116">Идентификатор результатов оценки угроз — это уникальный идентификатор глобального идентификатора (GUID).</span><span class="sxs-lookup"><span data-stu-id="033a3-116">The threat assessment result ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="033a3-117">message</span><span class="sxs-lookup"><span data-stu-id="033a3-117">message</span></span>|<span data-ttu-id="033a3-118">String</span><span class="sxs-lookup"><span data-stu-id="033a3-118">String</span></span>|<span data-ttu-id="033a3-119">Сообщение результата для каждой оценки угрозы.</span><span class="sxs-lookup"><span data-stu-id="033a3-119">The result message for each threat assessment.</span></span>|
|<span data-ttu-id="033a3-120">resultType</span><span class="sxs-lookup"><span data-stu-id="033a3-120">resultType</span></span>|[<span data-ttu-id="033a3-121">threatAssessmentResultType</span><span class="sxs-lookup"><span data-stu-id="033a3-121">threatAssessmentResultType</span></span>](enums.md#threatassessmentresulttype-values)|<span data-ttu-id="033a3-122">Тип результатов оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="033a3-122">The threat assessment result type.</span></span> <span data-ttu-id="033a3-123">Возможные значения: `checkPolicy`, `rescan`.</span><span class="sxs-lookup"><span data-stu-id="033a3-123">Possible values are: `checkPolicy`, `rescan`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="033a3-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="033a3-124">JSON representation</span></span>

<span data-ttu-id="033a3-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="033a3-125">The following is a JSON representation of the resource.</span></span>

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


