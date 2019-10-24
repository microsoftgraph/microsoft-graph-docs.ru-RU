---
title: Тип ресурса iPv4CidrRange
description: Представляет диапазон IPv4-адресов с использованием нотации CIDR.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4864388492f3dedec4add271904f2e07a3e85419
ms.sourcegitcommit: d189830649794365464e37539e02239f883011da
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/24/2019
ms.locfileid: "37653827"
---
# <a name="ipv4cidrrange-resource-type"></a><span data-ttu-id="4d62e-103">Тип ресурса iPv4CidrRange</span><span class="sxs-lookup"><span data-stu-id="4d62e-103">iPv4CidrRange resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d62e-104">Представляет диапазон IPv4-адресов с использованием нотации CIDR.</span><span class="sxs-lookup"><span data-stu-id="4d62e-104">Represents an IPv4 range using the CIDR notation.</span></span>

<span data-ttu-id="4d62e-105">Наследуется от ресурса [ipRange](../resources/iprange.md)</span><span class="sxs-lookup"><span data-stu-id="4d62e-105">Inherits from [ipRange](../resources/iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4d62e-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="4d62e-106">Properties</span></span>

| <span data-ttu-id="4d62e-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="4d62e-107">Property</span></span>     | <span data-ttu-id="4d62e-108">Тип</span><span class="sxs-lookup"><span data-stu-id="4d62e-108">Type</span></span>        | <span data-ttu-id="4d62e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4d62e-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4d62e-110">Цидраддресс</span><span class="sxs-lookup"><span data-stu-id="4d62e-110">cidrAddress</span></span>|<span data-ttu-id="4d62e-111">String</span><span class="sxs-lookup"><span data-stu-id="4d62e-111">String</span></span>|<span data-ttu-id="4d62e-112">IPv4-адрес в нотации CIDR</span><span class="sxs-lookup"><span data-stu-id="4d62e-112">IPv4 address in CIDR notation</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4d62e-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4d62e-113">JSON representation</span></span>

<span data-ttu-id="4d62e-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4d62e-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.iPv4CidrRange",
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
  "description": "iPv4CidrRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->