---
title: Тип ресурса Кондитионалакцессдевицестатес
description: Представляет состояния устройства в области политики.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 262657c015e4b3416baa9e6e533d1b8f76c1a536
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48040079"
---
# <a name="conditionalaccessdevicestates-resource-type"></a><span data-ttu-id="bb9f8-103">Тип ресурса Кондитионалакцессдевицестатес</span><span class="sxs-lookup"><span data-stu-id="bb9f8-103">conditionalAccessDeviceStates resource type</span></span>

<span data-ttu-id="bb9f8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb9f8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb9f8-105">Представляет состояния устройства в области политики.</span><span class="sxs-lookup"><span data-stu-id="bb9f8-105">Represents device states in the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="bb9f8-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="bb9f8-106">Properties</span></span>

| <span data-ttu-id="bb9f8-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="bb9f8-107">Property</span></span>     | <span data-ttu-id="bb9f8-108">Тип</span><span class="sxs-lookup"><span data-stu-id="bb9f8-108">Type</span></span>        | <span data-ttu-id="bb9f8-109">Описание</span><span class="sxs-lookup"><span data-stu-id="bb9f8-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="bb9f8-110">инклудестатес</span><span class="sxs-lookup"><span data-stu-id="bb9f8-110">includeStates</span></span> | <span data-ttu-id="bb9f8-111">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="bb9f8-111">String collection</span></span> | <span data-ttu-id="bb9f8-112">Состояния политики.</span><span class="sxs-lookup"><span data-stu-id="bb9f8-112">States in the scope of the policy.</span></span> <span data-ttu-id="bb9f8-113">`All` — Единственное допустимое значение.</span><span class="sxs-lookup"><span data-stu-id="bb9f8-113">`All` is the only allowed value.</span></span> |
| <span data-ttu-id="bb9f8-114">ексклудестатес</span><span class="sxs-lookup"><span data-stu-id="bb9f8-114">excludeStates</span></span> | <span data-ttu-id="bb9f8-115">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="bb9f8-115">String collection</span></span> | <span data-ttu-id="bb9f8-116">Состояния, исключенные из области применения политики.</span><span class="sxs-lookup"><span data-stu-id="bb9f8-116">States excluded from the scope of the policy.</span></span> <span data-ttu-id="bb9f8-117">Возможные значения: `Compliant` , `DomainJoined` .</span><span class="sxs-lookup"><span data-stu-id="bb9f8-117">Possible values: `Compliant`, `DomainJoined`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="bb9f8-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="bb9f8-118">Relationships</span></span>

<span data-ttu-id="bb9f8-119">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="bb9f8-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bb9f8-120">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="bb9f8-120">JSON representation</span></span>

<span data-ttu-id="bb9f8-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bb9f8-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "includeStates",
    "excludeStates"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessDeviceStates",
  "baseType": null
}-->

```json
{
  "includeStates": [ "String" ],
  "excludeStates": [ "String" ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessDeviceStates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

