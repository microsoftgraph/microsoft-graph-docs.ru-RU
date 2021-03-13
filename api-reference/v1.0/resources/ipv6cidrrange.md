---
title: тип ресурса iPv6CidrRange
description: Представляет диапазон IPv6 с помощью нотации CIDR.
localization_priority: Normal
author: videor
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: a8afeeed483b3610c5c1dde1afee5f4a24317ff4
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760864"
---
# <a name="ipv6cidrrange-resource-type"></a><span data-ttu-id="aa2e1-103">тип ресурса iPv6CidrRange</span><span class="sxs-lookup"><span data-stu-id="aa2e1-103">iPv6CidrRange resource type</span></span>

<span data-ttu-id="aa2e1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa2e1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="aa2e1-105">Представляет диапазон IPv6 с помощью нотации CIDR.</span><span class="sxs-lookup"><span data-stu-id="aa2e1-105">Represents an IPv6 range using the CIDR notation.</span></span>

<span data-ttu-id="aa2e1-106">Наследуется от ресурса [ipRange](../resources/iprange.md)</span><span class="sxs-lookup"><span data-stu-id="aa2e1-106">Inherits from [ipRange](../resources/iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="aa2e1-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="aa2e1-107">Properties</span></span>

| <span data-ttu-id="aa2e1-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="aa2e1-108">Property</span></span>     | <span data-ttu-id="aa2e1-109">Тип</span><span class="sxs-lookup"><span data-stu-id="aa2e1-109">Type</span></span>        | <span data-ttu-id="aa2e1-110">Описание</span><span class="sxs-lookup"><span data-stu-id="aa2e1-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="aa2e1-111">cidrAddress</span><span class="sxs-lookup"><span data-stu-id="aa2e1-111">cidrAddress</span></span>|<span data-ttu-id="aa2e1-112">String</span><span class="sxs-lookup"><span data-stu-id="aa2e1-112">String</span></span>|<span data-ttu-id="aa2e1-113">Адрес IPv6 в нотации CIDR</span><span class="sxs-lookup"><span data-stu-id="aa2e1-113">IPv6 address in CIDR notation</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aa2e1-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aa2e1-114">JSON representation</span></span>

<span data-ttu-id="aa2e1-115">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aa2e1-115">The following is a JSON representation of the resource.</span></span>

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
