---
title: Тип ресурса Рубриккуалитифидбаккмодел
description: Обратная связь, связанная с определенным качеством Едукатионрубрик
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 0a7c2b80a2cef18b50157ae9a54c66d35822fa51
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173302"
---
# <a name="rubricqualityfeedbackmodel-resource-type"></a><span data-ttu-id="7193e-103">Тип ресурса Рубриккуалитифидбаккмодел</span><span class="sxs-lookup"><span data-stu-id="7193e-103">rubricQualityFeedbackModel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7193e-104">Обратная связь, связанная с определенным [качеством](rubricquality.md) [едукатионрубрик](educationrubric.md).</span><span class="sxs-lookup"><span data-stu-id="7193e-104">Feedback related to a specific [quality](rubricquality.md) of an [educationRubric](educationrubric.md).</span></span>

## <a name="properties"></a><span data-ttu-id="7193e-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="7193e-105">Properties</span></span>

| <span data-ttu-id="7193e-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="7193e-106">Property</span></span>     | <span data-ttu-id="7193e-107">Тип</span><span class="sxs-lookup"><span data-stu-id="7193e-107">Type</span></span>        | <span data-ttu-id="7193e-108">Описание</span><span class="sxs-lookup"><span data-stu-id="7193e-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7193e-109">feedback</span><span class="sxs-lookup"><span data-stu-id="7193e-109">feedback</span></span>|[<span data-ttu-id="7193e-110">itemBody</span><span class="sxs-lookup"><span data-stu-id="7193e-110">itemBody</span></span>](itembody.md)|<span data-ttu-id="7193e-111">Особая обратная связь для одного качества этого Rubric.</span><span class="sxs-lookup"><span data-stu-id="7193e-111">Specific feedback for one quality of this rubric.</span></span>|
|<span data-ttu-id="7193e-112">Куалитид</span><span class="sxs-lookup"><span data-stu-id="7193e-112">qualityId</span></span>|<span data-ttu-id="7193e-113">String</span><span class="sxs-lookup"><span data-stu-id="7193e-113">String</span></span>|<span data-ttu-id="7193e-114">Идентификатор [рубриккуалити](rubricquality.md) , с которым связана эта обратная связь.</span><span class="sxs-lookup"><span data-stu-id="7193e-114">The ID of the [rubricQuality](rubricquality.md) that this feedback is related to.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7193e-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7193e-115">JSON representation</span></span>

<span data-ttu-id="7193e-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7193e-116">The following is a JSON representation of the resource.</span></span>

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