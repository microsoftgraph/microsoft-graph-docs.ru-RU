---
title: Тип ресурса Классификатионресулт
description: Представляет результат запроса классификации.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 719ce6fa70172a3ab323aec8c991147ef212bcb7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016830"
---
# <a name="classificationresult-resource-type"></a><span data-ttu-id="92067-103">Тип ресурса Классификатионресулт</span><span class="sxs-lookup"><span data-stu-id="92067-103">classificationResult resource type</span></span>

<span data-ttu-id="92067-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92067-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92067-105">Представляет результат операции классификации из модуля классификации Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="92067-105">Represents the result of a classification operation from the Microsoft Classification Engine.</span></span> <span data-ttu-id="92067-106">Результаты классификации данных в Azure Information Protection, Office и других службах Майкрософт могут возвращать [строго определенный набор типов классификации](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="92067-106">Data classification results from Azure Information Protection, Office, and other Microsoft services may return a [well-defined set of classification types](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span> <span data-ttu-id="92067-107">Эти типы можно предоставлять в API [евалуатеклассификатионресултс](../api/informationprotectionlabel-evaluateclassificationresults.md) для разрешения конфиденциальной информации в метку Microsoft Information Protection.</span><span class="sxs-lookup"><span data-stu-id="92067-107">These types can be provided to the [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) API to resolve a sensitive information to a Microsoft Information Protection label.</span></span> 

## <a name="properties"></a><span data-ttu-id="92067-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="92067-108">Properties</span></span>

| <span data-ttu-id="92067-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="92067-109">Property</span></span>        | <span data-ttu-id="92067-110">Тип</span><span class="sxs-lookup"><span data-stu-id="92067-110">Type</span></span>  | <span data-ttu-id="92067-111">Описание</span><span class="sxs-lookup"><span data-stu-id="92067-111">Description</span></span>                                                            |
| :-------------- | :---- | :--------------------------------------------------------------------- |
| <span data-ttu-id="92067-112">confidenceLevel</span><span class="sxs-lookup"><span data-stu-id="92067-112">confidenceLevel</span></span> | <span data-ttu-id="92067-113">Int32</span><span class="sxs-lookup"><span data-stu-id="92067-113">Int32</span></span> | <span data-ttu-id="92067-114">Степень вероятности результата — от 0 до 100.</span><span class="sxs-lookup"><span data-stu-id="92067-114">The confidence level, 0 to 100, of the result.</span></span>                         |
| <span data-ttu-id="92067-115">count</span><span class="sxs-lookup"><span data-stu-id="92067-115">count</span></span>           | <span data-ttu-id="92067-116">Int32</span><span class="sxs-lookup"><span data-stu-id="92067-116">Int32</span></span> | <span data-ttu-id="92067-117">Число экземпляров определенного типа данных во входных данных.</span><span class="sxs-lookup"><span data-stu-id="92067-117">The number of instances of the specific information type in the input.</span></span> |
| <span data-ttu-id="92067-118">сенситиветипеид</span><span class="sxs-lookup"><span data-stu-id="92067-118">sensitiveTypeId</span></span> | <span data-ttu-id="92067-119">GUID</span><span class="sxs-lookup"><span data-stu-id="92067-119">GUID</span></span>  | <span data-ttu-id="92067-120">GUID обнаруженного типа конфиденциальной информации.</span><span class="sxs-lookup"><span data-stu-id="92067-120">The GUID of the discovered sensitive information type.</span></span>                 |

## <a name="json-representation"></a><span data-ttu-id="92067-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="92067-121">JSON representation</span></span>

<span data-ttu-id="92067-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="92067-122">The following is a JSON representation of the resource.</span></span>

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


