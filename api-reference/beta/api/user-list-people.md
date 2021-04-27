---
title: Список людей
description: Получение списка объектов person, упорядоченных по их релевантности для пользователя, которая определяется его моделями общения и совместной работы, а также бизнес-отношениями.
author: dkershaw10
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 8df99c32c43e947863c4a7713c984b99fbd4bb73
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053358"
---
# <a name="list-people"></a><span data-ttu-id="c8d02-103">Список людей</span><span class="sxs-lookup"><span data-stu-id="c8d02-103">List people</span></span>

<span data-ttu-id="c8d02-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8d02-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8d02-105">Извлечение списка объектов [пользователя,](../resources/person.md) заказать по их релевантности для [пользователя,](../resources/user.md)который определяется шаблонами общения и совместной работы пользователя, а также деловыми отношениями.</span><span class="sxs-lookup"><span data-stu-id="c8d02-105">Retrieve a list of [person](../resources/person.md) objects ordered by their relevance to the [user](../resources/user.md), which is determined by the user's communication and collaboration patterns, and business relationships.</span></span>

## <a name="permissions"></a><span data-ttu-id="c8d02-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c8d02-106">Permissions</span></span>

<span data-ttu-id="c8d02-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8d02-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8d02-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c8d02-109">Permission type</span></span>      | <span data-ttu-id="c8d02-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c8d02-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c8d02-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c8d02-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c8d02-112">People.Read</span><span class="sxs-lookup"><span data-stu-id="c8d02-112">People.Read</span></span>    |
|<span data-ttu-id="c8d02-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c8d02-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8d02-114">People.Read</span><span class="sxs-lookup"><span data-stu-id="c8d02-114">People.Read</span></span>    |
|<span data-ttu-id="c8d02-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c8d02-115">Application</span></span> | <span data-ttu-id="c8d02-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8d02-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c8d02-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c8d02-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/people
GET /users/{id | userPrincipalName}/people
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c8d02-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c8d02-118">Optional query parameters</span></span>

<span data-ttu-id="c8d02-119">Этот метод поддерживает следующие параметры запроса OData, чтобы помочь настроить ответ.</span><span class="sxs-lookup"><span data-stu-id="c8d02-119">This method supports the following OData query parameters to help customize the response.</span></span>

|<span data-ttu-id="c8d02-120">Имя</span><span class="sxs-lookup"><span data-stu-id="c8d02-120">Name</span></span>|<span data-ttu-id="c8d02-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c8d02-121">Value</span></span>|<span data-ttu-id="c8d02-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c8d02-122">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="c8d02-123">$filter</span><span class="sxs-lookup"><span data-stu-id="c8d02-123">$filter</span></span>|<span data-ttu-id="c8d02-124">string</span><span class="sxs-lookup"><span data-stu-id="c8d02-124">string</span></span>|<span data-ttu-id="c8d02-125">Позволяет возвращать в отклике только тех людей, чьи записи содержат указанные критерии.</span><span class="sxs-lookup"><span data-stu-id="c8d02-125">Limits the response to only those people whose record contains the specified criteria.</span></span>|
|<span data-ttu-id="c8d02-126">$orderby</span><span class="sxs-lookup"><span data-stu-id="c8d02-126">$orderby</span></span>|<span data-ttu-id="c8d02-127">строка</span><span class="sxs-lookup"><span data-stu-id="c8d02-127">string</span></span>|<span data-ttu-id="c8d02-128">По умолчанию люди в ответе сортируются по степени соответствия запросу.</span><span class="sxs-lookup"><span data-stu-id="c8d02-128">By default the people in the response are sorted by their relevance to your query.</span></span> <span data-ttu-id="c8d02-129">Этот порядок можно изменить с помощью параметра *$orderby*.</span><span class="sxs-lookup"><span data-stu-id="c8d02-129">You can change the order of the people in the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="c8d02-130">$search</span><span class="sxs-lookup"><span data-stu-id="c8d02-130">$search</span></span>|<span data-ttu-id="c8d02-131">string</span><span class="sxs-lookup"><span data-stu-id="c8d02-131">string</span></span>|<span data-ttu-id="c8d02-132">Поиск пользователей по имени или псевдониму.</span><span class="sxs-lookup"><span data-stu-id="c8d02-132">Search for people by name or alias.</span></span> <span data-ttu-id="c8d02-133">Поддерживается нечеткое соответствие.</span><span class="sxs-lookup"><span data-stu-id="c8d02-133">Supports Fuzzy matching.</span></span> <span data-ttu-id="c8d02-134">Параметр применяется только для поиска людей, относящихся к вошедшему пользователю, а не для поиска людей, относящихся к другим пользователям.</span><span class="sxs-lookup"><span data-stu-id="c8d02-134">Parameter only works for searching the signed-in user's relevant people, not for searching people relevant to other users.</span></span> <span data-ttu-id="c8d02-135">Также поддерживает ключевое слово `topic` для поиска людей с учетом тем, извлеченных из бесед электронной почты с определенным человеком.</span><span class="sxs-lookup"><span data-stu-id="c8d02-135">Also supports the `topic` keyword to find people based on topics extracted from e-mail conversations with that person.</span></span> <span data-ttu-id="c8d02-136">Сведения и примеры см. в разделе *Нечеткий поиск* статьи [Получение релевантных сведений о людях](/graph/people-example#perform-a-fuzzy-search).</span><span class="sxs-lookup"><span data-stu-id="c8d02-136">See the *Perform a fuzzy search* section at [Get relevant information about people](/graph/people-example#perform-a-fuzzy-search) for information and examples.</span></span>|
|<span data-ttu-id="c8d02-137">$select</span><span class="sxs-lookup"><span data-stu-id="c8d02-137">$select</span></span>|<span data-ttu-id="c8d02-138">string</span><span class="sxs-lookup"><span data-stu-id="c8d02-138">string</span></span>|<span data-ttu-id="c8d02-p104">Список разделенных запятыми свойств, которые необходимо включить в отклик. Для оптимизации производительности выбирайте только необходимые свойства.</span><span class="sxs-lookup"><span data-stu-id="c8d02-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>|
|<span data-ttu-id="c8d02-141">$skip</span><span class="sxs-lookup"><span data-stu-id="c8d02-141">$skip</span></span>|<span data-ttu-id="c8d02-142">int</span><span class="sxs-lookup"><span data-stu-id="c8d02-142">int</span></span>|<span data-ttu-id="c8d02-p105">Пропуск первых n результатов; эту функцию удобно использовать при разбиении результатов на страницы. Эта возможность не поддерживается при использовании параметра *$search*.</span><span class="sxs-lookup"><span data-stu-id="c8d02-p105">Skip the first n results, useful for paging. This is not supported when using *$search*.</span></span>|
|<span data-ttu-id="c8d02-145">$top</span><span class="sxs-lookup"><span data-stu-id="c8d02-145">$top</span></span>|<span data-ttu-id="c8d02-146">int</span><span class="sxs-lookup"><span data-stu-id="c8d02-146">int</span></span>|<span data-ttu-id="c8d02-147">Количество возвращаемых результатов.</span><span class="sxs-lookup"><span data-stu-id="c8d02-147">Number of results to be returned.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="c8d02-148">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c8d02-148">Request headers</span></span>

| <span data-ttu-id="c8d02-149">Имя</span><span class="sxs-lookup"><span data-stu-id="c8d02-149">Name</span></span>      |<span data-ttu-id="c8d02-150">Описание</span><span class="sxs-lookup"><span data-stu-id="c8d02-150">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c8d02-151">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c8d02-151">Authorization</span></span>  | <span data-ttu-id="c8d02-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c8d02-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c8d02-154">Accept</span><span class="sxs-lookup"><span data-stu-id="c8d02-154">Accept</span></span> | <span data-ttu-id="c8d02-155">application/json</span><span class="sxs-lookup"><span data-stu-id="c8d02-155">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="c8d02-156">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c8d02-156">Request body</span></span>

<span data-ttu-id="c8d02-157">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c8d02-157">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8d02-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8d02-158">Response</span></span>

<span data-ttu-id="c8d02-159">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [лиц](../resources/person.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c8d02-159">If successful, this method returns a `200 OK` response code and a collection of [person](../resources/person.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c8d02-160">Примеры</span><span class="sxs-lookup"><span data-stu-id="c8d02-160">Examples</span></span>

### <a name="browse"></a><span data-ttu-id="c8d02-161">Просмотр</span><span class="sxs-lookup"><span data-stu-id="c8d02-161">Browse</span></span>

<span data-ttu-id="c8d02-162">Запросы в этом разделе получают людей, наиболее релевантных для пользователя, подписанного (), на основе связи, совместной работы `/me` и деловых отношений.</span><span class="sxs-lookup"><span data-stu-id="c8d02-162">The requests in this section get the people most relevant to the signed-in user (`/me`), based on communication, collaboration, and business relationships.</span></span>

<span data-ttu-id="c8d02-163">По умолчанию каждый ответ возвращает 10 записей, но изменить его можно с *помощью $top* параметра.</span><span class="sxs-lookup"><span data-stu-id="c8d02-163">By default, each response returns 10 records, but you can change this using the *$top* parameter.</span></span> <span data-ttu-id="c8d02-164">Эти запросы требуют разрешения People.Read.</span><span class="sxs-lookup"><span data-stu-id="c8d02-164">These requests require the People.Read permission.</span></span>

#### <a name="request"></a><span data-ttu-id="c8d02-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="c8d02-165">Request</span></span>

<span data-ttu-id="c8d02-166">Ниже приводится пример запроса по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="c8d02-166">The following is an example of the default request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c8d02-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="c8d02-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_person_collection_beta"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/people
```
# <a name="c"></a>[<span data-ttu-id="c8d02-168">C#</span><span class="sxs-lookup"><span data-stu-id="c8d02-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-person-collection-beta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c8d02-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c8d02-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-person-collection-beta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c8d02-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c8d02-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-person-collection-beta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c8d02-171">Java</span><span class="sxs-lookup"><span data-stu-id="c8d02-171">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-person-collection-beta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c8d02-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8d02-172">Response</span></span>

<span data-ttu-id="c8d02-173">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c8d02-173">The following is an example of the response.</span></span>
><span data-ttu-id="c8d02-174">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c8d02-174">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_person_collection_beta",
  "truncated": true,
  "@odata.type": "microsoft.graph.person",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1326

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
            "title": null,
            "companyName": null,
            "yomiCompany": "",
            "department": null,
            "officeLocation": null,
            "profession": "",
            "mailboxType": "GroupMailbox",
            "personType": "ModernGroup",
            "userPrincipalName": "",
            "emailAddresses": [
                {
                    "address": "Marketing@contoso.com",
                    "rank": 30
                }
            ],
            "phones": [],
            "postalAddresses": [],
            "websites": [],
            "sources": [
                {
                    "type": "Directory"
                }
            ]
        },
        {
            "id": "e3d0513b-449e-4198-ba6f-bd97ae7cae85",
            "displayName": "Isaiah Langer",
            "givenName": "Isaiah",
            "surname": "Langer",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "title": "Web Marketing Manager",
            "companyName": null,
            "yomiCompany": "",
            "department": "Sales & Marketing",
            "officeLocation": "20/1101",
            "profession": "",
            "mailboxType": "Mailbox",
            "personType": "Person",
            "userPrincipalName": "IsaiahL@contoso.com",
            "emailAddresses": [
                {
                    "address": "IsaiahL@contoso.com",
                    "rank": 20
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
            "sources": [
                {
                    "type": "Directory"
                }
            ]
        }
    ]
}
```

#### <a name="requesting-a-subsequent-page-of-people"></a><span data-ttu-id="c8d02-175">Запрос последующей страницы людей</span><span class="sxs-lookup"><span data-stu-id="c8d02-175">Requesting a subsequent page of people</span></span>

<span data-ttu-id="c8d02-p108">Если в первом отклике содержится неполный список релевантных людей, вы можете создать второй запрос, используя параметры *$top* и *$skip*, чтобы запросить дополнительные страницы информации. Если в предыдущем запросе есть дополнительная информация, то при последующем запросе будет получена следующая страница с людьми с сервера.</span><span class="sxs-lookup"><span data-stu-id="c8d02-p108">If the first response does not contain the complete list of relevant people, you can make a second request using *$top* and *$skip* to request additional pages of information. If the previous request has additional information, the following request gets the next page of people from the server.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$top=10&$skip=10
```

#### <a name="sort-the-response"></a><span data-ttu-id="c8d02-178">Сортировка в отклике</span><span class="sxs-lookup"><span data-stu-id="c8d02-178">Sort the response</span></span>

<span data-ttu-id="c8d02-179">По умолчанию люди в ответе сортируются по степени соответствия запросу.</span><span class="sxs-lookup"><span data-stu-id="c8d02-179">By default the people in the response are sorted by their relevance to your query.</span></span> <span data-ttu-id="c8d02-180">Этот порядок можно изменить с помощью параметра *$orderby*.</span><span class="sxs-lookup"><span data-stu-id="c8d02-180">You can change the order of the people in the response using the *$orderby* parameter.</span></span> <span data-ttu-id="c8d02-181">Этот запрос выбирает наиболее подходящих для вас людей, сортировать их по их имени отображения, а затем возвращает первых 10 человек в отсортировали список.</span><span class="sxs-lookup"><span data-stu-id="c8d02-181">This query selects the people most relevant to you, sorts them by their display name, and then returns the first 10 people on the sorted list.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$orderby=DisplayName
```

#### <a name="changing-the-number-of-people-returned-and-the-fields-returned"></a><span data-ttu-id="c8d02-182">Изменение количества возвращаемого и возвращаемого поля</span><span class="sxs-lookup"><span data-stu-id="c8d02-182">Changing the number of people returned and the fields returned</span></span>

<span data-ttu-id="c8d02-183">Вы можете изменить количество людей, возвращаемых в отклике, настроив параметр *$top*.</span><span class="sxs-lookup"><span data-stu-id="c8d02-183">You can change the number of people returned in the response by setting the *$top* parameter.</span></span>

<span data-ttu-id="c8d02-184">В следующем примере запрашивается 1000 человек, наиболее подходящих для `/me` .</span><span class="sxs-lookup"><span data-stu-id="c8d02-184">The following example requests the 1,000 people most relevant to `/me`.</span></span> <span data-ttu-id="c8d02-185">Запрос также ограничивает объем данных, отосланных с сервера, запрашивая только отображаемую фамилию человека.</span><span class="sxs-lookup"><span data-stu-id="c8d02-185">The request also limits the amount of data sent back from the server by requesting only the display name of the person.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$top=1000&$select=DisplayName
```

#### <a name="selecting-the-fields-to-return"></a><span data-ttu-id="c8d02-186">Выбор полей для возврата</span><span class="sxs-lookup"><span data-stu-id="c8d02-186">Selecting the fields to return</span></span>

<span data-ttu-id="c8d02-187">Можно ограничить количество данных, возвращаемого с сервера, с помощью *параметра $select* для выбора одного или более полей.</span><span class="sxs-lookup"><span data-stu-id="c8d02-187">You can limit the amount of data returned from the server by using the *$select* parameter to choose one or more fields.</span></span> <span data-ttu-id="c8d02-188">Поле *@odata.id* всегда возвращается.</span><span class="sxs-lookup"><span data-stu-id="c8d02-188">The *@odata.id* field is always returned.</span></span>

<span data-ttu-id="c8d02-189">В следующем примере ограничивается ответ *на displayName* и *EmailAddress* 10 наиболее релевантного пользователя.</span><span class="sxs-lookup"><span data-stu-id="c8d02-189">The following example limits the response to the *DisplayName* and *EmailAddress* of the 10 most relevant people.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$select=DisplayName,EmailAddresses
```

#### <a name="using-a-filter-to-limit-the-response"></a><span data-ttu-id="c8d02-190">Использование фильтра для ограничения отклика</span><span class="sxs-lookup"><span data-stu-id="c8d02-190">Using a filter to limit the response</span></span>

<span data-ttu-id="c8d02-191">Вы можете использовать параметр *$filter*, чтобы ограничить количество информации в отклике и возвращать только тех людей, записи которых содержат указанные критерии.</span><span class="sxs-lookup"><span data-stu-id="c8d02-191">You can use the *$filter* parameter to limit the response to only those people whose record contains the specified criteria.</span></span>

<span data-ttu-id="c8d02-192">Следующий запрос ограничивает ответ для людей с исходным кодом "Directory".</span><span class="sxs-lookup"><span data-stu-id="c8d02-192">The following query limits the response to people with the source "Directory."</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$filter=Sources/Any (source: source/Type  eq 'Directory')
```

#### <a name="selecting-the-fields-to-return-in-a-filtered-response"></a><span data-ttu-id="c8d02-193">Выбор полей для возврата в отфильтрованный ответ</span><span class="sxs-lookup"><span data-stu-id="c8d02-193">Selecting the fields to return in a filtered response</span></span>

<span data-ttu-id="c8d02-194">Сочетая параметры *$select* и *$filter*, вы можете создать настраиваемый список людей, релевантных для пользователя, и получать только те поля, которые необходимы вашему приложению.</span><span class="sxs-lookup"><span data-stu-id="c8d02-194">You can combine the *$select* and *$filter* parameters to create a custom list of people relevant to the user and get only the fields that your application needs.</span></span>

<span data-ttu-id="c8d02-195">В следующем примере *получается DisplayName* и *EmailAddress* людей, имя отображения которых равно указанному имени.</span><span class="sxs-lookup"><span data-stu-id="c8d02-195">The following example gets the *DisplayName* and *EmailAddress* of people whose display name equals the specified name.</span></span> <span data-ttu-id="c8d02-196">В этом примере возвращаются только те, чье имя отображения равно "Nestor Kellum".</span><span class="sxs-lookup"><span data-stu-id="c8d02-196">In this example, only people whose display name equals "Nestor Kellum" are returned.</span></span>

```http
+GET https://graph.microsoft.com/beta/me/people/?$select=DisplayName,EmailAddresses&$filter=DisplayName eq 'Nestor Kellum'
```

### <a name="search-people"></a><span data-ttu-id="c8d02-197">Поиск людей</span><span class="sxs-lookup"><span data-stu-id="c8d02-197">Search people</span></span>

<span data-ttu-id="c8d02-198">Запросы в этом разделе также получают людей, наиболее релевантные для пользователя, заявив о подписании `/me` ( ).</span><span class="sxs-lookup"><span data-stu-id="c8d02-198">The requests in this section also get the people most relevant to the signed-in user (`/me`).</span></span> <span data-ttu-id="c8d02-199">Запросы на поиск требуют разрешения People.Read.</span><span class="sxs-lookup"><span data-stu-id="c8d02-199">Search requests require the People.Read permission.</span></span>

#### <a name="using-search-to-select-people"></a><span data-ttu-id="c8d02-200">Использование поиска для выбора людей</span><span class="sxs-lookup"><span data-stu-id="c8d02-200">Using search to select people</span></span>

<span data-ttu-id="c8d02-201">Используйте параметр *$search* для выбора людей, удовлетворяющих определенному набору критериев.</span><span class="sxs-lookup"><span data-stu-id="c8d02-201">Use the *$search* parameter to select people who meet a particular set of criteria.</span></span>

<span data-ttu-id="c8d02-202">В следующем поисковом запросе возвращаются люди, для которых GivenName или Surname начинается с `/me` буквы "j".</span><span class="sxs-lookup"><span data-stu-id="c8d02-202">The following search query returns people relevant to `/me` whose GivenName or Surname begins with the letter "j".</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$search=j
```

#### <a name="using-search-to-specify-a-relevant-topic"></a><span data-ttu-id="c8d02-203">Использование поиска для указания соответствующей темы</span><span class="sxs-lookup"><span data-stu-id="c8d02-203">Using search to specify a relevant topic</span></span>

<span data-ttu-id="c8d02-204">Следующий запрос возвращает людей, имя которых содержит "ma" и которые имеют связь с `/me` "планированием функций".</span><span class="sxs-lookup"><span data-stu-id="c8d02-204">The following request returns people relevant to `/me` whose name contains "ma" and who have an association with "feature planning."</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$search="ma topic: feature planning"
```

#### <a name="performing-a-fuzzy-search"></a><span data-ttu-id="c8d02-205">Выполнение нечеткого поиска</span><span class="sxs-lookup"><span data-stu-id="c8d02-205">Performing a fuzzy search</span></span>

<span data-ttu-id="c8d02-206">Следующий запрос — поиск человека с именем "Hermaini Hall".</span><span class="sxs-lookup"><span data-stu-id="c8d02-206">The following request does a search for a person named "Hermaini Hall."</span></span> <span data-ttu-id="c8d02-207">Поскольку существует лицо с именем "Herminia Hull", соответствующее подписанной пользователю, возвращается информация для "Herminia Hull".</span><span class="sxs-lookup"><span data-stu-id="c8d02-207">Because there is a person named "Herminia Hull" relevant to the signed-in user, the information for "Herminia Hull" is returned.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$search="hermaini hall"
```

### <a name="related-people"></a><span data-ttu-id="c8d02-208">Связанные люди</span><span class="sxs-lookup"><span data-stu-id="c8d02-208">Related people</span></span>

<span data-ttu-id="c8d02-209">Следующий запрос получает людей, наиболее релевантные другому лицу в организации пользователя.</span><span class="sxs-lookup"><span data-stu-id="c8d02-209">The following request gets the people most relevant to another person in the user's organization.</span></span> <span data-ttu-id="c8d02-210">Для этого запроса требуется разрешение User.ReadBasic.All для людей.Read.All.</span><span class="sxs-lookup"><span data-stu-id="c8d02-210">This request requires the User.ReadBasic.All for People.Read.All permission.</span></span> <span data-ttu-id="c8d02-211">В этом примере отображаются соответствующие люди Nestor Kellum.</span><span class="sxs-lookup"><span data-stu-id="c8d02-211">In this example, Nestor Kellum's relevant people are displayed.</span></span>

```http
GET https://graph.microsoft.com/beta/users('nestork@contoso.com')/people/
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List people",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


