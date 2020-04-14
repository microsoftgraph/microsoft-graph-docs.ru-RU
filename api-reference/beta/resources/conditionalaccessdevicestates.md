---
title: Тип ресурса Кондитионалакцессдевицестатес
description: Представляет состояния устройства в области политики.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 03981fc5be0388e8146c163ab4500eae87d65704
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43413504"
---
# <a name="conditionalaccessdevicestates-resource-type"></a><span data-ttu-id="55cba-103">Тип ресурса Кондитионалакцессдевицестатес</span><span class="sxs-lookup"><span data-stu-id="55cba-103">conditionalAccessDeviceStates resource type</span></span>

<span data-ttu-id="55cba-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55cba-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55cba-105">Представляет состояния устройства в области политики.</span><span class="sxs-lookup"><span data-stu-id="55cba-105">Represents device states in the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="55cba-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="55cba-106">Properties</span></span>

| <span data-ttu-id="55cba-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="55cba-107">Property</span></span>     | <span data-ttu-id="55cba-108">Тип</span><span class="sxs-lookup"><span data-stu-id="55cba-108">Type</span></span>        | <span data-ttu-id="55cba-109">Описание</span><span class="sxs-lookup"><span data-stu-id="55cba-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="55cba-110">инклудестатес</span><span class="sxs-lookup"><span data-stu-id="55cba-110">includeStates</span></span> | <span data-ttu-id="55cba-111">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="55cba-111">String collection</span></span> | <span data-ttu-id="55cba-112">Состояния политики.</span><span class="sxs-lookup"><span data-stu-id="55cba-112">States in the scope of the policy.</span></span> <span data-ttu-id="55cba-113">`All`— Единственное допустимое значение.</span><span class="sxs-lookup"><span data-stu-id="55cba-113">`All` is the only allowed value.</span></span> |
| <span data-ttu-id="55cba-114">ексклудестатес</span><span class="sxs-lookup"><span data-stu-id="55cba-114">excludeStates</span></span> | <span data-ttu-id="55cba-115">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="55cba-115">String collection</span></span> | <span data-ttu-id="55cba-116">Состояния, исключенные из области применения политики.</span><span class="sxs-lookup"><span data-stu-id="55cba-116">States excluded from the scope of the policy.</span></span> <span data-ttu-id="55cba-117">Возможные значения: `Compliant`, `DomainJoined`.</span><span class="sxs-lookup"><span data-stu-id="55cba-117">Possible values: `Compliant`, `DomainJoined`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="55cba-118">Связи</span><span class="sxs-lookup"><span data-stu-id="55cba-118">Relationships</span></span>

<span data-ttu-id="55cba-119">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="55cba-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="55cba-120">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="55cba-120">JSON representation</span></span>

<span data-ttu-id="55cba-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="55cba-121">The following is a JSON representation of the resource.</span></span>

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