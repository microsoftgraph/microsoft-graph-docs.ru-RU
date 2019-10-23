---
title: Тип ресурса Кондитионалакцессгрантконтролс
description: Представляет элементы управления предоставлением, которые должны быть выполнены для передачи политики.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ebeb84ccf0e010ad792133f16f7819ca1d8b8ed0
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638500"
---
# <a name="conditionalaccessgrantcontrols-resource-type"></a><span data-ttu-id="de4b6-103">Тип ресурса Кондитионалакцессгрантконтролс</span><span class="sxs-lookup"><span data-stu-id="de4b6-103">conditionalAccessGrantControls resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de4b6-104">Представляет элементы управления предоставлением, которые должны быть выполнены для передачи политики.</span><span class="sxs-lookup"><span data-stu-id="de4b6-104">Represents grant controls that must be fulfilled to pass the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="de4b6-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="de4b6-105">Properties</span></span>

| <span data-ttu-id="de4b6-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="de4b6-106">Property</span></span> | <span data-ttu-id="de4b6-107">Тип</span><span class="sxs-lookup"><span data-stu-id="de4b6-107">Type</span></span> | <span data-ttu-id="de4b6-108">Описание</span><span class="sxs-lookup"><span data-stu-id="de4b6-108">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="de4b6-109">operator</span><span class="sxs-lookup"><span data-stu-id="de4b6-109">operator</span></span> | <span data-ttu-id="de4b6-110">String</span><span class="sxs-lookup"><span data-stu-id="de4b6-110">String</span></span> | <span data-ttu-id="de4b6-111">Определяет связь элементов управления предоставлением.</span><span class="sxs-lookup"><span data-stu-id="de4b6-111">Defines the relationship of the grant controls.</span></span> <span data-ttu-id="de4b6-112">Возможные значения: `AND`, `OR`.</span><span class="sxs-lookup"><span data-stu-id="de4b6-112">Possible values: `AND`, `OR`.</span></span> |
| <span data-ttu-id="de4b6-113">буилтинконтролс</span><span class="sxs-lookup"><span data-stu-id="de4b6-113">builtInControls</span></span> | <span data-ttu-id="de4b6-114">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="de4b6-114">String collection</span></span> | <span data-ttu-id="de4b6-115">Список значений встроенных элементов управления, необходимых для политики.</span><span class="sxs-lookup"><span data-stu-id="de4b6-115">List of values of built-in controls required by the policy.</span></span> <span data-ttu-id="de4b6-116">Возможные значения: `Block`, `Mfa`, `CompliantDevice`, `DomainJoinedDevice`, `ApprovedApplication`,`CompliantApplication`</span><span class="sxs-lookup"><span data-stu-id="de4b6-116">Possible values: `Block`, `Mfa`, `CompliantDevice`, `DomainJoinedDevice`, `ApprovedApplication`, `CompliantApplication`</span></span> |
| <span data-ttu-id="de4b6-117">кустомаусентикатионфакторс</span><span class="sxs-lookup"><span data-stu-id="de4b6-117">customAuthenticationFactors</span></span> | <span data-ttu-id="de4b6-118">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="de4b6-118">String collection</span></span> | <span data-ttu-id="de4b6-119">Список идентификаторов настраиваемых элементов управления, необходимых для политики.</span><span class="sxs-lookup"><span data-stu-id="de4b6-119">List of custom controls IDs required by the policy.</span></span> <span data-ttu-id="de4b6-120">Дополнительные сведения о настраиваемых элементах управления:https://docs.microsoft.com/azure/active-directory/conditional-access/controls#custom-controls-preview</span><span class="sxs-lookup"><span data-stu-id="de4b6-120">Learn more about custom controls here: https://docs.microsoft.com/azure/active-directory/conditional-access/controls#custom-controls-preview</span></span> |
| <span data-ttu-id="de4b6-121">термсофусе</span><span class="sxs-lookup"><span data-stu-id="de4b6-121">termsOfUse</span></span> | <span data-ttu-id="de4b6-122">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="de4b6-122">String collection</span></span> | <span data-ttu-id="de4b6-123">Список [условий использования](agreement.md) идентификаторов, необходимых для политики.</span><span class="sxs-lookup"><span data-stu-id="de4b6-123">List of [terms of use](agreement.md) IDs required by the policy.</span></span> |

## <a name="relationships"></a><span data-ttu-id="de4b6-124">Связи</span><span class="sxs-lookup"><span data-stu-id="de4b6-124">Relationships</span></span>

<span data-ttu-id="de4b6-125">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="de4b6-125">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="de4b6-126">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="de4b6-126">JSON representation</span></span>

<span data-ttu-id="de4b6-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="de4b6-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "operator",
    "builtInControls",
    "customAuthenticationFactors",
    "termsOfUse"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessGrantControls",
  "baseType": null
}-->

```json
{
  "builtInControls": ["String"],
  "customAuthenticationFactors": ["String"],
  "operator": "String",
  "termsOfUse": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessGrantControls resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->