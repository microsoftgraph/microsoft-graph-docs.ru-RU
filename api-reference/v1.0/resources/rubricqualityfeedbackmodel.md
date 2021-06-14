---
title: rubricQualityFeedbackModel type
description: Обратная связь, связанная с определенным качеством образованияRubric.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 8f96a1fd0ce0d007c138928c316316349a7b302e
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911519"
---
# <a name="rubricqualityfeedbackmodel-resource-type"></a><span data-ttu-id="5fff8-103">rubricQualityFeedbackModel type</span><span class="sxs-lookup"><span data-stu-id="5fff8-103">rubricQualityFeedbackModel resource type</span></span>

<span data-ttu-id="5fff8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5fff8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5fff8-105">Отзывы, связанные с [определенным качеством](rubricquality.md) [образованияRubric](educationrubric.md).</span><span class="sxs-lookup"><span data-stu-id="5fff8-105">Feedback related to a specific [quality](rubricquality.md) of an [educationRubric](educationrubric.md).</span></span>

## <a name="properties"></a><span data-ttu-id="5fff8-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="5fff8-106">Properties</span></span>

| <span data-ttu-id="5fff8-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="5fff8-107">Property</span></span>     | <span data-ttu-id="5fff8-108">Тип</span><span class="sxs-lookup"><span data-stu-id="5fff8-108">Type</span></span>        | <span data-ttu-id="5fff8-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5fff8-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5fff8-110">feedback</span><span class="sxs-lookup"><span data-stu-id="5fff8-110">feedback</span></span>|[<span data-ttu-id="5fff8-111">itemBody</span><span class="sxs-lookup"><span data-stu-id="5fff8-111">itemBody</span></span>](itembody.md)|<span data-ttu-id="5fff8-112">Конкретные отзывы по одному качеству этой рубрики.</span><span class="sxs-lookup"><span data-stu-id="5fff8-112">Specific feedback for one quality of this rubric.</span></span>|
|<span data-ttu-id="5fff8-113">qualityId</span><span class="sxs-lookup"><span data-stu-id="5fff8-113">qualityId</span></span>|<span data-ttu-id="5fff8-114">String</span><span class="sxs-lookup"><span data-stu-id="5fff8-114">String</span></span>|<span data-ttu-id="5fff8-115">ID [рубрикQuality,](rubricquality.md) с чем связана эта обратная связь.</span><span class="sxs-lookup"><span data-stu-id="5fff8-115">The ID of the [rubricQuality](rubricquality.md) that this feedback is related to.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5fff8-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5fff8-116">JSON representation</span></span>

<span data-ttu-id="5fff8-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5fff8-117">The following is a JSON representation of the resource.</span></span>

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

