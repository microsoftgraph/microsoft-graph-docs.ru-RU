---
title: Тип ресурса Инференцедата
description: Тип ресурса Инференцедата
localization_priority: Normal
author: kevinbellinger
ms.prod: profile
doc_type: resourcePageType
ms.openlocfilehash: 412d96d3eb497681e65dacd2f7a0576b4071a9aa
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016501"
---
# <a name="inferencedata-resource-type"></a><span data-ttu-id="dd1dd-103">Тип ресурса Инференцедата</span><span class="sxs-lookup"><span data-stu-id="dd1dd-103">inferenceData resource type</span></span>

<span data-ttu-id="dd1dd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd1dd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd1dd-105">Тип ресурса [инференцедата](inferencedata.md) предоставляет дополнительные сведения об объекте, который был создан с помощью получения сведений о пользователе.</span><span class="sxs-lookup"><span data-stu-id="dd1dd-105">The [inferenceData](inferencedata.md) resource type provides additional detail about an entity which has been created through inferring information about the user.</span></span> <span data-ttu-id="dd1dd-106">Эти сведения будут представлены, когда данные в определенной сущности появлялись на основе машинного обучения или другого процесса обработки данных.</span><span class="sxs-lookup"><span data-stu-id="dd1dd-106">This information will be present whenever the data within a particular entity was derived from a machine learning or other system process iterating over data.</span></span>

## <a name="properties"></a><span data-ttu-id="dd1dd-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="dd1dd-107">Properties</span></span>

| <span data-ttu-id="dd1dd-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="dd1dd-108">Property</span></span>              | <span data-ttu-id="dd1dd-109">Тип</span><span class="sxs-lookup"><span data-stu-id="dd1dd-109">Type</span></span>        | <span data-ttu-id="dd1dd-110">Описание</span><span class="sxs-lookup"><span data-stu-id="dd1dd-110">Description</span></span>                                                                     |
|:----------------------|:------------|:--------------------------------------------------------------------------------|
|<span data-ttu-id="dd1dd-111">конфиденцескоре</span><span class="sxs-lookup"><span data-stu-id="dd1dd-111">confidenceScore</span></span>        |<span data-ttu-id="dd1dd-112">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="dd1dd-112">Double</span></span>       | <span data-ttu-id="dd1dd-113">Показатель достоверности, отражающий точность данных, выведенных о пользователе.</span><span class="sxs-lookup"><span data-stu-id="dd1dd-113">Confidence score reflecting the accuracy of the data inferred about the user.</span></span>   |
|<span data-ttu-id="dd1dd-114">усерхасверифиедаккураци</span><span class="sxs-lookup"><span data-stu-id="dd1dd-114">userHasVerifiedAccuracy</span></span>|<span data-ttu-id="dd1dd-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd1dd-115">Boolean</span></span>      | <span data-ttu-id="dd1dd-116">Записывается, если пользователь подтвердил получение значения true или false.</span><span class="sxs-lookup"><span data-stu-id="dd1dd-116">Records if the user has confirmed this inference as being True or False.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="dd1dd-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dd1dd-117">JSON representation</span></span>

<span data-ttu-id="dd1dd-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dd1dd-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.inferenceData",
  "baseType": null
}-->

```json
{
  "confidenceScore": 1024,
  "userHasVerifiedAccuracy": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "inferenceData resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

