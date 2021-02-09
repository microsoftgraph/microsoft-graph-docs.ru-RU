---
title: Тип ресурса threatAssessmentResult
description: Представляет элемент результата оценки угрозы.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 35a5d10b631a22f19c881b1d3c2326ab6b09b46c
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155519"
---
# <a name="threatassessmentresult-resource-type"></a><span data-ttu-id="bbd8f-103">Тип ресурса threatAssessmentResult</span><span class="sxs-lookup"><span data-stu-id="bbd8f-103">threatAssessmentResult resource type</span></span>

<span data-ttu-id="bbd8f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bbd8f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bbd8f-105">Представляет элемент результата оценки угрозы.</span><span class="sxs-lookup"><span data-stu-id="bbd8f-105">Represents a threat assessment result item.</span></span>

## <a name="properties"></a><span data-ttu-id="bbd8f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="bbd8f-106">Properties</span></span>

| <span data-ttu-id="bbd8f-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="bbd8f-107">Property</span></span>     | <span data-ttu-id="bbd8f-108">Тип</span><span class="sxs-lookup"><span data-stu-id="bbd8f-108">Type</span></span>        | <span data-ttu-id="bbd8f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="bbd8f-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bbd8f-110">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bbd8f-110">createdDateTime</span></span>|<span data-ttu-id="bbd8f-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bbd8f-111">DateTimeOffset</span></span>|<span data-ttu-id="bbd8f-112">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="bbd8f-112">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="bbd8f-113">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="bbd8f-113">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="bbd8f-114">id</span><span class="sxs-lookup"><span data-stu-id="bbd8f-114">id</span></span>|<span data-ttu-id="bbd8f-115">String</span><span class="sxs-lookup"><span data-stu-id="bbd8f-115">String</span></span>|<span data-ttu-id="bbd8f-116">Идентификатор результата оценки угроз — это глобальный уникальный идентификатор (GUID).</span><span class="sxs-lookup"><span data-stu-id="bbd8f-116">The threat assessment result ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="bbd8f-117">message</span><span class="sxs-lookup"><span data-stu-id="bbd8f-117">message</span></span>|<span data-ttu-id="bbd8f-118">String</span><span class="sxs-lookup"><span data-stu-id="bbd8f-118">String</span></span>|<span data-ttu-id="bbd8f-119">Сообщение результата для каждой оценки угрозы.</span><span class="sxs-lookup"><span data-stu-id="bbd8f-119">The result message for each threat assessment.</span></span>|
|<span data-ttu-id="bbd8f-120">resultType</span><span class="sxs-lookup"><span data-stu-id="bbd8f-120">resultType</span></span>|[<span data-ttu-id="bbd8f-121">threatAssessmentResultType</span><span class="sxs-lookup"><span data-stu-id="bbd8f-121">threatAssessmentResultType</span></span>](enums.md#threatassessmentresulttype-values)|<span data-ttu-id="bbd8f-122">Тип результата оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="bbd8f-122">The threat assessment result type.</span></span> <span data-ttu-id="bbd8f-123">Возможные значения: `checkPolicy`, `rescan`.</span><span class="sxs-lookup"><span data-stu-id="bbd8f-123">Possible values are: `checkPolicy`, `rescan`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bbd8f-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bbd8f-124">JSON representation</span></span>

<span data-ttu-id="bbd8f-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bbd8f-125">The following is a JSON representation of the resource.</span></span>

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


