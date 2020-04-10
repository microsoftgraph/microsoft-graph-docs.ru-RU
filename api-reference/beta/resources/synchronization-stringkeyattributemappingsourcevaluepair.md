---
title: Тип ресурса Стрингкэйаттрибутемаппингсаурцевалуепаир
description: Представляет собой комбинацию "ключ-значение", в которой ключ является строкой, а значение — Аттрибутемаппингсаурце.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 88dd652e12a8ba7d5d866e2817685e0ad3a732eb
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217579"
---
# <a name="stringkeyattributemappingsourcevaluepair-resource-type"></a><span data-ttu-id="d1eb3-103">Тип ресурса Стрингкэйаттрибутемаппингсаурцевалуепаир</span><span class="sxs-lookup"><span data-stu-id="d1eb3-103">stringKeyAttributeMappingSourceValuePair resource type</span></span>

<span data-ttu-id="d1eb3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1eb3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1eb3-105">Представляет собой комбинацию "ключ-значение", в которой ключ является строкой, а значение — [аттрибутемаппингсаурце](synchronization-attributemappingsource.md).</span><span class="sxs-lookup"><span data-stu-id="d1eb3-105">Represents a key-value pair where the key is a string and the value is [attributeMappingSource](synchronization-attributemappingsource.md).</span></span>

## <a name="properties"></a><span data-ttu-id="d1eb3-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="d1eb3-106">Properties</span></span>
| <span data-ttu-id="d1eb3-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="d1eb3-107">Property</span></span>     | <span data-ttu-id="d1eb3-108">Тип</span><span class="sxs-lookup"><span data-stu-id="d1eb3-108">Type</span></span>   |<span data-ttu-id="d1eb3-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d1eb3-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d1eb3-110">key</span><span class="sxs-lookup"><span data-stu-id="d1eb3-110">key</span></span>|<span data-ttu-id="d1eb3-111">Строка</span><span class="sxs-lookup"><span data-stu-id="d1eb3-111">String</span></span>|<span data-ttu-id="d1eb3-112">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="d1eb3-112">The name of the parameter.</span></span>|
|<span data-ttu-id="d1eb3-113">значение</span><span class="sxs-lookup"><span data-stu-id="d1eb3-113">value</span></span>|[<span data-ttu-id="d1eb3-114">аттрибутемаппингсаурце</span><span class="sxs-lookup"><span data-stu-id="d1eb3-114">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)|<span data-ttu-id="d1eb3-115">Значение параметра.</span><span class="sxs-lookup"><span data-stu-id="d1eb3-115">The value of the parameter.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d1eb3-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d1eb3-116">JSON representation</span></span>

<span data-ttu-id="d1eb3-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d1eb3-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stringKeyAttributeMappingSourceValuePair"
}-->

```json
{
  "key": "String",
  "value": {"@odata.type": "microsoft.graph.attributeMappingSource"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "stringKeyAttributeMappingSourceValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
