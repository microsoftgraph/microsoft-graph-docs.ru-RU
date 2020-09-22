---
title: Тип ресурса Кондитионалакцессдевицес
description: Представляет устройства в области политики.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f0610fb376b265a261b8a88ab4181dd89bb9f6c1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48040077"
---
# <a name="conditionalaccessdevices-resource-type"></a><span data-ttu-id="df941-103">Тип ресурса Кондитионалакцессдевицес</span><span class="sxs-lookup"><span data-stu-id="df941-103">conditionalAccessDevices resource type</span></span>

<span data-ttu-id="df941-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df941-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df941-105">Представляет устройства в области политики.</span><span class="sxs-lookup"><span data-stu-id="df941-105">Represents devices in the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="df941-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="df941-106">Properties</span></span>

| <span data-ttu-id="df941-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="df941-107">Property</span></span>     | <span data-ttu-id="df941-108">Тип</span><span class="sxs-lookup"><span data-stu-id="df941-108">Type</span></span>        | <span data-ttu-id="df941-109">Описание</span><span class="sxs-lookup"><span data-stu-id="df941-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="df941-110">инклудедевицестатес</span><span class="sxs-lookup"><span data-stu-id="df941-110">includeDeviceStates</span></span> | <span data-ttu-id="df941-111">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="df941-111">String collection</span></span> | <span data-ttu-id="df941-112">Состояния политики.</span><span class="sxs-lookup"><span data-stu-id="df941-112">States in the scope of the policy.</span></span> <span data-ttu-id="df941-113">`All` — Единственное допустимое значение.</span><span class="sxs-lookup"><span data-stu-id="df941-113">`All` is the only allowed value.</span></span> |
| <span data-ttu-id="df941-114">ексклудедевицестатес</span><span class="sxs-lookup"><span data-stu-id="df941-114">excludeDeviceStates</span></span> | <span data-ttu-id="df941-115">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="df941-115">String collection</span></span> | <span data-ttu-id="df941-116">Состояния, исключенные из области применения политики.</span><span class="sxs-lookup"><span data-stu-id="df941-116">States excluded from the scope of the policy.</span></span> <span data-ttu-id="df941-117">Возможные значения: `Compliant` , `DomainJoined` .</span><span class="sxs-lookup"><span data-stu-id="df941-117">Possible values: `Compliant`, `DomainJoined`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="df941-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="df941-118">Relationships</span></span>

<span data-ttu-id="df941-119">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="df941-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="df941-120">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="df941-120">JSON representation</span></span>

<span data-ttu-id="df941-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="df941-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "includeDeviceStates",
    "excludeDeviceStates"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessDevices",
  "baseType": null
}-->

```json
{
  "includeDeviceStates": [ "String" ],
  "excludeDeviceStates": [ "String" ]
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


