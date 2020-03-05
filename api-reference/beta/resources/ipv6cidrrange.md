---
title: Тип ресурса iPv6CidrRange
description: Представляет диапазон IPv6-адресов с использованием нотации CIDR.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1b27b94762eeaa1c93d269ffaddf6e0ba1bc55d2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523144"
---
# <a name="ipv6cidrrange-resource-type"></a><span data-ttu-id="bbd2b-103">Тип ресурса iPv6CidrRange</span><span class="sxs-lookup"><span data-stu-id="bbd2b-103">iPv6CidrRange resource type</span></span>

<span data-ttu-id="bbd2b-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="bbd2b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bbd2b-105">Представляет диапазон IPv6-адресов с использованием нотации CIDR.</span><span class="sxs-lookup"><span data-stu-id="bbd2b-105">Represents an IPv6 range using the CIDR notation.</span></span>

<span data-ttu-id="bbd2b-106">Наследуется от ресурса [ipRange](../resources/iprange.md)</span><span class="sxs-lookup"><span data-stu-id="bbd2b-106">Inherits from [ipRange](../resources/iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bbd2b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="bbd2b-107">Properties</span></span>

| <span data-ttu-id="bbd2b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="bbd2b-108">Property</span></span>     | <span data-ttu-id="bbd2b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="bbd2b-109">Type</span></span>        | <span data-ttu-id="bbd2b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bbd2b-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bbd2b-111">Цидраддресс</span><span class="sxs-lookup"><span data-stu-id="bbd2b-111">cidrAddress</span></span>|<span data-ttu-id="bbd2b-112">String</span><span class="sxs-lookup"><span data-stu-id="bbd2b-112">String</span></span>|<span data-ttu-id="bbd2b-113">IPv6-адрес в нотации CIDR</span><span class="sxs-lookup"><span data-stu-id="bbd2b-113">IPv6 address in CIDR notation</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bbd2b-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bbd2b-114">JSON representation</span></span>

<span data-ttu-id="bbd2b-115">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bbd2b-115">The following is a JSON representation of the resource.</span></span>

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