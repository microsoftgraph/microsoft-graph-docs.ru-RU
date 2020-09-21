---
title: Тип ресурса Лабелингоптионс
description: Представляет параметры меток, которые могут быть предоставлены API оценки.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: da2231ae3eb95260663d2907f56f91b96e08278c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48084025"
---
# <a name="labelingoptions-resource-type"></a><span data-ttu-id="132ad-103">Тип ресурса Лабелингоптионс</span><span class="sxs-lookup"><span data-stu-id="132ad-103">labelingOptions resource type</span></span>

<span data-ttu-id="132ad-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="132ad-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="132ad-105">Представляет параметры меток, которые могут быть предоставлены API оценки.</span><span class="sxs-lookup"><span data-stu-id="132ad-105">Represents the labeling options that can be provided to the evaluation APIs.</span></span> <span data-ttu-id="132ad-106">**лабелингоптионс** необходимо передать в API [евалуатеаппликатион](../api/informationprotectionlabel-evaluateapplication.md) , чтобы указать сведения о метке, которую нужно применить.</span><span class="sxs-lookup"><span data-stu-id="132ad-106">**labelingOptions** must be passed in to the [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md) API to specify details about the label that is to be applied.</span></span> 

## <a name="properties"></a><span data-ttu-id="132ad-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="132ad-107">Properties</span></span>

| <span data-ttu-id="132ad-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="132ad-108">Property</span></span>               | <span data-ttu-id="132ad-109">Тип</span><span class="sxs-lookup"><span data-stu-id="132ad-109">Type</span></span>                                                | <span data-ttu-id="132ad-110">Описание</span><span class="sxs-lookup"><span data-stu-id="132ad-110">Description</span></span>                                                                                                                   |
| :--------------------- | :-------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="132ad-111">assignmentMethod</span><span class="sxs-lookup"><span data-stu-id="132ad-111">assignmentMethod</span></span>       | <span data-ttu-id="132ad-112">Строка</span><span class="sxs-lookup"><span data-stu-id="132ad-112">String</span></span>                                              | <span data-ttu-id="132ad-113">Возможные значения: `standard`, `privileged`, `auto`.</span><span class="sxs-lookup"><span data-stu-id="132ad-113">Possible values are: `standard`, `privileged`, `auto`.</span></span>                                                                        |
| <span data-ttu-id="132ad-114">довнградежустификатион</span><span class="sxs-lookup"><span data-stu-id="132ad-114">downgradeJustification</span></span> | [<span data-ttu-id="132ad-115">довнградежустификатион</span><span class="sxs-lookup"><span data-stu-id="132ad-115">downgradeJustification</span></span>](downgradejustification.md) | <span data-ttu-id="132ad-116">Объект выравнивания на более ранней версии, указывающий, было ли понижение по ширине, и, если да, то причина.</span><span class="sxs-lookup"><span data-stu-id="132ad-116">The downgrade justification object that indicates if downgrade was justified and, if so, the reason.</span></span>                          |
| <span data-ttu-id="132ad-117">екстендедпропертиес</span><span class="sxs-lookup"><span data-stu-id="132ad-117">extendedProperties</span></span>     | <span data-ttu-id="132ad-118">Коллекция [keyValuePair](keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="132ad-118">[keyValuePair](keyvaluepair.md) collection</span></span>          | <span data-ttu-id="132ad-119">Расширенные свойства будут проанализированы и возвращены в стандартном формате метаданных МИП в составе сведений о метке.</span><span class="sxs-lookup"><span data-stu-id="132ad-119">Extended properties will be parsed and returned in the standard MIP labeled metadata format as part of the label information.</span></span> |
| <span data-ttu-id="132ad-120">лабелид</span><span class="sxs-lookup"><span data-stu-id="132ad-120">labelId</span></span>                | <span data-ttu-id="132ad-121">Guid</span><span class="sxs-lookup"><span data-stu-id="132ad-121">Guid</span></span>                                                | <span data-ttu-id="132ad-122">GUID метки, которая должна быть применена к данным.</span><span class="sxs-lookup"><span data-stu-id="132ad-122">The GUID of the label that should be applied to the information.</span></span>                                                              |

## <a name="json-representation"></a><span data-ttu-id="132ad-123">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="132ad-123">JSON representation</span></span>

<span data-ttu-id="132ad-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="132ad-124">The following is a JSON representation of the resource.</span></span>

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

