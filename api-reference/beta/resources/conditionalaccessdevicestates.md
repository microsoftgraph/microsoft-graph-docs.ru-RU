---
title: Тип ресурса Кондитионалакцессдевицестатес
description: Представляет состояния устройства в области политики.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 822f819cd8e9ef0f93279c67b94972a1e9fb7929
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638584"
---
# <a name="conditionalaccessdevicestates-resource-type"></a><span data-ttu-id="42f18-103">Тип ресурса Кондитионалакцессдевицестатес</span><span class="sxs-lookup"><span data-stu-id="42f18-103">conditionalAccessDeviceStates resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42f18-104">Представляет состояния устройства в области политики.</span><span class="sxs-lookup"><span data-stu-id="42f18-104">Represents device states in the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="42f18-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="42f18-105">Properties</span></span>

| <span data-ttu-id="42f18-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="42f18-106">Property</span></span>     | <span data-ttu-id="42f18-107">Тип</span><span class="sxs-lookup"><span data-stu-id="42f18-107">Type</span></span>        | <span data-ttu-id="42f18-108">Описание</span><span class="sxs-lookup"><span data-stu-id="42f18-108">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="42f18-109">инклудестатес</span><span class="sxs-lookup"><span data-stu-id="42f18-109">includeStates</span></span> | <span data-ttu-id="42f18-110">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="42f18-110">String collection</span></span> | <span data-ttu-id="42f18-111">Состояния политики.</span><span class="sxs-lookup"><span data-stu-id="42f18-111">States in the scope of the policy.</span></span> <span data-ttu-id="42f18-112">`All`— Единственное допустимое значение.</span><span class="sxs-lookup"><span data-stu-id="42f18-112">`All` is the only allowed value.</span></span> |
| <span data-ttu-id="42f18-113">ексклудестатес</span><span class="sxs-lookup"><span data-stu-id="42f18-113">excludeStates</span></span> | <span data-ttu-id="42f18-114">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="42f18-114">String collection</span></span> | <span data-ttu-id="42f18-115">Состояния, исключенные из области применения политики.</span><span class="sxs-lookup"><span data-stu-id="42f18-115">States excluded from the scope of the policy.</span></span> <span data-ttu-id="42f18-116">Возможные значения: `Compliant`, `DomainJoined`.</span><span class="sxs-lookup"><span data-stu-id="42f18-116">Possible values: `Compliant`, `DomainJoined`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="42f18-117">Связи</span><span class="sxs-lookup"><span data-stu-id="42f18-117">Relationships</span></span>

<span data-ttu-id="42f18-118">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="42f18-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="42f18-119">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="42f18-119">JSON representation</span></span>

<span data-ttu-id="42f18-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="42f18-120">The following is a JSON representation of the resource.</span></span>

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