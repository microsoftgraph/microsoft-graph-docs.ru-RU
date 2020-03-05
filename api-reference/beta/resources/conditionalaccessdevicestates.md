---
title: Тип ресурса Кондитионалакцессдевицестатес
description: Представляет состояния устройства в области политики.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ff61b1d9713a0da322d01e3c302ebefc98dbee46
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507557"
---
# <a name="conditionalaccessdevicestates-resource-type"></a><span data-ttu-id="26efd-103">Тип ресурса Кондитионалакцессдевицестатес</span><span class="sxs-lookup"><span data-stu-id="26efd-103">conditionalAccessDeviceStates resource type</span></span>

<span data-ttu-id="26efd-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="26efd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26efd-105">Представляет состояния устройства в области политики.</span><span class="sxs-lookup"><span data-stu-id="26efd-105">Represents device states in the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="26efd-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="26efd-106">Properties</span></span>

| <span data-ttu-id="26efd-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="26efd-107">Property</span></span>     | <span data-ttu-id="26efd-108">Тип</span><span class="sxs-lookup"><span data-stu-id="26efd-108">Type</span></span>        | <span data-ttu-id="26efd-109">Описание</span><span class="sxs-lookup"><span data-stu-id="26efd-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="26efd-110">инклудестатес</span><span class="sxs-lookup"><span data-stu-id="26efd-110">includeStates</span></span> | <span data-ttu-id="26efd-111">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="26efd-111">String collection</span></span> | <span data-ttu-id="26efd-112">Состояния политики.</span><span class="sxs-lookup"><span data-stu-id="26efd-112">States in the scope of the policy.</span></span> <span data-ttu-id="26efd-113">`All`— Единственное допустимое значение.</span><span class="sxs-lookup"><span data-stu-id="26efd-113">`All` is the only allowed value.</span></span> |
| <span data-ttu-id="26efd-114">ексклудестатес</span><span class="sxs-lookup"><span data-stu-id="26efd-114">excludeStates</span></span> | <span data-ttu-id="26efd-115">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="26efd-115">String collection</span></span> | <span data-ttu-id="26efd-116">Состояния, исключенные из области применения политики.</span><span class="sxs-lookup"><span data-stu-id="26efd-116">States excluded from the scope of the policy.</span></span> <span data-ttu-id="26efd-117">Возможные значения: `Compliant`, `DomainJoined`.</span><span class="sxs-lookup"><span data-stu-id="26efd-117">Possible values: `Compliant`, `DomainJoined`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="26efd-118">Связи</span><span class="sxs-lookup"><span data-stu-id="26efd-118">Relationships</span></span>

<span data-ttu-id="26efd-119">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="26efd-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="26efd-120">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="26efd-120">JSON representation</span></span>

<span data-ttu-id="26efd-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="26efd-121">The following is a JSON representation of the resource.</span></span>

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