---
title: Тип ресурса Среатассессментресулт
description: Представляет элемент результатов оценки угроз.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b6f3b9bdf72a7bf7224693e694ba58868c0ed3ce
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48090888"
---
# <a name="threatassessmentresult-resource-type"></a><span data-ttu-id="0cc9e-103">Тип ресурса Среатассессментресулт</span><span class="sxs-lookup"><span data-stu-id="0cc9e-103">threatAssessmentResult resource type</span></span>

<span data-ttu-id="0cc9e-104">Представляет элемент результатов оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="0cc9e-104">Represents a threat assessment result item.</span></span>

## <a name="properties"></a><span data-ttu-id="0cc9e-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="0cc9e-105">Properties</span></span>

| <span data-ttu-id="0cc9e-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="0cc9e-106">Property</span></span>     | <span data-ttu-id="0cc9e-107">Тип</span><span class="sxs-lookup"><span data-stu-id="0cc9e-107">Type</span></span>        | <span data-ttu-id="0cc9e-108">Описание</span><span class="sxs-lookup"><span data-stu-id="0cc9e-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0cc9e-109">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0cc9e-109">createdDateTime</span></span>|<span data-ttu-id="0cc9e-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0cc9e-110">DateTimeOffset</span></span>|<span data-ttu-id="0cc9e-111">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="0cc9e-111">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0cc9e-112">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="0cc9e-112">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="0cc9e-113">id</span><span class="sxs-lookup"><span data-stu-id="0cc9e-113">id</span></span>|<span data-ttu-id="0cc9e-114">Строка</span><span class="sxs-lookup"><span data-stu-id="0cc9e-114">String</span></span>|<span data-ttu-id="0cc9e-115">Идентификатор результатов оценки угроз — это глобальный уникальный идентификатор (GUID).</span><span class="sxs-lookup"><span data-stu-id="0cc9e-115">The threat assessment result ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="0cc9e-116">message</span><span class="sxs-lookup"><span data-stu-id="0cc9e-116">message</span></span>|<span data-ttu-id="0cc9e-117">String</span><span class="sxs-lookup"><span data-stu-id="0cc9e-117">String</span></span>|<span data-ttu-id="0cc9e-118">Сообщение о результатах для оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="0cc9e-118">The result message for each threat assessment.</span></span>|
|<span data-ttu-id="0cc9e-119">resultType</span><span class="sxs-lookup"><span data-stu-id="0cc9e-119">resultType</span></span>|[<span data-ttu-id="0cc9e-120">среатассессментресулттипе</span><span class="sxs-lookup"><span data-stu-id="0cc9e-120">threatAssessmentResultType</span></span>](enums.md#threatassessmentresulttype-values)|<span data-ttu-id="0cc9e-121">Тип результата оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="0cc9e-121">The threat assessment result type.</span></span> <span data-ttu-id="0cc9e-122">Возможные значения: `checkPolicy`, `rescan`.</span><span class="sxs-lookup"><span data-stu-id="0cc9e-122">Possible values are: `checkPolicy`, `rescan`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0cc9e-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0cc9e-123">JSON representation</span></span>

<span data-ttu-id="0cc9e-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0cc9e-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.threatAssessmentResult",
  "baseType": "",
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

