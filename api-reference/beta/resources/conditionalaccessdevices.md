---
title: Тип ресурса Кондитионалакцессдевицес
description: Представляет устройства в области политики.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8ada9dc6b9b9714941f4086d3ca49761fcbeb2ac
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43805671"
---
# <a name="conditionalaccessdevices-resource-type"></a><span data-ttu-id="4c58f-103">Тип ресурса Кондитионалакцессдевицес</span><span class="sxs-lookup"><span data-stu-id="4c58f-103">conditionalAccessDevices resource type</span></span>

<span data-ttu-id="4c58f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c58f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c58f-105">Представляет устройства в области политики.</span><span class="sxs-lookup"><span data-stu-id="4c58f-105">Represents devices in the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="4c58f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="4c58f-106">Properties</span></span>

| <span data-ttu-id="4c58f-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="4c58f-107">Property</span></span>     | <span data-ttu-id="4c58f-108">Тип</span><span class="sxs-lookup"><span data-stu-id="4c58f-108">Type</span></span>        | <span data-ttu-id="4c58f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4c58f-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="4c58f-110">инклудедевицестатес</span><span class="sxs-lookup"><span data-stu-id="4c58f-110">includeDeviceStates</span></span> | <span data-ttu-id="4c58f-111">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="4c58f-111">String collection</span></span> | <span data-ttu-id="4c58f-112">Состояния политики.</span><span class="sxs-lookup"><span data-stu-id="4c58f-112">States in the scope of the policy.</span></span> <span data-ttu-id="4c58f-113">`All`— Единственное допустимое значение.</span><span class="sxs-lookup"><span data-stu-id="4c58f-113">`All` is the only allowed value.</span></span> |
| <span data-ttu-id="4c58f-114">ексклудедевицестатес</span><span class="sxs-lookup"><span data-stu-id="4c58f-114">excludeDeviceStates</span></span> | <span data-ttu-id="4c58f-115">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="4c58f-115">String collection</span></span> | <span data-ttu-id="4c58f-116">Состояния, исключенные из области применения политики.</span><span class="sxs-lookup"><span data-stu-id="4c58f-116">States excluded from the scope of the policy.</span></span> <span data-ttu-id="4c58f-117">Возможные значения: `Compliant`, `DomainJoined`.</span><span class="sxs-lookup"><span data-stu-id="4c58f-117">Possible values: `Compliant`, `DomainJoined`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="4c58f-118">Связи</span><span class="sxs-lookup"><span data-stu-id="4c58f-118">Relationships</span></span>

<span data-ttu-id="4c58f-119">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4c58f-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4c58f-120">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4c58f-120">JSON representation</span></span>

<span data-ttu-id="4c58f-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4c58f-121">The following is a JSON representation of the resource.</span></span>

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
