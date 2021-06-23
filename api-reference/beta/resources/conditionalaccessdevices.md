---
title: тип ресурса conditionalAccessDevices
description: Представляет устройства в области политики.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: cbb542420228a4a383dea4e165323fbb6e8abb17
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082358"
---
# <a name="conditionalaccessdevices-resource-type"></a><span data-ttu-id="5b7c7-103">тип ресурса conditionalAccessDevices</span><span class="sxs-lookup"><span data-stu-id="5b7c7-103">conditionalAccessDevices resource type</span></span>

<span data-ttu-id="5b7c7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b7c7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b7c7-105">Представляет устройства в области политики.</span><span class="sxs-lookup"><span data-stu-id="5b7c7-105">Represents devices in the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="5b7c7-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="5b7c7-106">Properties</span></span>

| <span data-ttu-id="5b7c7-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="5b7c7-107">Property</span></span>     | <span data-ttu-id="5b7c7-108">Тип</span><span class="sxs-lookup"><span data-stu-id="5b7c7-108">Type</span></span>        | <span data-ttu-id="5b7c7-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5b7c7-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="5b7c7-110">includeDevices</span><span class="sxs-lookup"><span data-stu-id="5b7c7-110">includeDevices</span></span> | <span data-ttu-id="5b7c7-111">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="5b7c7-111">String collection</span></span> | <span data-ttu-id="5b7c7-112">Состояния в области политики.</span><span class="sxs-lookup"><span data-stu-id="5b7c7-112">States in the scope of the policy.</span></span> <span data-ttu-id="5b7c7-113">`All` является единственным допустимым значением.</span><span class="sxs-lookup"><span data-stu-id="5b7c7-113">`All` is the only allowed value.</span></span> <span data-ttu-id="5b7c7-114">Невозможно установить, если *установлено устройствоFIlter.*</span><span class="sxs-lookup"><span data-stu-id="5b7c7-114">Cannot be set if *deviceFIlter* is set.</span></span> |
| <span data-ttu-id="5b7c7-115">excludeDevices</span><span class="sxs-lookup"><span data-stu-id="5b7c7-115">excludeDevices</span></span> | <span data-ttu-id="5b7c7-116">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="5b7c7-116">String collection</span></span> | <span data-ttu-id="5b7c7-117">Государства, исключенные из сферы действия политики.</span><span class="sxs-lookup"><span data-stu-id="5b7c7-117">States excluded from the scope of the policy.</span></span> <span data-ttu-id="5b7c7-118">Возможные значения: `Compliant` , `DomainJoined` .</span><span class="sxs-lookup"><span data-stu-id="5b7c7-118">Possible values: `Compliant`, `DomainJoined`.</span></span> <span data-ttu-id="5b7c7-119">Невозможно установить, если **установлено устройствоFIlter.**</span><span class="sxs-lookup"><span data-stu-id="5b7c7-119">Cannot be set if **deviceFIlter** is set.</span></span> |
| <span data-ttu-id="5b7c7-120">deviceFilter</span><span class="sxs-lookup"><span data-stu-id="5b7c7-120">deviceFilter</span></span> | [<span data-ttu-id="5b7c7-121">conditionalAccessFilter</span><span class="sxs-lookup"><span data-stu-id="5b7c7-121">conditionalAccessFilter</span></span>](conditionalaccessfilter.md) | <span data-ttu-id="5b7c7-122">Фильтр, определяющий правило динамического устройства и синтаксиса, чтобы включить или исключить устройства.</span><span class="sxs-lookup"><span data-stu-id="5b7c7-122">Filter defining the dynamic-device-syntax rule to include/exclude devices.</span></span> <span data-ttu-id="5b7c7-123">Фильтр может использовать свойства устройств (например, атрибуты расширения), чтобы включить или исключить их.</span><span class="sxs-lookup"><span data-stu-id="5b7c7-123">A filter can use device properties (such as extension attributes) to include/exclude them.</span></span> <span data-ttu-id="5b7c7-124">Невозможно установить, **если задают includeDevices** или **excludeDevices.**</span><span class="sxs-lookup"><span data-stu-id="5b7c7-124">Cannot be set if **includeDevices** or **excludeDevices** is set.</span></span> |
| <span data-ttu-id="5b7c7-125">includeDeviceStates (deprecated)</span><span class="sxs-lookup"><span data-stu-id="5b7c7-125">includeDeviceStates (deprecated)</span></span>| <span data-ttu-id="5b7c7-126">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="5b7c7-126">String collection</span></span> | <span data-ttu-id="5b7c7-127">Состояния в области политики.</span><span class="sxs-lookup"><span data-stu-id="5b7c7-127">States in the scope of the policy.</span></span> <span data-ttu-id="5b7c7-128">`All` является единственным допустимым значением.</span><span class="sxs-lookup"><span data-stu-id="5b7c7-128">`All` is the only allowed value.</span></span> |
| <span data-ttu-id="5b7c7-129">excludeDeviceStates (deprecated)</span><span class="sxs-lookup"><span data-stu-id="5b7c7-129">excludeDeviceStates (deprecated)</span></span>| <span data-ttu-id="5b7c7-130">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="5b7c7-130">String collection</span></span> | <span data-ttu-id="5b7c7-131">Государства, исключенные из сферы действия политики.</span><span class="sxs-lookup"><span data-stu-id="5b7c7-131">States excluded from the scope of the policy.</span></span> <span data-ttu-id="5b7c7-132">Возможные значения: `Compliant` , `DomainJoined` .</span><span class="sxs-lookup"><span data-stu-id="5b7c7-132">Possible values: `Compliant`, `DomainJoined`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="5b7c7-133">Связи</span><span class="sxs-lookup"><span data-stu-id="5b7c7-133">Relationships</span></span>

<span data-ttu-id="5b7c7-134">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="5b7c7-134">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5b7c7-135">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="5b7c7-135">JSON representation</span></span>

<span data-ttu-id="5b7c7-136">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5b7c7-136">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "includeDevices",
    "excludeDevices",
    "deviceFilter"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessDevices",
  "baseType": null
}-->

```json
{
  "includeDevices": [ "String" ],
  "excludeDevices": [ "String" ],
  "deviceFilter": {"@odata.type": "microsoft.graph.conditionalAccessFilter"}
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


