---
title: Список людей
description: Получите коллекцию объектов person, упорядоченных по их релевантности для пользователя, которая определяется его моделями общения и совместной работы, а также бизнес-отношениями.
author: dkershaw10
localization_priority: Priority
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 1acc5a963939381ad132defdc3942db9e7d7a920
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42509040"
---
# <a name="list-people"></a><span data-ttu-id="1326b-103">Список людей</span><span class="sxs-lookup"><span data-stu-id="1326b-103">List people</span></span>

<span data-ttu-id="1326b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1326b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1326b-105">Получите коллекцию объектов [person](../resources/person.md), упорядоченных по их релевантности для [пользователя](../resources/user.md), которая определяется его моделями общения и совместной работы, а также бизнес-отношениями.</span><span class="sxs-lookup"><span data-stu-id="1326b-105">Retrieve a collection of [person](../resources/person.md) objects ordered by their relevance to the [user](../resources/user.md), which is determined by the user's communication and collaboration patterns, and business relationships.</span></span>

<span data-ttu-id="1326b-p101">Для получения этих сведений используйте API службы "Люди". Примеры см. в разделе [Примеры](#examples) и статье о том, как [получить релевантную информацию о людях](/graph/people-example).</span><span class="sxs-lookup"><span data-stu-id="1326b-p101">You can get this information via the People API. For examples, see the [Examples](#examples) section and the article [Get relevant information about people](/graph/people-example).</span></span>

## <a name="permissions"></a><span data-ttu-id="1326b-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1326b-108">Permissions</span></span>

<span data-ttu-id="1326b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1326b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1326b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1326b-111">Permission type</span></span>      | <span data-ttu-id="1326b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1326b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1326b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1326b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="1326b-114">People.Read, People.Read.All</span><span class="sxs-lookup"><span data-stu-id="1326b-114">People.Read, People.Read.All</span></span>    |
|<span data-ttu-id="1326b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1326b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1326b-116">People.Read</span><span class="sxs-lookup"><span data-stu-id="1326b-116">People.Read</span></span>    |
|<span data-ttu-id="1326b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1326b-117">Application</span></span> | <span data-ttu-id="1326b-118">People.Read.All</span><span class="sxs-lookup"><span data-stu-id="1326b-118">People.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1326b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1326b-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/people
GET /users/{id | userPrincipalName}/people
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1326b-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1326b-120">Optional query parameters</span></span>

<span data-ttu-id="1326b-121">Этот метод поддерживает [параметры запроса OData](/graph/query-parameters) также для настройки ответа. Примеры см. в статье [Получение релевантной информации о людях](/graph/people-example).</span><span class="sxs-lookup"><span data-stu-id="1326b-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, as shown in the examples in the article [Get relevant information about people](/graph/people-example).</span></span>

|<span data-ttu-id="1326b-122">Имя</span><span class="sxs-lookup"><span data-stu-id="1326b-122">Name</span></span>|<span data-ttu-id="1326b-123">Значение</span><span class="sxs-lookup"><span data-stu-id="1326b-123">Value</span></span>|<span data-ttu-id="1326b-124">Описание</span><span class="sxs-lookup"><span data-stu-id="1326b-124">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="1326b-125">$filter</span><span class="sxs-lookup"><span data-stu-id="1326b-125">$filter</span></span>|<span data-ttu-id="1326b-126">string</span><span class="sxs-lookup"><span data-stu-id="1326b-126">string</span></span>|<span data-ttu-id="1326b-127">Позволяет возвращать в отклике только тех людей, чьи записи содержат указанные критерии.</span><span class="sxs-lookup"><span data-stu-id="1326b-127">Limits the response to only those people whose record contains the specified criteria.</span></span>|
|<span data-ttu-id="1326b-128">$orderby</span><span class="sxs-lookup"><span data-stu-id="1326b-128">$orderby</span></span>|<span data-ttu-id="1326b-129">строка</span><span class="sxs-lookup"><span data-stu-id="1326b-129">string</span></span>|<span data-ttu-id="1326b-130">По умолчанию люди в ответе сортируются по степени соответствия запросу.</span><span class="sxs-lookup"><span data-stu-id="1326b-130">By default the people in the response are sorted by their relevance to your query.</span></span> <span data-ttu-id="1326b-131">Этот порядок можно изменить с помощью параметра *$orderby*.</span><span class="sxs-lookup"><span data-stu-id="1326b-131">You can change the order of the people in the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="1326b-132">$search</span><span class="sxs-lookup"><span data-stu-id="1326b-132">$search</span></span>|<span data-ttu-id="1326b-133">string</span><span class="sxs-lookup"><span data-stu-id="1326b-133">string</span></span>|<span data-ttu-id="1326b-134">Поиск пользователей по имени или псевдониму.</span><span class="sxs-lookup"><span data-stu-id="1326b-134">Search for people by name or alias.</span></span> <span data-ttu-id="1326b-135">Поддерживается нечеткое соответствие.</span><span class="sxs-lookup"><span data-stu-id="1326b-135">Supports Fuzzy matching.</span></span> <span data-ttu-id="1326b-136">Параметр применяется только для поиска людей, относящихся к вошедшему пользователю, а не для поиска людей, относящихся к другим пользователям.</span><span class="sxs-lookup"><span data-stu-id="1326b-136">Parameter only works for searching the signed-in user's relevant people, not for searching people relevant to other users.</span></span> <span data-ttu-id="1326b-137">Также поддерживает ключевое слово `topic` для поиска людей с учетом тем, извлеченных из бесед электронной почты с определенным человеком.</span><span class="sxs-lookup"><span data-stu-id="1326b-137">Also supports the `topic` keyword to find people based on topics extracted from e-mail conversations with that person.</span></span> <span data-ttu-id="1326b-138">Сведения и примеры см. в разделе *Нечеткий поиск* статьи [Получение релевантных сведений о людях](/graph/people-example#perform-a-fuzzy-search).</span><span class="sxs-lookup"><span data-stu-id="1326b-138">See the *Perform a fuzzy search* section at [Get relevant information about people](/graph/people-example#perform-a-fuzzy-search) for information and examples.</span></span> |
|<span data-ttu-id="1326b-139">$select</span><span class="sxs-lookup"><span data-stu-id="1326b-139">$select</span></span>|<span data-ttu-id="1326b-140">string</span><span class="sxs-lookup"><span data-stu-id="1326b-140">string</span></span>|<span data-ttu-id="1326b-p105">Список разделенных запятыми свойств, которые необходимо включить в отклик. Для оптимизации производительности выбирайте только необходимые свойства.</span><span class="sxs-lookup"><span data-stu-id="1326b-p105">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>|
|<span data-ttu-id="1326b-143">$skip</span><span class="sxs-lookup"><span data-stu-id="1326b-143">$skip</span></span>|<span data-ttu-id="1326b-144">int</span><span class="sxs-lookup"><span data-stu-id="1326b-144">int</span></span>|<span data-ttu-id="1326b-p106">Пропуск первых n результатов; эту функцию удобно использовать при разбиении результатов на страницы. Эта возможность не поддерживается при использовании параметра *$search*.</span><span class="sxs-lookup"><span data-stu-id="1326b-p106">Skip the first n results, useful for paging. This is not supported when using *$search*.</span></span>|
|<span data-ttu-id="1326b-147">$top</span><span class="sxs-lookup"><span data-stu-id="1326b-147">$top</span></span>|<span data-ttu-id="1326b-148">int</span><span class="sxs-lookup"><span data-stu-id="1326b-148">int</span></span>|<span data-ttu-id="1326b-149">Количество возвращаемых результатов.</span><span class="sxs-lookup"><span data-stu-id="1326b-149">Number of results to be returned.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="1326b-150">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1326b-150">Request headers</span></span>

| <span data-ttu-id="1326b-151">Имя</span><span class="sxs-lookup"><span data-stu-id="1326b-151">Name</span></span>      |<span data-ttu-id="1326b-152">Описание</span><span class="sxs-lookup"><span data-stu-id="1326b-152">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1326b-153">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1326b-153">Authorization</span></span>  | <span data-ttu-id="1326b-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1326b-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1326b-156">Accept</span><span class="sxs-lookup"><span data-stu-id="1326b-156">Accept</span></span> | <span data-ttu-id="1326b-157">application/json</span><span class="sxs-lookup"><span data-stu-id="1326b-157">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="1326b-158">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1326b-158">Request body</span></span>

<span data-ttu-id="1326b-159">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1326b-159">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1326b-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="1326b-160">Response</span></span>

<span data-ttu-id="1326b-p108">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [person](../resources/person.md) в тексте ответа. Отклик может содержать один объект person либо коллекцию объектов person.</span><span class="sxs-lookup"><span data-stu-id="1326b-p108">If successful, this method returns a `200 OK` response code and a collection of [person](../resources/person.md) objects in the response body. The response can contain one person object or a collection of person objects.</span></span>

## <a name="examples"></a><span data-ttu-id="1326b-163">Примеры</span><span class="sxs-lookup"><span data-stu-id="1326b-163">Examples</span></span>

#### <a name="request"></a><span data-ttu-id="1326b-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="1326b-164">Request</span></span>

<span data-ttu-id="1326b-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1326b-165">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="1326b-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="1326b-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_person_collection"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/people
```
# <a name="c"></a>[<span data-ttu-id="1326b-167">C#</span><span class="sxs-lookup"><span data-stu-id="1326b-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-person-collection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1326b-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1326b-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-person-collection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1326b-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1326b-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-person-collection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1326b-170">Java</span><span class="sxs-lookup"><span data-stu-id="1326b-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-person-collection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1326b-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="1326b-171">Response</span></span>

<span data-ttu-id="1326b-172">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="1326b-172">The following is an example of the response.</span></span>

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

<span data-ttu-id="1326b-173">Другие примеры см. в статье [Получение релевантной информации о людях](/graph/people-example).</span><span class="sxs-lookup"><span data-stu-id="1326b-173">For more examples, see the article [Get relevant information about people](/graph/people-example).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List people",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
