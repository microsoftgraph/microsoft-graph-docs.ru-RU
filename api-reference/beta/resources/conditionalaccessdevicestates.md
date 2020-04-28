---
title: Тип ресурса Кондитионалакцессдевицестатес
description: Представляет состояния устройства в области политики.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c23406f63ae94a494e972d4063277c277d655423
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2020
ms.locfileid: "43916804"
---
# <a name="conditionalaccessdevicestates-resource-type"></a><span data-ttu-id="85cb9-103">Тип ресурса Кондитионалакцессдевицестатес</span><span class="sxs-lookup"><span data-stu-id="85cb9-103">conditionalAccessDeviceStates resource type</span></span>

<span data-ttu-id="85cb9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85cb9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85cb9-105">Представляет состояния устройства в области политики.</span><span class="sxs-lookup"><span data-stu-id="85cb9-105">Represents device states in the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="85cb9-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="85cb9-106">Properties</span></span>

| <span data-ttu-id="85cb9-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="85cb9-107">Property</span></span>     | <span data-ttu-id="85cb9-108">Тип</span><span class="sxs-lookup"><span data-stu-id="85cb9-108">Type</span></span>        | <span data-ttu-id="85cb9-109">Описание</span><span class="sxs-lookup"><span data-stu-id="85cb9-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="85cb9-110">инклудестатес</span><span class="sxs-lookup"><span data-stu-id="85cb9-110">includeStates</span></span> | <span data-ttu-id="85cb9-111">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="85cb9-111">String collection</span></span> | <span data-ttu-id="85cb9-112">Состояния политики.</span><span class="sxs-lookup"><span data-stu-id="85cb9-112">States in the scope of the policy.</span></span> <span data-ttu-id="85cb9-113">`All`— Единственное допустимое значение.</span><span class="sxs-lookup"><span data-stu-id="85cb9-113">`All` is the only allowed value.</span></span> |
| <span data-ttu-id="85cb9-114">ексклудестатес</span><span class="sxs-lookup"><span data-stu-id="85cb9-114">excludeStates</span></span> | <span data-ttu-id="85cb9-115">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="85cb9-115">String collection</span></span> | <span data-ttu-id="85cb9-116">Состояния, исключенные из области применения политики.</span><span class="sxs-lookup"><span data-stu-id="85cb9-116">States excluded from the scope of the policy.</span></span> <span data-ttu-id="85cb9-117">Возможные значения: `Compliant`, `DomainJoined`.</span><span class="sxs-lookup"><span data-stu-id="85cb9-117">Possible values: `Compliant`, `DomainJoined`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="85cb9-118">Связи</span><span class="sxs-lookup"><span data-stu-id="85cb9-118">Relationships</span></span>

<span data-ttu-id="85cb9-119">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="85cb9-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="85cb9-120">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="85cb9-120">JSON representation</span></span>

<span data-ttu-id="85cb9-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="85cb9-121">The following is a JSON representation of the resource.</span></span>

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