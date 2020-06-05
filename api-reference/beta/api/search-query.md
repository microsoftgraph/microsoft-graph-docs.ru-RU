---
title: 'Поиск: запрос'
description: Выполняет запрос, указанный в теле запроса. Результаты поиска предоставляются в ответе.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: c86a6bb7533fbda16c1796d4b4a7023c0463e4fe
ms.sourcegitcommit: 093d89c7583bb6880c8395e9498a1f33cdd938b4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/05/2020
ms.locfileid: "44568826"
---
# <a name="search-query"></a><span data-ttu-id="c046c-104">Поиск: запрос</span><span class="sxs-lookup"><span data-stu-id="c046c-104">search: query</span></span>

<span data-ttu-id="c046c-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c046c-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c046c-106">Выполняет запрос, указанный в теле запроса.</span><span class="sxs-lookup"><span data-stu-id="c046c-106">Runs the query specified in the request body.</span></span> <span data-ttu-id="c046c-107">Результаты поиска предоставляются в ответе.</span><span class="sxs-lookup"><span data-stu-id="c046c-107">Search results are provided in the response.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="c046c-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c046c-108">Permissions</span></span>

<span data-ttu-id="c046c-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c046c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c046c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c046c-111">Permission type</span></span>                        | <span data-ttu-id="c046c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c046c-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c046c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c046c-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="c046c-114">Mail. Read, Files. Read. ALL, Calendars. Read, Екстерналитем. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="c046c-114">Mail.Read, Files.Read.All, Calendars.Read, ExternalItem.Read.All</span></span> |
| <span data-ttu-id="c046c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c046c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c046c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c046c-116">Not supported.</span></span> |
| <span data-ttu-id="c046c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c046c-117">Application</span></span>                            | <span data-ttu-id="c046c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c046c-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c046c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c046c-119">HTTP request</span></span>

```HTTP
POST /search/query
```

## <a name="request-headers"></a><span data-ttu-id="c046c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c046c-120">Request headers</span></span>

| <span data-ttu-id="c046c-121">Имя</span><span class="sxs-lookup"><span data-stu-id="c046c-121">Name</span></span>          | <span data-ttu-id="c046c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c046c-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="c046c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c046c-123">Authorization</span></span> | <span data-ttu-id="c046c-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c046c-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c046c-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c046c-126">Content-type</span></span> | <span data-ttu-id="c046c-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c046c-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c046c-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c046c-129">Request body</span></span>

<span data-ttu-id="c046c-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="c046c-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c046c-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="c046c-131">Parameter</span></span>    | <span data-ttu-id="c046c-132">Тип</span><span class="sxs-lookup"><span data-stu-id="c046c-132">Type</span></span>        | <span data-ttu-id="c046c-133">Описание</span><span class="sxs-lookup"><span data-stu-id="c046c-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c046c-134">обращения</span><span class="sxs-lookup"><span data-stu-id="c046c-134">requests</span></span>|<span data-ttu-id="c046c-135">Коллекция [сеарчрекуест](../resources/searchrequest.md)</span><span class="sxs-lookup"><span data-stu-id="c046c-135">[searchRequest](../resources/searchrequest.md) collection</span></span>|<span data-ttu-id="c046c-136">Запрос поиска, отправляемый в конечную точку запроса, отформатированное в большом двоичном объекте JSON.</span><span class="sxs-lookup"><span data-stu-id="c046c-136">The search request to be sent to the query endpoint formatted in a JSON blob.</span></span> <span data-ttu-id="c046c-137">Он содержит тип сущностей, ожидаемых в ответе, базовые источники, параметры разбиения по страницам, запрашиваемые поля и фактический поисковый запрос.</span><span class="sxs-lookup"><span data-stu-id="c046c-137">It contains the type of entities expected in the response, the underlying sources, the paging parameters, the requested fields, and the actual search query.</span></span>|

## <a name="response"></a><span data-ttu-id="c046c-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="c046c-138">Response</span></span>

<span data-ttu-id="c046c-139">В случае успешного выполнения этот метод возвращает `HTTP 200 OK` код отклика и объект коллекции [сеарчреспонсе](../resources/searchresponse.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c046c-139">If successful, this method returns `HTTP 200 OK` response code and a [searchResponse](../resources/searchresponse.md) collection object in the response body.</span></span>

## <a name="common-use-cases"></a><span data-ttu-id="c046c-140">Основные варианты использования</span><span class="sxs-lookup"><span data-stu-id="c046c-140">Common use cases</span></span>

- <span data-ttu-id="c046c-141">Поиск в [сообщениях электронной почты](/graph/search-concept-messages)</span><span class="sxs-lookup"><span data-stu-id="c046c-141">Search [mail messages](/graph/search-concept-messages)</span></span>
- <span data-ttu-id="c046c-142">Поиск [событий календаря](/graph/search-concept-events)</span><span class="sxs-lookup"><span data-stu-id="c046c-142">Search [calendar events](/graph/search-concept-events)</span></span>
- <span data-ttu-id="c046c-143">Поиск [файлов](/graph/search-concept-files)</span><span class="sxs-lookup"><span data-stu-id="c046c-143">Search [files](/graph/search-concept-files)</span></span>
- <span data-ttu-id="c046c-144">Данные о [настраиваемых типах (соединителях)](/graph/search-concept-custom-types) поиска</span><span class="sxs-lookup"><span data-stu-id="c046c-144">Search [custom types (Connectors)](/graph/search-concept-custom-types) data</span></span>

## <a name="examples"></a><span data-ttu-id="c046c-145">Примеры</span><span class="sxs-lookup"><span data-stu-id="c046c-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c046c-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="c046c-146">Request</span></span>

<span data-ttu-id="c046c-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c046c-147">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c046c-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="c046c-148">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="c046c-149">C#</span><span class="sxs-lookup"><span data-stu-id="c046c-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/search-query-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c046c-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c046c-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/search-query-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c046c-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c046c-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/search-query-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c046c-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="c046c-152">Response</span></span>

<span data-ttu-id="c046c-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c046c-153">The following is an example of the response.</span></span>

> <span data-ttu-id="c046c-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c046c-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
