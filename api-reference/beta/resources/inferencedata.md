---
title: Тип ресурса Инференцедата
description: Тип ресурса Инференцедата
localization_priority: Normal
author: kevinbellinger
ms.prod: profile
doc_type: resourcePageType
ms.openlocfilehash: 2097dc14de984f3d1517b4d17e8043f38411b89a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42496175"
---
# <a name="inferencedata-resource-type"></a><span data-ttu-id="1a193-103">Тип ресурса Инференцедата</span><span class="sxs-lookup"><span data-stu-id="1a193-103">inferenceData resource type</span></span>

<span data-ttu-id="1a193-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a193-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a193-105">Тип ресурса [инференцедата](inferencedata.md) предоставляет дополнительные сведения об объекте, который был создан с помощью получения сведений о пользователе.</span><span class="sxs-lookup"><span data-stu-id="1a193-105">The [inferenceData](inferencedata.md) resource type provides additional detail about an entity which has been created through inferring information about the user.</span></span> <span data-ttu-id="1a193-106">Эти сведения будут представлены, когда данные в определенной сущности появлялись на основе машинного обучения или другого процесса обработки данных.</span><span class="sxs-lookup"><span data-stu-id="1a193-106">This information will be present whenever the data within a particular entity was derived from a machine learning or other system process iterating over data.</span></span>

## <a name="properties"></a><span data-ttu-id="1a193-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1a193-107">Properties</span></span>

| <span data-ttu-id="1a193-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="1a193-108">Property</span></span>              | <span data-ttu-id="1a193-109">Тип</span><span class="sxs-lookup"><span data-stu-id="1a193-109">Type</span></span>        | <span data-ttu-id="1a193-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1a193-110">Description</span></span>                                                                     |
|:----------------------|:------------|:--------------------------------------------------------------------------------|
|<span data-ttu-id="1a193-111">конфиденцескоре</span><span class="sxs-lookup"><span data-stu-id="1a193-111">confidenceScore</span></span>        |<span data-ttu-id="1a193-112">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="1a193-112">Double</span></span>       | <span data-ttu-id="1a193-113">Показатель достоверности, отражающий точность данных, выведенных о пользователе.</span><span class="sxs-lookup"><span data-stu-id="1a193-113">Confidence score reflecting the accuracy of the data inferred about the user.</span></span>   |
|<span data-ttu-id="1a193-114">усерхасверифиедаккураци</span><span class="sxs-lookup"><span data-stu-id="1a193-114">userHasVerifiedAccuracy</span></span>|<span data-ttu-id="1a193-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a193-115">Boolean</span></span>      | <span data-ttu-id="1a193-116">Записывается, если пользователь подтвердил получение значения true или false.</span><span class="sxs-lookup"><span data-stu-id="1a193-116">Records if the user has confirmed this inference as being True or False.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="1a193-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1a193-117">JSON representation</span></span>

<span data-ttu-id="1a193-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1a193-118">The following is a JSON representation of the resource.</span></span>

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