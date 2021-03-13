---
title: conditionalAccessDeviceStates Тип ресурса
description: Представляет состояния устройств в области политики.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 152c4edbd641d68f6211111cb29e9794e2a88260
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761802"
---
# <a name="conditionalaccessdevicestates-resource-type"></a><span data-ttu-id="569c7-103">conditionalAccessDeviceStates Тип ресурса</span><span class="sxs-lookup"><span data-stu-id="569c7-103">conditionalAccessDeviceStates resource type</span></span>

<span data-ttu-id="569c7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="569c7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="569c7-105">Представляет состояния устройств в области политики.</span><span class="sxs-lookup"><span data-stu-id="569c7-105">Represents device states in the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="569c7-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="569c7-106">Properties</span></span>

| <span data-ttu-id="569c7-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="569c7-107">Property</span></span>     | <span data-ttu-id="569c7-108">Тип</span><span class="sxs-lookup"><span data-stu-id="569c7-108">Type</span></span>        | <span data-ttu-id="569c7-109">Описание</span><span class="sxs-lookup"><span data-stu-id="569c7-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="569c7-110">includeStates</span><span class="sxs-lookup"><span data-stu-id="569c7-110">includeStates</span></span> | <span data-ttu-id="569c7-111">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="569c7-111">String collection</span></span> | <span data-ttu-id="569c7-112">Состояния в области политики.</span><span class="sxs-lookup"><span data-stu-id="569c7-112">States in the scope of the policy.</span></span> <span data-ttu-id="569c7-113">`All` является единственным допустимым значением.</span><span class="sxs-lookup"><span data-stu-id="569c7-113">`All` is the only allowed value.</span></span> |
| <span data-ttu-id="569c7-114">excludeStates</span><span class="sxs-lookup"><span data-stu-id="569c7-114">excludeStates</span></span> | <span data-ttu-id="569c7-115">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="569c7-115">String collection</span></span> | <span data-ttu-id="569c7-116">Государства, исключенные из сферы действия политики.</span><span class="sxs-lookup"><span data-stu-id="569c7-116">States excluded from the scope of the policy.</span></span> <span data-ttu-id="569c7-117">Возможные значения: `Compliant` , `DomainJoined` .</span><span class="sxs-lookup"><span data-stu-id="569c7-117">Possible values: `Compliant`, `DomainJoined`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="569c7-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="569c7-118">Relationships</span></span>

<span data-ttu-id="569c7-119">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="569c7-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="569c7-120">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="569c7-120">JSON representation</span></span>

<span data-ttu-id="569c7-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="569c7-121">The following is a JSON representation of the resource.</span></span>

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

