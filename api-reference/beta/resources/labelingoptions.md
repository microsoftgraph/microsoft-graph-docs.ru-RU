---
title: Тип ресурса Лабелингоптионс
description: Представляет параметры меток, которые могут быть предоставлены API оценки.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 97557ad6e233506e5e074c408ffb04f83297f0af
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523004"
---
# <a name="labelingoptions-resource-type"></a><span data-ttu-id="51ec9-103">Тип ресурса Лабелингоптионс</span><span class="sxs-lookup"><span data-stu-id="51ec9-103">labelingOptions resource type</span></span>

<span data-ttu-id="51ec9-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="51ec9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51ec9-105">Представляет параметры меток, которые могут быть предоставлены API оценки.</span><span class="sxs-lookup"><span data-stu-id="51ec9-105">Represents the labeling options that can be provided to the evaluation APIs.</span></span> <span data-ttu-id="51ec9-106">**лабелингоптионс** необходимо передать в API [евалуатеаппликатион](../api/informationprotectionlabel-evaluateapplication.md) , чтобы указать сведения о метке, которую нужно применить.</span><span class="sxs-lookup"><span data-stu-id="51ec9-106">**labelingOptions** must be passed in to the [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md) API to specify details about the label that is to be applied.</span></span> 

## <a name="properties"></a><span data-ttu-id="51ec9-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="51ec9-107">Properties</span></span>

| <span data-ttu-id="51ec9-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="51ec9-108">Property</span></span>               | <span data-ttu-id="51ec9-109">Тип</span><span class="sxs-lookup"><span data-stu-id="51ec9-109">Type</span></span>                                                | <span data-ttu-id="51ec9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="51ec9-110">Description</span></span>                                                                                                                   |
| :--------------------- | :-------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="51ec9-111">assignmentMethod</span><span class="sxs-lookup"><span data-stu-id="51ec9-111">assignmentMethod</span></span>       | <span data-ttu-id="51ec9-112">String</span><span class="sxs-lookup"><span data-stu-id="51ec9-112">String</span></span>                                              | <span data-ttu-id="51ec9-113">Возможные значения: `standard`, `privileged`, `auto`.</span><span class="sxs-lookup"><span data-stu-id="51ec9-113">Possible values are: `standard`, `privileged`, `auto`.</span></span>                                                                        |
| <span data-ttu-id="51ec9-114">довнградежустификатион</span><span class="sxs-lookup"><span data-stu-id="51ec9-114">downgradeJustification</span></span> | [<span data-ttu-id="51ec9-115">довнградежустификатион</span><span class="sxs-lookup"><span data-stu-id="51ec9-115">downgradeJustification</span></span>](downgradejustification.md) | <span data-ttu-id="51ec9-116">Объект выравнивания на более ранней версии, указывающий, было ли понижение по ширине, и, если да, то причина.</span><span class="sxs-lookup"><span data-stu-id="51ec9-116">The downgrade justification object that indicates if downgrade was justified and, if so, the reason.</span></span>                          |
| <span data-ttu-id="51ec9-117">екстендедпропертиес</span><span class="sxs-lookup"><span data-stu-id="51ec9-117">extendedProperties</span></span>     | <span data-ttu-id="51ec9-118">Коллекция [keyValuePair](keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="51ec9-118">[keyValuePair](keyvaluepair.md) collection</span></span>          | <span data-ttu-id="51ec9-119">Расширенные свойства будут проанализированы и возвращены в стандартном формате метаданных МИП в составе сведений о метке.</span><span class="sxs-lookup"><span data-stu-id="51ec9-119">Extended properties will be parsed and returned in the standard MIP labeled metadata format as part of the label information.</span></span> |
| <span data-ttu-id="51ec9-120">лабелид</span><span class="sxs-lookup"><span data-stu-id="51ec9-120">labelId</span></span>                | <span data-ttu-id="51ec9-121">GUID</span><span class="sxs-lookup"><span data-stu-id="51ec9-121">Guid</span></span>                                                | <span data-ttu-id="51ec9-122">GUID метки, которая должна быть применена к данным.</span><span class="sxs-lookup"><span data-stu-id="51ec9-122">The GUID of the label that should be applied to the information.</span></span>                                                              |

## <a name="json-representation"></a><span data-ttu-id="51ec9-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="51ec9-123">JSON representation</span></span>

<span data-ttu-id="51ec9-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="51ec9-124">The following is a JSON representation of the resource.</span></span>

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