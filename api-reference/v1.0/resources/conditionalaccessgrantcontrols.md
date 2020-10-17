---
title: Тип ресурса Кондитионалакцессгрантконтролс
description: Представляет элементы управления предоставлением, которые должны быть выполнены для передачи политики.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 431ea73f20b36b189ae7638cc56a01239c1f113f
ms.sourcegitcommit: 577bfd3bb8a2e2679ef1c5942a4a496c2aa3a277
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/17/2020
ms.locfileid: "48582130"
---
# <a name="conditionalaccessgrantcontrols-resource-type"></a><span data-ttu-id="87d88-103">Тип ресурса Кондитионалакцессгрантконтролс</span><span class="sxs-lookup"><span data-stu-id="87d88-103">conditionalAccessGrantControls resource type</span></span>

<span data-ttu-id="87d88-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87d88-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="87d88-105">Представляет элементы управления предоставлением, которые должны быть выполнены для передачи политики.</span><span class="sxs-lookup"><span data-stu-id="87d88-105">Represents grant controls that must be fulfilled to pass the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="87d88-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="87d88-106">Properties</span></span>

| <span data-ttu-id="87d88-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="87d88-107">Property</span></span> | <span data-ttu-id="87d88-108">Тип</span><span class="sxs-lookup"><span data-stu-id="87d88-108">Type</span></span> | <span data-ttu-id="87d88-109">Описание</span><span class="sxs-lookup"><span data-stu-id="87d88-109">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="87d88-110">operator</span><span class="sxs-lookup"><span data-stu-id="87d88-110">operator</span></span> | <span data-ttu-id="87d88-111">String</span><span class="sxs-lookup"><span data-stu-id="87d88-111">String</span></span> | <span data-ttu-id="87d88-112">Определяет связь элементов управления предоставлением.</span><span class="sxs-lookup"><span data-stu-id="87d88-112">Defines the relationship of the grant controls.</span></span> <span data-ttu-id="87d88-113">Возможные значения: `AND` , `OR` .</span><span class="sxs-lookup"><span data-stu-id="87d88-113">Possible values: `AND`, `OR`.</span></span> |
| <span data-ttu-id="87d88-114">буилтинконтролс</span><span class="sxs-lookup"><span data-stu-id="87d88-114">builtInControls</span></span> | <span data-ttu-id="87d88-115">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="87d88-115">String collection</span></span> | <span data-ttu-id="87d88-116">Список значений встроенных элементов управления, необходимых для политики.</span><span class="sxs-lookup"><span data-stu-id="87d88-116">List of values of built-in controls required by the policy.</span></span> <span data-ttu-id="87d88-117">Возможные значения: `Block` , `Mfa` , `CompliantDevice` , `DomainJoinedDevice` , `ApprovedApplication` , `CompliantApplication`</span><span class="sxs-lookup"><span data-stu-id="87d88-117">Possible values: `Block`, `Mfa`, `CompliantDevice`, `DomainJoinedDevice`, `ApprovedApplication`, `CompliantApplication`</span></span> |
| <span data-ttu-id="87d88-118">кустомаусентикатионфакторс</span><span class="sxs-lookup"><span data-stu-id="87d88-118">customAuthenticationFactors</span></span> | <span data-ttu-id="87d88-119">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="87d88-119">String collection</span></span> | <span data-ttu-id="87d88-120">Список идентификаторов настраиваемых элементов управления, необходимых для политики.</span><span class="sxs-lookup"><span data-stu-id="87d88-120">List of custom controls IDs required by the policy.</span></span> <span data-ttu-id="87d88-121">Более подробную информацию можно узнать в статье [настраиваемые элементы управления](/azure/active-directory/conditional-access/controls).</span><span class="sxs-lookup"><span data-stu-id="87d88-121">For more information, see [Custom controls](/azure/active-directory/conditional-access/controls).</span></span> |
| <span data-ttu-id="87d88-122">термсофусе</span><span class="sxs-lookup"><span data-stu-id="87d88-122">termsOfUse</span></span> | <span data-ttu-id="87d88-123">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="87d88-123">String collection</span></span> | <span data-ttu-id="87d88-124">Список [условий использования](/graph/api/resources/agreement) идентификаторов, необходимых для политики.</span><span class="sxs-lookup"><span data-stu-id="87d88-124">List of [terms of use](/graph/api/resources/agreement) IDs required by the policy.</span></span> |

## <a name="relationships"></a><span data-ttu-id="87d88-125">Связи</span><span class="sxs-lookup"><span data-stu-id="87d88-125">Relationships</span></span>

<span data-ttu-id="87d88-126">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="87d88-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="87d88-127">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="87d88-127">JSON representation</span></span>

<span data-ttu-id="87d88-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="87d88-128">The following is a JSON representation of the resource.</span></span>

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