---
title: Поиск
description: Получение поискового ресурса, используемого для выполнения запросов
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: bb38d281895ac11d97a026a4352f68b93e8ba801
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/19/2019
ms.locfileid: "38704064"
---
# <a name="search-resource-type"></a><span data-ttu-id="a8f97-103">Тип ресурса поиска</span><span class="sxs-lookup"><span data-stu-id="a8f97-103">search resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8f97-104">Ресурс поиска — это объект верхнего уровня, представляющий конечную точку поиска.</span><span class="sxs-lookup"><span data-stu-id="a8f97-104">The search resource is the top level object representing the search endpoint.</span></span> <span data-ttu-id="a8f97-105">Он выступает в качестве привязки к действию [запроса](../api/search-query.md) .</span><span class="sxs-lookup"><span data-stu-id="a8f97-105">It serves as an anchor to the [query](../api/search-query.md) action.</span></span>

<span data-ttu-id="a8f97-106">Этот ресурс не должен вызываться таким образом.</span><span class="sxs-lookup"><span data-stu-id="a8f97-106">This resource is not expected to be called as such.</span></span> <span data-ttu-id="a8f97-107">Любой запрос к ресурсу повлечет некорректный запрос.</span><span class="sxs-lookup"><span data-stu-id="a8f97-107">Any request on the resource will incur a Bad Request.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="json-representation"></a><span data-ttu-id="a8f97-108">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a8f97-108">JSON representation</span></span>

<span data-ttu-id="a8f97-109">Нет</span><span class="sxs-lookup"><span data-stu-id="a8f97-109">None</span></span>

## <a name="properties"></a><span data-ttu-id="a8f97-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="a8f97-110">Properties</span></span>

<span data-ttu-id="a8f97-111">Нет</span><span class="sxs-lookup"><span data-stu-id="a8f97-111">None</span></span>

## <a name="relationships"></a><span data-ttu-id="a8f97-112">Связи</span><span class="sxs-lookup"><span data-stu-id="a8f97-112">Relationships</span></span>

<span data-ttu-id="a8f97-113">Нет</span><span class="sxs-lookup"><span data-stu-id="a8f97-113">None</span></span>

## <a name="methods"></a><span data-ttu-id="a8f97-114">Методы</span><span class="sxs-lookup"><span data-stu-id="a8f97-114">Methods</span></span>

| <span data-ttu-id="a8f97-115">Метод</span><span class="sxs-lookup"><span data-stu-id="a8f97-115">Method</span></span>       | <span data-ttu-id="a8f97-116">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a8f97-116">Return Type</span></span> | <span data-ttu-id="a8f97-117">Описание</span><span class="sxs-lookup"><span data-stu-id="a8f97-117">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="a8f97-118">query</span><span class="sxs-lookup"><span data-stu-id="a8f97-118">query</span></span>](../api/search-query.md) | <span data-ttu-id="a8f97-119">[сеарчреспонсе](searchresponse.md) Семейства</span><span class="sxs-lookup"><span data-stu-id="a8f97-119">[searchResponse](searchresponse.md) Collection</span></span>| <span data-ttu-id="a8f97-120">Выполняет запрос, указанный в элементе [сеарчрекуест](../resources/searchrequest.md)</span><span class="sxs-lookup"><span data-stu-id="a8f97-120">Executes the query specified in the [searchRequest](../resources/searchrequest.md)</span></span> |

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get search",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
