---
title: 'объект поиска: запрос'
description: Выполняет запрос, указанный в теле запроса. Результаты поиска предоставляются в ответе.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 688fb39ef0c4170feb5e134e439e6b1c538ecbc6
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053484"
---
# <a name="searchentity-query"></a><span data-ttu-id="8c3fd-104">объект поиска: запрос</span><span class="sxs-lookup"><span data-stu-id="8c3fd-104">searchEntity: query</span></span>

<span data-ttu-id="8c3fd-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c3fd-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c3fd-106">Выполняет запрос, указанный в теле запроса.</span><span class="sxs-lookup"><span data-stu-id="8c3fd-106">Runs the query specified in the request body.</span></span> <span data-ttu-id="8c3fd-107">Результаты поиска предоставляются в ответе.</span><span class="sxs-lookup"><span data-stu-id="8c3fd-107">Search results are provided in the response.</span></span>

[!INCLUDE [search-api-deprecation](../../includes/search-api-deprecation.md)]

## <a name="permissions"></a><span data-ttu-id="8c3fd-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8c3fd-108">Permissions</span></span>

<span data-ttu-id="8c3fd-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c3fd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span> 

| <span data-ttu-id="8c3fd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c3fd-111">Permission type</span></span>                        | <span data-ttu-id="8c3fd-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8c3fd-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8c3fd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c3fd-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="8c3fd-114">Mail.Read, Calendars.Read, Files.Read.All, Sites.Read.All, ExternalItem.Read.All</span><span class="sxs-lookup"><span data-stu-id="8c3fd-114">Mail.Read, Calendars.Read, Files.Read.All, Sites.Read.All, ExternalItem.Read.All</span></span> |
| <span data-ttu-id="8c3fd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c3fd-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c3fd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c3fd-116">Not supported.</span></span> |
| <span data-ttu-id="8c3fd-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8c3fd-117">Application</span></span>                            | <span data-ttu-id="8c3fd-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c3fd-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c3fd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8c3fd-119">HTTP request</span></span>

```HTTP
POST /search/query
```

## <a name="request-headers"></a><span data-ttu-id="8c3fd-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8c3fd-120">Request headers</span></span>

| <span data-ttu-id="8c3fd-121">Имя</span><span class="sxs-lookup"><span data-stu-id="8c3fd-121">Name</span></span>          | <span data-ttu-id="8c3fd-122">Описание</span><span class="sxs-lookup"><span data-stu-id="8c3fd-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8c3fd-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8c3fd-123">Authorization</span></span> | <span data-ttu-id="8c3fd-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8c3fd-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8c3fd-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8c3fd-126">Content-type</span></span> | <span data-ttu-id="8c3fd-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8c3fd-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8c3fd-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8c3fd-129">Request body</span></span>

<span data-ttu-id="8c3fd-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="8c3fd-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8c3fd-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="8c3fd-131">Parameter</span></span>    | <span data-ttu-id="8c3fd-132">Тип</span><span class="sxs-lookup"><span data-stu-id="8c3fd-132">Type</span></span>        | <span data-ttu-id="8c3fd-133">Описание</span><span class="sxs-lookup"><span data-stu-id="8c3fd-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8c3fd-134">запросы</span><span class="sxs-lookup"><span data-stu-id="8c3fd-134">requests</span></span>|<span data-ttu-id="8c3fd-135">[коллекция searchRequest](../resources/searchrequest.md)</span><span class="sxs-lookup"><span data-stu-id="8c3fd-135">[searchRequest](../resources/searchrequest.md) collection</span></span>|<span data-ttu-id="8c3fd-136">Коллекция из одного или более запросов поиска, каждый из которых отформатирован в BLOB JSON.</span><span class="sxs-lookup"><span data-stu-id="8c3fd-136">A collection of one or more search requests each formatted in a JSON blob.</span></span> <span data-ttu-id="8c3fd-137">Каждая blob JSON содержит типы ресурсов, ожидаемых в ответе, основные источники, параметры paging, запрашиваемого поля и фактический запрос поиска.</span><span class="sxs-lookup"><span data-stu-id="8c3fd-137">Each JSON blob contains the types of resources expected in the response, the underlying sources, paging parameters, requested fields, and actual search query.</span></span> <br> <span data-ttu-id="8c3fd-138">Будьте в курсе [известных ограничений](../resources/search-api-overview.md#known-limitations) на поиск определенных комбинаций типов сущностей, а также сортировку или агрегирование результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="8c3fd-138">Be aware of [known limitations](../resources/search-api-overview.md#known-limitations) on searching specific combinations of entity types, and sorting or aggregating search results.</span></span> |

## <a name="response"></a><span data-ttu-id="8c3fd-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c3fd-139">Response</span></span>

<span data-ttu-id="8c3fd-140">В случае успешной работы этот метод возвращает код отклика и объект `HTTP 200 OK` [коллекции searchResponse](../resources/searchresponse.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="8c3fd-140">If successful, this method returns `HTTP 200 OK` response code and a [searchResponse](../resources/searchresponse.md) collection object in the response body.</span></span>
 

## <a name="examples"></a><span data-ttu-id="8c3fd-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="8c3fd-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8c3fd-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="8c3fd-142">Request</span></span>

<span data-ttu-id="8c3fd-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8c3fd-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8c3fd-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="8c3fd-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "search_query"
}-->

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-type: application/json

{
  "requests": [
    {
      "entityTypes": [
        "externalItem"
      ],
      "contentSources": [
        "/external/connections/connectionfriendlyname"
      ],
      "query": {
        "queryString": "contoso product"
      },
      "from": 0,
      "size": 25,
      "fields": [
        "title",
        "description"
      ]
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="8c3fd-145">C#</span><span class="sxs-lookup"><span data-stu-id="8c3fd-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/search-query-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8c3fd-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8c3fd-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/search-query-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8c3fd-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8c3fd-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/search-query-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8c3fd-148">Java</span><span class="sxs-lookup"><span data-stu-id="8c3fd-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/search-query-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8c3fd-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c3fd-149">Response</span></span>

<span data-ttu-id="8c3fd-150">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8c3fd-150">The following is an example of the response.</span></span>

> <span data-ttu-id="8c3fd-151">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8c3fd-151">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.searchResponse",
  "isCollection": true
} -->

```HTTP
HTTP/1.1 200 OK
Content-type: application/json
```

```json
{
  "value": [
    {
      "searchTerms": [
        "searchTerms-value"
      ],
      "hitsContainers": [
        {
          "hits": [
            {
              "hitId": "1",
              "rank": 1,
              "summary": "_summary-value",
              "resource": "The source field will contain the underlying graph entity part of the response"
            }
          ],
          "total": 47,
          "moreResultsAvailable": true
        }
      ]
    }
  ]
}
```

## <a name="see-also"></a><span data-ttu-id="8c3fd-152">См. также</span><span class="sxs-lookup"><span data-stu-id="8c3fd-152">See also</span></span>
- <span data-ttu-id="8c3fd-153">Поиск [сообщений почты](/graph/search-concept-messages)</span><span class="sxs-lookup"><span data-stu-id="8c3fd-153">Search [mail messages](/graph/search-concept-messages)</span></span>
- <span data-ttu-id="8c3fd-154">События [календаря поиска](/graph/search-concept-events)</span><span class="sxs-lookup"><span data-stu-id="8c3fd-154">Search [calendar events](/graph/search-concept-events)</span></span>
- <span data-ttu-id="8c3fd-155">Поиск контента в SharePoint и OneDrive[(файлы, списки и сайты)](/graph/search-concept-files)</span><span class="sxs-lookup"><span data-stu-id="8c3fd-155">Search content in SharePoint and OneDrive ([files, lists and sites](/graph/search-concept-files))</span></span>
- <span data-ttu-id="8c3fd-156">Пользовательские [типы поиска (Graph соединители)](/graph/search-concept-custom-types) данных</span><span class="sxs-lookup"><span data-stu-id="8c3fd-156">Search [custom types (Graph Connectors)](/graph/search-concept-custom-types) data</span></span>
- <span data-ttu-id="8c3fd-157">[Сортировка](/graph/search-concept-sort) результатов поиска</span><span class="sxs-lookup"><span data-stu-id="8c3fd-157">[Sort](/graph/search-concept-sort) search results</span></span>
- <span data-ttu-id="8c3fd-158">Использование [агрегаций для](/graph/search-concept-aggregations) уточнения результатов поиска</span><span class="sxs-lookup"><span data-stu-id="8c3fd-158">Use [aggregations](/graph/search-concept-aggregations) to refine search results</span></span>


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "search: query",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


