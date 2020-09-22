---
title: Тип ресурса Фаилуреинфо
description: Тип Фаилуреинфо
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 5edd2a501b3e1a5633f0bd01ac36815201eb927d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48064376"
---
# <a name="failureinfo-resource-type"></a><span data-ttu-id="a4f3c-103">Тип ресурса Фаилуреинфо</span><span class="sxs-lookup"><span data-stu-id="a4f3c-103">failureInfo resource type</span></span>

<span data-ttu-id="a4f3c-104">Пространство имен: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="a4f3c-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4f3c-105">Представляет сведения о причине сбоя вызова или части вызова.</span><span class="sxs-lookup"><span data-stu-id="a4f3c-105">Represents information about why a call or portion of a call failed.</span></span>

<span data-ttu-id="a4f3c-106">Ошибка может относиться к двум типам:</span><span class="sxs-lookup"><span data-stu-id="a4f3c-106">The failure can be of two types:</span></span> 

- <span data-ttu-id="a4f3c-107">Сбой при установке вызовов</span><span class="sxs-lookup"><span data-stu-id="a4f3c-107">Call setup failure</span></span>
- <span data-ttu-id="a4f3c-108">Метод MID — Drop</span><span class="sxs-lookup"><span data-stu-id="a4f3c-108">Mid-call drop</span></span>

<span data-ttu-id="a4f3c-109">Если один или несколько потоков мультимедиа имеют какие-либо из этих ошибок, то этот сбой распространяется на уровне сегмента.</span><span class="sxs-lookup"><span data-stu-id="a4f3c-109">If one or more media streams have any of these failures, that failure is propagated at the segment level.</span></span> <span data-ttu-id="a4f3c-110">Если один или несколько сегментов имеют какие-либо из этих ошибок, то этот сбой распространяется на уровне сеанса.</span><span class="sxs-lookup"><span data-stu-id="a4f3c-110">If one or more segments have any of these failures, that failure is propagated at the session level.</span></span>

## <a name="properties"></a><span data-ttu-id="a4f3c-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="a4f3c-111">Properties</span></span>

| <span data-ttu-id="a4f3c-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="a4f3c-112">Property</span></span>     | <span data-ttu-id="a4f3c-113">Тип</span><span class="sxs-lookup"><span data-stu-id="a4f3c-113">Type</span></span>        | <span data-ttu-id="a4f3c-114">Описание</span><span class="sxs-lookup"><span data-stu-id="a4f3c-114">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a4f3c-115">reason</span><span class="sxs-lookup"><span data-stu-id="a4f3c-115">reason</span></span>|<span data-ttu-id="a4f3c-116">String</span><span class="sxs-lookup"><span data-stu-id="a4f3c-116">String</span></span>|<span data-ttu-id="a4f3c-117">Классификация причин сбоя вызова или части вызова.</span><span class="sxs-lookup"><span data-stu-id="a4f3c-117">Classification of why a call or portion of a call failed.</span></span>|
|<span data-ttu-id="a4f3c-118">разместить</span><span class="sxs-lookup"><span data-stu-id="a4f3c-118">stage</span></span>|<span data-ttu-id="a4f3c-119">Microsoft. Graph. Каллрекордс. Фаилурестаже</span><span class="sxs-lookup"><span data-stu-id="a4f3c-119">microsoft.graph.callRecords.failureStage</span></span>|<span data-ttu-id="a4f3c-120">Рабочая область при возникновении ошибки.</span><span class="sxs-lookup"><span data-stu-id="a4f3c-120">The stage when the failure occurred.</span></span> <span data-ttu-id="a4f3c-121">Возможные значения: `unknown`, `callSetup`, `midcall`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="a4f3c-121">Possible values are: `unknown`, `callSetup`, `midcall`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a4f3c-122">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a4f3c-122">JSON representation</span></span>

<span data-ttu-id="a4f3c-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a4f3c-123">The following is a JSON representation of the resource.</span></span>

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


