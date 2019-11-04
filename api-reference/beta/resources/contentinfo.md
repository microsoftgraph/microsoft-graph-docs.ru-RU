---
title: Тип ресурса Контентинфо
description: Представляет текущее состояние некоторых сведений, которые необходимо подписать.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5191be0533810f0a9da3b0ea83f209d69cc67297
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938879"
---
# <a name="contentinfo-resource-type"></a><span data-ttu-id="4f334-103">Тип ресурса Контентинфо</span><span class="sxs-lookup"><span data-stu-id="4f334-103">contentInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f334-104">Представляет текущее состояние некоторых сведений, которые необходимо подписать.</span><span class="sxs-lookup"><span data-stu-id="4f334-104">Represents the current state of some information that is to be labeled.</span></span> <span data-ttu-id="4f334-105">**контентинфо** передается в API [евалуатеремовал](../api/informationprotectionlabel-evaluateRemoval.md), [ЕВАЛУАТЕАППЛИКАТИОН](../api/informationprotectionlabel-evaluateApplication.md)и [евалуатеклассификатионресултс](../api/informationprotectionlabel-evaluateClassificationResults.md) для описания API текущего состояния информации.</span><span class="sxs-lookup"><span data-stu-id="4f334-105">**contentInfo** is passed in to the [evaluateRemoval](../api/informationprotectionlabel-evaluateRemoval.md), [evaluateApplication](../api/informationprotectionlabel-evaluateApplication.md), and [evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md) APIs to describe to the API the current state of the information.</span></span> <span data-ttu-id="4f334-106">В этом **контентинфо** подробные сведения о том, какие метаданные, маркировка содержимого и защита должны добавляться или удаляться при применении, обновлении или удалении метки.</span><span class="sxs-lookup"><span data-stu-id="4f334-106">This **contentInfo** detail drives the results on what metadata, content marking, and protection should be added or removed when the label is applied, updated, or removed.</span></span> 

## <a name="properties"></a><span data-ttu-id="4f334-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4f334-107">Properties</span></span>

| <span data-ttu-id="4f334-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="4f334-108">Property</span></span>   | <span data-ttu-id="4f334-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4f334-109">Type</span></span>                                       | <span data-ttu-id="4f334-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4f334-110">Description</span></span>                                                                                                                     |
| :--------- | :----------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="4f334-111">format</span><span class="sxs-lookup"><span data-stu-id="4f334-111">format</span></span>     | <span data-ttu-id="4f334-112">String</span><span class="sxs-lookup"><span data-stu-id="4f334-112">String</span></span>                                     | <span data-ttu-id="4f334-113">Возможные значения: `default`, `email`.</span><span class="sxs-lookup"><span data-stu-id="4f334-113">Possible values are: `default`, `email`.</span></span>                                                                                        |
| <span data-ttu-id="4f334-114">идентификатор</span><span class="sxs-lookup"><span data-stu-id="4f334-114">identifier</span></span> | <span data-ttu-id="4f334-115">Строка</span><span class="sxs-lookup"><span data-stu-id="4f334-115">String</span></span>                                     | <span data-ttu-id="4f334-116">Идентификатор, используемый для аналитики Azure Information Protection.</span><span class="sxs-lookup"><span data-stu-id="4f334-116">Identifier used for Azure Information Protection Analytics.</span></span>                                                                     |
| <span data-ttu-id="4f334-117">метаданных</span><span class="sxs-lookup"><span data-stu-id="4f334-117">metadata</span></span>   | <span data-ttu-id="4f334-118">Коллекция [keyValuePair](keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="4f334-118">[keyValuePair](keyvaluepair.md) collection</span></span> | <span data-ttu-id="4f334-119">Существующие метаданные Microsoft Information Protection передаются в виде пар "ключ-значение", где ключ является MSIP_Label_GUID_PropName.</span><span class="sxs-lookup"><span data-stu-id="4f334-119">Existing Microsoft Information Protection metadata is passed as key/value pairs, where the key is the MSIP_Label_GUID_PropName.</span></span> |
| <span data-ttu-id="4f334-120">state</span><span class="sxs-lookup"><span data-stu-id="4f334-120">state</span></span>      | <span data-ttu-id="4f334-121">String</span><span class="sxs-lookup"><span data-stu-id="4f334-121">String</span></span>                                     | <span data-ttu-id="4f334-122">Возможные значения: `rest`, `motion`, `use`.</span><span class="sxs-lookup"><span data-stu-id="4f334-122">Possible values are: `rest`, `motion`, `use`.</span></span>                                                                                   |

## <a name="json-representation"></a><span data-ttu-id="4f334-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4f334-123">JSON representation</span></span>

<span data-ttu-id="4f334-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4f334-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.contentInfo",
  "baseType": null
}-->

```json
{
  "format": "String",
  "identifier": "String",
  "metadata": [{"@odata.type": "microsoft.graph.keyValuePair"}],
  "state": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contentInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->