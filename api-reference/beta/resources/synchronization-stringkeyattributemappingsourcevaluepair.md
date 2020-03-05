---
title: Тип ресурса Стрингкэйаттрибутемаппингсаурцевалуепаир
description: Представляет собой комбинацию "ключ-значение", в которой ключ является строкой, а значение — Аттрибутемаппингсаурце.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f28b58b5f6bdadf33412a125a841d1c614285557
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520109"
---
# <a name="stringkeyattributemappingsourcevaluepair-resource-type"></a><span data-ttu-id="59267-103">Тип ресурса Стрингкэйаттрибутемаппингсаурцевалуепаир</span><span class="sxs-lookup"><span data-stu-id="59267-103">stringKeyAttributeMappingSourceValuePair resource type</span></span>

<span data-ttu-id="59267-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="59267-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59267-105">Представляет собой комбинацию "ключ-значение", в которой ключ является строкой, а значение — [аттрибутемаппингсаурце](synchronization-attributemappingsource.md).</span><span class="sxs-lookup"><span data-stu-id="59267-105">Represents a key-value pair where the key is a string and the value is [attributeMappingSource](synchronization-attributemappingsource.md).</span></span>

## <a name="properties"></a><span data-ttu-id="59267-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="59267-106">Properties</span></span>
| <span data-ttu-id="59267-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="59267-107">Property</span></span>     | <span data-ttu-id="59267-108">Тип</span><span class="sxs-lookup"><span data-stu-id="59267-108">Type</span></span>   |<span data-ttu-id="59267-109">Описание</span><span class="sxs-lookup"><span data-stu-id="59267-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="59267-110">key</span><span class="sxs-lookup"><span data-stu-id="59267-110">key</span></span>|<span data-ttu-id="59267-111">String</span><span class="sxs-lookup"><span data-stu-id="59267-111">String</span></span>|<span data-ttu-id="59267-112">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="59267-112">The name of the parameter.</span></span>|
|<span data-ttu-id="59267-113">значение</span><span class="sxs-lookup"><span data-stu-id="59267-113">value</span></span>|[<span data-ttu-id="59267-114">аттрибутемаппингсаурце</span><span class="sxs-lookup"><span data-stu-id="59267-114">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)|<span data-ttu-id="59267-115">Значение параметра.</span><span class="sxs-lookup"><span data-stu-id="59267-115">The value of the parameter.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="59267-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="59267-116">JSON representation</span></span>

<span data-ttu-id="59267-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="59267-117">The following is a JSON representation of the resource.</span></span>

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
