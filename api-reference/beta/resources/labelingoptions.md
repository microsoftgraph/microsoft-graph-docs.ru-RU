---
title: Тип ресурса labelingOptions
description: Представляет параметры маркировки, которые могут быть предоставлены API оценки.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 7d2409bf538de3d37ca32cdf2fd1afb78a659817
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950309"
---
# <a name="labelingoptions-resource-type"></a><span data-ttu-id="60ac1-103">Тип ресурса labelingOptions</span><span class="sxs-lookup"><span data-stu-id="60ac1-103">labelingOptions resource type</span></span>

<span data-ttu-id="60ac1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60ac1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60ac1-105">Представляет параметры маркировки, которые могут быть предоставлены API оценки.</span><span class="sxs-lookup"><span data-stu-id="60ac1-105">Represents the labeling options that can be provided to the evaluation APIs.</span></span> <span data-ttu-id="60ac1-106">**LabelingOptions** необходимо передать в API [evaluateApplication,](../api/informationprotectionlabel-evaluateapplication.md) чтобы указать сведения о метки, которая должна быть применена.</span><span class="sxs-lookup"><span data-stu-id="60ac1-106">**labelingOptions** must be passed in to the [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md) API to specify details about the label that is to be applied.</span></span> 

## <a name="properties"></a><span data-ttu-id="60ac1-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="60ac1-107">Properties</span></span>

| <span data-ttu-id="60ac1-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="60ac1-108">Property</span></span>               | <span data-ttu-id="60ac1-109">Тип</span><span class="sxs-lookup"><span data-stu-id="60ac1-109">Type</span></span>                                                | <span data-ttu-id="60ac1-110">Описание</span><span class="sxs-lookup"><span data-stu-id="60ac1-110">Description</span></span>                                                                                                                   |
| :--------------------- | :-------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="60ac1-111">assignmentMethod</span><span class="sxs-lookup"><span data-stu-id="60ac1-111">assignmentMethod</span></span>       | <span data-ttu-id="60ac1-112">Строка</span><span class="sxs-lookup"><span data-stu-id="60ac1-112">String</span></span>                                              | <span data-ttu-id="60ac1-113">Возможные значения: `standard`, `privileged`, `auto`.</span><span class="sxs-lookup"><span data-stu-id="60ac1-113">Possible values are: `standard`, `privileged`, `auto`.</span></span>                                                                        |
| <span data-ttu-id="60ac1-114">downgradeJustification</span><span class="sxs-lookup"><span data-stu-id="60ac1-114">downgradeJustification</span></span> | [<span data-ttu-id="60ac1-115">downgradeJustification</span><span class="sxs-lookup"><span data-stu-id="60ac1-115">downgradeJustification</span></span>](downgradejustification.md) | <span data-ttu-id="60ac1-116">Объект обоснования понижения, который указывает, было ли понижение оправдано, и если да, то причина.</span><span class="sxs-lookup"><span data-stu-id="60ac1-116">The downgrade justification object that indicates if downgrade was justified and, if so, the reason.</span></span>                          |
| <span data-ttu-id="60ac1-117">расширенные свойства</span><span class="sxs-lookup"><span data-stu-id="60ac1-117">extendedProperties</span></span>     | <span data-ttu-id="60ac1-118">Коллекция [keyValuePair](keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="60ac1-118">[keyValuePair](keyvaluepair.md) collection</span></span>          | <span data-ttu-id="60ac1-119">Расширенные свойства будут разобрано и возвращены в стандартном формате метаданных MIP с меткой в качестве части сведений о метки.</span><span class="sxs-lookup"><span data-stu-id="60ac1-119">Extended properties will be parsed and returned in the standard MIP labeled metadata format as part of the label information.</span></span> |
| <span data-ttu-id="60ac1-120">labelId</span><span class="sxs-lookup"><span data-stu-id="60ac1-120">labelId</span></span>                | <span data-ttu-id="60ac1-121">Guid</span><span class="sxs-lookup"><span data-stu-id="60ac1-121">Guid</span></span>                                                | <span data-ttu-id="60ac1-122">GUID метки, которая должна применяться к данным.</span><span class="sxs-lookup"><span data-stu-id="60ac1-122">The GUID of the label that should be applied to the information.</span></span>                                                              |

## <a name="json-representation"></a><span data-ttu-id="60ac1-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="60ac1-123">JSON representation</span></span>

<span data-ttu-id="60ac1-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="60ac1-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.labelingOptions",
  "baseType": null
}-->

```json
{
  "assignmentMethod": "String",
  "downgradeJustification": {"@odata.type": "microsoft.graph.downgradeJustification"},
  "extendedProperties": [{"@odata.type": "microsoft.graph.keyValuePair"}],
  "labelId": "Guid"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "labelingOptions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

