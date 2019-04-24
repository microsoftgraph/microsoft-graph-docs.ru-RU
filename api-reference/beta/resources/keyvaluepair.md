---
title: Тип ресурса keyValuePair
description: Ключевое значение для параметров Action.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 86a5415c20721f717947238838341345ec9a4250
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522687"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="e6b1c-103">Тип ресурса keyValuePair</span><span class="sxs-lookup"><span data-stu-id="e6b1c-103">keyValuePair resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6b1c-104">Ключевое значение для параметров Action.</span><span class="sxs-lookup"><span data-stu-id="e6b1c-104">Key value pair for action parameters.</span></span>

## <a name="properties"></a><span data-ttu-id="e6b1c-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="e6b1c-105">Properties</span></span>

| <span data-ttu-id="e6b1c-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="e6b1c-106">Property</span></span>     | <span data-ttu-id="e6b1c-107">Тип</span><span class="sxs-lookup"><span data-stu-id="e6b1c-107">Type</span></span>        | <span data-ttu-id="e6b1c-108">Описание</span><span class="sxs-lookup"><span data-stu-id="e6b1c-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e6b1c-109">name</span><span class="sxs-lookup"><span data-stu-id="e6b1c-109">name</span></span>|<span data-ttu-id="e6b1c-110">String</span><span class="sxs-lookup"><span data-stu-id="e6b1c-110">String</span></span>|<span data-ttu-id="e6b1c-111">Имя для этой пары "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="e6b1c-111">Name for this key-value pair</span></span>|
|<span data-ttu-id="e6b1c-112">value</span><span class="sxs-lookup"><span data-stu-id="e6b1c-112">value</span></span>|<span data-ttu-id="e6b1c-113">String</span><span class="sxs-lookup"><span data-stu-id="e6b1c-113">String</span></span>|<span data-ttu-id="e6b1c-114">Значение для этой пары "ключ-значение"</span><span class="sxs-lookup"><span data-stu-id="e6b1c-114">Value for this key-value pair</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e6b1c-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e6b1c-115">JSON representation</span></span>

<span data-ttu-id="e6b1c-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e6b1c-116">The following is a JSON representation of the resource.</span></span>

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