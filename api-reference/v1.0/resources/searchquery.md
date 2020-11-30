---
title: Тип ресурса searchQuery
description: searchQuery
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 3745083b404a8de6f68844af9b1767ac2319059f
ms.sourcegitcommit: 5345c2f3265ede107fa0faaff7a3f1c2afee3810
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378020"
---
# <a name="searchquery-resource-type"></a><span data-ttu-id="dd17a-103">Тип ресурса searchQuery</span><span class="sxs-lookup"><span data-stu-id="dd17a-103">searchQuery resource type</span></span>

<span data-ttu-id="dd17a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd17a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dd17a-105">Представляет поисковый запрос, содержащий поисковые термины и необязательные фильтры.</span><span class="sxs-lookup"><span data-stu-id="dd17a-105">Represents a search query that contains search terms and optional filters.</span></span>

## <a name="properties"></a><span data-ttu-id="dd17a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="dd17a-106">Properties</span></span>

| <span data-ttu-id="dd17a-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="dd17a-107">Property</span></span>     | <span data-ttu-id="dd17a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="dd17a-108">Type</span></span>        | <span data-ttu-id="dd17a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="dd17a-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="dd17a-110">queryString</span><span class="sxs-lookup"><span data-stu-id="dd17a-110">queryString</span></span>|<span data-ttu-id="dd17a-111">Строка</span><span class="sxs-lookup"><span data-stu-id="dd17a-111">String</span></span>|<span data-ttu-id="dd17a-112">Поисковый запрос, содержащий условия поиска.</span><span class="sxs-lookup"><span data-stu-id="dd17a-112">The search query containing the search terms.</span></span> <span data-ttu-id="dd17a-113">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="dd17a-113">Required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dd17a-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dd17a-114">JSON representation</span></span>

<span data-ttu-id="dd17a-115">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dd17a-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchQuery",
  "baseType": null
}-->

```json
{
  "queryString": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchQuery resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

