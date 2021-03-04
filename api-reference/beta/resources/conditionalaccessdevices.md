---
title: тип ресурса conditionalAccessDevices
description: Представляет устройства в области политики.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a42e6023ace493c5efb230ffd53eb9c4caee7d16
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440530"
---
# <a name="conditionalaccessdevices-resource-type"></a><span data-ttu-id="27a9f-103">тип ресурса conditionalAccessDevices</span><span class="sxs-lookup"><span data-stu-id="27a9f-103">conditionalAccessDevices resource type</span></span>

<span data-ttu-id="27a9f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27a9f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27a9f-105">Представляет устройства в области политики.</span><span class="sxs-lookup"><span data-stu-id="27a9f-105">Represents devices in the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="27a9f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="27a9f-106">Properties</span></span>

| <span data-ttu-id="27a9f-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="27a9f-107">Property</span></span>     | <span data-ttu-id="27a9f-108">Тип</span><span class="sxs-lookup"><span data-stu-id="27a9f-108">Type</span></span>        | <span data-ttu-id="27a9f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="27a9f-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="27a9f-110">includeDevices</span><span class="sxs-lookup"><span data-stu-id="27a9f-110">includeDevices</span></span> | <span data-ttu-id="27a9f-111">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="27a9f-111">String collection</span></span> | <span data-ttu-id="27a9f-112">Состояния в области политики.</span><span class="sxs-lookup"><span data-stu-id="27a9f-112">States in the scope of the policy.</span></span> <span data-ttu-id="27a9f-113">`All` является единственным допустимым значением.</span><span class="sxs-lookup"><span data-stu-id="27a9f-113">`All` is the only allowed value.</span></span> |
| <span data-ttu-id="27a9f-114">excludeDevices</span><span class="sxs-lookup"><span data-stu-id="27a9f-114">excludeDevices</span></span> | <span data-ttu-id="27a9f-115">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="27a9f-115">String collection</span></span> | <span data-ttu-id="27a9f-116">Государства, исключенные из сферы действия политики.</span><span class="sxs-lookup"><span data-stu-id="27a9f-116">States excluded from the scope of the policy.</span></span> <span data-ttu-id="27a9f-117">Возможные значения: `Compliant` , `DomainJoined` .</span><span class="sxs-lookup"><span data-stu-id="27a9f-117">Possible values: `Compliant`, `DomainJoined`.</span></span> |
| <span data-ttu-id="27a9f-118">includeDeviceStates (deprecated)</span><span class="sxs-lookup"><span data-stu-id="27a9f-118">includeDeviceStates (deprecated)</span></span>| <span data-ttu-id="27a9f-119">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="27a9f-119">String collection</span></span> | <span data-ttu-id="27a9f-120">Состояния в области политики.</span><span class="sxs-lookup"><span data-stu-id="27a9f-120">States in the scope of the policy.</span></span> <span data-ttu-id="27a9f-121">`All` является единственным допустимым значением.</span><span class="sxs-lookup"><span data-stu-id="27a9f-121">`All` is the only allowed value.</span></span> |
| <span data-ttu-id="27a9f-122">excludeDeviceStates (deprecated)</span><span class="sxs-lookup"><span data-stu-id="27a9f-122">excludeDeviceStates (deprecated)</span></span>| <span data-ttu-id="27a9f-123">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="27a9f-123">String collection</span></span> | <span data-ttu-id="27a9f-124">Государства, исключенные из сферы действия политики.</span><span class="sxs-lookup"><span data-stu-id="27a9f-124">States excluded from the scope of the policy.</span></span> <span data-ttu-id="27a9f-125">Возможные значения: `Compliant` , `DomainJoined` .</span><span class="sxs-lookup"><span data-stu-id="27a9f-125">Possible values: `Compliant`, `DomainJoined`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="27a9f-126">Связи</span><span class="sxs-lookup"><span data-stu-id="27a9f-126">Relationships</span></span>

<span data-ttu-id="27a9f-127">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="27a9f-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="27a9f-128">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="27a9f-128">JSON representation</span></span>

<span data-ttu-id="27a9f-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="27a9f-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "includeDevices",
    "excludeDevices"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessDevices",
  "baseType": null
}-->

```json
{
  "includeDevices": [ "String" ],
  "excludeDevices": [ "String" ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessDevices resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


