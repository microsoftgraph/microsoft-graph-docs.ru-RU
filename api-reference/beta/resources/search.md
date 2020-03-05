---
title: Поиск
description: Получение поискового ресурса, используемого для выполнения запросов
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 8cb963c0fda545ea88e8d8e4335954ffb455102f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520937"
---
# <a name="search-resource-type"></a><span data-ttu-id="54b56-103">Тип ресурса поиска</span><span class="sxs-lookup"><span data-stu-id="54b56-103">search resource type</span></span>

<span data-ttu-id="54b56-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="54b56-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54b56-105">Ресурс поиска — это объект верхнего уровня, представляющий конечную точку поиска.</span><span class="sxs-lookup"><span data-stu-id="54b56-105">The search resource is the top level object representing the search endpoint.</span></span> <span data-ttu-id="54b56-106">Он выступает в качестве привязки к действию [запроса](../api/search-query.md) .</span><span class="sxs-lookup"><span data-stu-id="54b56-106">It serves as an anchor to the [query](../api/search-query.md) action.</span></span>

<span data-ttu-id="54b56-107">Этот ресурс не должен вызываться таким образом.</span><span class="sxs-lookup"><span data-stu-id="54b56-107">This resource is not expected to be called as such.</span></span> <span data-ttu-id="54b56-108">Любой запрос к ресурсу повлечет некорректный запрос.</span><span class="sxs-lookup"><span data-stu-id="54b56-108">Any request on the resource will incur a Bad Request.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="json-representation"></a><span data-ttu-id="54b56-109">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="54b56-109">JSON representation</span></span>

<span data-ttu-id="54b56-110">Нет</span><span class="sxs-lookup"><span data-stu-id="54b56-110">None</span></span>

## <a name="properties"></a><span data-ttu-id="54b56-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="54b56-111">Properties</span></span>

<span data-ttu-id="54b56-112">Нет</span><span class="sxs-lookup"><span data-stu-id="54b56-112">None</span></span>

## <a name="relationships"></a><span data-ttu-id="54b56-113">Связи</span><span class="sxs-lookup"><span data-stu-id="54b56-113">Relationships</span></span>

<span data-ttu-id="54b56-114">Нет</span><span class="sxs-lookup"><span data-stu-id="54b56-114">None</span></span>

## <a name="methods"></a><span data-ttu-id="54b56-115">Методы</span><span class="sxs-lookup"><span data-stu-id="54b56-115">Methods</span></span>

| <span data-ttu-id="54b56-116">Метод</span><span class="sxs-lookup"><span data-stu-id="54b56-116">Method</span></span>       | <span data-ttu-id="54b56-117">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="54b56-117">Return Type</span></span> | <span data-ttu-id="54b56-118">Описание</span><span class="sxs-lookup"><span data-stu-id="54b56-118">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="54b56-119">query</span><span class="sxs-lookup"><span data-stu-id="54b56-119">query</span></span>](../api/search-query.md) | <span data-ttu-id="54b56-120">[сеарчреспонсе](searchresponse.md) Семейства</span><span class="sxs-lookup"><span data-stu-id="54b56-120">[searchResponse](searchresponse.md) Collection</span></span>| <span data-ttu-id="54b56-121">Выполняет запрос, указанный в элементе [сеарчрекуест](../resources/searchrequest.md)</span><span class="sxs-lookup"><span data-stu-id="54b56-121">Executes the query specified in the [searchRequest](../resources/searchrequest.md)</span></span> |

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get search",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
