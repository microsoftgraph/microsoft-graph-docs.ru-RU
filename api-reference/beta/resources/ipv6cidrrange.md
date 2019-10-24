---
title: Тип ресурса iPv6CidrRange
description: Представляет диапазон IPv6-адресов с использованием нотации CIDR.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7201a95013551aa9629032bffc808f93156f66a0
ms.sourcegitcommit: d189830649794365464e37539e02239f883011da
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/24/2019
ms.locfileid: "37653848"
---
# <a name="ipv6cidrrange-resource-type"></a><span data-ttu-id="a1af0-103">Тип ресурса iPv6CidrRange</span><span class="sxs-lookup"><span data-stu-id="a1af0-103">iPv6CidrRange resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a1af0-104">Представляет диапазон IPv6-адресов с использованием нотации CIDR.</span><span class="sxs-lookup"><span data-stu-id="a1af0-104">Represents an IPv6 range using the CIDR notation.</span></span>

<span data-ttu-id="a1af0-105">Наследуется от ресурса [ipRange](../resources/iprange.md)</span><span class="sxs-lookup"><span data-stu-id="a1af0-105">Inherits from [ipRange](../resources/iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a1af0-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a1af0-106">Properties</span></span>

| <span data-ttu-id="a1af0-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="a1af0-107">Property</span></span>     | <span data-ttu-id="a1af0-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a1af0-108">Type</span></span>        | <span data-ttu-id="a1af0-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a1af0-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a1af0-110">Цидраддресс</span><span class="sxs-lookup"><span data-stu-id="a1af0-110">cidrAddress</span></span>|<span data-ttu-id="a1af0-111">String</span><span class="sxs-lookup"><span data-stu-id="a1af0-111">String</span></span>|<span data-ttu-id="a1af0-112">IPv6-адрес в нотации CIDR</span><span class="sxs-lookup"><span data-stu-id="a1af0-112">IPv6 address in CIDR notation</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a1af0-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a1af0-113">JSON representation</span></span>

<span data-ttu-id="a1af0-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a1af0-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.iPv6CidrRange",
  "baseType": "microsoft.graph.ipRange"
}-->

```json
{
  "cidrAddress": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "iPv6CidrRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->