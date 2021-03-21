---
title: тип ресурса contentInfo
description: Представляет текущее состояние некоторых сведений, которые должны быть помечены.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 939d7730c0de2ffb13d4dbdcade6f7c2fbce5de4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962653"
---
# <a name="contentinfo-resource-type"></a><span data-ttu-id="eeff6-103">тип ресурса contentInfo</span><span class="sxs-lookup"><span data-stu-id="eeff6-103">contentInfo resource type</span></span>

<span data-ttu-id="eeff6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eeff6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eeff6-105">Представляет текущее состояние некоторых сведений, которые должны быть помечены.</span><span class="sxs-lookup"><span data-stu-id="eeff6-105">Represents the current state of some information that is to be labeled.</span></span> <span data-ttu-id="eeff6-106">**contentInfo** передается в a [evaluateRemoval,](../api/informationprotectionlabel-evaluateRemoval.md) [evaluateApplication](../api/informationprotectionlabel-evaluateApplication.md)и [evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md) API, чтобы описать API текущее состояние информации.</span><span class="sxs-lookup"><span data-stu-id="eeff6-106">**contentInfo** is passed in to the [evaluateRemoval](../api/informationprotectionlabel-evaluateRemoval.md), [evaluateApplication](../api/informationprotectionlabel-evaluateApplication.md), and [evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md) APIs to describe to the API the current state of the information.</span></span> <span data-ttu-id="eeff6-107">В **этом содержимогоInfo** приводится информация о том, какие метаданные, маркировка контента и защита должны быть добавлены или удалены при нанесении, обновлении или удалении метки.</span><span class="sxs-lookup"><span data-stu-id="eeff6-107">This **contentInfo** detail drives the results on what metadata, content marking, and protection should be added or removed when the label is applied, updated, or removed.</span></span> 

## <a name="properties"></a><span data-ttu-id="eeff6-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="eeff6-108">Properties</span></span>

| <span data-ttu-id="eeff6-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="eeff6-109">Property</span></span>   | <span data-ttu-id="eeff6-110">Тип</span><span class="sxs-lookup"><span data-stu-id="eeff6-110">Type</span></span>                                       | <span data-ttu-id="eeff6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="eeff6-111">Description</span></span>                                                                                                                     |
| :--------- | :----------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="eeff6-112">format</span><span class="sxs-lookup"><span data-stu-id="eeff6-112">format</span></span>     | <span data-ttu-id="eeff6-113">String</span><span class="sxs-lookup"><span data-stu-id="eeff6-113">String</span></span>                                     | <span data-ttu-id="eeff6-114">Возможные значения: `default`, `email`.</span><span class="sxs-lookup"><span data-stu-id="eeff6-114">Possible values are: `default`, `email`.</span></span>                                                                                        |
| <span data-ttu-id="eeff6-115">идентификатор</span><span class="sxs-lookup"><span data-stu-id="eeff6-115">identifier</span></span> | <span data-ttu-id="eeff6-116">Строка</span><span class="sxs-lookup"><span data-stu-id="eeff6-116">String</span></span>                                     | <span data-ttu-id="eeff6-117">Идентификатор, используемый для Azure Information Protection Analytics.</span><span class="sxs-lookup"><span data-stu-id="eeff6-117">Identifier used for Azure Information Protection Analytics.</span></span>                                                                     |
| <span data-ttu-id="eeff6-118">метаданные</span><span class="sxs-lookup"><span data-stu-id="eeff6-118">metadata</span></span>   | <span data-ttu-id="eeff6-119">Коллекция [keyValuePair](keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="eeff6-119">[keyValuePair](keyvaluepair.md) collection</span></span> | <span data-ttu-id="eeff6-120">Существующие метаданные Microsoft Information Protection передаются в виде пар ключей и значений, где ключом является MSIP_Label_GUID_PropName.</span><span class="sxs-lookup"><span data-stu-id="eeff6-120">Existing Microsoft Information Protection metadata is passed as key/value pairs, where the key is the MSIP_Label_GUID_PropName.</span></span> |
| <span data-ttu-id="eeff6-121">state</span><span class="sxs-lookup"><span data-stu-id="eeff6-121">state</span></span>      | <span data-ttu-id="eeff6-122">String</span><span class="sxs-lookup"><span data-stu-id="eeff6-122">String</span></span>                                     | <span data-ttu-id="eeff6-123">Возможные значения: `rest`, `motion`, `use`.</span><span class="sxs-lookup"><span data-stu-id="eeff6-123">Possible values are: `rest`, `motion`, `use`.</span></span>                                                                                   |

## <a name="json-representation"></a><span data-ttu-id="eeff6-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eeff6-124">JSON representation</span></span>

<span data-ttu-id="eeff6-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eeff6-125">The following is a JSON representation of the resource.</span></span>

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

