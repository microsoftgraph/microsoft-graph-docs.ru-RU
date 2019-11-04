---
title: Поиск
description: Получение поискового ресурса, используемого для выполнения запросов
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 65a099ea0ae57b116bcf6a251170e507945226c9
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938774"
---
# <a name="search-resource-type"></a><span data-ttu-id="e6252-103">Тип ресурса поиска</span><span class="sxs-lookup"><span data-stu-id="e6252-103">search resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6252-104">Ресурс поиска — это объект верхнего уровня, представляющий конечную точку поиска.</span><span class="sxs-lookup"><span data-stu-id="e6252-104">The search resource is the top level object representing the search endpoint.</span></span> <span data-ttu-id="e6252-105">Он выступает в качестве привязки к действию [запроса](../api/search-query.md) .</span><span class="sxs-lookup"><span data-stu-id="e6252-105">It serves as an anchor to the [query](../api/search-query.md) action.</span></span>

<span data-ttu-id="e6252-106">Этот ресурс не должен вызываться таким образом.</span><span class="sxs-lookup"><span data-stu-id="e6252-106">This resource is not expected to be called as such.</span></span> <span data-ttu-id="e6252-107">Любой запрос к ресурсу повлечет некорректный запрос.</span><span class="sxs-lookup"><span data-stu-id="e6252-107">Any request on the resource will incur a Bad Request.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e6252-108">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e6252-108">JSON representation</span></span>

<span data-ttu-id="e6252-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="e6252-109">None</span></span>

## <a name="properties"></a><span data-ttu-id="e6252-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="e6252-110">Properties</span></span>

<span data-ttu-id="e6252-111">Нет</span><span class="sxs-lookup"><span data-stu-id="e6252-111">None</span></span>

## <a name="relationships"></a><span data-ttu-id="e6252-112">Связи</span><span class="sxs-lookup"><span data-stu-id="e6252-112">Relationships</span></span>

<span data-ttu-id="e6252-113">Нет</span><span class="sxs-lookup"><span data-stu-id="e6252-113">None</span></span>

## <a name="methods"></a><span data-ttu-id="e6252-114">Методы</span><span class="sxs-lookup"><span data-stu-id="e6252-114">Methods</span></span>

| <span data-ttu-id="e6252-115">Метод</span><span class="sxs-lookup"><span data-stu-id="e6252-115">Method</span></span>       | <span data-ttu-id="e6252-116">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e6252-116">Return Type</span></span> | <span data-ttu-id="e6252-117">Описание</span><span class="sxs-lookup"><span data-stu-id="e6252-117">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e6252-118">подчинен</span><span class="sxs-lookup"><span data-stu-id="e6252-118">query</span></span>](../api/search-query.md) | <span data-ttu-id="e6252-119">[сеарчреспонсе](searchresponse.md) Семейства</span><span class="sxs-lookup"><span data-stu-id="e6252-119">[searchResponse](searchresponse.md) Collection</span></span>| <span data-ttu-id="e6252-120">Выполняет запрос, указанный в элементе [сеарчрекуест](../resources/searchrequest.md)</span><span class="sxs-lookup"><span data-stu-id="e6252-120">Executes the query specified in the [searchRequest](../resources/searchrequest.md)</span></span> |

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get search",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
