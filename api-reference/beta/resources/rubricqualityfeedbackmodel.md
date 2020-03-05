---
title: Тип ресурса Рубриккуалитифидбаккмодел
description: Обратная связь, связанная с определенным качеством Едукатионрубрик
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 22c69292441f4b71238e820229e9d733bd9cabb9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521000"
---
# <a name="rubricqualityfeedbackmodel-resource-type"></a><span data-ttu-id="601c5-103">Тип ресурса Рубриккуалитифидбаккмодел</span><span class="sxs-lookup"><span data-stu-id="601c5-103">rubricQualityFeedbackModel resource type</span></span>

<span data-ttu-id="601c5-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="601c5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="601c5-105">Обратная связь, связанная с определенным [качеством](rubricquality.md) [едукатионрубрик](educationrubric.md).</span><span class="sxs-lookup"><span data-stu-id="601c5-105">Feedback related to a specific [quality](rubricquality.md) of an [educationRubric](educationrubric.md).</span></span>

## <a name="properties"></a><span data-ttu-id="601c5-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="601c5-106">Properties</span></span>

| <span data-ttu-id="601c5-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="601c5-107">Property</span></span>     | <span data-ttu-id="601c5-108">Тип</span><span class="sxs-lookup"><span data-stu-id="601c5-108">Type</span></span>        | <span data-ttu-id="601c5-109">Описание</span><span class="sxs-lookup"><span data-stu-id="601c5-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="601c5-110">feedback</span><span class="sxs-lookup"><span data-stu-id="601c5-110">feedback</span></span>|[<span data-ttu-id="601c5-111">itemBody</span><span class="sxs-lookup"><span data-stu-id="601c5-111">itemBody</span></span>](itembody.md)|<span data-ttu-id="601c5-112">Особая обратная связь для одного качества этого Rubric.</span><span class="sxs-lookup"><span data-stu-id="601c5-112">Specific feedback for one quality of this rubric.</span></span>|
|<span data-ttu-id="601c5-113">куалитид</span><span class="sxs-lookup"><span data-stu-id="601c5-113">qualityId</span></span>|<span data-ttu-id="601c5-114">String</span><span class="sxs-lookup"><span data-stu-id="601c5-114">String</span></span>|<span data-ttu-id="601c5-115">Идентификатор [рубриккуалити](rubricquality.md) , с которым связана эта обратная связь.</span><span class="sxs-lookup"><span data-stu-id="601c5-115">The ID of the [rubricQuality](rubricquality.md) that this feedback is related to.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="601c5-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="601c5-116">JSON representation</span></span>

<span data-ttu-id="601c5-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="601c5-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rubricQualityFeedbackModel",
  "baseType": null
}-->

```json
{
  "feedback": {"@odata.type": "microsoft.graph.itemBody"},
  "qualityId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rubricQualityFeedbackModel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->