---
title: Тип ресурса Сеарчкуеристринг
description: сеарчкуеристринг
localization_priority: Normal
author: nmoreau
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: b273d9ec15b949019b780dd5ce9f1a6184191763
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520908"
---
# <a name="searchquerystring-resource-type"></a><span data-ttu-id="1b708-103">Тип ресурса Сеарчкуеристринг</span><span class="sxs-lookup"><span data-stu-id="1b708-103">searchQueryString resource type</span></span>

<span data-ttu-id="1b708-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b708-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b708-105">Условия поиска для запроса.</span><span class="sxs-lookup"><span data-stu-id="1b708-105">The search terms for the query.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="1b708-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="1b708-106">Properties</span></span>

| <span data-ttu-id="1b708-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="1b708-107">Property</span></span>     | <span data-ttu-id="1b708-108">Тип</span><span class="sxs-lookup"><span data-stu-id="1b708-108">Type</span></span>        | <span data-ttu-id="1b708-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1b708-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1b708-110">Запрос</span><span class="sxs-lookup"><span data-stu-id="1b708-110">query</span></span>|<span data-ttu-id="1b708-111">String</span><span class="sxs-lookup"><span data-stu-id="1b708-111">String</span></span>|<span data-ttu-id="1b708-112">Содержит фактические условия поиска запроса.</span><span class="sxs-lookup"><span data-stu-id="1b708-112">Contains the actual search terms of the request.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1b708-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1b708-113">JSON representation</span></span>

<span data-ttu-id="1b708-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1b708-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchQueryString",
  "baseType": null
}-->

```json
{
  "query": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchQueryString resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->