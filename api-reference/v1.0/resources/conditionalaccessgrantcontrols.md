---
title: Тип ресурса Кондитионалакцессгрантконтролс
description: Представляет элементы управления предоставлением, которые должны быть выполнены для передачи политики.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: aadf38ac5cff15e4c085f77df36aa6fd48fa272f
ms.sourcegitcommit: fec7d5002dbeb8d58587c89f1b678d4a54645422
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/23/2020
ms.locfileid: "45384684"
---
# <a name="conditionalaccessgrantcontrols-resource-type"></a><span data-ttu-id="0bd8f-103">Тип ресурса Кондитионалакцессгрантконтролс</span><span class="sxs-lookup"><span data-stu-id="0bd8f-103">conditionalAccessGrantControls resource type</span></span>

<span data-ttu-id="0bd8f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0bd8f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0bd8f-105">Представляет элементы управления предоставлением, которые должны быть выполнены для передачи политики.</span><span class="sxs-lookup"><span data-stu-id="0bd8f-105">Represents grant controls that must be fulfilled to pass the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="0bd8f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="0bd8f-106">Properties</span></span>

| <span data-ttu-id="0bd8f-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="0bd8f-107">Property</span></span> | <span data-ttu-id="0bd8f-108">Тип</span><span class="sxs-lookup"><span data-stu-id="0bd8f-108">Type</span></span> | <span data-ttu-id="0bd8f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0bd8f-109">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="0bd8f-110">operator</span><span class="sxs-lookup"><span data-stu-id="0bd8f-110">operator</span></span> | <span data-ttu-id="0bd8f-111">String</span><span class="sxs-lookup"><span data-stu-id="0bd8f-111">String</span></span> | <span data-ttu-id="0bd8f-112">Определяет связь элементов управления предоставлением.</span><span class="sxs-lookup"><span data-stu-id="0bd8f-112">Defines the relationship of the grant controls.</span></span> <span data-ttu-id="0bd8f-113">Возможные значения: `AND` , `OR` .</span><span class="sxs-lookup"><span data-stu-id="0bd8f-113">Possible values: `AND`, `OR`.</span></span> |
| <span data-ttu-id="0bd8f-114">буилтинконтролс</span><span class="sxs-lookup"><span data-stu-id="0bd8f-114">builtInControls</span></span> | <span data-ttu-id="0bd8f-115">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="0bd8f-115">String collection</span></span> | <span data-ttu-id="0bd8f-116">Список значений встроенных элементов управления, необходимых для политики.</span><span class="sxs-lookup"><span data-stu-id="0bd8f-116">List of values of built-in controls required by the policy.</span></span> <span data-ttu-id="0bd8f-117">Возможные значения: `Block` , `Mfa` , `CompliantDevice` , `DomainJoinedDevice` , `ApprovedApplication` ,`CompliantApplication`</span><span class="sxs-lookup"><span data-stu-id="0bd8f-117">Possible values: `Block`, `Mfa`, `CompliantDevice`, `DomainJoinedDevice`, `ApprovedApplication`, `CompliantApplication`</span></span> |
| <span data-ttu-id="0bd8f-118">кустомаусентикатионфакторс</span><span class="sxs-lookup"><span data-stu-id="0bd8f-118">customAuthenticationFactors</span></span> | <span data-ttu-id="0bd8f-119">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="0bd8f-119">String collection</span></span> | <span data-ttu-id="0bd8f-120">Список идентификаторов настраиваемых элементов управления, необходимых для политики.</span><span class="sxs-lookup"><span data-stu-id="0bd8f-120">List of custom controls IDs required by the policy.</span></span> <span data-ttu-id="0bd8f-121">Более подробную информацию можно узнать в статье [настраиваемые элементы управления](https://docs.microsoft.com/azure/active-directory/conditional-access/controls).</span><span class="sxs-lookup"><span data-stu-id="0bd8f-121">For more information, see [Custom controls](https://docs.microsoft.com/azure/active-directory/conditional-access/controls).</span></span> |
| <span data-ttu-id="0bd8f-122">термсофусе</span><span class="sxs-lookup"><span data-stu-id="0bd8f-122">termsOfUse</span></span> | <span data-ttu-id="0bd8f-123">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="0bd8f-123">String collection</span></span> | <span data-ttu-id="0bd8f-124">Список [условий использования](https://docs.microsoft.com/graph/api/resources/agreement) идентификаторов, необходимых для политики.</span><span class="sxs-lookup"><span data-stu-id="0bd8f-124">List of [terms of use](https://docs.microsoft.com/graph/api/resources/agreement) IDs required by the policy.</span></span> |

## <a name="relationships"></a><span data-ttu-id="0bd8f-125">Связи</span><span class="sxs-lookup"><span data-stu-id="0bd8f-125">Relationships</span></span>

<span data-ttu-id="0bd8f-126">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="0bd8f-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0bd8f-127">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="0bd8f-127">JSON representation</span></span>

<span data-ttu-id="0bd8f-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0bd8f-128">The following is a JSON representation of the resource.</span></span>

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
