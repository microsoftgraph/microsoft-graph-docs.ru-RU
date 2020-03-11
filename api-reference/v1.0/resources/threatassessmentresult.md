---
title: Тип ресурса Среатассессментресулт
description: Представляет элемент результатов оценки угроз.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e654c3c8878db10f160a4c4909fe2a8ca8b5d184
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2020
ms.locfileid: "42591504"
---
# <a name="threatassessmentresult-resource-type"></a><span data-ttu-id="13d56-103">Тип ресурса Среатассессментресулт</span><span class="sxs-lookup"><span data-stu-id="13d56-103">threatAssessmentResult resource type</span></span>

<span data-ttu-id="13d56-104">Представляет элемент результатов оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="13d56-104">Represents a threat assessment result item.</span></span>

## <a name="properties"></a><span data-ttu-id="13d56-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="13d56-105">Properties</span></span>

| <span data-ttu-id="13d56-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="13d56-106">Property</span></span>     | <span data-ttu-id="13d56-107">Тип</span><span class="sxs-lookup"><span data-stu-id="13d56-107">Type</span></span>        | <span data-ttu-id="13d56-108">Описание</span><span class="sxs-lookup"><span data-stu-id="13d56-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="13d56-109">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="13d56-109">createdDateTime</span></span>|<span data-ttu-id="13d56-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13d56-110">DateTimeOffset</span></span>|<span data-ttu-id="13d56-111">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="13d56-111">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="13d56-112">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="13d56-112">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="13d56-113">id</span><span class="sxs-lookup"><span data-stu-id="13d56-113">id</span></span>|<span data-ttu-id="13d56-114">Строка</span><span class="sxs-lookup"><span data-stu-id="13d56-114">String</span></span>|<span data-ttu-id="13d56-115">Идентификатор результатов оценки угроз — это глобальный уникальный идентификатор (GUID).</span><span class="sxs-lookup"><span data-stu-id="13d56-115">The threat assessment result ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="13d56-116">message</span><span class="sxs-lookup"><span data-stu-id="13d56-116">message</span></span>|<span data-ttu-id="13d56-117">String</span><span class="sxs-lookup"><span data-stu-id="13d56-117">String</span></span>|<span data-ttu-id="13d56-118">Сообщение о результатах для оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="13d56-118">The result message for each threat assessment.</span></span>|
|<span data-ttu-id="13d56-119">resultType</span><span class="sxs-lookup"><span data-stu-id="13d56-119">resultType</span></span>|[<span data-ttu-id="13d56-120">среатассессментресулттипе</span><span class="sxs-lookup"><span data-stu-id="13d56-120">threatAssessmentResultType</span></span>](enums.md#threatassessmentresulttype-values)|<span data-ttu-id="13d56-121">Тип результата оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="13d56-121">The threat assessment result type.</span></span> <span data-ttu-id="13d56-122">Возможные значения: `checkPolicy`, `rescan`.</span><span class="sxs-lookup"><span data-stu-id="13d56-122">Possible values are: `checkPolicy`, `rescan`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="13d56-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="13d56-123">JSON representation</span></span>

<span data-ttu-id="13d56-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="13d56-124">The following is a JSON representation of the resource.</span></span>

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
