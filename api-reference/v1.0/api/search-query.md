---
title: 'объект поиска: запрос'
description: Выполняет запрос, указанный в теле запроса. Результаты поиска предоставляются в ответе.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 8194b23ede8856f0237b179aa4d50a5ce0c1ebc9
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920112"
---
# <a name="searchentity-query"></a><span data-ttu-id="b1c1d-104">объект поиска: запрос</span><span class="sxs-lookup"><span data-stu-id="b1c1d-104">searchEntity: query</span></span>

<span data-ttu-id="b1c1d-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1c1d-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b1c1d-106">Выполняет запрос, указанный в теле запроса.</span><span class="sxs-lookup"><span data-stu-id="b1c1d-106">Runs the query specified in the request body.</span></span> <span data-ttu-id="b1c1d-107">Результаты поиска предоставляются в ответе.</span><span class="sxs-lookup"><span data-stu-id="b1c1d-107">Search results are provided in the response.</span></span>


## <a name="permissions"></a><span data-ttu-id="b1c1d-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b1c1d-108">Permissions</span></span>

<span data-ttu-id="b1c1d-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1c1d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span> 

| <span data-ttu-id="b1c1d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b1c1d-111">Permission type</span></span>                        | <span data-ttu-id="b1c1d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b1c1d-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b1c1d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b1c1d-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="b1c1d-114">Mail.Read, Calendars.Read, Files.Read.All, Sites.Read.All, ExternalItem.Read.All</span><span class="sxs-lookup"><span data-stu-id="b1c1d-114">Mail.Read, Calendars.Read, Files.Read.All, Sites.Read.All, ExternalItem.Read.All</span></span> |
| <span data-ttu-id="b1c1d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b1c1d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1c1d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1c1d-116">Not supported.</span></span> |
| <span data-ttu-id="b1c1d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b1c1d-117">Application</span></span>                            | <span data-ttu-id="b1c1d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1c1d-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b1c1d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b1c1d-119">HTTP request</span></span>

```HTTP
POST /search/query
```

## <a name="request-headers"></a><span data-ttu-id="b1c1d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b1c1d-120">Request headers</span></span>

| <span data-ttu-id="b1c1d-121">Имя</span><span class="sxs-lookup"><span data-stu-id="b1c1d-121">Name</span></span>          | <span data-ttu-id="b1c1d-122">Описание</span><span class="sxs-lookup"><span data-stu-id="b1c1d-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b1c1d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b1c1d-123">Authorization</span></span> | <span data-ttu-id="b1c1d-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b1c1d-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b1c1d-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b1c1d-126">Content-type</span></span> | <span data-ttu-id="b1c1d-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b1c1d-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b1c1d-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b1c1d-129">Request body</span></span>

<span data-ttu-id="b1c1d-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="b1c1d-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b1c1d-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="b1c1d-131">Parameter</span></span>    | <span data-ttu-id="b1c1d-132">Тип</span><span class="sxs-lookup"><span data-stu-id="b1c1d-132">Type</span></span>        | <span data-ttu-id="b1c1d-133">Описание</span><span class="sxs-lookup"><span data-stu-id="b1c1d-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b1c1d-134">запросы</span><span class="sxs-lookup"><span data-stu-id="b1c1d-134">requests</span></span>|<span data-ttu-id="b1c1d-135">[коллекция searchRequest](../resources/searchrequest.md)</span><span class="sxs-lookup"><span data-stu-id="b1c1d-135">[searchRequest](../resources/searchrequest.md) collection</span></span>|<span data-ttu-id="b1c1d-136">Коллекция из одного или более запросов поиска, каждый из которых отформатирован в BLOB JSON.</span><span class="sxs-lookup"><span data-stu-id="b1c1d-136">A collection of one or more search requests each formatted in a JSON blob.</span></span> <span data-ttu-id="b1c1d-137">Каждая blob JSON содержит типы ресурсов, ожидаемых в ответе, основные источники, параметры paging, запрашиваемого поля и фактический запрос поиска.</span><span class="sxs-lookup"><span data-stu-id="b1c1d-137">Each JSON blob contains the types of resources expected in the response, the underlying sources, paging parameters, requested fields, and actual search query.</span></span> <br> <span data-ttu-id="b1c1d-138">Будьте в курсе [известных ограничений](../resources/search-api-overview.md#known-limitations) на поиск определенных комбинаций типов сущностей, а также сортировку или агрегирование результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="b1c1d-138">Be aware of [known limitations](../resources/search-api-overview.md#known-limitations) on searching specific combinations of entity types, and sorting or aggregating search results.</span></span> |

## <a name="response"></a><span data-ttu-id="b1c1d-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1c1d-139">Response</span></span>

<span data-ttu-id="b1c1d-140">В случае успешной работы этот метод возвращает код отклика и объект `HTTP 200 OK` [коллекции searchResponse](../resources/searchresponse.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b1c1d-140">If successful, this method returns `HTTP 200 OK` response code and a [searchResponse](../resources/searchresponse.md) collection object in the response body.</span></span>
 

## <a name="examples"></a><span data-ttu-id="b1c1d-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="b1c1d-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b1c1d-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="b1c1d-142">Request</span></span>

<span data-ttu-id="b1c1d-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b1c1d-143">The following is an example of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="b1c1d-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1c1d-144">Response</span></span>

<span data-ttu-id="b1c1d-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b1c1d-145">The following is an example of the response.</span></span>

> <span data-ttu-id="b1c1d-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b1c1d-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
                            "summary": "...Identity Protection Weekly Digest <c0>Contoso</c0> New risky users detected <https://azure.microsoft.com/email/?destination=https%3A%2F%2Fportal.azure.com%2Fcontoso.com%23blade%2FMicrosoft_AAD_IAM%2FIdentityProtectionMenuBlade%2FRiskyUsers%2F...",
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
                                "bodyPreview": "...Identity Protection Weekly Digest Contoso New risky users detected <https://azure.microsoft.com/email/?destination=https%3A%2F%2Fportal.azure.com%2Fcontoso.com%23blade%2FMicrosoft_AAD_IAM%2FIdentityProtectionMenuBlade%2FRiskyUsers%2F...",
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
                                        "address": "azure-noreply@contoso.com"
                                    }
                                },
                                "from": {
                                    "emailAddress": {
                                        "name": "Microsoft Azure",
                                        "address": "azure-noreply@contoso.com"
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

## <a name="see-also"></a><span data-ttu-id="b1c1d-148">См. также</span><span class="sxs-lookup"><span data-stu-id="b1c1d-148">See also</span></span>
- <span data-ttu-id="b1c1d-149">Поиск [сообщений почты](/graph/search-concept-messages)</span><span class="sxs-lookup"><span data-stu-id="b1c1d-149">Search [mail messages](/graph/search-concept-messages)</span></span>
- <span data-ttu-id="b1c1d-150">События [календаря поиска](/graph/search-concept-events)</span><span class="sxs-lookup"><span data-stu-id="b1c1d-150">Search [calendar events](/graph/search-concept-events)</span></span>
- <span data-ttu-id="b1c1d-151">Поиск контента в SharePoint и OneDrive[(файлы, списки и сайты)](/graph/search-concept-files)</span><span class="sxs-lookup"><span data-stu-id="b1c1d-151">Search content in SharePoint and OneDrive ([files, lists and sites](/graph/search-concept-files))</span></span>
- <span data-ttu-id="b1c1d-152">Пользовательские [типы поиска (графовые соединители)](/graph/search-concept-custom-types) данных</span><span class="sxs-lookup"><span data-stu-id="b1c1d-152">Search [custom types (Graph Connectors)](/graph/search-concept-custom-types) data</span></span>


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "search: query",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


