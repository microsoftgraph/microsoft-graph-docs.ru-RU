---
title: Тип ресурса Кондитионалакцессдевицес
description: Представляет устройства в области политики.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b10bef4904d443ca975f5f98834b3b2d1c72a7e7
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2020
ms.locfileid: "43916818"
---
# <a name="conditionalaccessdevices-resource-type"></a><span data-ttu-id="4cc99-103">Тип ресурса Кондитионалакцессдевицес</span><span class="sxs-lookup"><span data-stu-id="4cc99-103">conditionalAccessDevices resource type</span></span>

<span data-ttu-id="4cc99-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4cc99-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4cc99-105">Представляет устройства в области политики.</span><span class="sxs-lookup"><span data-stu-id="4cc99-105">Represents devices in the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="4cc99-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="4cc99-106">Properties</span></span>

| <span data-ttu-id="4cc99-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="4cc99-107">Property</span></span>     | <span data-ttu-id="4cc99-108">Тип</span><span class="sxs-lookup"><span data-stu-id="4cc99-108">Type</span></span>        | <span data-ttu-id="4cc99-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4cc99-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="4cc99-110">инклудедевицестатес</span><span class="sxs-lookup"><span data-stu-id="4cc99-110">includeDeviceStates</span></span> | <span data-ttu-id="4cc99-111">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="4cc99-111">String collection</span></span> | <span data-ttu-id="4cc99-112">Состояния политики.</span><span class="sxs-lookup"><span data-stu-id="4cc99-112">States in the scope of the policy.</span></span> <span data-ttu-id="4cc99-113">`All`— Единственное допустимое значение.</span><span class="sxs-lookup"><span data-stu-id="4cc99-113">`All` is the only allowed value.</span></span> |
| <span data-ttu-id="4cc99-114">ексклудедевицестатес</span><span class="sxs-lookup"><span data-stu-id="4cc99-114">excludeDeviceStates</span></span> | <span data-ttu-id="4cc99-115">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="4cc99-115">String collection</span></span> | <span data-ttu-id="4cc99-116">Состояния, исключенные из области применения политики.</span><span class="sxs-lookup"><span data-stu-id="4cc99-116">States excluded from the scope of the policy.</span></span> <span data-ttu-id="4cc99-117">Возможные значения: `Compliant`, `DomainJoined`.</span><span class="sxs-lookup"><span data-stu-id="4cc99-117">Possible values: `Compliant`, `DomainJoined`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="4cc99-118">Связи</span><span class="sxs-lookup"><span data-stu-id="4cc99-118">Relationships</span></span>

<span data-ttu-id="4cc99-119">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4cc99-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4cc99-120">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4cc99-120">JSON representation</span></span>

<span data-ttu-id="4cc99-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4cc99-121">The following is a JSON representation of the resource.</span></span>

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
