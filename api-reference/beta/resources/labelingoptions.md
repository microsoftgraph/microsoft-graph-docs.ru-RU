---
title: Тип ресурса Лабелингоптионс
description: Представляет параметры меток, которые могут быть предоставлены API оценки.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f8883c08bbd1f351dc5de003988f36c727ef85d7
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939301"
---
# <a name="labelingoptions-resource-type"></a><span data-ttu-id="12604-103">Тип ресурса Лабелингоптионс</span><span class="sxs-lookup"><span data-stu-id="12604-103">labelingOptions resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12604-104">Представляет параметры меток, которые могут быть предоставлены API оценки.</span><span class="sxs-lookup"><span data-stu-id="12604-104">Represents the labeling options that can be provided to the evaluation APIs.</span></span> <span data-ttu-id="12604-105">**лабелингоптионс** необходимо передать в API [евалуатеаппликатион](../api/informationprotectionlabel-evaluateapplication.md) , чтобы указать сведения о метке, которую нужно применить.</span><span class="sxs-lookup"><span data-stu-id="12604-105">**labelingOptions** must be passed in to the [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md) API to specify details about the label that is to be applied.</span></span> 

## <a name="properties"></a><span data-ttu-id="12604-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="12604-106">Properties</span></span>

| <span data-ttu-id="12604-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="12604-107">Property</span></span>               | <span data-ttu-id="12604-108">Тип</span><span class="sxs-lookup"><span data-stu-id="12604-108">Type</span></span>                                                | <span data-ttu-id="12604-109">Описание</span><span class="sxs-lookup"><span data-stu-id="12604-109">Description</span></span>                                                                                                                   |
| :--------------------- | :-------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="12604-110">assignmentMethod</span><span class="sxs-lookup"><span data-stu-id="12604-110">assignmentMethod</span></span>       | <span data-ttu-id="12604-111">Строка</span><span class="sxs-lookup"><span data-stu-id="12604-111">String</span></span>                                              | <span data-ttu-id="12604-112">Возможные значения: `standard`, `privileged`, `auto`.</span><span class="sxs-lookup"><span data-stu-id="12604-112">Possible values are: `standard`, `privileged`, `auto`.</span></span>                                                                        |
| <span data-ttu-id="12604-113">довнградежустификатион</span><span class="sxs-lookup"><span data-stu-id="12604-113">downgradeJustification</span></span> | [<span data-ttu-id="12604-114">довнградежустификатион</span><span class="sxs-lookup"><span data-stu-id="12604-114">downgradeJustification</span></span>](downgradejustification.md) | <span data-ttu-id="12604-115">Объект выравнивания на более ранней версии, указывающий, было ли понижение по ширине, и, если да, то причина.</span><span class="sxs-lookup"><span data-stu-id="12604-115">The downgrade justification object that indicates if downgrade was justified and, if so, the reason.</span></span>                          |
| <span data-ttu-id="12604-116">екстендедпропертиес</span><span class="sxs-lookup"><span data-stu-id="12604-116">extendedProperties</span></span>     | <span data-ttu-id="12604-117">Коллекция [keyValuePair](keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="12604-117">[keyValuePair](keyvaluepair.md) collection</span></span>          | <span data-ttu-id="12604-118">Расширенные свойства будут проанализированы и возвращены в стандартном формате метаданных МИП в составе сведений о метке.</span><span class="sxs-lookup"><span data-stu-id="12604-118">Extended properties will be parsed and returned in the standard MIP labeled metadata format as part of the label information.</span></span> |
| <span data-ttu-id="12604-119">лабелид</span><span class="sxs-lookup"><span data-stu-id="12604-119">labelId</span></span>                | <span data-ttu-id="12604-120">GUID</span><span class="sxs-lookup"><span data-stu-id="12604-120">Guid</span></span>                                                | <span data-ttu-id="12604-121">GUID метки, которая должна быть применена к данным.</span><span class="sxs-lookup"><span data-stu-id="12604-121">The GUID of the label that should be applied to the information.</span></span>                                                              |

## <a name="json-representation"></a><span data-ttu-id="12604-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="12604-122">JSON representation</span></span>

<span data-ttu-id="12604-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="12604-123">The following is a JSON representation of the resource.</span></span>

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