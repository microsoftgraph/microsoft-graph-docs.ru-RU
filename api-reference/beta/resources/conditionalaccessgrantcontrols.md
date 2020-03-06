---
title: Тип ресурса Кондитионалакцессгрантконтролс
description: Представляет элементы управления предоставлением, которые должны быть выполнены для передачи политики.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b91afb44cc43c3c6ac4970afc36914abcb08c4c9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507550"
---
# <a name="conditionalaccessgrantcontrols-resource-type"></a><span data-ttu-id="37373-103">Тип ресурса Кондитионалакцессгрантконтролс</span><span class="sxs-lookup"><span data-stu-id="37373-103">conditionalAccessGrantControls resource type</span></span>

<span data-ttu-id="37373-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37373-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37373-105">Представляет элементы управления предоставлением, которые должны быть выполнены для передачи политики.</span><span class="sxs-lookup"><span data-stu-id="37373-105">Represents grant controls that must be fulfilled to pass the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="37373-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="37373-106">Properties</span></span>

| <span data-ttu-id="37373-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="37373-107">Property</span></span> | <span data-ttu-id="37373-108">Тип</span><span class="sxs-lookup"><span data-stu-id="37373-108">Type</span></span> | <span data-ttu-id="37373-109">Описание</span><span class="sxs-lookup"><span data-stu-id="37373-109">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="37373-110">operator</span><span class="sxs-lookup"><span data-stu-id="37373-110">operator</span></span> | <span data-ttu-id="37373-111">Строка</span><span class="sxs-lookup"><span data-stu-id="37373-111">String</span></span> | <span data-ttu-id="37373-112">Определяет связь элементов управления предоставлением.</span><span class="sxs-lookup"><span data-stu-id="37373-112">Defines the relationship of the grant controls.</span></span> <span data-ttu-id="37373-113">Возможные значения: `AND`, `OR`.</span><span class="sxs-lookup"><span data-stu-id="37373-113">Possible values: `AND`, `OR`.</span></span> |
| <span data-ttu-id="37373-114">буилтинконтролс</span><span class="sxs-lookup"><span data-stu-id="37373-114">builtInControls</span></span> | <span data-ttu-id="37373-115">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="37373-115">String collection</span></span> | <span data-ttu-id="37373-116">Список значений встроенных элементов управления, необходимых для политики.</span><span class="sxs-lookup"><span data-stu-id="37373-116">List of values of built-in controls required by the policy.</span></span> <span data-ttu-id="37373-117">Возможные значения: `Block`, `Mfa`, `CompliantDevice`, `DomainJoinedDevice`, `ApprovedApplication`,`CompliantApplication`</span><span class="sxs-lookup"><span data-stu-id="37373-117">Possible values: `Block`, `Mfa`, `CompliantDevice`, `DomainJoinedDevice`, `ApprovedApplication`, `CompliantApplication`</span></span> |
| <span data-ttu-id="37373-118">кустомаусентикатионфакторс</span><span class="sxs-lookup"><span data-stu-id="37373-118">customAuthenticationFactors</span></span> | <span data-ttu-id="37373-119">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="37373-119">String collection</span></span> | <span data-ttu-id="37373-120">Список идентификаторов настраиваемых элементов управления, необходимых для политики.</span><span class="sxs-lookup"><span data-stu-id="37373-120">List of custom controls IDs required by the policy.</span></span> <span data-ttu-id="37373-121">Дополнительные сведения о настраиваемых элементах управления:https://docs.microsoft.com/azure/active-directory/conditional-access/controls#custom-controls-preview</span><span class="sxs-lookup"><span data-stu-id="37373-121">Learn more about custom controls here: https://docs.microsoft.com/azure/active-directory/conditional-access/controls#custom-controls-preview</span></span> |
| <span data-ttu-id="37373-122">термсофусе</span><span class="sxs-lookup"><span data-stu-id="37373-122">termsOfUse</span></span> | <span data-ttu-id="37373-123">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="37373-123">String collection</span></span> | <span data-ttu-id="37373-124">Список [условий использования](agreement.md) идентификаторов, необходимых для политики.</span><span class="sxs-lookup"><span data-stu-id="37373-124">List of [terms of use](agreement.md) IDs required by the policy.</span></span> |

## <a name="relationships"></a><span data-ttu-id="37373-125">Связи</span><span class="sxs-lookup"><span data-stu-id="37373-125">Relationships</span></span>

<span data-ttu-id="37373-126">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="37373-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="37373-127">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="37373-127">JSON representation</span></span>

<span data-ttu-id="37373-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="37373-128">The following is a JSON representation of the resource.</span></span>

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