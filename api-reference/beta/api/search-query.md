---
title: 'Сеарчентити: запрос'
description: Выполняет запрос, указанный в теле запроса. Результаты поиска предоставляются в ответе.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: c699dab1c97d5b7650f42d4282e36d35b2769a31
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48401809"
---
# <a name="searchentity-query"></a><span data-ttu-id="ac0af-104">Сеарчентити: запрос</span><span class="sxs-lookup"><span data-stu-id="ac0af-104">searchEntity: query</span></span>

<span data-ttu-id="ac0af-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac0af-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac0af-106">Выполняет запрос, указанный в теле запроса.</span><span class="sxs-lookup"><span data-stu-id="ac0af-106">Runs the query specified in the request body.</span></span> <span data-ttu-id="ac0af-107">Результаты поиска предоставляются в ответе.</span><span class="sxs-lookup"><span data-stu-id="ac0af-107">Search results are provided in the response.</span></span>

[!INCLUDE [search-api-deprecation](../../includes/search-api-deprecation.md)]

## <a name="permissions"></a><span data-ttu-id="ac0af-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ac0af-108">Permissions</span></span>

<span data-ttu-id="ac0af-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac0af-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span> 

| <span data-ttu-id="ac0af-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ac0af-111">Permission type</span></span>                        | <span data-ttu-id="ac0af-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ac0af-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ac0af-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ac0af-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="ac0af-114">Mail. Read, mail. ReadWrite, Calendars. Read, Calendars. ReadWrite, Files. Read. ALL, Files. ReadWrite. ALL, sites. Read. ALL, sites. ReadWrite. ALL, Екстерналитем. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="ac0af-114">Mail.Read, Mail.ReadWrite, Calendars.Read, Calendars.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All, ExternalItem.Read.All</span></span> |
| <span data-ttu-id="ac0af-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ac0af-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac0af-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ac0af-116">Not supported.</span></span> |
| <span data-ttu-id="ac0af-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ac0af-117">Application</span></span>                            | <span data-ttu-id="ac0af-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ac0af-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ac0af-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ac0af-119">HTTP request</span></span>

```HTTP
POST /search/query
```

## <a name="request-headers"></a><span data-ttu-id="ac0af-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ac0af-120">Request headers</span></span>

| <span data-ttu-id="ac0af-121">Имя</span><span class="sxs-lookup"><span data-stu-id="ac0af-121">Name</span></span>          | <span data-ttu-id="ac0af-122">Описание</span><span class="sxs-lookup"><span data-stu-id="ac0af-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ac0af-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ac0af-123">Authorization</span></span> | <span data-ttu-id="ac0af-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ac0af-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ac0af-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ac0af-126">Content-type</span></span> | <span data-ttu-id="ac0af-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ac0af-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ac0af-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ac0af-129">Request body</span></span>

<span data-ttu-id="ac0af-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="ac0af-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ac0af-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="ac0af-131">Parameter</span></span>    | <span data-ttu-id="ac0af-132">Тип</span><span class="sxs-lookup"><span data-stu-id="ac0af-132">Type</span></span>        | <span data-ttu-id="ac0af-133">Описание</span><span class="sxs-lookup"><span data-stu-id="ac0af-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ac0af-134">обращения</span><span class="sxs-lookup"><span data-stu-id="ac0af-134">requests</span></span>|<span data-ttu-id="ac0af-135">Коллекция [сеарчрекуест](../resources/searchrequest.md)</span><span class="sxs-lookup"><span data-stu-id="ac0af-135">[searchRequest](../resources/searchrequest.md) collection</span></span>|<span data-ttu-id="ac0af-136">Коллекция из одного или нескольких запросов на поиск, отформатированных в большом двоичном объекте JSON.</span><span class="sxs-lookup"><span data-stu-id="ac0af-136">A collection of one or more search requests each formatted in a JSON blob.</span></span> <span data-ttu-id="ac0af-137">Каждый большой двоичный объект JSON содержит типы ресурсов, ожидаемых в ответе, базовые источники, параметры разбиения по страницам, запрашиваемые поля и фактический поисковый запрос.</span><span class="sxs-lookup"><span data-stu-id="ac0af-137">Each JSON blob contains the types of resources expected in the response, the underlying sources, paging parameters, requested fields, and actual search query.</span></span> <br> <span data-ttu-id="ac0af-138">Помните об [известных ограничениях](../resources/search-api-overview.md#known-limitations) на поиск определенных комбинаций типов сущностей, сортировку или статистическую обработку результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="ac0af-138">Be aware of [known limitations](../resources/search-api-overview.md#known-limitations) on searching specific combinations of entity types, and sorting or aggregating search results.</span></span> |

## <a name="response"></a><span data-ttu-id="ac0af-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac0af-139">Response</span></span>

<span data-ttu-id="ac0af-140">В случае успешного выполнения этот метод возвращает `HTTP 200 OK` код отклика и объект коллекции [сеарчреспонсе](../resources/searchresponse.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ac0af-140">If successful, this method returns `HTTP 200 OK` response code and a [searchResponse](../resources/searchresponse.md) collection object in the response body.</span></span>
 

## <a name="examples"></a><span data-ttu-id="ac0af-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="ac0af-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ac0af-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="ac0af-142">Request</span></span>

<span data-ttu-id="ac0af-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ac0af-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ac0af-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="ac0af-144">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="ac0af-145">C#</span><span class="sxs-lookup"><span data-stu-id="ac0af-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/search-query-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ac0af-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ac0af-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/search-query-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ac0af-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ac0af-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/search-query-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ac0af-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac0af-148">Response</span></span>

<span data-ttu-id="ac0af-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ac0af-149">The following is an example of the response.</span></span>

> <span data-ttu-id="ac0af-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ac0af-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="ac0af-152">См. также</span><span class="sxs-lookup"><span data-stu-id="ac0af-152">See also</span></span>
- <span data-ttu-id="ac0af-153">Поиск в [сообщениях электронной почты](/graph/search-concept-messages)</span><span class="sxs-lookup"><span data-stu-id="ac0af-153">Search [mail messages](/graph/search-concept-messages)</span></span>
- <span data-ttu-id="ac0af-154">Поиск [событий календаря](/graph/search-concept-events)</span><span class="sxs-lookup"><span data-stu-id="ac0af-154">Search [calendar events](/graph/search-concept-events)</span></span>
- <span data-ttu-id="ac0af-155">Поиск контента в SharePoint и OneDrive ([файлы, списки и сайты](/graph/search-concept-files))</span><span class="sxs-lookup"><span data-stu-id="ac0af-155">Search content in SharePoint and OneDrive ([files, lists and sites](/graph/search-concept-files))</span></span>
- <span data-ttu-id="ac0af-156">Данные о [настраиваемых типах поиска (соединители Graph)](/graph/search-concept-custom-types)</span><span class="sxs-lookup"><span data-stu-id="ac0af-156">Search [custom types (Graph Connectors)](/graph/search-concept-custom-types) data</span></span>
- <span data-ttu-id="ac0af-157">[Сортировка](/graph/search-concept-sort) результатов поиска</span><span class="sxs-lookup"><span data-stu-id="ac0af-157">[Sort](/graph/search-concept-sort) search results</span></span>
- <span data-ttu-id="ac0af-158">Использование [агрегатов](/graph/search-concept-aggregations) для уточнения результатов поиска</span><span class="sxs-lookup"><span data-stu-id="ac0af-158">Use [aggregations](/graph/search-concept-aggregations) to refine search results</span></span>


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "search: query",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


