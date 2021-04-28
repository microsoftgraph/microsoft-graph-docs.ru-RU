---
title: Поиск
description: Извлечение ресурса поиска, используемой для выполнения запросов
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 123d57b05950203434ac23fd85e9c29dfa41476d
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067098"
---
# <a name="search-resource-type"></a><span data-ttu-id="81ece-103">Тип ресурса поиска</span><span class="sxs-lookup"><span data-stu-id="81ece-103">search resource type</span></span>

<span data-ttu-id="81ece-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81ece-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81ece-105">Ресурс поиска — это объект верхнего уровня, представляющий конечную точку поиска.</span><span class="sxs-lookup"><span data-stu-id="81ece-105">The search resource is the top level object representing the search endpoint.</span></span> <span data-ttu-id="81ece-106">Он служит якорем для [действия запроса.](../api/search-query.md)</span><span class="sxs-lookup"><span data-stu-id="81ece-106">It serves as an anchor to the [query](../api/search-query.md) action.</span></span>

<span data-ttu-id="81ece-107">Этот ресурс не будет называться как таковой.</span><span class="sxs-lookup"><span data-stu-id="81ece-107">This resource is not expected to be called as such.</span></span> <span data-ttu-id="81ece-108">Любой запрос на ресурс будет понести bad request.</span><span class="sxs-lookup"><span data-stu-id="81ece-108">Any request on the resource will incur a Bad Request.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="json-representation"></a><span data-ttu-id="81ece-109">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="81ece-109">JSON representation</span></span>

<span data-ttu-id="81ece-110">Нет</span><span class="sxs-lookup"><span data-stu-id="81ece-110">None</span></span>

## <a name="properties"></a><span data-ttu-id="81ece-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="81ece-111">Properties</span></span>

<span data-ttu-id="81ece-112">Нет</span><span class="sxs-lookup"><span data-stu-id="81ece-112">None</span></span>

## <a name="relationships"></a><span data-ttu-id="81ece-113">Связи</span><span class="sxs-lookup"><span data-stu-id="81ece-113">Relationships</span></span>

<span data-ttu-id="81ece-114">Нет</span><span class="sxs-lookup"><span data-stu-id="81ece-114">None</span></span>

## <a name="methods"></a><span data-ttu-id="81ece-115">Методы</span><span class="sxs-lookup"><span data-stu-id="81ece-115">Methods</span></span>

| <span data-ttu-id="81ece-116">Метод</span><span class="sxs-lookup"><span data-stu-id="81ece-116">Method</span></span>       | <span data-ttu-id="81ece-117">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="81ece-117">Return Type</span></span> | <span data-ttu-id="81ece-118">Описание</span><span class="sxs-lookup"><span data-stu-id="81ece-118">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="81ece-119">query</span><span class="sxs-lookup"><span data-stu-id="81ece-119">query</span></span>](../api/search-query.md) | [<span data-ttu-id="81ece-120">searchResponse</span><span class="sxs-lookup"><span data-stu-id="81ece-120">searchResponse</span></span>](searchresponse.md)| <span data-ttu-id="81ece-121">Выполняет запрос, указанный в [searchRequest](../resources/searchrequest.md)</span><span class="sxs-lookup"><span data-stu-id="81ece-121">Executes the query specified in the [searchRequest](../resources/searchrequest.md)</span></span> |

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get search",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


