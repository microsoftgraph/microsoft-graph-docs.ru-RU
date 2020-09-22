---
title: Тип ресурса Фаилуреинфо
description: Тип Фаилуреинфо
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: cd720663e3025525b19ffff62d8ef9b061d154b2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48069472"
---
# <a name="failureinfo-resource-type"></a><span data-ttu-id="a329e-103">Тип ресурса Фаилуреинфо</span><span class="sxs-lookup"><span data-stu-id="a329e-103">failureInfo resource type</span></span>

<span data-ttu-id="a329e-104">Пространство имен: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="a329e-104">Namespace: microsoft.graph.callRecords</span></span>

<span data-ttu-id="a329e-105">Представляет сведения о причине сбоя вызова или части вызова.</span><span class="sxs-lookup"><span data-stu-id="a329e-105">Represents information about why a call or portion of a call failed.</span></span>

## <a name="properties"></a><span data-ttu-id="a329e-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a329e-106">Properties</span></span>

| <span data-ttu-id="a329e-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="a329e-107">Property</span></span>     | <span data-ttu-id="a329e-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a329e-108">Type</span></span>        | <span data-ttu-id="a329e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a329e-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a329e-110">reason</span><span class="sxs-lookup"><span data-stu-id="a329e-110">reason</span></span>|<span data-ttu-id="a329e-111">Строка</span><span class="sxs-lookup"><span data-stu-id="a329e-111">String</span></span>|<span data-ttu-id="a329e-112">Классификация причин сбоя вызова или части вызова.</span><span class="sxs-lookup"><span data-stu-id="a329e-112">Classification of why a call or portion of a call failed.</span></span>|
|<span data-ttu-id="a329e-113">разместить</span><span class="sxs-lookup"><span data-stu-id="a329e-113">stage</span></span>|<span data-ttu-id="a329e-114">Microsoft. Graph. Каллрекордс. Фаилурестаже</span><span class="sxs-lookup"><span data-stu-id="a329e-114">microsoft.graph.callRecords.failureStage</span></span>|<span data-ttu-id="a329e-115">Рабочая область при возникновении ошибки.</span><span class="sxs-lookup"><span data-stu-id="a329e-115">The stage when the failure occurred.</span></span> <span data-ttu-id="a329e-116">Возможные значения: `unknown`, `callSetup`, `midcall`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="a329e-116">Possible values are: `unknown`, `callSetup`, `midcall`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a329e-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a329e-117">JSON representation</span></span>

<span data-ttu-id="a329e-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a329e-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.failureInfo",
  "baseType": null
}-->

```json
{
  "reason": "String",
  "stage": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "failureInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
