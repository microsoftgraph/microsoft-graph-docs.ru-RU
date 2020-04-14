---
title: Тип ресурса iPv6CidrRange
description: Представляет диапазон IPv6-адресов с использованием нотации CIDR.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 46c4742a65ec8826f363187eaaba05a1bfb8f893
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43384964"
---
# <a name="ipv6cidrrange-resource-type"></a><span data-ttu-id="0a597-103">Тип ресурса iPv6CidrRange</span><span class="sxs-lookup"><span data-stu-id="0a597-103">iPv6CidrRange resource type</span></span>

<span data-ttu-id="0a597-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a597-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a597-105">Представляет диапазон IPv6-адресов с использованием нотации CIDR.</span><span class="sxs-lookup"><span data-stu-id="0a597-105">Represents an IPv6 range using the CIDR notation.</span></span>

<span data-ttu-id="0a597-106">Наследуется от ресурса [ipRange](../resources/iprange.md)</span><span class="sxs-lookup"><span data-stu-id="0a597-106">Inherits from [ipRange](../resources/iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0a597-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="0a597-107">Properties</span></span>

| <span data-ttu-id="0a597-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="0a597-108">Property</span></span>     | <span data-ttu-id="0a597-109">Тип</span><span class="sxs-lookup"><span data-stu-id="0a597-109">Type</span></span>        | <span data-ttu-id="0a597-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0a597-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0a597-111">Цидраддресс</span><span class="sxs-lookup"><span data-stu-id="0a597-111">cidrAddress</span></span>|<span data-ttu-id="0a597-112">String</span><span class="sxs-lookup"><span data-stu-id="0a597-112">String</span></span>|<span data-ttu-id="0a597-113">IPv6-адрес в нотации CIDR</span><span class="sxs-lookup"><span data-stu-id="0a597-113">IPv6 address in CIDR notation</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0a597-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0a597-114">JSON representation</span></span>

<span data-ttu-id="0a597-115">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0a597-115">The following is a JSON representation of the resource.</span></span>

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