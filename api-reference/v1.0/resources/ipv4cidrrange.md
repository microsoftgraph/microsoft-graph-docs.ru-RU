---
title: Тип ресурса iPv4CidrRange
description: Представляет диапазон IPv4-адресов с использованием нотации CIDR.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1b4276d038fd6c59460ed906ad30dcad925a3631
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48041283"
---
# <a name="ipv4cidrrange-resource-type"></a><span data-ttu-id="14035-103">Тип ресурса iPv4CidrRange</span><span class="sxs-lookup"><span data-stu-id="14035-103">iPv4CidrRange resource type</span></span>

<span data-ttu-id="14035-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14035-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="14035-105">Представляет диапазон IPv4-адресов с использованием нотации CIDR.</span><span class="sxs-lookup"><span data-stu-id="14035-105">Represents an IPv4 range using the CIDR notation.</span></span>

<span data-ttu-id="14035-106">Наследуется от ресурса [ipRange](../resources/iprange.md)</span><span class="sxs-lookup"><span data-stu-id="14035-106">Inherits from [ipRange](../resources/iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="14035-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="14035-107">Properties</span></span>

| <span data-ttu-id="14035-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="14035-108">Property</span></span>     | <span data-ttu-id="14035-109">Тип</span><span class="sxs-lookup"><span data-stu-id="14035-109">Type</span></span>        | <span data-ttu-id="14035-110">Описание</span><span class="sxs-lookup"><span data-stu-id="14035-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="14035-111">Цидраддресс</span><span class="sxs-lookup"><span data-stu-id="14035-111">cidrAddress</span></span>|<span data-ttu-id="14035-112">String</span><span class="sxs-lookup"><span data-stu-id="14035-112">String</span></span>|<span data-ttu-id="14035-113">IPv4-адрес в нотации CIDR</span><span class="sxs-lookup"><span data-stu-id="14035-113">IPv4 address in CIDR notation</span></span>|

## <a name="json-representation"></a><span data-ttu-id="14035-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="14035-114">JSON representation</span></span>

<span data-ttu-id="14035-115">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="14035-115">The following is a JSON representation of the resource.</span></span>

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
