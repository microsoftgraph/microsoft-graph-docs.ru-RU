---
title: изменен тип ресурсаQueryToken
description: Представляет измененные сегменты в отношении исходного пользовательского запроса.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 03e6f010fdcd77e07fc6ce3cc7e8c8c285fde73f
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52068233"
---
# <a name="alteredquerytoken-resource-type"></a><span data-ttu-id="a5ec8-103">изменен тип ресурсаQueryToken</span><span class="sxs-lookup"><span data-stu-id="a5ec8-103">alteredQueryToken resource type</span></span>

<span data-ttu-id="a5ec8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5ec8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5ec8-105">Представляет измененные сегменты в отношении исходного пользовательского запроса.</span><span class="sxs-lookup"><span data-stu-id="a5ec8-105">Represents changed segments with respect to original user query.</span></span>

## <a name="properties"></a><span data-ttu-id="a5ec8-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a5ec8-106">Properties</span></span>

| <span data-ttu-id="a5ec8-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="a5ec8-107">Property</span></span>     | <span data-ttu-id="a5ec8-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a5ec8-108">Type</span></span>        | <span data-ttu-id="a5ec8-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a5ec8-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a5ec8-110">смещение</span><span class="sxs-lookup"><span data-stu-id="a5ec8-110">offset</span></span>|<span data-ttu-id="a5ec8-111">Int32</span><span class="sxs-lookup"><span data-stu-id="a5ec8-111">Int32</span></span>| <span data-ttu-id="a5ec8-112">Определяет смещение измененного сегмента.</span><span class="sxs-lookup"><span data-stu-id="a5ec8-112">Defines the offset of a changed segment.</span></span>|
|<span data-ttu-id="a5ec8-113">length</span><span class="sxs-lookup"><span data-stu-id="a5ec8-113">length</span></span>|<span data-ttu-id="a5ec8-114">Int32</span><span class="sxs-lookup"><span data-stu-id="a5ec8-114">Int32</span></span>| <span data-ttu-id="a5ec8-115">Определяет длину измененного сегмента.</span><span class="sxs-lookup"><span data-stu-id="a5ec8-115">Defines the length of a changed segment.</span></span>|
|<span data-ttu-id="a5ec8-116">предложение</span><span class="sxs-lookup"><span data-stu-id="a5ec8-116">suggestion</span></span>|<span data-ttu-id="a5ec8-117">String</span><span class="sxs-lookup"><span data-stu-id="a5ec8-117">String</span></span>| <span data-ttu-id="a5ec8-118">Представляет строку исправленного сегмента.</span><span class="sxs-lookup"><span data-stu-id="a5ec8-118">Represents the corrected segment string.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a5ec8-119">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a5ec8-119">JSON representation</span></span>

<span data-ttu-id="a5ec8-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a5ec8-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.alteredQueryToken",
  "baseType": null
}-->

```json
{
  "offset": 0,
  "length": 6,
  "suggestion": "String"
}
```
