---
title: Тип ресурса Среатассессментресулт
description: Представляет элемент результатов оценки угроз.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5e90c574ba5c89dc527f5cee236d721514834875
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519773"
---
# <a name="threatassessmentresult-resource-type"></a><span data-ttu-id="3c705-103">Тип ресурса Среатассессментресулт</span><span class="sxs-lookup"><span data-stu-id="3c705-103">threatAssessmentResult resource type</span></span>

<span data-ttu-id="3c705-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3c705-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c705-105">Представляет элемент результатов оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="3c705-105">Represents a threat assessment result item.</span></span>

## <a name="properties"></a><span data-ttu-id="3c705-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="3c705-106">Properties</span></span>

| <span data-ttu-id="3c705-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="3c705-107">Property</span></span>     | <span data-ttu-id="3c705-108">Тип</span><span class="sxs-lookup"><span data-stu-id="3c705-108">Type</span></span>        | <span data-ttu-id="3c705-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3c705-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3c705-110">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3c705-110">createdDateTime</span></span>|<span data-ttu-id="3c705-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c705-111">DateTimeOffset</span></span>|<span data-ttu-id="3c705-112">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="3c705-112">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3c705-113">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="3c705-113">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="3c705-114">id</span><span class="sxs-lookup"><span data-stu-id="3c705-114">id</span></span>|<span data-ttu-id="3c705-115">Строка</span><span class="sxs-lookup"><span data-stu-id="3c705-115">String</span></span>|<span data-ttu-id="3c705-116">Идентификатор результатов оценки угроз — это глобальный уникальный идентификатор (GUID).</span><span class="sxs-lookup"><span data-stu-id="3c705-116">The threat assessment result ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="3c705-117">message</span><span class="sxs-lookup"><span data-stu-id="3c705-117">message</span></span>|<span data-ttu-id="3c705-118">String</span><span class="sxs-lookup"><span data-stu-id="3c705-118">String</span></span>|<span data-ttu-id="3c705-119">Сообщение о результатах для оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="3c705-119">The result message for each threat assessment.</span></span>|
|<span data-ttu-id="3c705-120">resultType</span><span class="sxs-lookup"><span data-stu-id="3c705-120">resultType</span></span>|[<span data-ttu-id="3c705-121">среатассессментресулттипе</span><span class="sxs-lookup"><span data-stu-id="3c705-121">threatAssessmentResultType</span></span>](enums.md#threatassessmentresulttype-values)|<span data-ttu-id="3c705-122">Тип результата оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="3c705-122">The threat assessment result type.</span></span> <span data-ttu-id="3c705-123">Возможные значения: `checkPolicy`, `rescan`.</span><span class="sxs-lookup"><span data-stu-id="3c705-123">Possible values are: `checkPolicy`, `rescan`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3c705-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3c705-124">JSON representation</span></span>

<span data-ttu-id="3c705-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3c705-125">The following is a JSON representation of the resource.</span></span>

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
