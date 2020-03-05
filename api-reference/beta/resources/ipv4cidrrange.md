---
title: Тип ресурса iPv4CidrRange
description: Представляет диапазон IPv4-адресов с использованием нотации CIDR.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a6aa9202310ac2c0edcb70bac07fd49f5de668c8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523151"
---
# <a name="ipv4cidrrange-resource-type"></a><span data-ttu-id="0324f-103">Тип ресурса iPv4CidrRange</span><span class="sxs-lookup"><span data-stu-id="0324f-103">iPv4CidrRange resource type</span></span>

<span data-ttu-id="0324f-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0324f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0324f-105">Представляет диапазон IPv4-адресов с использованием нотации CIDR.</span><span class="sxs-lookup"><span data-stu-id="0324f-105">Represents an IPv4 range using the CIDR notation.</span></span>

<span data-ttu-id="0324f-106">Наследуется от ресурса [ipRange](../resources/iprange.md)</span><span class="sxs-lookup"><span data-stu-id="0324f-106">Inherits from [ipRange](../resources/iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0324f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="0324f-107">Properties</span></span>

| <span data-ttu-id="0324f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="0324f-108">Property</span></span>     | <span data-ttu-id="0324f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="0324f-109">Type</span></span>        | <span data-ttu-id="0324f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0324f-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0324f-111">Цидраддресс</span><span class="sxs-lookup"><span data-stu-id="0324f-111">cidrAddress</span></span>|<span data-ttu-id="0324f-112">String</span><span class="sxs-lookup"><span data-stu-id="0324f-112">String</span></span>|<span data-ttu-id="0324f-113">IPv4-адрес в нотации CIDR</span><span class="sxs-lookup"><span data-stu-id="0324f-113">IPv4 address in CIDR notation</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0324f-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0324f-114">JSON representation</span></span>

<span data-ttu-id="0324f-115">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0324f-115">The following is a JSON representation of the resource.</span></span>

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