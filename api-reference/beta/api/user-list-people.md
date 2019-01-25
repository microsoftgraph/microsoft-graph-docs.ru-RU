---
title: Список людей
description: Получение списка объектов person, упорядоченные по их важности для пользователя, который определяет, какие связи и совместной работы шаблоны и устанавливать деловые контакты пользователя.
author: dkershaw10
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: deb9fd929a2b0b8ce4da9392cb465497c2236b0c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517815"
---
# <a name="list-people"></a><span data-ttu-id="19c91-103">Список людей</span><span class="sxs-lookup"><span data-stu-id="19c91-103">List people</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19c91-104">Получение списка объектов [person](../resources/person.md) , упорядоченные по их важности для [пользователя](../resources/user.md), который определяет, какие связи и совместной работы шаблоны и устанавливать деловые контакты пользователя.</span><span class="sxs-lookup"><span data-stu-id="19c91-104">Retrieve a list of [person](../resources/person.md) objects ordered by their relevance to the [user](../resources/user.md), which is determined by the user's communication and collaboration patterns, and business relationships.</span></span>

## <a name="permissions"></a><span data-ttu-id="19c91-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="19c91-105">Permissions</span></span>

<span data-ttu-id="19c91-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19c91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19c91-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="19c91-108">Permission type</span></span>      | <span data-ttu-id="19c91-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="19c91-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="19c91-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="19c91-110">Delegated (work or school account)</span></span> | <span data-ttu-id="19c91-111">People.Read</span><span class="sxs-lookup"><span data-stu-id="19c91-111">People.Read</span></span>    |
|<span data-ttu-id="19c91-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="19c91-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19c91-113">People.Read</span><span class="sxs-lookup"><span data-stu-id="19c91-113">People.Read</span></span>    |
|<span data-ttu-id="19c91-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="19c91-114">Application</span></span> | <span data-ttu-id="19c91-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19c91-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="19c91-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="19c91-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/people
GET /users/{id | userPrincipalName}/people
```

## <a name="optional-query-parameters"></a><span data-ttu-id="19c91-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="19c91-117">Optional query parameters</span></span>

<span data-ttu-id="19c91-118">Этот метод поддерживает следующие параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="19c91-118">This method supports the following OData query parameters to help customize the response.</span></span>

|<span data-ttu-id="19c91-119">Имя</span><span class="sxs-lookup"><span data-stu-id="19c91-119">Name</span></span>|<span data-ttu-id="19c91-120">Значение</span><span class="sxs-lookup"><span data-stu-id="19c91-120">Value</span></span>|<span data-ttu-id="19c91-121">Описание</span><span class="sxs-lookup"><span data-stu-id="19c91-121">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="19c91-122">$filter</span><span class="sxs-lookup"><span data-stu-id="19c91-122">$filter</span></span>|<span data-ttu-id="19c91-123">string</span><span class="sxs-lookup"><span data-stu-id="19c91-123">string</span></span>|<span data-ttu-id="19c91-124">Позволяет возвращать в отклике только тех людей, чьи записи содержат указанные критерии.</span><span class="sxs-lookup"><span data-stu-id="19c91-124">Limits the response to only those people whose record contains the specified criteria.</span></span>|
|<span data-ttu-id="19c91-125">$orderby</span><span class="sxs-lookup"><span data-stu-id="19c91-125">$orderby</span></span>|<span data-ttu-id="19c91-126">строка</span><span class="sxs-lookup"><span data-stu-id="19c91-126">string</span></span>|<span data-ttu-id="19c91-127">По умолчанию люди в ответе сортируются по степени соответствия запросу.</span><span class="sxs-lookup"><span data-stu-id="19c91-127">By default the people in the response are sorted by their relevance to your query.</span></span> <span data-ttu-id="19c91-128">Этот порядок можно изменить с помощью параметра *$orderby*.</span><span class="sxs-lookup"><span data-stu-id="19c91-128">You can change the order of the people in the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="19c91-129">$search</span><span class="sxs-lookup"><span data-stu-id="19c91-129">$search</span></span>|<span data-ttu-id="19c91-130">string</span><span class="sxs-lookup"><span data-stu-id="19c91-130">string</span></span>|<span data-ttu-id="19c91-131">Поиск пользователей по имени или псевдониму.</span><span class="sxs-lookup"><span data-stu-id="19c91-131">Search for people by name or alias.</span></span> <span data-ttu-id="19c91-132">Поддерживается нечеткое соответствие.</span><span class="sxs-lookup"><span data-stu-id="19c91-132">Supports Fuzzy matching.</span></span> <span data-ttu-id="19c91-133">Параметр работает только при поиске людей соответствующий пользователь выполнил вход, не для поиска людей, предназначенных для других пользователей.</span><span class="sxs-lookup"><span data-stu-id="19c91-133">Parameter only works for searching the signed-in user's relevant people, not for searching people relevant to other users.</span></span> <span data-ttu-id="19c91-134">Также поддерживает `topic` ключевое слово для поиска людей на основании разделы, извлеченные из сообщений электронной почты с этим контактом.</span><span class="sxs-lookup"><span data-stu-id="19c91-134">Also supports the `topic` keyword to find people based on topics extracted from e-mail conversations with that person.</span></span> <span data-ttu-id="19c91-135">В разделе *Perform Нечеткое поиска* в [получить информацию о пользователях](/graph/people-example#perform-a-fuzzy-search) сведения и примеры.</span><span class="sxs-lookup"><span data-stu-id="19c91-135">See the *Perform a fuzzy search* section at [Get relevant information about people](/graph/people-example#perform-a-fuzzy-search) for information and examples.</span></span>|
|<span data-ttu-id="19c91-136">$select</span><span class="sxs-lookup"><span data-stu-id="19c91-136">$select</span></span>|<span data-ttu-id="19c91-137">string</span><span class="sxs-lookup"><span data-stu-id="19c91-137">string</span></span>|<span data-ttu-id="19c91-p104">Список разделенных запятыми свойств, которые необходимо включить в отклик. Для оптимизации производительности выбирайте только необходимые свойства.</span><span class="sxs-lookup"><span data-stu-id="19c91-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>|
|<span data-ttu-id="19c91-140">$skip</span><span class="sxs-lookup"><span data-stu-id="19c91-140">$skip</span></span>|<span data-ttu-id="19c91-141">int</span><span class="sxs-lookup"><span data-stu-id="19c91-141">int</span></span>|<span data-ttu-id="19c91-p105">Пропуск первых n результатов; эту функцию удобно использовать при разбиении результатов на страницы. Эта возможность не поддерживается при использовании параметра *$search*.</span><span class="sxs-lookup"><span data-stu-id="19c91-p105">Skip the first n results, useful for paging. This is not supported when using *$search*.</span></span>|
|<span data-ttu-id="19c91-144">$top</span><span class="sxs-lookup"><span data-stu-id="19c91-144">$top</span></span>|<span data-ttu-id="19c91-145">int</span><span class="sxs-lookup"><span data-stu-id="19c91-145">int</span></span>|<span data-ttu-id="19c91-146">Количество возвращаемых результатов.</span><span class="sxs-lookup"><span data-stu-id="19c91-146">Number of results to be returned.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="19c91-147">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="19c91-147">Request headers</span></span>

| <span data-ttu-id="19c91-148">Название</span><span class="sxs-lookup"><span data-stu-id="19c91-148">Name</span></span>      |<span data-ttu-id="19c91-149">Описание</span><span class="sxs-lookup"><span data-stu-id="19c91-149">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="19c91-150">Авторизация</span><span class="sxs-lookup"><span data-stu-id="19c91-150">Authorization</span></span>  | <span data-ttu-id="19c91-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="19c91-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="19c91-153">Accept</span><span class="sxs-lookup"><span data-stu-id="19c91-153">Accept</span></span> | <span data-ttu-id="19c91-154">application/json</span><span class="sxs-lookup"><span data-stu-id="19c91-154">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="19c91-155">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="19c91-155">Request body</span></span>

<span data-ttu-id="19c91-156">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="19c91-156">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="19c91-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="19c91-157">Response</span></span>

<span data-ttu-id="19c91-158">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [человека](../resources/person.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="19c91-158">If successful, this method returns a `200 OK` response code and a collection of [person](../resources/person.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="19c91-159">Примеры</span><span class="sxs-lookup"><span data-stu-id="19c91-159">Examples</span></span>

### <a name="browse"></a><span data-ttu-id="19c91-160">Обзор</span><span class="sxs-lookup"><span data-stu-id="19c91-160">Browse</span></span>

<span data-ttu-id="19c91-161">Запросы в этом разделе получить наиболее важные, чтобы пользователь выполнил вход пользователей (`/me`), в зависимости от связи, совместной работы и деловыми отношениями.</span><span class="sxs-lookup"><span data-stu-id="19c91-161">The requests in this section get the people most relevant to the signed-in user (`/me`), based on communication, collaboration, and business relationships.</span></span>

<span data-ttu-id="19c91-162">По умолчанию каждый отклик возвращает 10 записей, но его можно изменить с помощью параметра *$top* .</span><span class="sxs-lookup"><span data-stu-id="19c91-162">By default, each response returns 10 records, but you can change this using the *$top* parameter.</span></span> <span data-ttu-id="19c91-163">Эти запросы требуется разрешение People.Read.</span><span class="sxs-lookup"><span data-stu-id="19c91-163">These requests require the People.Read permission.</span></span>

#### <a name="request"></a><span data-ttu-id="19c91-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="19c91-164">Request</span></span>

<span data-ttu-id="19c91-165">Ниже приведен пример запроса по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="19c91-165">The following is an example of the default request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_person_collection_beta"
}-->

```http
GET https://graph.microsoft.com/beta/me/people
```

#### <a name="response"></a><span data-ttu-id="19c91-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="19c91-166">Response</span></span>

<span data-ttu-id="19c91-167">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="19c91-167">The following is an example of the response.</span></span>
><span data-ttu-id="19c91-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="19c91-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

#### <a name="requesting-a-subsequent-page-of-people"></a><span data-ttu-id="19c91-170">Разрешения на запрос следующей странице людей</span><span class="sxs-lookup"><span data-stu-id="19c91-170">Requesting a subsequent page of people</span></span>

<span data-ttu-id="19c91-p109">Если в первом отклике содержится неполный список релевантных людей, вы можете создать второй запрос, используя параметры *$top* и *$skip*, чтобы запросить дополнительные страницы информации. Если в предыдущем запросе есть дополнительная информация, то при последующем запросе будет получена следующая страница с людьми с сервера.</span><span class="sxs-lookup"><span data-stu-id="19c91-p109">If the first response does not contain the complete list of relevant people, you can make a second request using *$top* and *$skip* to request additional pages of information. If the previous request has additional information, the following request gets the next page of people from the server.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$top=10&$skip=10
```

#### <a name="sort-the-response"></a><span data-ttu-id="19c91-173">Сортировка в отклике</span><span class="sxs-lookup"><span data-stu-id="19c91-173">Sort the response</span></span>

<span data-ttu-id="19c91-174">По умолчанию люди в ответе сортируются по степени соответствия запросу.</span><span class="sxs-lookup"><span data-stu-id="19c91-174">By default the people in the response are sorted by their relevance to your query.</span></span> <span data-ttu-id="19c91-175">Этот порядок можно изменить с помощью параметра *$orderby*.</span><span class="sxs-lookup"><span data-stu-id="19c91-175">You can change the order of the people in the response using the *$orderby* parameter.</span></span> <span data-ttu-id="19c91-176">Этот запрос выбирает наиболее важные для вас людей, их сортировка по их отображаемое имя и затем возвращаются первые 10 пользователей на отсортированный список.</span><span class="sxs-lookup"><span data-stu-id="19c91-176">This query selects the people most relevant to you, sorts them by their display name, and then returns the first 10 people on the sorted list.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$orderby=DisplayName
```

#### <a name="changing-the-number-of-people-returned-and-the-fields-returned"></a><span data-ttu-id="19c91-177">Изменение числа возвращаемых людей и поля</span><span class="sxs-lookup"><span data-stu-id="19c91-177">Changing the number of people returned and the fields returned</span></span>

<span data-ttu-id="19c91-178">Вы можете изменить количество людей, возвращаемых в отклике, настроив параметр *$top*.</span><span class="sxs-lookup"><span data-stu-id="19c91-178">You can change the number of people returned in the response by setting the *$top* parameter.</span></span>

<span data-ttu-id="19c91-179">Следующий пример запрашивает 1 000 пользователей, наиболее подходящих для `/me`.</span><span class="sxs-lookup"><span data-stu-id="19c91-179">The following example requests the 1,000 people most relevant to `/me`.</span></span> <span data-ttu-id="19c91-180">Запрос также ограничивает объем данных, отправленных с сервера, запрашивая только отображаемое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="19c91-180">The request also limits the amount of data sent back from the server by requesting only the display name of the person.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$top=1000&$select=DisplayName
```

#### <a name="selecting-the-fields-to-return"></a><span data-ttu-id="19c91-181">Выбор полей для возврата</span><span class="sxs-lookup"><span data-stu-id="19c91-181">Selecting the fields to return</span></span>

<span data-ttu-id="19c91-182">Можно ограничить объем данных, возвращаемых с сервера с помощью параметра *$select* выбрать одно или несколько полей.</span><span class="sxs-lookup"><span data-stu-id="19c91-182">You can limit the amount of data returned from the server by using the *$select* parameter to choose one or more fields.</span></span> <span data-ttu-id="19c91-183">В поле *@odata.id* всегда возвращается.</span><span class="sxs-lookup"><span data-stu-id="19c91-183">The *@odata.id* field is always returned.</span></span>

<span data-ttu-id="19c91-184">В следующем примере ограничиваются ответ на *DisplayName* и *EmailAddress* 10 наиболее подходящих людей.</span><span class="sxs-lookup"><span data-stu-id="19c91-184">The following example limits the response to the *DisplayName* and *EmailAddress* of the 10 most relevant people.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$select=DisplayName,EmailAddresses
```

#### <a name="using-a-filter-to-limit-the-response"></a><span data-ttu-id="19c91-185">С помощью фильтра для ограничения ответа</span><span class="sxs-lookup"><span data-stu-id="19c91-185">Using a filter to limit the response</span></span>

<span data-ttu-id="19c91-186">Вы можете использовать параметр *$filter*, чтобы ограничить количество информации в отклике и возвращать только тех людей, записи которых содержат указанные критерии.</span><span class="sxs-lookup"><span data-stu-id="19c91-186">You can use the *$filter* parameter to limit the response to only those people whose record contains the specified criteria.</span></span>

<span data-ttu-id="19c91-187">Следующий запрос ограничивает ответа для людей с источником «Каталог».</span><span class="sxs-lookup"><span data-stu-id="19c91-187">The following query limits the response to people with the source "Directory."</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$filter=Sources/Any (source: source/Type  eq 'Directory')
```

#### <a name="selecting-the-fields-to-return-in-a-filtered-response"></a><span data-ttu-id="19c91-188">Выбор полей для возврата в отфильтрованные ответа</span><span class="sxs-lookup"><span data-stu-id="19c91-188">Selecting the fields to return in a filtered response</span></span>

<span data-ttu-id="19c91-189">Сочетая параметры *$select* и *$filter*, вы можете создать настраиваемый список людей, релевантных для пользователя, и получать только те поля, которые необходимы вашему приложению.</span><span class="sxs-lookup"><span data-stu-id="19c91-189">You can combine the *$select* and *$filter* parameters to create a custom list of people relevant to the user and get only the fields that your application needs.</span></span>

<span data-ttu-id="19c91-190">В следующем примере получается *DisplayName* и *EmailAddress* людей, отображаемое имя равно указанному имени.</span><span class="sxs-lookup"><span data-stu-id="19c91-190">The following example gets the *DisplayName* and *EmailAddress* of people whose display name equals the specified name.</span></span> <span data-ttu-id="19c91-191">В этом примере возвращаются только тех, отображаемое имя равно «Nestor Kellum».</span><span class="sxs-lookup"><span data-stu-id="19c91-191">In this example, only people whose display name equals "Nestor Kellum" are returned.</span></span>

```http
+GET https://graph.microsoft.com/beta/me/people/?$select=DisplayName,EmailAddresses&$filter=DisplayName eq 'Nestor Kellum'
```

### <a name="search-people"></a><span data-ttu-id="19c91-192">Поиск людей</span><span class="sxs-lookup"><span data-stu-id="19c91-192">Search people</span></span>

<span data-ttu-id="19c91-193">Запросы в этом разделе также получить людей самые точные, чтобы пользователь выполнил вход (`/me`).</span><span class="sxs-lookup"><span data-stu-id="19c91-193">The requests in this section also get the people most relevant to the signed-in user (`/me`).</span></span> <span data-ttu-id="19c91-194">Запросы поиска требуется разрешение People.Read.</span><span class="sxs-lookup"><span data-stu-id="19c91-194">Search requests require the People.Read permission.</span></span>

#### <a name="using-search-to-select-people"></a><span data-ttu-id="19c91-195">Использование поиска для выбора людей</span><span class="sxs-lookup"><span data-stu-id="19c91-195">Using search to select people</span></span>

<span data-ttu-id="19c91-196">Используйте параметр *$search* для выбора людей, удовлетворяющих определенному набору критериев.</span><span class="sxs-lookup"><span data-stu-id="19c91-196">Use the *$search* parameter to select people who meet a particular set of criteria.</span></span>

<span data-ttu-id="19c91-197">Следующий запрос поиска возвращает людей, относящиеся к `/me` , GivenName или фамилию начинается с буквы «j».</span><span class="sxs-lookup"><span data-stu-id="19c91-197">The following search query returns people relevant to `/me` whose GivenName or Surname begins with the letter "j".</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$search=j
```

#### <a name="using-search-to-specify-a-relevant-topic"></a><span data-ttu-id="19c91-198">Использование поиска для указания соответствующей темы</span><span class="sxs-lookup"><span data-stu-id="19c91-198">Using search to specify a relevant topic</span></span>

<span data-ttu-id="19c91-199">Следующий запрос возвращает людей, относящиеся к `/me` , имя которого содержит «ma» и пользователей, которые имеют связь с «планирование компонентов».</span><span class="sxs-lookup"><span data-stu-id="19c91-199">The following request returns people relevant to `/me` whose name contains "ma" and who have an association with "feature planning."</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$search="ma topic: feature planning"
```

#### <a name="performing-a-fuzzy-search"></a><span data-ttu-id="19c91-200">Для выполнения Нечеткое поиска</span><span class="sxs-lookup"><span data-stu-id="19c91-200">Performing a fuzzy search</span></span>

<span data-ttu-id="19c91-201">Следующий запрос поиска для пользователя с именем «Зал Hermaini».</span><span class="sxs-lookup"><span data-stu-id="19c91-201">The following request does a search for a person named "Hermaini Hall."</span></span> <span data-ttu-id="19c91-202">Так как пользователь с именем «Herminia оболочка» относится к пользователь выполнил вход, возвращается информация для «Herminia оболочка».</span><span class="sxs-lookup"><span data-stu-id="19c91-202">Because there is a person named "Herminia Hull" relevant to the signed-in user, the information for "Herminia Hull" is returned.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$search="hermaini hall"
```

### <a name="related-people"></a><span data-ttu-id="19c91-203">Связанные людей</span><span class="sxs-lookup"><span data-stu-id="19c91-203">Related people</span></span>

<span data-ttu-id="19c91-204">Следующий запрос получает наиболее подходящих другому пользователю людей в организации пользователя.</span><span class="sxs-lookup"><span data-stu-id="19c91-204">The following request gets the people most relevant to another person in the user's organization.</span></span> <span data-ttu-id="19c91-205">Этот запрос требует User.ReadBasic.All People.Read.All разрешения.</span><span class="sxs-lookup"><span data-stu-id="19c91-205">This request requires the User.ReadBasic.All for People.Read.All permission.</span></span> <span data-ttu-id="19c91-206">В этом примере отображаются Nestor Kellum соответствующих пользователей.</span><span class="sxs-lookup"><span data-stu-id="19c91-206">In this example, Nestor Kellum's relevant people are displayed.</span></span>

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
    "Error: /api-reference/beta/api/user-list-people.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
