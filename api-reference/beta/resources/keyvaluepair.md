---
title: Тип ресурса keyValuePair
description: Ключевое значение для параметров Action.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 2417ada5a3fa3937d6560f62a47c99f6b47d44e0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523018"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="a8e2b-103">Тип ресурса keyValuePair</span><span class="sxs-lookup"><span data-stu-id="a8e2b-103">keyValuePair resource type</span></span>

<span data-ttu-id="a8e2b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8e2b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8e2b-105">Ключевое значение для параметров Action.</span><span class="sxs-lookup"><span data-stu-id="a8e2b-105">Key value pair for action parameters.</span></span>

## <a name="properties"></a><span data-ttu-id="a8e2b-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a8e2b-106">Properties</span></span>

| <span data-ttu-id="a8e2b-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="a8e2b-107">Property</span></span>     | <span data-ttu-id="a8e2b-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a8e2b-108">Type</span></span>        | <span data-ttu-id="a8e2b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a8e2b-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a8e2b-110">name</span><span class="sxs-lookup"><span data-stu-id="a8e2b-110">name</span></span>|<span data-ttu-id="a8e2b-111">String</span><span class="sxs-lookup"><span data-stu-id="a8e2b-111">String</span></span>|<span data-ttu-id="a8e2b-112">Имя для этой пары "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="a8e2b-112">Name for this key-value pair</span></span>|
|<span data-ttu-id="a8e2b-113">value</span><span class="sxs-lookup"><span data-stu-id="a8e2b-113">value</span></span>|<span data-ttu-id="a8e2b-114">String</span><span class="sxs-lookup"><span data-stu-id="a8e2b-114">String</span></span>|<span data-ttu-id="a8e2b-115">Значение для этой пары "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="a8e2b-115">Value for this key-value pair</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a8e2b-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a8e2b-116">JSON representation</span></span>

<span data-ttu-id="a8e2b-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a8e2b-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.keyValuePair",
  "baseType": null
}-->

```json
{
  "name": "String",
  "value": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "keyValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->