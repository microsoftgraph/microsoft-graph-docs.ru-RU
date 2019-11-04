---
title: Тип ресурса Инференцедата
description: Тип ресурса Инференцедата
localization_priority: Normal
author: kevinbellinger
ms.prod: profile
doc_type: resourcePageType
ms.openlocfilehash: 43d6585243eed560a6a8f77268305b7d7f5824a8
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938851"
---
# <a name="inferencedata-resource-type"></a><span data-ttu-id="8c9f2-103">Тип ресурса Инференцедата</span><span class="sxs-lookup"><span data-stu-id="8c9f2-103">inferenceData resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c9f2-104">Тип ресурса [инференцедата](inferencedata.md) предоставляет дополнительные сведения об объекте, который был создан с помощью получения сведений о пользователе.</span><span class="sxs-lookup"><span data-stu-id="8c9f2-104">The [inferenceData](inferencedata.md) resource type provides additional detail about an entity which has been created through inferring information about the user.</span></span> <span data-ttu-id="8c9f2-105">Эти сведения будут представлены, когда данные в определенной сущности появлялись на основе машинного обучения или другого процесса обработки данных.</span><span class="sxs-lookup"><span data-stu-id="8c9f2-105">This information will be present whenever the data within a particular entity was derived from a machine learning or other system process iterating over data.</span></span>

## <a name="properties"></a><span data-ttu-id="8c9f2-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="8c9f2-106">Properties</span></span>

| <span data-ttu-id="8c9f2-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="8c9f2-107">Property</span></span>              | <span data-ttu-id="8c9f2-108">Тип</span><span class="sxs-lookup"><span data-stu-id="8c9f2-108">Type</span></span>        | <span data-ttu-id="8c9f2-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8c9f2-109">Description</span></span>                                                                     |
|:----------------------|:------------|:--------------------------------------------------------------------------------|
|<span data-ttu-id="8c9f2-110">конфиденцескоре</span><span class="sxs-lookup"><span data-stu-id="8c9f2-110">confidenceScore</span></span>        |<span data-ttu-id="8c9f2-111">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="8c9f2-111">Double</span></span>       | <span data-ttu-id="8c9f2-112">Показатель достоверности, отражающий точность данных, выведенных о пользователе.</span><span class="sxs-lookup"><span data-stu-id="8c9f2-112">Confidence score reflecting the accuracy of the data inferred about the user.</span></span>   |
|<span data-ttu-id="8c9f2-113">усерхасверифиедаккураци</span><span class="sxs-lookup"><span data-stu-id="8c9f2-113">userHasVerifiedAccuracy</span></span>|<span data-ttu-id="8c9f2-114">Логический</span><span class="sxs-lookup"><span data-stu-id="8c9f2-114">Boolean</span></span>      | <span data-ttu-id="8c9f2-115">Записывается, если пользователь подтвердил получение значения true или false.</span><span class="sxs-lookup"><span data-stu-id="8c9f2-115">Records if the user has confirmed this inference as being True or False.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="8c9f2-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8c9f2-116">JSON representation</span></span>

<span data-ttu-id="8c9f2-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8c9f2-117">The following is a JSON representation of the resource.</span></span>

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