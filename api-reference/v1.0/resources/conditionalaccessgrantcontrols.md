---
title: Тип ресурса Кондитионалакцессгрантконтролс
description: Представляет элементы управления предоставлением, которые должны быть выполнены для передачи политики.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e48d179e53111cc69b72eb8aa61c52ae105764df
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48018909"
---
# <a name="conditionalaccessgrantcontrols-resource-type"></a><span data-ttu-id="77d14-103">Тип ресурса Кондитионалакцессгрантконтролс</span><span class="sxs-lookup"><span data-stu-id="77d14-103">conditionalAccessGrantControls resource type</span></span>

<span data-ttu-id="77d14-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77d14-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="77d14-105">Представляет элементы управления предоставлением, которые должны быть выполнены для передачи политики.</span><span class="sxs-lookup"><span data-stu-id="77d14-105">Represents grant controls that must be fulfilled to pass the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="77d14-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="77d14-106">Properties</span></span>

| <span data-ttu-id="77d14-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="77d14-107">Property</span></span> | <span data-ttu-id="77d14-108">Тип</span><span class="sxs-lookup"><span data-stu-id="77d14-108">Type</span></span> | <span data-ttu-id="77d14-109">Описание</span><span class="sxs-lookup"><span data-stu-id="77d14-109">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="77d14-110">operator</span><span class="sxs-lookup"><span data-stu-id="77d14-110">operator</span></span> | <span data-ttu-id="77d14-111">String</span><span class="sxs-lookup"><span data-stu-id="77d14-111">String</span></span> | <span data-ttu-id="77d14-112">Определяет связь элементов управления предоставлением.</span><span class="sxs-lookup"><span data-stu-id="77d14-112">Defines the relationship of the grant controls.</span></span> <span data-ttu-id="77d14-113">Возможные значения: `AND` , `OR` .</span><span class="sxs-lookup"><span data-stu-id="77d14-113">Possible values: `AND`, `OR`.</span></span> |
| <span data-ttu-id="77d14-114">буилтинконтролс</span><span class="sxs-lookup"><span data-stu-id="77d14-114">builtInControls</span></span> | <span data-ttu-id="77d14-115">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="77d14-115">String collection</span></span> | <span data-ttu-id="77d14-116">Список значений встроенных элементов управления, необходимых для политики.</span><span class="sxs-lookup"><span data-stu-id="77d14-116">List of values of built-in controls required by the policy.</span></span> <span data-ttu-id="77d14-117">Возможные значения: `Block` , `Mfa` , `CompliantDevice` , `DomainJoinedDevice` , `ApprovedApplication` , `CompliantApplication`</span><span class="sxs-lookup"><span data-stu-id="77d14-117">Possible values: `Block`, `Mfa`, `CompliantDevice`, `DomainJoinedDevice`, `ApprovedApplication`, `CompliantApplication`</span></span> |
| <span data-ttu-id="77d14-118">кустомаусентикатионфакторс</span><span class="sxs-lookup"><span data-stu-id="77d14-118">customAuthenticationFactors</span></span> | <span data-ttu-id="77d14-119">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="77d14-119">String collection</span></span> | <span data-ttu-id="77d14-120">Список идентификаторов настраиваемых элементов управления, необходимых для политики.</span><span class="sxs-lookup"><span data-stu-id="77d14-120">List of custom controls IDs required by the policy.</span></span> <span data-ttu-id="77d14-121">Более подробную информацию можно узнать в статье [настраиваемые элементы управления](https://docs.microsoft.com/azure/active-directory/conditional-access/controls).</span><span class="sxs-lookup"><span data-stu-id="77d14-121">For more information, see [Custom controls](https://docs.microsoft.com/azure/active-directory/conditional-access/controls).</span></span> |
| <span data-ttu-id="77d14-122">термсофусе</span><span class="sxs-lookup"><span data-stu-id="77d14-122">termsOfUse</span></span> | <span data-ttu-id="77d14-123">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="77d14-123">String collection</span></span> | <span data-ttu-id="77d14-124">Список [условий использования](https://docs.microsoft.com/graph/api/resources/agreement) идентификаторов, необходимых для политики.</span><span class="sxs-lookup"><span data-stu-id="77d14-124">List of [terms of use](https://docs.microsoft.com/graph/api/resources/agreement) IDs required by the policy.</span></span> |

## <a name="relationships"></a><span data-ttu-id="77d14-125">Связи</span><span class="sxs-lookup"><span data-stu-id="77d14-125">Relationships</span></span>

<span data-ttu-id="77d14-126">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="77d14-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="77d14-127">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="77d14-127">JSON representation</span></span>

<span data-ttu-id="77d14-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="77d14-128">The following is a JSON representation of the resource.</span></span>

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

