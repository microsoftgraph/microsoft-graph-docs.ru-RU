---
title: Тип ресурса extension
description: Абстрактный тип для поддержки открытого типа openTypeExtension в OData 4-й версии.
ms.openlocfilehash: 1b3d735e0997ca128b539bff9a05c9c7c56799df
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024643"
---
# <a name="extension-resource-type"></a><span data-ttu-id="c618e-103">Тип ресурса extension</span><span class="sxs-lookup"><span data-stu-id="c618e-103">extension resource type</span></span>

<span data-ttu-id="c618e-104">Абстрактный тип для поддержки открытого типа [openTypeExtension](opentypeextension.md) в OData 4-й версии.</span><span class="sxs-lookup"><span data-stu-id="c618e-104">An abstract type to support the OData v4 open type [openTypeExtension](opentypeextension.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="c618e-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c618e-105">JSON representation</span></span>

<span data-ttu-id="c618e-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="c618e-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "abstract": "true",
  "baseType": "microsoft.graph.entity",
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.extension"
}-->

```json
{
  "id": "string (identifier)"
}

```
## <a name="properties"></a><span data-ttu-id="c618e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c618e-107">Properties</span></span>
| <span data-ttu-id="c618e-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c618e-108">Property</span></span>     | <span data-ttu-id="c618e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c618e-109">Type</span></span>   |<span data-ttu-id="c618e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c618e-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c618e-111">id</span><span class="sxs-lookup"><span data-stu-id="c618e-111">id</span></span>|<span data-ttu-id="c618e-112">String</span><span class="sxs-lookup"><span data-stu-id="c618e-112">String</span></span>| <span data-ttu-id="c618e-113">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c618e-113">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c618e-114">Связи</span><span class="sxs-lookup"><span data-stu-id="c618e-114">Relationships</span></span>
<span data-ttu-id="c618e-115">Нет</span><span class="sxs-lookup"><span data-stu-id="c618e-115">None</span></span>


## <a name="methods"></a><span data-ttu-id="c618e-116">Методы</span><span class="sxs-lookup"><span data-stu-id="c618e-116">Methods</span></span>

<span data-ttu-id="c618e-117">Фактически поддерживаемые методы указаны в описании производного типа [openTypeExtension](opentypeextension.md).</span><span class="sxs-lookup"><span data-stu-id="c618e-117">See the methods of the derived type [openTypeExtension](opentypeextension.md) for actually supported methods.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "extension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->