---
title: 'Сеарчентити: запрос'
description: Выполняет запрос, указанный в теле запроса. Результаты поиска предоставляются в ответе.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: b5b49bd8bb370089774afb63593d282864191b66
ms.sourcegitcommit: 5345c2f3265ede107fa0faaff7a3f1c2afee3810
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378026"
---
# <a name="searchentity-query"></a><span data-ttu-id="a8ecf-104">Сеарчентити: запрос</span><span class="sxs-lookup"><span data-stu-id="a8ecf-104">searchEntity: query</span></span>

<span data-ttu-id="a8ecf-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8ecf-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a8ecf-106">Выполняет запрос, указанный в теле запроса.</span><span class="sxs-lookup"><span data-stu-id="a8ecf-106">Runs the query specified in the request body.</span></span> <span data-ttu-id="a8ecf-107">Результаты поиска предоставляются в ответе.</span><span class="sxs-lookup"><span data-stu-id="a8ecf-107">Search results are provided in the response.</span></span>


## <a name="permissions"></a><span data-ttu-id="a8ecf-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a8ecf-108">Permissions</span></span>

<span data-ttu-id="a8ecf-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8ecf-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span> 

| <span data-ttu-id="a8ecf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a8ecf-111">Permission type</span></span>                        | <span data-ttu-id="a8ecf-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a8ecf-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a8ecf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a8ecf-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="a8ecf-114">Mail. Read, mail. ReadWrite, Calendars. Read, Calendars. ReadWrite, Files. Read. ALL, Files. ReadWrite. ALL, sites. Read. ALL, sites. ReadWrite. ALL, Екстерналитем. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="a8ecf-114">Mail.Read, Mail.ReadWrite, Calendars.Read, Calendars.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All, ExternalItem.Read.All</span></span> |
| <span data-ttu-id="a8ecf-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a8ecf-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8ecf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8ecf-116">Not supported.</span></span> |
| <span data-ttu-id="a8ecf-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a8ecf-117">Application</span></span>                            | <span data-ttu-id="a8ecf-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8ecf-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a8ecf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a8ecf-119">HTTP request</span></span>

```HTTP
POST /search/query
```

## <a name="request-headers"></a><span data-ttu-id="a8ecf-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a8ecf-120">Request headers</span></span>

| <span data-ttu-id="a8ecf-121">Имя</span><span class="sxs-lookup"><span data-stu-id="a8ecf-121">Name</span></span>          | <span data-ttu-id="a8ecf-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a8ecf-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="a8ecf-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a8ecf-123">Authorization</span></span> | <span data-ttu-id="a8ecf-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a8ecf-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a8ecf-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a8ecf-126">Content-type</span></span> | <span data-ttu-id="a8ecf-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a8ecf-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a8ecf-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a8ecf-129">Request body</span></span>

<span data-ttu-id="a8ecf-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="a8ecf-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a8ecf-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="a8ecf-131">Parameter</span></span>    | <span data-ttu-id="a8ecf-132">Тип</span><span class="sxs-lookup"><span data-stu-id="a8ecf-132">Type</span></span>        | <span data-ttu-id="a8ecf-133">Описание</span><span class="sxs-lookup"><span data-stu-id="a8ecf-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a8ecf-134">обращения</span><span class="sxs-lookup"><span data-stu-id="a8ecf-134">requests</span></span>|<span data-ttu-id="a8ecf-135">Коллекция [сеарчрекуест](../resources/searchrequest.md)</span><span class="sxs-lookup"><span data-stu-id="a8ecf-135">[searchRequest](../resources/searchrequest.md) collection</span></span>|<span data-ttu-id="a8ecf-136">Коллекция из одного или нескольких запросов на поиск, отформатированных в большом двоичном объекте JSON.</span><span class="sxs-lookup"><span data-stu-id="a8ecf-136">A collection of one or more search requests each formatted in a JSON blob.</span></span> <span data-ttu-id="a8ecf-137">Каждый большой двоичный объект JSON содержит типы ресурсов, ожидаемых в ответе, базовые источники, параметры разбиения по страницам, запрашиваемые поля и фактический поисковый запрос.</span><span class="sxs-lookup"><span data-stu-id="a8ecf-137">Each JSON blob contains the types of resources expected in the response, the underlying sources, paging parameters, requested fields, and actual search query.</span></span> <br> <span data-ttu-id="a8ecf-138">Помните об [известных ограничениях](../resources/search-api-overview.md#known-limitations) на поиск определенных комбинаций типов сущностей, сортировку или статистическую обработку результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="a8ecf-138">Be aware of [known limitations](../resources/search-api-overview.md#known-limitations) on searching specific combinations of entity types, and sorting or aggregating search results.</span></span> |

## <a name="response"></a><span data-ttu-id="a8ecf-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="a8ecf-139">Response</span></span>

<span data-ttu-id="a8ecf-140">В случае успешного выполнения этот метод возвращает `HTTP 200 OK` код отклика и объект коллекции [сеарчреспонсе](../resources/searchresponse.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a8ecf-140">If successful, this method returns `HTTP 200 OK` response code and a [searchResponse](../resources/searchresponse.md) collection object in the response body.</span></span>
 

## <a name="examples"></a><span data-ttu-id="a8ecf-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="a8ecf-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a8ecf-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="a8ecf-142">Request</span></span>

<span data-ttu-id="a8ecf-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a8ecf-143">The following is an example of the request.</span></span>

```HTTP
POST https://graph.microsoft.com/v1.0/search/query
Content-type: application/json

{
  "requests": [
    {
      "entityTypes": [
        "message"
      ],
      "query": {
        "queryString": "contoso"
      },
      "from": 0,
      "size": 25
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="a8ecf-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="a8ecf-144">Response</span></span>

<span data-ttu-id="a8ecf-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a8ecf-145">The following is an example of the response.</span></span>

> <span data-ttu-id="a8ecf-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a8ecf-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
                            "hitId": "AAMkADdmODdhN2NjLTMwZWYtNDBiNy1iMDYxLWZhZTkyOGM4YmRhZABGAAAAAACsLZF5BeQoRLYm4UlvnOXZBwCav2PZy/7/R52ssyzmS9f0AAAAAAEMAACav2PZy/7/R52ssyzmS9f0AABM0pr/AAA=",
                            "rank": 1,
                            "summary": "...Identity Protection Weekly Digest <c0>Contoso</c0> New risky users detected <https://azure.microsoft.com/email/?destination=https%3A%2F%2Fportal.azure.com%2FM365x231305.onmicrosoft.com%23blade%2FMicrosoft_AAD_IAM%2FIdentityProtectionMenuBlade%2FRiskyUsers%2F...",
                            "resource": {
                                "@odata.type": "#microsoft.graph.message",
                                "createdDateTime": "2020-11-17T16:02:34Z",
                                "lastModifiedDateTime": "2020-11-17T16:02:37Z",
                                "changeKey": "CQAAAA==",
                                "receivedDateTime": "2020-11-17T16:02:34Z",
                                "sentDateTime": "2020-11-17T16:02:27Z",
                                "hasAttachments": false,
                                "internetMessageId": "<1e506769-c6da-4f44-bb54-6ba1bd59d300@az.northcentralus.production.microsoft.com>",
                                "subject": "Azure AD Identity Protection Weekly Digest",
                                "bodyPreview": "...Identity Protection Weekly Digest Contoso New risky users detected <https://azure.microsoft.com/email/?destination=https%3A%2F%2Fportal.azure.com%2FM365x231305.onmicrosoft.com%23blade%2FMicrosoft_AAD_IAM%2FIdentityProtectionMenuBlade%2FRiskyUsers%2F...",
                                "importance": "normal",
                                "parentFolderId": "AQMkADdmODdhN2NjAC0zMGVmLTQwYjctYjA2MS1mYWU5MjhjOGJkYWQALgAAA6wtkXkF5ChEtibhSW+c5dkBAJq/Y9nL/v9HnayzLOZL1/QAAAIBDAAAAA==",
                                "conversationId": "AAQkADdmODdhN2NjLTMwZWYtNDBiNy1iMDYxLWZhZTkyOGM4YmRhZAAQAKQ6a/rTEmVCtGMTER183jw=",
                                "isRead": false,
                                "isDraft": false,
                                "webLink": "https://outlook.office365.com/owa/?ItemID=AAMkADdmODdhN2NjLTMwZWYtNDBiNy1iMDYxLWZhZTkyOGM4YmRhZABGAAAAAACsLZF5BeQoRLYm4UlvnOXZBwCav2PZy%2F7%2FR52ssyzmS9f0AAAAAAEMAACav2PZy%2F7%2FR52ssyzmS9f0AABM0pr%2FAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
                                "inferenceClassification": "focused",
                                "replyTo": [
                                    {
                                        "emailAddress": {
                                            "name": "MOD Administrator"
                                        }
                                    }
                                ],
                                "sender": {
                                    "emailAddress": {
                                        "name": "Microsoft Azure",
                                        "address": "azure-noreply@microsoft.com"
                                    }
                                },
                                "from": {
                                    "emailAddress": {
                                        "name": "Microsoft Azure",
                                        "address": "azure-noreply@microsoft.com"
                                    }
                                }
                            }
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

## <a name="see-also"></a><span data-ttu-id="a8ecf-148">См. также</span><span class="sxs-lookup"><span data-stu-id="a8ecf-148">See also</span></span>
- <span data-ttu-id="a8ecf-149">Поиск в [сообщениях электронной почты](/graph/search-concept-messages)</span><span class="sxs-lookup"><span data-stu-id="a8ecf-149">Search [mail messages](/graph/search-concept-messages)</span></span>
- <span data-ttu-id="a8ecf-150">Поиск [событий календаря](/graph/search-concept-events)</span><span class="sxs-lookup"><span data-stu-id="a8ecf-150">Search [calendar events](/graph/search-concept-events)</span></span>
- <span data-ttu-id="a8ecf-151">Поиск контента в SharePoint и OneDrive ([файлы, списки и сайты](/graph/search-concept-files))</span><span class="sxs-lookup"><span data-stu-id="a8ecf-151">Search content in SharePoint and OneDrive ([files, lists and sites](/graph/search-concept-files))</span></span>
- <span data-ttu-id="a8ecf-152">Данные о [настраиваемых типах поиска (соединители Graph)](/graph/search-concept-custom-types)</span><span class="sxs-lookup"><span data-stu-id="a8ecf-152">Search [custom types (Graph Connectors)](/graph/search-concept-custom-types) data</span></span>


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "search: query",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


