---
title: 'Поиск: запрос'
description: УКАЖИТЕ ОПИСАНИЕ
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: cc0e750f34af4bc6013d5e4bfbae4b007347b270
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937625"
---
# <a name="search-query"></a><span data-ttu-id="d4e1e-103">Поиск: запрос</span><span class="sxs-lookup"><span data-stu-id="d4e1e-103">search: query</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4e1e-104">Выполняет запрос, указанный в теле запроса.</span><span class="sxs-lookup"><span data-stu-id="d4e1e-104">Executes the query specified in the request body.</span></span> <span data-ttu-id="d4e1e-105">Результаты поиска предоставляются в ответе.</span><span class="sxs-lookup"><span data-stu-id="d4e1e-105">Search results are provided in the response.</span></span>

## <a name="permissions"></a><span data-ttu-id="d4e1e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d4e1e-106">Permissions</span></span>

<span data-ttu-id="d4e1e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4e1e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d4e1e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d4e1e-109">Permission type</span></span>                        | <span data-ttu-id="d4e1e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d4e1e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d4e1e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d4e1e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d4e1e-112">Mail. Read, Files. Read. ALL, Calendars. Read, Екстерналитем. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="d4e1e-112">Mail.Read, Files.Read.All, Calendars.Read, ExternalItem.Read.All</span></span> |
| <span data-ttu-id="d4e1e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d4e1e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4e1e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4e1e-114">Not supported.</span></span> |
| <span data-ttu-id="d4e1e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d4e1e-115">Application</span></span>                            | <span data-ttu-id="d4e1e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4e1e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d4e1e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d4e1e-117">HTTP request</span></span>

```HTTP
POST /search/query
```

## <a name="request-headers"></a><span data-ttu-id="d4e1e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d4e1e-118">Request headers</span></span>

| <span data-ttu-id="d4e1e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="d4e1e-119">Name</span></span>          | <span data-ttu-id="d4e1e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="d4e1e-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="d4e1e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4e1e-121">Authorization</span></span> | <span data-ttu-id="d4e1e-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="d4e1e-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="d4e1e-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d4e1e-123">Request body</span></span>

<span data-ttu-id="d4e1e-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="d4e1e-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d4e1e-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="d4e1e-125">Parameter</span></span>    | <span data-ttu-id="d4e1e-126">Тип</span><span class="sxs-lookup"><span data-stu-id="d4e1e-126">Type</span></span>        | <span data-ttu-id="d4e1e-127">Описание</span><span class="sxs-lookup"><span data-stu-id="d4e1e-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d4e1e-128">обращения</span><span class="sxs-lookup"><span data-stu-id="d4e1e-128">requests</span></span>|<span data-ttu-id="d4e1e-129">Коллекция [сеарчрекуест](../resources/searchrequest.md)</span><span class="sxs-lookup"><span data-stu-id="d4e1e-129">[searchRequest](../resources/searchrequest.md) collection</span></span>|<span data-ttu-id="d4e1e-130">Запрос поиска, отправляемый в конечную точку запроса, отформатированное в большом двоичном объекте JSON.</span><span class="sxs-lookup"><span data-stu-id="d4e1e-130">The search request to be sent to the query endpoint formatted in a JSON blob.</span></span> <span data-ttu-id="d4e1e-131">Он содержит тип сущностей, ожидаемых в ответе, базовые источники, параметры разбиения по страницам, запрашиваемые поля и фактический поисковый запрос.</span><span class="sxs-lookup"><span data-stu-id="d4e1e-131">It contains the type of entities expected in the response, the underlying sources, the paging parameters, the requested fields, and the actual search query.</span></span>|

## <a name="response"></a><span data-ttu-id="d4e1e-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4e1e-132">Response</span></span>

<span data-ttu-id="d4e1e-133">В случае успешного выполнения этот метод `HTTP 200 OK` возвращает код отклика и объект коллекции [сеарчреспонсе](../resources/searchresponse.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d4e1e-133">If successful, this method returns `HTTP 200 OK` response code and a [searchResponse](../resources/searchresponse.md) collection object in the response body.</span></span>

## <a name="common-use-cases"></a><span data-ttu-id="d4e1e-134">Основные варианты использования</span><span class="sxs-lookup"><span data-stu-id="d4e1e-134">Common use cases</span></span>

- <span data-ttu-id="d4e1e-135">Поиск в [сообщениях электронной почты](/graph/search-concept-messages)</span><span class="sxs-lookup"><span data-stu-id="d4e1e-135">Search [mail messages](/graph/search-concept-messages)</span></span>
- <span data-ttu-id="d4e1e-136">Поиск [событий календаря](/graph/search-concept-events)</span><span class="sxs-lookup"><span data-stu-id="d4e1e-136">Search [calendar events](/graph/search-concept-events)</span></span>
- <span data-ttu-id="d4e1e-137">Поиск [файлов](/graph/search-concept-files)</span><span class="sxs-lookup"><span data-stu-id="d4e1e-137">Search [files](/graph/search-concept-files)</span></span>
- <span data-ttu-id="d4e1e-138">Данные о [настраиваемых типах (соединителях)](/graph/search-concept-custom-types) поиска</span><span class="sxs-lookup"><span data-stu-id="d4e1e-138">Search [custom types (Connectors)](/graph/search-concept-custom-types) data</span></span>

## <a name="examples"></a><span data-ttu-id="d4e1e-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="d4e1e-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d4e1e-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="d4e1e-140">Request</span></span>

<span data-ttu-id="d4e1e-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d4e1e-141">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d4e1e-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4e1e-142">Response</span></span>

<span data-ttu-id="d4e1e-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d4e1e-143">The following is an example of the response.</span></span>

> <span data-ttu-id="d4e1e-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d4e1e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
