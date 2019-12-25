---
title: 'Поиск: запрос'
description: Выполняет запрос, указанный в теле запроса. Результаты поиска предоставляются в ответе.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: ff5d67dc749ce60797ec6c6387d79795718409c5
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40868851"
---
# <a name="search-query"></a><span data-ttu-id="c8bbc-104">Поиск: запрос</span><span class="sxs-lookup"><span data-stu-id="c8bbc-104">search: query</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8bbc-105">Выполняет запрос, указанный в теле запроса.</span><span class="sxs-lookup"><span data-stu-id="c8bbc-105">Runs the query specified in the request body.</span></span> <span data-ttu-id="c8bbc-106">Результаты поиска предоставляются в ответе.</span><span class="sxs-lookup"><span data-stu-id="c8bbc-106">Search results are provided in the response.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="c8bbc-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c8bbc-107">Permissions</span></span>

<span data-ttu-id="c8bbc-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8bbc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c8bbc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c8bbc-110">Permission type</span></span>                        | <span data-ttu-id="c8bbc-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c8bbc-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c8bbc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c8bbc-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="c8bbc-113">Mail. Read, Files. Read. ALL, Calendars. Read, Екстерналитем. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="c8bbc-113">Mail.Read, Files.Read.All, Calendars.Read, ExternalItem.Read.All</span></span> |
| <span data-ttu-id="c8bbc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c8bbc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8bbc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8bbc-115">Not supported.</span></span> |
| <span data-ttu-id="c8bbc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c8bbc-116">Application</span></span>                            | <span data-ttu-id="c8bbc-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8bbc-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c8bbc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c8bbc-118">HTTP request</span></span>

```HTTP
POST /search/query
```

## <a name="request-headers"></a><span data-ttu-id="c8bbc-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c8bbc-119">Request headers</span></span>

| <span data-ttu-id="c8bbc-120">Имя</span><span class="sxs-lookup"><span data-stu-id="c8bbc-120">Name</span></span>          | <span data-ttu-id="c8bbc-121">Описание</span><span class="sxs-lookup"><span data-stu-id="c8bbc-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="c8bbc-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c8bbc-122">Authorization</span></span> | <span data-ttu-id="c8bbc-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c8bbc-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c8bbc-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c8bbc-125">Content-type</span></span> | <span data-ttu-id="c8bbc-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c8bbc-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c8bbc-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c8bbc-128">Request body</span></span>

<span data-ttu-id="c8bbc-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="c8bbc-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c8bbc-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="c8bbc-130">Parameter</span></span>    | <span data-ttu-id="c8bbc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c8bbc-131">Type</span></span>        | <span data-ttu-id="c8bbc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c8bbc-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c8bbc-133">обращения</span><span class="sxs-lookup"><span data-stu-id="c8bbc-133">requests</span></span>|<span data-ttu-id="c8bbc-134">Коллекция [сеарчрекуест](../resources/searchrequest.md)</span><span class="sxs-lookup"><span data-stu-id="c8bbc-134">[searchRequest](../resources/searchrequest.md) collection</span></span>|<span data-ttu-id="c8bbc-135">Запрос поиска, отправляемый в конечную точку запроса, отформатированное в большом двоичном объекте JSON.</span><span class="sxs-lookup"><span data-stu-id="c8bbc-135">The search request to be sent to the query endpoint formatted in a JSON blob.</span></span> <span data-ttu-id="c8bbc-136">Он содержит тип сущностей, ожидаемых в ответе, базовые источники, параметры разбиения по страницам, запрашиваемые поля и фактический поисковый запрос.</span><span class="sxs-lookup"><span data-stu-id="c8bbc-136">It contains the type of entities expected in the response, the underlying sources, the paging parameters, the requested fields, and the actual search query.</span></span>|

## <a name="response"></a><span data-ttu-id="c8bbc-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="c8bbc-137">Response</span></span>

<span data-ttu-id="c8bbc-138">В случае успешного выполнения этот метод `HTTP 200 OK` возвращает код отклика и объект коллекции [сеарчреспонсе](../resources/searchresponse.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c8bbc-138">If successful, this method returns `HTTP 200 OK` response code and a [searchResponse](../resources/searchresponse.md) collection object in the response body.</span></span>

## <a name="common-use-cases"></a><span data-ttu-id="c8bbc-139">Основные варианты использования</span><span class="sxs-lookup"><span data-stu-id="c8bbc-139">Common use cases</span></span>

- <span data-ttu-id="c8bbc-140">Поиск в [сообщениях электронной почты](/graph/search-concept-messages)</span><span class="sxs-lookup"><span data-stu-id="c8bbc-140">Search [mail messages](/graph/search-concept-messages)</span></span>
- <span data-ttu-id="c8bbc-141">Поиск [событий календаря](/graph/search-concept-events)</span><span class="sxs-lookup"><span data-stu-id="c8bbc-141">Search [calendar events](/graph/search-concept-events)</span></span>
- <span data-ttu-id="c8bbc-142">Поиск [файлов](/graph/search-concept-files)</span><span class="sxs-lookup"><span data-stu-id="c8bbc-142">Search [files](/graph/search-concept-files)</span></span>
- <span data-ttu-id="c8bbc-143">Данные о [настраиваемых типах (соединителях)](/graph/search-concept-custom-types) поиска</span><span class="sxs-lookup"><span data-stu-id="c8bbc-143">Search [custom types (Connectors)](/graph/search-concept-custom-types) data</span></span>

## <a name="examples"></a><span data-ttu-id="c8bbc-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="c8bbc-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c8bbc-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="c8bbc-145">Request</span></span>

<span data-ttu-id="c8bbc-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c8bbc-146">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c8bbc-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="c8bbc-147">HTTP</span></span>](#tab/http)
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
        "microsoft.graph.externalItem"
      ],
      "contentSources": [
        "/external/connections/connectionfriendlyname"
      ],
      "query": {
        "query_string": {
          "query": "contoso product"
        }
      },
      "from": 0,
      "size": 25,
      "stored_fields": [
        "title",
        "description"
      ]
    }
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c8bbc-148">C#</span><span class="sxs-lookup"><span data-stu-id="c8bbc-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/search-query-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c8bbc-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c8bbc-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/search-query-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c8bbc-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c8bbc-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/search-query-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c8bbc-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8bbc-151">Response</span></span>

<span data-ttu-id="c8bbc-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c8bbc-152">The following is an example of the response.</span></span>

> <span data-ttu-id="c8bbc-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c8bbc-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
              "_id": "1",
              "_score": 1,
              "_sortField": "Relevance",
              "_summary": "_summary-value",
              "_source": "The source field will contain the underlying graph entity part of the response"
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

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "search: query",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
