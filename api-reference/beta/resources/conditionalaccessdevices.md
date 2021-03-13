---
title: тип ресурса conditionalAccessDevices
description: Представляет устройства в области политики.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 94115e97c597bc34f03d843b8098f707ed39cd51
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761809"
---
# <a name="conditionalaccessdevices-resource-type"></a><span data-ttu-id="6aa8a-103">тип ресурса conditionalAccessDevices</span><span class="sxs-lookup"><span data-stu-id="6aa8a-103">conditionalAccessDevices resource type</span></span>

<span data-ttu-id="6aa8a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6aa8a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6aa8a-105">Представляет устройства в области политики.</span><span class="sxs-lookup"><span data-stu-id="6aa8a-105">Represents devices in the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="6aa8a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="6aa8a-106">Properties</span></span>

| <span data-ttu-id="6aa8a-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="6aa8a-107">Property</span></span>     | <span data-ttu-id="6aa8a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="6aa8a-108">Type</span></span>        | <span data-ttu-id="6aa8a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6aa8a-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="6aa8a-110">includeDevices</span><span class="sxs-lookup"><span data-stu-id="6aa8a-110">includeDevices</span></span> | <span data-ttu-id="6aa8a-111">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6aa8a-111">String collection</span></span> | <span data-ttu-id="6aa8a-112">Состояния в области политики.</span><span class="sxs-lookup"><span data-stu-id="6aa8a-112">States in the scope of the policy.</span></span> <span data-ttu-id="6aa8a-113">`All` является единственным допустимым значением.</span><span class="sxs-lookup"><span data-stu-id="6aa8a-113">`All` is the only allowed value.</span></span> |
| <span data-ttu-id="6aa8a-114">excludeDevices</span><span class="sxs-lookup"><span data-stu-id="6aa8a-114">excludeDevices</span></span> | <span data-ttu-id="6aa8a-115">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6aa8a-115">String collection</span></span> | <span data-ttu-id="6aa8a-116">Государства, исключенные из сферы действия политики.</span><span class="sxs-lookup"><span data-stu-id="6aa8a-116">States excluded from the scope of the policy.</span></span> <span data-ttu-id="6aa8a-117">Возможные значения: `Compliant` , `DomainJoined` .</span><span class="sxs-lookup"><span data-stu-id="6aa8a-117">Possible values: `Compliant`, `DomainJoined`.</span></span> |
| <span data-ttu-id="6aa8a-118">includeDeviceStates (deprecated)</span><span class="sxs-lookup"><span data-stu-id="6aa8a-118">includeDeviceStates (deprecated)</span></span>| <span data-ttu-id="6aa8a-119">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6aa8a-119">String collection</span></span> | <span data-ttu-id="6aa8a-120">Состояния в области политики.</span><span class="sxs-lookup"><span data-stu-id="6aa8a-120">States in the scope of the policy.</span></span> <span data-ttu-id="6aa8a-121">`All` является единственным допустимым значением.</span><span class="sxs-lookup"><span data-stu-id="6aa8a-121">`All` is the only allowed value.</span></span> |
| <span data-ttu-id="6aa8a-122">excludeDeviceStates (deprecated)</span><span class="sxs-lookup"><span data-stu-id="6aa8a-122">excludeDeviceStates (deprecated)</span></span>| <span data-ttu-id="6aa8a-123">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6aa8a-123">String collection</span></span> | <span data-ttu-id="6aa8a-124">Государства, исключенные из сферы действия политики.</span><span class="sxs-lookup"><span data-stu-id="6aa8a-124">States excluded from the scope of the policy.</span></span> <span data-ttu-id="6aa8a-125">Возможные значения: `Compliant` , `DomainJoined` .</span><span class="sxs-lookup"><span data-stu-id="6aa8a-125">Possible values: `Compliant`, `DomainJoined`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="6aa8a-126">Отношения</span><span class="sxs-lookup"><span data-stu-id="6aa8a-126">Relationships</span></span>

<span data-ttu-id="6aa8a-127">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="6aa8a-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6aa8a-128">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="6aa8a-128">JSON representation</span></span>

<span data-ttu-id="6aa8a-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6aa8a-129">The following is a JSON representation of the resource.</span></span>

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


