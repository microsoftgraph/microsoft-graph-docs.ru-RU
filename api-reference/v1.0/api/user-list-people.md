---
title: Список людей
description: Получите коллекцию объектов person, упорядоченных по их релевантности для пользователя, которая определяется его моделями общения и совместной работы, а также бизнес-отношениями.
author: dkershaw10
localization_priority: Priority
ms.prod: insights
ms.openlocfilehash: be4bb525cbc37781ad49312041da26cc84299459
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35274013"
---
# <a name="list-people"></a><span data-ttu-id="6dce7-103">Список людей</span><span class="sxs-lookup"><span data-stu-id="6dce7-103">List people</span></span>

<span data-ttu-id="6dce7-104">Получите коллекцию объектов [person](../resources/person.md), упорядоченных по их релевантности для [пользователя](../resources/user.md), которая определяется его моделями общения и совместной работы, а также бизнес-отношениями.</span><span class="sxs-lookup"><span data-stu-id="6dce7-104">Retrieve a collection of [person](../resources/person.md) objects ordered by their relevance to the [user](../resources/user.md), which is determined by the user's communication and collaboration patterns, and business relationships.</span></span>

<span data-ttu-id="6dce7-p101">Для получения этих сведений используйте API службы "Люди". Примеры см. в разделе [Примеры](#examples) и статье о том, как [получить релевантную информацию о людях](/graph/people-example).</span><span class="sxs-lookup"><span data-stu-id="6dce7-p101">You can get this information via the People API. For examples, see the [Examples](#examples) section and the article [Get relevant information about people](/graph/people-example).</span></span>

## <a name="permissions"></a><span data-ttu-id="6dce7-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6dce7-107">Permissions</span></span>

<span data-ttu-id="6dce7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6dce7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6dce7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6dce7-110">Permission type</span></span>      | <span data-ttu-id="6dce7-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6dce7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6dce7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6dce7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6dce7-113">People.Read, People.Read.All</span><span class="sxs-lookup"><span data-stu-id="6dce7-113">People.Read, People.Read.All</span></span>    |
|<span data-ttu-id="6dce7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6dce7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6dce7-115">People.Read</span><span class="sxs-lookup"><span data-stu-id="6dce7-115">People.Read</span></span>    |
|<span data-ttu-id="6dce7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6dce7-116">Application</span></span> | <span data-ttu-id="6dce7-117">People.Read.All</span><span class="sxs-lookup"><span data-stu-id="6dce7-117">People.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6dce7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6dce7-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/people
GET /users/{id | userPrincipalName}/people
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6dce7-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6dce7-119">Optional query parameters</span></span>

<span data-ttu-id="6dce7-120">Этот метод поддерживает [параметры запроса OData](/graph/query-parameters) также для настройки ответа. Примеры см. в статье [Получение релевантной информации о людях](/graph/people-example).</span><span class="sxs-lookup"><span data-stu-id="6dce7-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, as shown in the examples in the article [Get relevant information about people](/graph/people-example).</span></span>

|<span data-ttu-id="6dce7-121">Имя</span><span class="sxs-lookup"><span data-stu-id="6dce7-121">Name</span></span>|<span data-ttu-id="6dce7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6dce7-122">Value</span></span>|<span data-ttu-id="6dce7-123">Описание</span><span class="sxs-lookup"><span data-stu-id="6dce7-123">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="6dce7-124">$filter</span><span class="sxs-lookup"><span data-stu-id="6dce7-124">$filter</span></span>|<span data-ttu-id="6dce7-125">string</span><span class="sxs-lookup"><span data-stu-id="6dce7-125">string</span></span>|<span data-ttu-id="6dce7-126">Позволяет возвращать в отклике только тех людей, чьи записи содержат указанные критерии.</span><span class="sxs-lookup"><span data-stu-id="6dce7-126">Limits the response to only those people whose record contains the specified criteria.</span></span>|
|<span data-ttu-id="6dce7-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="6dce7-127">$orderby</span></span>|<span data-ttu-id="6dce7-128">строка</span><span class="sxs-lookup"><span data-stu-id="6dce7-128">string</span></span>|<span data-ttu-id="6dce7-129">По умолчанию люди в ответе сортируются по степени соответствия запросу.</span><span class="sxs-lookup"><span data-stu-id="6dce7-129">By default the people in the response are sorted by their relevance to your query.</span></span> <span data-ttu-id="6dce7-130">Этот порядок можно изменить с помощью параметра *$orderby*.</span><span class="sxs-lookup"><span data-stu-id="6dce7-130">You can change the order of the people in the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="6dce7-131">$search</span><span class="sxs-lookup"><span data-stu-id="6dce7-131">$search</span></span>|<span data-ttu-id="6dce7-132">string</span><span class="sxs-lookup"><span data-stu-id="6dce7-132">string</span></span>|<span data-ttu-id="6dce7-133">Поиск пользователей по имени или псевдониму.</span><span class="sxs-lookup"><span data-stu-id="6dce7-133">Search for people by name or alias.</span></span> <span data-ttu-id="6dce7-134">Поддерживается нечеткое соответствие.</span><span class="sxs-lookup"><span data-stu-id="6dce7-134">Supports Fuzzy matching.</span></span> <span data-ttu-id="6dce7-135">Параметр применяется только для поиска людей, относящихся к вошедшему пользователю, а не для поиска людей, относящихся к другим пользователям.</span><span class="sxs-lookup"><span data-stu-id="6dce7-135">Parameter only works for searching the signed-in user's relevant people, not for searching people relevant to other users.</span></span> <span data-ttu-id="6dce7-136">Также поддерживает ключевое слово `topic` для поиска людей с учетом тем, извлеченных из бесед электронной почты с определенным человеком.</span><span class="sxs-lookup"><span data-stu-id="6dce7-136">Also supports the `topic` keyword to find people based on topics extracted from e-mail conversations with that person.</span></span> <span data-ttu-id="6dce7-137">Сведения и примеры см. в разделе *Нечеткий поиск* статьи [Получение релевантных сведений о людях](/graph/people-example#perform-a-fuzzy-search).</span><span class="sxs-lookup"><span data-stu-id="6dce7-137">See the *Perform a fuzzy search* section at [Get relevant information about people](/graph/people-example#perform-a-fuzzy-search) for information and examples.</span></span> |
|<span data-ttu-id="6dce7-138">$select</span><span class="sxs-lookup"><span data-stu-id="6dce7-138">$select</span></span>|<span data-ttu-id="6dce7-139">string</span><span class="sxs-lookup"><span data-stu-id="6dce7-139">string</span></span>|<span data-ttu-id="6dce7-p105">Список разделенных запятыми свойств, которые необходимо включить в отклик. Для оптимизации производительности выбирайте только необходимые свойства.</span><span class="sxs-lookup"><span data-stu-id="6dce7-p105">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>|
|<span data-ttu-id="6dce7-142">$skip</span><span class="sxs-lookup"><span data-stu-id="6dce7-142">$skip</span></span>|<span data-ttu-id="6dce7-143">int</span><span class="sxs-lookup"><span data-stu-id="6dce7-143">int</span></span>|<span data-ttu-id="6dce7-p106">Пропуск первых n результатов; эту функцию удобно использовать при разбиении результатов на страницы. Эта возможность не поддерживается при использовании параметра *$search*.</span><span class="sxs-lookup"><span data-stu-id="6dce7-p106">Skip the first n results, useful for paging. This is not supported when using *$search*.</span></span>|
|<span data-ttu-id="6dce7-146">$top</span><span class="sxs-lookup"><span data-stu-id="6dce7-146">$top</span></span>|<span data-ttu-id="6dce7-147">int</span><span class="sxs-lookup"><span data-stu-id="6dce7-147">int</span></span>|<span data-ttu-id="6dce7-148">Количество возвращаемых результатов.</span><span class="sxs-lookup"><span data-stu-id="6dce7-148">Number of results to be returned.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="6dce7-149">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6dce7-149">Request headers</span></span>

| <span data-ttu-id="6dce7-150">Имя</span><span class="sxs-lookup"><span data-stu-id="6dce7-150">Name</span></span>      |<span data-ttu-id="6dce7-151">Описание</span><span class="sxs-lookup"><span data-stu-id="6dce7-151">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6dce7-152">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6dce7-152">Authorization</span></span>  | <span data-ttu-id="6dce7-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6dce7-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6dce7-155">Accept</span><span class="sxs-lookup"><span data-stu-id="6dce7-155">Accept</span></span> | <span data-ttu-id="6dce7-156">application/json</span><span class="sxs-lookup"><span data-stu-id="6dce7-156">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="6dce7-157">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6dce7-157">Request body</span></span>

<span data-ttu-id="6dce7-158">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6dce7-158">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6dce7-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="6dce7-159">Response</span></span>

<span data-ttu-id="6dce7-p108">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [person](../resources/person.md) в тексте ответа. Отклик может содержать один объект person либо коллекцию объектов person.</span><span class="sxs-lookup"><span data-stu-id="6dce7-p108">If successful, this method returns a `200 OK` response code and a collection of [person](../resources/person.md) objects in the response body. The response can contain one person object or a collection of person objects.</span></span>

## <a name="examples"></a><span data-ttu-id="6dce7-162">Примеры</span><span class="sxs-lookup"><span data-stu-id="6dce7-162">Examples</span></span>

#### <a name="request"></a><span data-ttu-id="6dce7-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="6dce7-163">Request</span></span>

<span data-ttu-id="6dce7-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6dce7-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_person_collection"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/people
```

#### <a name="response"></a><span data-ttu-id="6dce7-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="6dce7-165">Response</span></span>

<span data-ttu-id="6dce7-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6dce7-166">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_person_collection",
  "truncated": true,
  "@odata.type": "microsoft.graph.person",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1370

{
    "value": [
        {
            "id": "33b43a5b-87d6-41ec-91f8-a2610048105f",
            "displayName": "Marketing",
            "givenName": null,
            "surname": null,
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": null,
            "companyName": null,
            "yomiCompany": "",
            "department": null,
            "officeLocation": null,
            "profession": "",
            "userPrincipalName": "",
            "imAddress": null,
            "scoredEmailAddresses": [
                {
                    "address": "Marketing@contoso.com",
                    "relevanceScore": 30.0
                }
            ],
            "phones": [],
            "postalAddresses": [],
            "websites": [],
            "personType": {
                "class": "Group",
                "subclass": "UnifiedGroup"
            }
        },
        {
            "id": "e3d0513b-449e-4198-ba6f-bd97ae7cae85",
            "displayName": "Isaiah Langer",
            "givenName": "Isaiah",
            "surname": "Langer",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "Web Marketing Manager",
            "companyName": null,
            "yomiCompany": "",
            "department": "Sales & Marketing",
            "officeLocation": "20/1101",
            "profession": "",
            "userPrincipalName": "IsaiahL@contoso.com",
            "imAddress": "sip:isaiahl@contoso.com",
            "scoredEmailAddresses": [
                {
                    "address": "IsaiahL@contoso.com",
                    "relevanceScore": 20.0
                }
            ],
            "phones": [
                {
                    "type": "business",
                    "number": "+1 918 555 0101"
                }
            ],
            "postalAddresses": [],
            "websites": [],
            "personType": {
                "class": "Person",
                "subclass": "OrganizationUser"
            }
        }
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="6dce7-167">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="6dce7-167">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="6dce7-168">C#</span><span class="sxs-lookup"><span data-stu-id="6dce7-168">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_person_collection-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6dce7-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6dce7-169">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_person_collection-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="6dce7-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6dce7-170">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_person_collection-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="6dce7-171">Другие примеры см. в статье [Получение релевантной информации о людях](/graph/people-example).</span><span class="sxs-lookup"><span data-stu-id="6dce7-171">For more examples, see the article [Get relevant information about people](/graph/people-example).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List people",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/user-list-people.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/user-list-people.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/user-list-people.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
