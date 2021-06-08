---
title: 'объект поиска: запрос'
description: Выполняет запрос, указанный в теле запроса. Результаты поиска предоставляются в ответе.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 7f83ce0b5cf4565897245647a0e1f41e428b8e1d
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786764"
---
# <a name="searchentity-query"></a><span data-ttu-id="bbd32-104">объект поиска: запрос</span><span class="sxs-lookup"><span data-stu-id="bbd32-104">searchEntity: query</span></span>

<span data-ttu-id="bbd32-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bbd32-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bbd32-106">Выполняет запрос, указанный в теле запроса.</span><span class="sxs-lookup"><span data-stu-id="bbd32-106">Runs the query specified in the request body.</span></span> <span data-ttu-id="bbd32-107">Результаты поиска предоставляются в ответе.</span><span class="sxs-lookup"><span data-stu-id="bbd32-107">Search results are provided in the response.</span></span>

[!INCLUDE [search-api-deprecation](../../includes/search-api-deprecation.md)]

## <a name="permissions"></a><span data-ttu-id="bbd32-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bbd32-108">Permissions</span></span>

<span data-ttu-id="bbd32-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bbd32-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span> 

| <span data-ttu-id="bbd32-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bbd32-111">Permission type</span></span>                        | <span data-ttu-id="bbd32-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bbd32-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="bbd32-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bbd32-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="bbd32-114">Mail.Read, Calendars.Read, Files.Read.All, Sites.Read.All, ExternalItem.Read.All</span><span class="sxs-lookup"><span data-stu-id="bbd32-114">Mail.Read, Calendars.Read, Files.Read.All, Sites.Read.All, ExternalItem.Read.All</span></span> |
| <span data-ttu-id="bbd32-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bbd32-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bbd32-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bbd32-116">Not supported.</span></span> |
| <span data-ttu-id="bbd32-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bbd32-117">Application</span></span>                            | <span data-ttu-id="bbd32-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bbd32-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bbd32-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bbd32-119">HTTP request</span></span>

```HTTP
POST /search/query
```

## <a name="request-headers"></a><span data-ttu-id="bbd32-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bbd32-120">Request headers</span></span>

| <span data-ttu-id="bbd32-121">Имя</span><span class="sxs-lookup"><span data-stu-id="bbd32-121">Name</span></span>          | <span data-ttu-id="bbd32-122">Описание</span><span class="sxs-lookup"><span data-stu-id="bbd32-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="bbd32-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bbd32-123">Authorization</span></span> | <span data-ttu-id="bbd32-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bbd32-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bbd32-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bbd32-126">Content-type</span></span> | <span data-ttu-id="bbd32-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bbd32-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bbd32-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bbd32-129">Request body</span></span>

<span data-ttu-id="bbd32-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="bbd32-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="bbd32-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="bbd32-131">Parameter</span></span>    | <span data-ttu-id="bbd32-132">Тип</span><span class="sxs-lookup"><span data-stu-id="bbd32-132">Type</span></span>        | <span data-ttu-id="bbd32-133">Описание</span><span class="sxs-lookup"><span data-stu-id="bbd32-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bbd32-134">запросы</span><span class="sxs-lookup"><span data-stu-id="bbd32-134">requests</span></span>|<span data-ttu-id="bbd32-135">[коллекция searchRequest](../resources/searchrequest.md)</span><span class="sxs-lookup"><span data-stu-id="bbd32-135">[searchRequest](../resources/searchrequest.md) collection</span></span>|<span data-ttu-id="bbd32-136">Коллекция из одного или более запросов поиска, каждый из которых отформатирован в BLOB JSON.</span><span class="sxs-lookup"><span data-stu-id="bbd32-136">A collection of one or more search requests each formatted in a JSON blob.</span></span> <span data-ttu-id="bbd32-137">Каждая blob JSON содержит типы ресурсов, ожидаемых в ответе, основные источники, параметры paging, запрашиваемого поля и фактический запрос поиска.</span><span class="sxs-lookup"><span data-stu-id="bbd32-137">Each JSON blob contains the types of resources expected in the response, the underlying sources, paging parameters, requested fields, and actual search query.</span></span> <br> <span data-ttu-id="bbd32-138">Будьте в курсе [известных ограничений](../resources/search-api-overview.md#known-limitations) на поиск определенных комбинаций типов сущностей, а также сортировку или агрегирование результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="bbd32-138">Be aware of [known limitations](../resources/search-api-overview.md#known-limitations) on searching specific combinations of entity types, and sorting or aggregating search results.</span></span> |
|<span data-ttu-id="bbd32-139">queryAlterationOptions</span><span class="sxs-lookup"><span data-stu-id="bbd32-139">queryAlterationOptions</span></span>|[<span data-ttu-id="bbd32-140">searchAlterationOptions</span><span class="sxs-lookup"><span data-stu-id="bbd32-140">searchAlterationOptions</span></span>](../resources/searchalterationoptions.md)|<span data-ttu-id="bbd32-141">Параметры изменения запроса, отформатированные в blob JSON, который содержит два необязательных флага для коррекции орфографии.</span><span class="sxs-lookup"><span data-stu-id="bbd32-141">Query alteration options formatted in a JSON blob that contains two optional flags to for spelling correction.</span></span> <span data-ttu-id="bbd32-142">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="bbd32-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="bbd32-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="bbd32-143">Response</span></span>

<span data-ttu-id="bbd32-144">В случае успешной работы этот метод возвращает код отклика и `HTTP 200 OK` [объект searchResponse](../resources/searchresponse.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="bbd32-144">If successful, this method returns a `HTTP 200 OK` response code and a [searchResponse](../resources/searchresponse.md) object in the response body.</span></span>
 

## <a name="examples"></a><span data-ttu-id="bbd32-145">Примеры</span><span class="sxs-lookup"><span data-stu-id="bbd32-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bbd32-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="bbd32-146">Request</span></span>

<span data-ttu-id="bbd32-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bbd32-147">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bbd32-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="bbd32-148">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="bbd32-149">C#</span><span class="sxs-lookup"><span data-stu-id="bbd32-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/search-query-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bbd32-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bbd32-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/search-query-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bbd32-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bbd32-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/search-query-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bbd32-152">Java</span><span class="sxs-lookup"><span data-stu-id="bbd32-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/search-query-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bbd32-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="bbd32-153">Response</span></span>

<span data-ttu-id="bbd32-154">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="bbd32-154">The following is an example of the response.</span></span>

> <span data-ttu-id="bbd32-155">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="bbd32-155">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.searchResponse",
  "isCollection": true
} -->

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

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

## <a name="see-also"></a><span data-ttu-id="bbd32-156">Дополнительные материалы</span><span class="sxs-lookup"><span data-stu-id="bbd32-156">See also</span></span>
- <span data-ttu-id="bbd32-157">Поиск [сообщений почты](/graph/search-concept-messages)</span><span class="sxs-lookup"><span data-stu-id="bbd32-157">Search [mail messages](/graph/search-concept-messages)</span></span>
- <span data-ttu-id="bbd32-158">События [календаря поиска](/graph/search-concept-events)</span><span class="sxs-lookup"><span data-stu-id="bbd32-158">Search [calendar events](/graph/search-concept-events)</span></span>
- <span data-ttu-id="bbd32-159">Поиск контента в SharePoint и OneDrive[(файлы, списки и сайты)](/graph/search-concept-files)</span><span class="sxs-lookup"><span data-stu-id="bbd32-159">Search content in SharePoint and OneDrive ([files, lists and sites](/graph/search-concept-files))</span></span>
- <span data-ttu-id="bbd32-160">Пользовательские [типы поиска (Graph соединители)](/graph/search-concept-custom-types) данных</span><span class="sxs-lookup"><span data-stu-id="bbd32-160">Search [custom types (Graph Connectors)](/graph/search-concept-custom-types) data</span></span>
- <span data-ttu-id="bbd32-161">[Сортировка](/graph/search-concept-sort) результатов поиска</span><span class="sxs-lookup"><span data-stu-id="bbd32-161">[Sort](/graph/search-concept-sort) search results</span></span>
- <span data-ttu-id="bbd32-162">Использование [агрегаций для](/graph/search-concept-aggregations) уточнения результатов поиска</span><span class="sxs-lookup"><span data-stu-id="bbd32-162">Use [aggregations](/graph/search-concept-aggregations) to refine search results</span></span>
- <span data-ttu-id="bbd32-163">Включить [исправления орфографии](/graph/search-concept-speller) в результатах поиска</span><span class="sxs-lookup"><span data-stu-id="bbd32-163">Enable [spell corrections](/graph/search-concept-speller) in search results</span></span>


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "search: query",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


