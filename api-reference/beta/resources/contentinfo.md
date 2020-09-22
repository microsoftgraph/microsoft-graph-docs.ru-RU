---
title: Тип ресурса Контентинфо
description: Представляет текущее состояние некоторых сведений, которые необходимо подписать.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d7e0c159d46cb680329efc6a93896ca3df7270f7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998923"
---
# <a name="contentinfo-resource-type"></a><span data-ttu-id="56932-103">Тип ресурса Контентинфо</span><span class="sxs-lookup"><span data-stu-id="56932-103">contentInfo resource type</span></span>

<span data-ttu-id="56932-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56932-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56932-105">Представляет текущее состояние некоторых сведений, которые необходимо подписать.</span><span class="sxs-lookup"><span data-stu-id="56932-105">Represents the current state of some information that is to be labeled.</span></span> <span data-ttu-id="56932-106">**контентинфо** передается в API [евалуатеремовал](../api/informationprotectionlabel-evaluateRemoval.md), [ЕВАЛУАТЕАППЛИКАТИОН](../api/informationprotectionlabel-evaluateApplication.md)и [евалуатеклассификатионресултс](../api/informationprotectionlabel-evaluateClassificationResults.md) для описания API текущего состояния информации.</span><span class="sxs-lookup"><span data-stu-id="56932-106">**contentInfo** is passed in to the [evaluateRemoval](../api/informationprotectionlabel-evaluateRemoval.md), [evaluateApplication](../api/informationprotectionlabel-evaluateApplication.md), and [evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md) APIs to describe to the API the current state of the information.</span></span> <span data-ttu-id="56932-107">В этом **контентинфо** подробные сведения о том, какие метаданные, маркировка содержимого и защита должны добавляться или удаляться при применении, обновлении или удалении метки.</span><span class="sxs-lookup"><span data-stu-id="56932-107">This **contentInfo** detail drives the results on what metadata, content marking, and protection should be added or removed when the label is applied, updated, or removed.</span></span> 

## <a name="properties"></a><span data-ttu-id="56932-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="56932-108">Properties</span></span>

| <span data-ttu-id="56932-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="56932-109">Property</span></span>   | <span data-ttu-id="56932-110">Тип</span><span class="sxs-lookup"><span data-stu-id="56932-110">Type</span></span>                                       | <span data-ttu-id="56932-111">Описание</span><span class="sxs-lookup"><span data-stu-id="56932-111">Description</span></span>                                                                                                                     |
| :--------- | :----------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="56932-112">format</span><span class="sxs-lookup"><span data-stu-id="56932-112">format</span></span>     | <span data-ttu-id="56932-113">String</span><span class="sxs-lookup"><span data-stu-id="56932-113">String</span></span>                                     | <span data-ttu-id="56932-114">Возможные значения: `default`, `email`.</span><span class="sxs-lookup"><span data-stu-id="56932-114">Possible values are: `default`, `email`.</span></span>                                                                                        |
| <span data-ttu-id="56932-115">идентификатор</span><span class="sxs-lookup"><span data-stu-id="56932-115">identifier</span></span> | <span data-ttu-id="56932-116">String</span><span class="sxs-lookup"><span data-stu-id="56932-116">String</span></span>                                     | <span data-ttu-id="56932-117">Идентификатор, используемый для аналитики Azure Information Protection.</span><span class="sxs-lookup"><span data-stu-id="56932-117">Identifier used for Azure Information Protection Analytics.</span></span>                                                                     |
| <span data-ttu-id="56932-118">метаданных</span><span class="sxs-lookup"><span data-stu-id="56932-118">metadata</span></span>   | <span data-ttu-id="56932-119">Коллекция [keyValuePair](keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="56932-119">[keyValuePair](keyvaluepair.md) collection</span></span> | <span data-ttu-id="56932-120">Существующие метаданные Microsoft Information Protection передаются в виде пар "ключ-значение", где ключ — это MSIP_Label_GUID_PropName.</span><span class="sxs-lookup"><span data-stu-id="56932-120">Existing Microsoft Information Protection metadata is passed as key/value pairs, where the key is the MSIP_Label_GUID_PropName.</span></span> |
| <span data-ttu-id="56932-121">state</span><span class="sxs-lookup"><span data-stu-id="56932-121">state</span></span>      | <span data-ttu-id="56932-122">String</span><span class="sxs-lookup"><span data-stu-id="56932-122">String</span></span>                                     | <span data-ttu-id="56932-123">Возможные значения: `rest`, `motion`, `use`.</span><span class="sxs-lookup"><span data-stu-id="56932-123">Possible values are: `rest`, `motion`, `use`.</span></span>                                                                                   |

## <a name="json-representation"></a><span data-ttu-id="56932-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="56932-124">JSON representation</span></span>

<span data-ttu-id="56932-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="56932-125">The following is a JSON representation of the resource.</span></span>

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

