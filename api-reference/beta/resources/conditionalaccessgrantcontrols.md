---
title: Тип ресурса Кондитионалакцессгрантконтролс
description: Представляет элементы управления предоставлением, которые должны быть выполнены для передачи политики.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a4312accf3b908689a0037d3c16a7ba2242c2ddf
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2020
ms.locfileid: "43916793"
---
# <a name="conditionalaccessgrantcontrols-resource-type"></a><span data-ttu-id="64218-103">Тип ресурса Кондитионалакцессгрантконтролс</span><span class="sxs-lookup"><span data-stu-id="64218-103">conditionalAccessGrantControls resource type</span></span>

<span data-ttu-id="64218-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64218-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64218-105">Представляет элементы управления предоставлением, которые должны быть выполнены для передачи политики.</span><span class="sxs-lookup"><span data-stu-id="64218-105">Represents grant controls that must be fulfilled to pass the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="64218-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="64218-106">Properties</span></span>

| <span data-ttu-id="64218-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="64218-107">Property</span></span> | <span data-ttu-id="64218-108">Тип</span><span class="sxs-lookup"><span data-stu-id="64218-108">Type</span></span> | <span data-ttu-id="64218-109">Описание</span><span class="sxs-lookup"><span data-stu-id="64218-109">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="64218-110">operator</span><span class="sxs-lookup"><span data-stu-id="64218-110">operator</span></span> | <span data-ttu-id="64218-111">String</span><span class="sxs-lookup"><span data-stu-id="64218-111">String</span></span> | <span data-ttu-id="64218-112">Определяет связь элементов управления предоставлением.</span><span class="sxs-lookup"><span data-stu-id="64218-112">Defines the relationship of the grant controls.</span></span> <span data-ttu-id="64218-113">Возможные значения: `AND`, `OR`.</span><span class="sxs-lookup"><span data-stu-id="64218-113">Possible values: `AND`, `OR`.</span></span> |
| <span data-ttu-id="64218-114">буилтинконтролс</span><span class="sxs-lookup"><span data-stu-id="64218-114">builtInControls</span></span> | <span data-ttu-id="64218-115">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="64218-115">String collection</span></span> | <span data-ttu-id="64218-116">Список значений встроенных элементов управления, необходимых для политики.</span><span class="sxs-lookup"><span data-stu-id="64218-116">List of values of built-in controls required by the policy.</span></span> <span data-ttu-id="64218-117">Возможные значения: `Block`, `Mfa`, `CompliantDevice`, `DomainJoinedDevice`, `ApprovedApplication`,`CompliantApplication`</span><span class="sxs-lookup"><span data-stu-id="64218-117">Possible values: `Block`, `Mfa`, `CompliantDevice`, `DomainJoinedDevice`, `ApprovedApplication`, `CompliantApplication`</span></span> |
| <span data-ttu-id="64218-118">кустомаусентикатионфакторс</span><span class="sxs-lookup"><span data-stu-id="64218-118">customAuthenticationFactors</span></span> | <span data-ttu-id="64218-119">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="64218-119">String collection</span></span> | <span data-ttu-id="64218-120">Список идентификаторов настраиваемых элементов управления, необходимых для политики.</span><span class="sxs-lookup"><span data-stu-id="64218-120">List of custom controls IDs required by the policy.</span></span> <span data-ttu-id="64218-121">Дополнительные сведения о настраиваемых элементах управления:https://docs.microsoft.com/azure/active-directory/conditional-access/controls#custom-controls-preview</span><span class="sxs-lookup"><span data-stu-id="64218-121">Learn more about custom controls here: https://docs.microsoft.com/azure/active-directory/conditional-access/controls#custom-controls-preview</span></span> |
| <span data-ttu-id="64218-122">термсофусе</span><span class="sxs-lookup"><span data-stu-id="64218-122">termsOfUse</span></span> | <span data-ttu-id="64218-123">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="64218-123">String collection</span></span> | <span data-ttu-id="64218-124">Список [условий использования](agreement.md) идентификаторов, необходимых для политики.</span><span class="sxs-lookup"><span data-stu-id="64218-124">List of [terms of use](agreement.md) IDs required by the policy.</span></span> |

## <a name="relationships"></a><span data-ttu-id="64218-125">Связи</span><span class="sxs-lookup"><span data-stu-id="64218-125">Relationships</span></span>

<span data-ttu-id="64218-126">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="64218-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="64218-127">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="64218-127">JSON representation</span></span>

<span data-ttu-id="64218-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="64218-128">The following is a JSON representation of the resource.</span></span>

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