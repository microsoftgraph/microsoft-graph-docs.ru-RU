---
title: тип ресурса classificationResult
description: Представляет результат запроса классификации.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 5ecc16197ef4671c6e83883bc69aed45b3ffa200
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941825"
---
# <a name="classificationresult-resource-type"></a><span data-ttu-id="16134-103">тип ресурса classificationResult</span><span class="sxs-lookup"><span data-stu-id="16134-103">classificationResult resource type</span></span>

<span data-ttu-id="16134-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16134-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16134-105">Представляет результат операции классификации из системы классификации Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="16134-105">Represents the result of a classification operation from the Microsoft Classification Engine.</span></span> <span data-ttu-id="16134-106">Классификация данных из служб Azure Information Protection, Office и других служб Майкрософт может возвращать четко определенный набор [типов классификации.](/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="16134-106">Data classification results from Azure Information Protection, Office, and other Microsoft services may return a [well-defined set of classification types](/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span> <span data-ttu-id="16134-107">Эти типы могут быть предоставлены API [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) для разрешения конфиденциальной информации на метку Microsoft Information Protection.</span><span class="sxs-lookup"><span data-stu-id="16134-107">These types can be provided to the [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) API to resolve a sensitive information to a Microsoft Information Protection label.</span></span> 

## <a name="properties"></a><span data-ttu-id="16134-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="16134-108">Properties</span></span>

| <span data-ttu-id="16134-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="16134-109">Property</span></span>        | <span data-ttu-id="16134-110">Тип</span><span class="sxs-lookup"><span data-stu-id="16134-110">Type</span></span>  | <span data-ttu-id="16134-111">Описание</span><span class="sxs-lookup"><span data-stu-id="16134-111">Description</span></span>                                                            |
| :-------------- | :---- | :--------------------------------------------------------------------- |
| <span data-ttu-id="16134-112">confidenceLevel</span><span class="sxs-lookup"><span data-stu-id="16134-112">confidenceLevel</span></span> | <span data-ttu-id="16134-113">Int32</span><span class="sxs-lookup"><span data-stu-id="16134-113">Int32</span></span> | <span data-ttu-id="16134-114">Уровень доверия от 0 до 100 результатов.</span><span class="sxs-lookup"><span data-stu-id="16134-114">The confidence level, 0 to 100, of the result.</span></span>                         |
| <span data-ttu-id="16134-115">count</span><span class="sxs-lookup"><span data-stu-id="16134-115">count</span></span>           | <span data-ttu-id="16134-116">Int32</span><span class="sxs-lookup"><span data-stu-id="16134-116">Int32</span></span> | <span data-ttu-id="16134-117">Количество экземпляров определенного типа сведений в вводе.</span><span class="sxs-lookup"><span data-stu-id="16134-117">The number of instances of the specific information type in the input.</span></span> |
| <span data-ttu-id="16134-118">sensitiveTypeId</span><span class="sxs-lookup"><span data-stu-id="16134-118">sensitiveTypeId</span></span> | <span data-ttu-id="16134-119">GUID</span><span class="sxs-lookup"><span data-stu-id="16134-119">GUID</span></span>  | <span data-ttu-id="16134-120">GUID обнаруженного типа конфиденциальной информации.</span><span class="sxs-lookup"><span data-stu-id="16134-120">The GUID of the discovered sensitive information type.</span></span>                 |

## <a name="json-representation"></a><span data-ttu-id="16134-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="16134-121">JSON representation</span></span>

<span data-ttu-id="16134-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="16134-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.classificationResult",
  "baseType": null
}-->

```json
{
  "confidenceLevel": 1024,
  "count": 1024,
  "sensitiveTypeId": "Guid"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "classificationResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->