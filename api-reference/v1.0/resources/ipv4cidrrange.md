---
title: тип ресурса iPv4CidrRange
description: Представляет диапазон IPv4 с помощью нотации CIDR.
localization_priority: Normal
author: videor
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 0b1af8d424d3e8dfc6f1791fa83a633e571310e6
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760871"
---
# <a name="ipv4cidrrange-resource-type"></a><span data-ttu-id="3b4b6-103">тип ресурса iPv4CidrRange</span><span class="sxs-lookup"><span data-stu-id="3b4b6-103">iPv4CidrRange resource type</span></span>

<span data-ttu-id="3b4b6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b4b6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3b4b6-105">Представляет диапазон IPv4 с помощью нотации CIDR.</span><span class="sxs-lookup"><span data-stu-id="3b4b6-105">Represents an IPv4 range using the CIDR notation.</span></span>

<span data-ttu-id="3b4b6-106">Наследуется от ресурса [ipRange](../resources/iprange.md)</span><span class="sxs-lookup"><span data-stu-id="3b4b6-106">Inherits from [ipRange](../resources/iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3b4b6-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="3b4b6-107">Properties</span></span>

| <span data-ttu-id="3b4b6-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="3b4b6-108">Property</span></span>     | <span data-ttu-id="3b4b6-109">Тип</span><span class="sxs-lookup"><span data-stu-id="3b4b6-109">Type</span></span>        | <span data-ttu-id="3b4b6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3b4b6-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3b4b6-111">cidrAddress</span><span class="sxs-lookup"><span data-stu-id="3b4b6-111">cidrAddress</span></span>|<span data-ttu-id="3b4b6-112">String</span><span class="sxs-lookup"><span data-stu-id="3b4b6-112">String</span></span>|<span data-ttu-id="3b4b6-113">Адрес IPv4 в нотации CIDR</span><span class="sxs-lookup"><span data-stu-id="3b4b6-113">IPv4 address in CIDR notation</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3b4b6-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3b4b6-114">JSON representation</span></span>

<span data-ttu-id="3b4b6-115">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3b4b6-115">The following is a JSON representation of the resource.</span></span>

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
