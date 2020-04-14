---
title: Тип ресурса Кондитионалакцессгрантконтролс
description: Представляет элементы управления предоставлением, которые должны быть выполнены для передачи политики.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9746bfb37dd3887def0f070256d90e46efecbdb6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43413433"
---
# <a name="conditionalaccessgrantcontrols-resource-type"></a><span data-ttu-id="e90e1-103">Тип ресурса Кондитионалакцессгрантконтролс</span><span class="sxs-lookup"><span data-stu-id="e90e1-103">conditionalAccessGrantControls resource type</span></span>

<span data-ttu-id="e90e1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e90e1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e90e1-105">Представляет элементы управления предоставлением, которые должны быть выполнены для передачи политики.</span><span class="sxs-lookup"><span data-stu-id="e90e1-105">Represents grant controls that must be fulfilled to pass the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="e90e1-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e90e1-106">Properties</span></span>

| <span data-ttu-id="e90e1-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="e90e1-107">Property</span></span> | <span data-ttu-id="e90e1-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e90e1-108">Type</span></span> | <span data-ttu-id="e90e1-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e90e1-109">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="e90e1-110">operator</span><span class="sxs-lookup"><span data-stu-id="e90e1-110">operator</span></span> | <span data-ttu-id="e90e1-111">String</span><span class="sxs-lookup"><span data-stu-id="e90e1-111">String</span></span> | <span data-ttu-id="e90e1-112">Определяет связь элементов управления предоставлением.</span><span class="sxs-lookup"><span data-stu-id="e90e1-112">Defines the relationship of the grant controls.</span></span> <span data-ttu-id="e90e1-113">Возможные значения: `AND`, `OR`.</span><span class="sxs-lookup"><span data-stu-id="e90e1-113">Possible values: `AND`, `OR`.</span></span> |
| <span data-ttu-id="e90e1-114">буилтинконтролс</span><span class="sxs-lookup"><span data-stu-id="e90e1-114">builtInControls</span></span> | <span data-ttu-id="e90e1-115">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e90e1-115">String collection</span></span> | <span data-ttu-id="e90e1-116">Список значений встроенных элементов управления, необходимых для политики.</span><span class="sxs-lookup"><span data-stu-id="e90e1-116">List of values of built-in controls required by the policy.</span></span> <span data-ttu-id="e90e1-117">Возможные значения: `Block`, `Mfa`, `CompliantDevice`, `DomainJoinedDevice`, `ApprovedApplication`,`CompliantApplication`</span><span class="sxs-lookup"><span data-stu-id="e90e1-117">Possible values: `Block`, `Mfa`, `CompliantDevice`, `DomainJoinedDevice`, `ApprovedApplication`, `CompliantApplication`</span></span> |
| <span data-ttu-id="e90e1-118">кустомаусентикатионфакторс</span><span class="sxs-lookup"><span data-stu-id="e90e1-118">customAuthenticationFactors</span></span> | <span data-ttu-id="e90e1-119">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e90e1-119">String collection</span></span> | <span data-ttu-id="e90e1-120">Список идентификаторов настраиваемых элементов управления, необходимых для политики.</span><span class="sxs-lookup"><span data-stu-id="e90e1-120">List of custom controls IDs required by the policy.</span></span> <span data-ttu-id="e90e1-121">Дополнительные сведения о настраиваемых элементах управления:https://docs.microsoft.com/azure/active-directory/conditional-access/controls#custom-controls-preview</span><span class="sxs-lookup"><span data-stu-id="e90e1-121">Learn more about custom controls here: https://docs.microsoft.com/azure/active-directory/conditional-access/controls#custom-controls-preview</span></span> |
| <span data-ttu-id="e90e1-122">термсофусе</span><span class="sxs-lookup"><span data-stu-id="e90e1-122">termsOfUse</span></span> | <span data-ttu-id="e90e1-123">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e90e1-123">String collection</span></span> | <span data-ttu-id="e90e1-124">Список [условий использования](agreement.md) идентификаторов, необходимых для политики.</span><span class="sxs-lookup"><span data-stu-id="e90e1-124">List of [terms of use](agreement.md) IDs required by the policy.</span></span> |

## <a name="relationships"></a><span data-ttu-id="e90e1-125">Связи</span><span class="sxs-lookup"><span data-stu-id="e90e1-125">Relationships</span></span>

<span data-ttu-id="e90e1-126">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e90e1-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e90e1-127">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e90e1-127">JSON representation</span></span>

<span data-ttu-id="e90e1-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e90e1-128">The following is a JSON representation of the resource.</span></span>

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