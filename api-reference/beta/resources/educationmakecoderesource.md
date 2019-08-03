---
title: Тип ресурса Едукатионмакекодересаурце
description: Ресурс Макекоде
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: e983f217af71b6e27f750599ee2f8db295da5fec
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173372"
---
# <a name="educationmakecoderesource-resource-type"></a><span data-ttu-id="f1201-103">Тип ресурса Едукатионмакекодересаурце</span><span class="sxs-lookup"><span data-stu-id="f1201-103">educationMakeCodeResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1201-104">Ресурс, представляющий проект [макекоде](https://www.microsoft.com/en-us/makecode) .</span><span class="sxs-lookup"><span data-stu-id="f1201-104">A resource representing a [MakeCode](https://www.microsoft.com/en-us/makecode) project.</span></span>

## <a name="properties"></a><span data-ttu-id="f1201-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="f1201-105">Properties</span></span>

| <span data-ttu-id="f1201-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="f1201-106">Property</span></span>     | <span data-ttu-id="f1201-107">Тип</span><span class="sxs-lookup"><span data-stu-id="f1201-107">Type</span></span>        | <span data-ttu-id="f1201-108">Описание</span><span class="sxs-lookup"><span data-stu-id="f1201-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f1201-109">мккд</span><span class="sxs-lookup"><span data-stu-id="f1201-109">mkcd</span></span>|<span data-ttu-id="f1201-110">String</span><span class="sxs-lookup"><span data-stu-id="f1201-110">String</span></span>|<span data-ttu-id="f1201-111">ИДЕНТИФИКАТОР проекта Макекоде</span><span class="sxs-lookup"><span data-stu-id="f1201-111">ID of the MakeCode project</span></span>|
|<span data-ttu-id="f1201-112">url</span><span class="sxs-lookup"><span data-stu-id="f1201-112">url</span></span>|<span data-ttu-id="f1201-113">String</span><span class="sxs-lookup"><span data-stu-id="f1201-113">String</span></span>|<span data-ttu-id="f1201-114">Узел для типа ресурса Макекоде (например, аркаде, Микробит)</span><span class="sxs-lookup"><span data-stu-id="f1201-114">Host for the type of MakeCode resource (for example, arcade, microbit)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f1201-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f1201-115">JSON representation</span></span>

<span data-ttu-id="f1201-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f1201-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationMakeCodeResource",
  "baseType": "microsoft.graph.educationResource"
}-->

```json
{
  "mkcd": "String",
  "url": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationMakeCodeResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->