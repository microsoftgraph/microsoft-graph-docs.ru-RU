---
title: Список людей
description: Получение списка объектов person, упорядоченные по их важности для пользователя, который определяет, какие связи и совместной работы шаблоны и устанавливать деловые контакты пользователя.
author: dkershaw10
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 4233c0bc4015525bb474499366c084483ceaefe7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925044"
---
# <a name="list-people"></a><span data-ttu-id="7fa47-103">Список людей</span><span class="sxs-lookup"><span data-stu-id="7fa47-103">List people</span></span>

> <span data-ttu-id="7fa47-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7fa47-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7fa47-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7fa47-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7fa47-106">Получение списка объектов [person](../resources/person.md) , упорядоченные по их важности для [пользователя](../resources/user.md), который определяет, какие связи и совместной работы шаблоны и устанавливать деловые контакты пользователя.</span><span class="sxs-lookup"><span data-stu-id="7fa47-106">Retrieve a list of [person](../resources/person.md) objects ordered by their relevance to the [user](../resources/user.md), which is determined by the user's communication and collaboration patterns, and business relationships.</span></span>

## <a name="permissions"></a><span data-ttu-id="7fa47-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7fa47-107">Permissions</span></span>

<span data-ttu-id="7fa47-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7fa47-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7fa47-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7fa47-110">Permission type</span></span>      | <span data-ttu-id="7fa47-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7fa47-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7fa47-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7fa47-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7fa47-113">People.Read</span><span class="sxs-lookup"><span data-stu-id="7fa47-113">People.Read</span></span>    |
|<span data-ttu-id="7fa47-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7fa47-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7fa47-115">People.Read</span><span class="sxs-lookup"><span data-stu-id="7fa47-115">People.Read</span></span>    |
|<span data-ttu-id="7fa47-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7fa47-116">Application</span></span> | <span data-ttu-id="7fa47-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7fa47-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7fa47-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7fa47-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/people
GET /users/{id | userPrincipalName}/people
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7fa47-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7fa47-119">Optional query parameters</span></span>

<span data-ttu-id="7fa47-120">Этот метод поддерживает следующие параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7fa47-120">This method supports the following OData query parameters to help customize the response.</span></span>

|<span data-ttu-id="7fa47-121">Имя</span><span class="sxs-lookup"><span data-stu-id="7fa47-121">Name</span></span>|<span data-ttu-id="7fa47-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7fa47-122">Value</span></span>|<span data-ttu-id="7fa47-123">Описание</span><span class="sxs-lookup"><span data-stu-id="7fa47-123">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="7fa47-124">$filter</span><span class="sxs-lookup"><span data-stu-id="7fa47-124">$filter</span></span>|<span data-ttu-id="7fa47-125">string</span><span class="sxs-lookup"><span data-stu-id="7fa47-125">string</span></span>|<span data-ttu-id="7fa47-126">Позволяет возвращать в отклике только тех людей, чьи записи содержат указанные критерии.</span><span class="sxs-lookup"><span data-stu-id="7fa47-126">Limits the response to only those people whose record contains the specified criteria.</span></span>|
|<span data-ttu-id="7fa47-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="7fa47-127">$orderby</span></span>|<span data-ttu-id="7fa47-128">строка</span><span class="sxs-lookup"><span data-stu-id="7fa47-128">string</span></span>|<span data-ttu-id="7fa47-129">По умолчанию люди в ответе сортируются по степени соответствия запросу.</span><span class="sxs-lookup"><span data-stu-id="7fa47-129">By default the people in the response are sorted by their relevance to your query.</span></span> <span data-ttu-id="7fa47-130">Этот порядок можно изменить с помощью параметра *$orderby*.</span><span class="sxs-lookup"><span data-stu-id="7fa47-130">You can change the order of the people in the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="7fa47-131">$search</span><span class="sxs-lookup"><span data-stu-id="7fa47-131">$search</span></span>|<span data-ttu-id="7fa47-132">string</span><span class="sxs-lookup"><span data-stu-id="7fa47-132">string</span></span>|<span data-ttu-id="7fa47-133">Поиск пользователей по имени или псевдониму.</span><span class="sxs-lookup"><span data-stu-id="7fa47-133">Search for people by name or alias.</span></span> <span data-ttu-id="7fa47-134">Поддерживается нечеткое соответствие.</span><span class="sxs-lookup"><span data-stu-id="7fa47-134">Supports Fuzzy matching.</span></span> <span data-ttu-id="7fa47-135">Параметр работает только при поиске людей соответствующий пользователь выполнил вход, не для поиска людей, предназначенных для других пользователей.</span><span class="sxs-lookup"><span data-stu-id="7fa47-135">Parameter only works for searching the signed-in user's relevant people, not for searching people relevant to other users.</span></span> <span data-ttu-id="7fa47-136">Также поддерживает `topic` ключевое слово для поиска людей на основании разделы, извлеченные из сообщений электронной почты с этим контактом.</span><span class="sxs-lookup"><span data-stu-id="7fa47-136">Also supports the `topic` keyword to find people based on topics extracted from e-mail conversations with that person.</span></span> <span data-ttu-id="7fa47-137">В разделе *Perform Нечеткое поиска* в [получить информацию о пользователях](/graph/people-example#perform-a-fuzzy-search) сведения и примеры.</span><span class="sxs-lookup"><span data-stu-id="7fa47-137">See the *Perform a fuzzy search* section at [Get relevant information about people](/graph/people-example#perform-a-fuzzy-search) for information and examples.</span></span>|
|<span data-ttu-id="7fa47-138">$select</span><span class="sxs-lookup"><span data-stu-id="7fa47-138">$select</span></span>|<span data-ttu-id="7fa47-139">string</span><span class="sxs-lookup"><span data-stu-id="7fa47-139">string</span></span>|<span data-ttu-id="7fa47-p105">Список разделенных запятыми свойств, которые необходимо включить в отклик. Для оптимизации производительности выбирайте только необходимые свойства.</span><span class="sxs-lookup"><span data-stu-id="7fa47-p105">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>|
|<span data-ttu-id="7fa47-142">$skip</span><span class="sxs-lookup"><span data-stu-id="7fa47-142">$skip</span></span>|<span data-ttu-id="7fa47-143">int</span><span class="sxs-lookup"><span data-stu-id="7fa47-143">int</span></span>|<span data-ttu-id="7fa47-p106">Пропуск первых n результатов; эту функцию удобно использовать при разбиении результатов на страницы. Эта возможность не поддерживается при использовании параметра *$search*.</span><span class="sxs-lookup"><span data-stu-id="7fa47-p106">Skip the first n results, useful for paging. This is not supported when using *$search*.</span></span>|
|<span data-ttu-id="7fa47-146">$top</span><span class="sxs-lookup"><span data-stu-id="7fa47-146">$top</span></span>|<span data-ttu-id="7fa47-147">int</span><span class="sxs-lookup"><span data-stu-id="7fa47-147">int</span></span>|<span data-ttu-id="7fa47-148">Количество возвращаемых результатов.</span><span class="sxs-lookup"><span data-stu-id="7fa47-148">Number of results to be returned.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="7fa47-149">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7fa47-149">Request headers</span></span>

| <span data-ttu-id="7fa47-150">Имя</span><span class="sxs-lookup"><span data-stu-id="7fa47-150">Name</span></span>      |<span data-ttu-id="7fa47-151">Описание</span><span class="sxs-lookup"><span data-stu-id="7fa47-151">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7fa47-152">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7fa47-152">Authorization</span></span>  | <span data-ttu-id="7fa47-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7fa47-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7fa47-155">Accept</span><span class="sxs-lookup"><span data-stu-id="7fa47-155">Accept</span></span> | <span data-ttu-id="7fa47-156">application/json</span><span class="sxs-lookup"><span data-stu-id="7fa47-156">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="7fa47-157">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7fa47-157">Request body</span></span>

<span data-ttu-id="7fa47-158">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7fa47-158">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7fa47-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="7fa47-159">Response</span></span>

<span data-ttu-id="7fa47-160">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [человека](../resources/person.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="7fa47-160">If successful, this method returns a `200 OK` response code and a collection of [person](../resources/person.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7fa47-161">Примеры</span><span class="sxs-lookup"><span data-stu-id="7fa47-161">Examples</span></span>

### <a name="browse"></a><span data-ttu-id="7fa47-162">Обзор</span><span class="sxs-lookup"><span data-stu-id="7fa47-162">Browse</span></span>

<span data-ttu-id="7fa47-163">Запросы в этом разделе получить наиболее важные, чтобы пользователь выполнил вход пользователей (`/me`), в зависимости от связи, совместной работы и деловыми отношениями.</span><span class="sxs-lookup"><span data-stu-id="7fa47-163">The requests in this section get the people most relevant to the signed-in user (`/me`), based on communication, collaboration, and business relationships.</span></span>

<span data-ttu-id="7fa47-164">По умолчанию каждый отклик возвращает 10 записей, но его можно изменить с помощью параметра *$top* .</span><span class="sxs-lookup"><span data-stu-id="7fa47-164">By default, each response returns 10 records, but you can change this using the *$top* parameter.</span></span> <span data-ttu-id="7fa47-165">Эти запросы требуется разрешение People.Read.</span><span class="sxs-lookup"><span data-stu-id="7fa47-165">These requests require the People.Read permission.</span></span>

#### <a name="request"></a><span data-ttu-id="7fa47-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="7fa47-166">Request</span></span>

<span data-ttu-id="7fa47-167">Ниже приведен пример запроса по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="7fa47-167">The following is an example of the default request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_person_collection_beta"
}-->

```http
GET https://graph.microsoft.com/beta/me/people
```

#### <a name="response"></a><span data-ttu-id="7fa47-168">Ответ</span><span class="sxs-lookup"><span data-stu-id="7fa47-168">Response</span></span>

<span data-ttu-id="7fa47-169">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7fa47-169">The following is an example of the response.</span></span>
><span data-ttu-id="7fa47-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7fa47-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

#### <a name="requesting-a-subsequent-page-of-people"></a><span data-ttu-id="7fa47-172">Разрешения на запрос следующей странице людей</span><span class="sxs-lookup"><span data-stu-id="7fa47-172">Requesting a subsequent page of people</span></span>

<span data-ttu-id="7fa47-p110">Если в первом отклике содержится неполный список релевантных людей, вы можете создать второй запрос, используя параметры *$top* и *$skip*, чтобы запросить дополнительные страницы информации. Если в предыдущем запросе есть дополнительная информация, то при последующем запросе будет получена следующая страница с людьми с сервера.</span><span class="sxs-lookup"><span data-stu-id="7fa47-p110">If the first response does not contain the complete list of relevant people, you can make a second request using *$top* and *$skip* to request additional pages of information. If the previous request has additional information, the following request gets the next page of people from the server.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$top=10&$skip=10
```

#### <a name="sort-the-response"></a><span data-ttu-id="7fa47-175">Сортировка в отклике</span><span class="sxs-lookup"><span data-stu-id="7fa47-175">Sort the response</span></span>

<span data-ttu-id="7fa47-176">По умолчанию люди в ответе сортируются по степени соответствия запросу.</span><span class="sxs-lookup"><span data-stu-id="7fa47-176">By default the people in the response are sorted by their relevance to your query.</span></span> <span data-ttu-id="7fa47-177">Этот порядок можно изменить с помощью параметра *$orderby*.</span><span class="sxs-lookup"><span data-stu-id="7fa47-177">You can change the order of the people in the response using the *$orderby* parameter.</span></span> <span data-ttu-id="7fa47-178">Этот запрос выбирает наиболее важные для вас людей, их сортировка по их отображаемое имя и затем возвращаются первые 10 пользователей на отсортированный список.</span><span class="sxs-lookup"><span data-stu-id="7fa47-178">This query selects the people most relevant to you, sorts them by their display name, and then returns the first 10 people on the sorted list.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$orderby=DisplayName
```

#### <a name="changing-the-number-of-people-returned-and-the-fields-returned"></a><span data-ttu-id="7fa47-179">Изменение числа возвращаемых людей и поля</span><span class="sxs-lookup"><span data-stu-id="7fa47-179">Changing the number of people returned and the fields returned</span></span>

<span data-ttu-id="7fa47-180">Вы можете изменить количество людей, возвращаемых в отклике, настроив параметр *$top*.</span><span class="sxs-lookup"><span data-stu-id="7fa47-180">You can change the number of people returned in the response by setting the *$top* parameter.</span></span>

<span data-ttu-id="7fa47-181">Следующий пример запрашивает 1 000 пользователей, наиболее подходящих для `/me`.</span><span class="sxs-lookup"><span data-stu-id="7fa47-181">The following example requests the 1,000 people most relevant to `/me`.</span></span> <span data-ttu-id="7fa47-182">Запрос также ограничивает объем данных, отправленных с сервера, запрашивая только отображаемое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="7fa47-182">The request also limits the amount of data sent back from the server by requesting only the display name of the person.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$top=1000&$select=DisplayName
```

#### <a name="selecting-the-fields-to-return"></a><span data-ttu-id="7fa47-183">Выбор полей для возврата</span><span class="sxs-lookup"><span data-stu-id="7fa47-183">Selecting the fields to return</span></span>

<span data-ttu-id="7fa47-184">Можно ограничить объем данных, возвращаемых с сервера с помощью параметра *$select* выбрать одно или несколько полей.</span><span class="sxs-lookup"><span data-stu-id="7fa47-184">You can limit the amount of data returned from the server by using the *$select* parameter to choose one or more fields.</span></span> <span data-ttu-id="7fa47-185">В поле *@odata.id* всегда возвращается.</span><span class="sxs-lookup"><span data-stu-id="7fa47-185">The *@odata.id* field is always returned.</span></span>

<span data-ttu-id="7fa47-186">В следующем примере ограничиваются ответ на *DisplayName* и *EmailAddress* 10 наиболее подходящих людей.</span><span class="sxs-lookup"><span data-stu-id="7fa47-186">The following example limits the response to the *DisplayName* and *EmailAddress* of the 10 most relevant people.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$select=DisplayName,EmailAddresses
```

#### <a name="using-a-filter-to-limit-the-response"></a><span data-ttu-id="7fa47-187">С помощью фильтра для ограничения ответа</span><span class="sxs-lookup"><span data-stu-id="7fa47-187">Using a filter to limit the response</span></span>

<span data-ttu-id="7fa47-188">Вы можете использовать параметр *$filter*, чтобы ограничить количество информации в отклике и возвращать только тех людей, записи которых содержат указанные критерии.</span><span class="sxs-lookup"><span data-stu-id="7fa47-188">You can use the *$filter* parameter to limit the response to only those people whose record contains the specified criteria.</span></span>

<span data-ttu-id="7fa47-189">Следующий запрос ограничивает ответа для людей с источником «Каталог».</span><span class="sxs-lookup"><span data-stu-id="7fa47-189">The following query limits the response to people with the source "Directory."</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$filter=Sources/Any (source: source/Type  eq 'Directory')
```

#### <a name="selecting-the-fields-to-return-in-a-filtered-response"></a><span data-ttu-id="7fa47-190">Выбор полей для возврата в отфильтрованные ответа</span><span class="sxs-lookup"><span data-stu-id="7fa47-190">Selecting the fields to return in a filtered response</span></span>

<span data-ttu-id="7fa47-191">Сочетая параметры *$select* и *$filter*, вы можете создать настраиваемый список людей, релевантных для пользователя, и получать только те поля, которые необходимы вашему приложению.</span><span class="sxs-lookup"><span data-stu-id="7fa47-191">You can combine the *$select* and *$filter* parameters to create a custom list of people relevant to the user and get only the fields that your application needs.</span></span>

<span data-ttu-id="7fa47-192">В следующем примере получается *DisplayName* и *EmailAddress* людей, отображаемое имя равно указанному имени.</span><span class="sxs-lookup"><span data-stu-id="7fa47-192">The following example gets the *DisplayName* and *EmailAddress* of people whose display name equals the specified name.</span></span> <span data-ttu-id="7fa47-193">В этом примере возвращаются только тех, отображаемое имя равно «Nestor Kellum».</span><span class="sxs-lookup"><span data-stu-id="7fa47-193">In this example, only people whose display name equals "Nestor Kellum" are returned.</span></span>

```http
+GET https://graph.microsoft.com/beta/me/people/?$select=DisplayName,EmailAddresses&$filter=DisplayName eq 'Nestor Kellum'
```

### <a name="search-people"></a><span data-ttu-id="7fa47-194">Поиск людей</span><span class="sxs-lookup"><span data-stu-id="7fa47-194">Search people</span></span>

<span data-ttu-id="7fa47-195">Запросы в этом разделе также получить людей самые точные, чтобы пользователь выполнил вход (`/me`).</span><span class="sxs-lookup"><span data-stu-id="7fa47-195">The requests in this section also get the people most relevant to the signed-in user (`/me`).</span></span> <span data-ttu-id="7fa47-196">Запросы поиска требуется разрешение People.Read.</span><span class="sxs-lookup"><span data-stu-id="7fa47-196">Search requests require the People.Read permission.</span></span>

#### <a name="using-search-to-select-people"></a><span data-ttu-id="7fa47-197">Использование поиска для выбора людей</span><span class="sxs-lookup"><span data-stu-id="7fa47-197">Using search to select people</span></span>

<span data-ttu-id="7fa47-198">Используйте параметр *$search* для выбора людей, удовлетворяющих определенному набору критериев.</span><span class="sxs-lookup"><span data-stu-id="7fa47-198">Use the *$search* parameter to select people who meet a particular set of criteria.</span></span>

<span data-ttu-id="7fa47-199">Следующий запрос поиска возвращает людей, относящиеся к `/me` , GivenName или фамилию начинается с буквы «j».</span><span class="sxs-lookup"><span data-stu-id="7fa47-199">The following search query returns people relevant to `/me` whose GivenName or Surname begins with the letter "j".</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$search=j
```

#### <a name="using-search-to-specify-a-relevant-topic"></a><span data-ttu-id="7fa47-200">Использование поиска для указания соответствующей темы</span><span class="sxs-lookup"><span data-stu-id="7fa47-200">Using search to specify a relevant topic</span></span>

<span data-ttu-id="7fa47-201">Следующий запрос возвращает людей, относящиеся к `/me` , имя которого содержит «ma» и пользователей, которые имеют связь с «планирование компонентов».</span><span class="sxs-lookup"><span data-stu-id="7fa47-201">The following request returns people relevant to `/me` whose name contains "ma" and who have an association with "feature planning."</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$search="ma topic: feature planning"
```

#### <a name="performing-a-fuzzy-search"></a><span data-ttu-id="7fa47-202">Для выполнения Нечеткое поиска</span><span class="sxs-lookup"><span data-stu-id="7fa47-202">Performing a fuzzy search</span></span>

<span data-ttu-id="7fa47-203">Следующий запрос поиска для пользователя с именем «Зал Hermaini».</span><span class="sxs-lookup"><span data-stu-id="7fa47-203">The following request does a search for a person named "Hermaini Hall."</span></span> <span data-ttu-id="7fa47-204">Так как пользователь с именем «Herminia оболочка» относится к пользователь выполнил вход, возвращается информация для «Herminia оболочка».</span><span class="sxs-lookup"><span data-stu-id="7fa47-204">Because there is a person named "Herminia Hull" relevant to the signed-in user, the information for "Herminia Hull" is returned.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$search="hermaini hall"
```

### <a name="related-people"></a><span data-ttu-id="7fa47-205">Связанные людей</span><span class="sxs-lookup"><span data-stu-id="7fa47-205">Related people</span></span>

<span data-ttu-id="7fa47-206">Следующий запрос получает наиболее подходящих другому пользователю людей в организации пользователя.</span><span class="sxs-lookup"><span data-stu-id="7fa47-206">The following request gets the people most relevant to another person in the user's organization.</span></span> <span data-ttu-id="7fa47-207">Этот запрос требует User.ReadBasic.All People.Read.All разрешения.</span><span class="sxs-lookup"><span data-stu-id="7fa47-207">This request requires the User.ReadBasic.All for People.Read.All permission.</span></span> <span data-ttu-id="7fa47-208">В этом примере отображаются Nestor Kellum соответствующих пользователей.</span><span class="sxs-lookup"><span data-stu-id="7fa47-208">In this example, Nestor Kellum's relevant people are displayed.</span></span>

```http
GET https://graph.microsoft.com/beta/users('nestork@contoso.com')/people/
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List people",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
