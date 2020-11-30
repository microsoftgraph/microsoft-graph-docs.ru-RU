---
title: Поиск
description: Получение поискового ресурса, используемого для выполнения запросов
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 8e9d8bc133a050701543f2a978e56b662bafcc33
ms.sourcegitcommit: 5345c2f3265ede107fa0faaff7a3f1c2afee3810
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378041"
---
# <a name="search-resource-type"></a><span data-ttu-id="c0ad2-103">Тип ресурса поиска</span><span class="sxs-lookup"><span data-stu-id="c0ad2-103">search resource type</span></span>

<span data-ttu-id="c0ad2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0ad2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c0ad2-105">Ресурс поиска — это объект верхнего уровня, представляющий конечную точку поиска.</span><span class="sxs-lookup"><span data-stu-id="c0ad2-105">The search resource is the top level object representing the search endpoint.</span></span> <span data-ttu-id="c0ad2-106">Он выступает в качестве привязки к действию [запроса](../api/search-query.md) .</span><span class="sxs-lookup"><span data-stu-id="c0ad2-106">It serves as an anchor to the [query](../api/search-query.md) action.</span></span>

<span data-ttu-id="c0ad2-107">Этот ресурс не должен вызываться таким образом.</span><span class="sxs-lookup"><span data-stu-id="c0ad2-107">This resource is not expected to be called as such.</span></span> <span data-ttu-id="c0ad2-108">Любой запрос к ресурсу повлечет некорректный запрос.</span><span class="sxs-lookup"><span data-stu-id="c0ad2-108">Any request on the resource will incur a Bad Request.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="json-representation"></a><span data-ttu-id="c0ad2-109">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c0ad2-109">JSON representation</span></span>

<span data-ttu-id="c0ad2-110">Нет</span><span class="sxs-lookup"><span data-stu-id="c0ad2-110">None</span></span>

## <a name="properties"></a><span data-ttu-id="c0ad2-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="c0ad2-111">Properties</span></span>

<span data-ttu-id="c0ad2-112">Нет</span><span class="sxs-lookup"><span data-stu-id="c0ad2-112">None</span></span>

## <a name="relationships"></a><span data-ttu-id="c0ad2-113">Связи</span><span class="sxs-lookup"><span data-stu-id="c0ad2-113">Relationships</span></span>

<span data-ttu-id="c0ad2-114">Нет</span><span class="sxs-lookup"><span data-stu-id="c0ad2-114">None</span></span>

## <a name="methods"></a><span data-ttu-id="c0ad2-115">Методы</span><span class="sxs-lookup"><span data-stu-id="c0ad2-115">Methods</span></span>

| <span data-ttu-id="c0ad2-116">Метод</span><span class="sxs-lookup"><span data-stu-id="c0ad2-116">Method</span></span>       | <span data-ttu-id="c0ad2-117">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c0ad2-117">Return Type</span></span> | <span data-ttu-id="c0ad2-118">Описание</span><span class="sxs-lookup"><span data-stu-id="c0ad2-118">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="c0ad2-119">query</span><span class="sxs-lookup"><span data-stu-id="c0ad2-119">query</span></span>](../api/search-query.md) | <span data-ttu-id="c0ad2-120">[сеарчреспонсе](searchresponse.md) Семейства</span><span class="sxs-lookup"><span data-stu-id="c0ad2-120">[searchResponse](searchresponse.md) Collection</span></span>| <span data-ttu-id="c0ad2-121">Выполняет запрос, указанный в элементе [сеарчрекуест](../resources/searchrequest.md)</span><span class="sxs-lookup"><span data-stu-id="c0ad2-121">Executes the query specified in the [searchRequest](../resources/searchrequest.md)</span></span> |

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get search",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


