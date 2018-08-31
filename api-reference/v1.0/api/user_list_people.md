# <a name="list-people"></a><span data-ttu-id="661c3-101">Список людей</span><span class="sxs-lookup"><span data-stu-id="661c3-101">List people</span></span>

<span data-ttu-id="661c3-102">Получите коллекцию объектов [person](../resources/person.md), упорядоченных по их релевантности для [пользователя](../resources/user.md), которая определяется его моделями общения и совместной работы, а также бизнес-отношениями.</span><span class="sxs-lookup"><span data-stu-id="661c3-102">Retrieve a collection of [person](../resources/person.md) objects ordered by their relevance to the [user](../resources/user.md), which is determined by the user's communication and collaboration patterns, and business relationships.</span></span>

<span data-ttu-id="661c3-p101">Для получения этих сведений используйте API службы "Люди". Примеры см. в разделе [Примеры](#examples) и статье о том, как [получить релевантную информацию о людях](../../../concepts/people_example.md).</span><span class="sxs-lookup"><span data-stu-id="661c3-p101">You can get this information via the People API. For examples, see the [Examples](#examples) section and the article [Get relevant information about people](../../../concepts/people_example.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="661c3-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="661c3-105">Permissions</span></span>

<span data-ttu-id="661c3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="661c3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="661c3-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="661c3-108">Permission type</span></span>      | <span data-ttu-id="661c3-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="661c3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="661c3-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="661c3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="661c3-111">People.Read, People.Read.All</span><span class="sxs-lookup"><span data-stu-id="661c3-111">People.Read, People.Read.All</span></span>    |
|<span data-ttu-id="661c3-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="661c3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="661c3-113">People.Read</span><span class="sxs-lookup"><span data-stu-id="661c3-113">People.Read</span></span>    |
|<span data-ttu-id="661c3-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="661c3-114">Application</span></span> | <span data-ttu-id="661c3-115">People.Read.All</span><span class="sxs-lookup"><span data-stu-id="661c3-115">People.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="661c3-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="661c3-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/people
GET /users/{id | userPrincipalName}/people
```

## <a name="optional-query-parameters"></a><span data-ttu-id="661c3-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="661c3-117">Optional query parameters</span></span>

<span data-ttu-id="661c3-118">Этот метод поддерживает [параметры запроса OData](../../../concepts/query_parameters.md) также для настройки ответа. Примеры см. в статье [Получение релевантной информации о людях](../../../concepts/people_example.md).</span><span class="sxs-lookup"><span data-stu-id="661c3-118">This method supports the [OData query parameters](../../../concepts/query_parameters.md) to help customize the response, as shown in the examples in the article [Get relevant information about people](../../../concepts/people_example.md).</span></span>

|<span data-ttu-id="661c3-119">Имя</span><span class="sxs-lookup"><span data-stu-id="661c3-119">Name</span></span>|<span data-ttu-id="661c3-120">Значение</span><span class="sxs-lookup"><span data-stu-id="661c3-120">Value</span></span>|<span data-ttu-id="661c3-121">Описание</span><span class="sxs-lookup"><span data-stu-id="661c3-121">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="661c3-122">$filter</span><span class="sxs-lookup"><span data-stu-id="661c3-122">$filter</span></span>|<span data-ttu-id="661c3-123">string</span><span class="sxs-lookup"><span data-stu-id="661c3-123">string</span></span>|<span data-ttu-id="661c3-124">Позволяет возвращать в отклике только тех людей, чьи записи содержат указанные критерии.</span><span class="sxs-lookup"><span data-stu-id="661c3-124">Limits the response to only those people whose record contains the specified criteria.</span></span>|
|<span data-ttu-id="661c3-125">$orderby</span><span class="sxs-lookup"><span data-stu-id="661c3-125">$orderby</span></span>|<span data-ttu-id="661c3-126">строка</span><span class="sxs-lookup"><span data-stu-id="661c3-126">string</span></span>|<span data-ttu-id="661c3-127">По умолчанию люди в ответе сортируются по степени соответствия запросу.</span><span class="sxs-lookup"><span data-stu-id="661c3-127">By default the people in the response are sorted by their relevance to your query.</span></span> <span data-ttu-id="661c3-128">Этот порядок можно изменить с помощью параметра *$orderby*.</span><span class="sxs-lookup"><span data-stu-id="661c3-128">You can change the order of the people in the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="661c3-129">$search</span><span class="sxs-lookup"><span data-stu-id="661c3-129">$search</span></span>|<span data-ttu-id="661c3-130">string</span><span class="sxs-lookup"><span data-stu-id="661c3-130">string</span></span>|<span data-ttu-id="661c3-131">Поиск пользователей по имени или псевдониму.</span><span class="sxs-lookup"><span data-stu-id="661c3-131">Search for people by name or alias.</span></span> <span data-ttu-id="661c3-132">Поддерживается нечеткое соответствие.</span><span class="sxs-lookup"><span data-stu-id="661c3-132">Supports Fuzzy matching.</span></span> <span data-ttu-id="661c3-133">Параметр работает только для поиска людей, относящихся к вошедшему в систему пользователю, а не для поиска людей, относящихся к другим пользователям.</span><span class="sxs-lookup"><span data-stu-id="661c3-133">Parameter only works for searching the signed-in user's relevant people, not for searching people relevant to other users.</span></span> <span data-ttu-id="661c3-134">Также поддерживает ключевое слово `topic` для поиска людей на основании тем, извлеченных из бесед по электронной почте с этим человеком.</span><span class="sxs-lookup"><span data-stu-id="661c3-134">Also supports the `topic` keyword to find people based on topics extracted from e-mail conversations with that person.</span></span> <span data-ttu-id="661c3-135">Для получения сведений и примеров см. раздел *Выполнение нечеткого поиска* в статье [Получение соответствующей информации о людях](../../../concepts/people_example.md#perform-a-fuzzy-search).</span><span class="sxs-lookup"><span data-stu-id="661c3-135">See the *Perform a fuzzy search* section at [Get relevant information about people](../../../concepts/people_example.md#perform-a-fuzzy-search) for information and examples.</span></span> |
|<span data-ttu-id="661c3-136">$select</span><span class="sxs-lookup"><span data-stu-id="661c3-136">$select</span></span>|<span data-ttu-id="661c3-137">string</span><span class="sxs-lookup"><span data-stu-id="661c3-137">string</span></span>|<span data-ttu-id="661c3-p105">Список разделенных запятыми свойств, которые необходимо включить в отклик. Для оптимизации производительности выбирайте только необходимые свойства.</span><span class="sxs-lookup"><span data-stu-id="661c3-p105">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>|
|<span data-ttu-id="661c3-140">$skip</span><span class="sxs-lookup"><span data-stu-id="661c3-140">$skip</span></span>|<span data-ttu-id="661c3-141">int</span><span class="sxs-lookup"><span data-stu-id="661c3-141">int</span></span>|<span data-ttu-id="661c3-p106">Пропуск первых n результатов; эту функцию удобно использовать при разбиении результатов на страницы. Эта возможность не поддерживается при использовании параметра *$search*.</span><span class="sxs-lookup"><span data-stu-id="661c3-p106">Skip the first n results, useful for paging. This is not supported when using *$search*.</span></span>|
|<span data-ttu-id="661c3-144">$top</span><span class="sxs-lookup"><span data-stu-id="661c3-144">$top</span></span>|<span data-ttu-id="661c3-145">int</span><span class="sxs-lookup"><span data-stu-id="661c3-145">int</span></span>|<span data-ttu-id="661c3-146">Количество возвращаемых результатов.</span><span class="sxs-lookup"><span data-stu-id="661c3-146">Number of results to be returned.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="661c3-147">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="661c3-147">Request headers</span></span>

| <span data-ttu-id="661c3-148">Имя</span><span class="sxs-lookup"><span data-stu-id="661c3-148">Name</span></span>      |<span data-ttu-id="661c3-149">Описание</span><span class="sxs-lookup"><span data-stu-id="661c3-149">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="661c3-150">Авторизация</span><span class="sxs-lookup"><span data-stu-id="661c3-150">Authorization</span></span>  | <span data-ttu-id="661c3-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="661c3-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="661c3-153">Accept</span><span class="sxs-lookup"><span data-stu-id="661c3-153">Accept</span></span> | <span data-ttu-id="661c3-154">application/json</span><span class="sxs-lookup"><span data-stu-id="661c3-154">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="661c3-155">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="661c3-155">Request body</span></span>

<span data-ttu-id="661c3-156">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="661c3-156">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="661c3-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="661c3-157">Response</span></span>

<span data-ttu-id="661c3-p108">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [person](../resources/person.md) в тексте ответа. Отклик может содержать один объект person либо коллекцию объектов person.</span><span class="sxs-lookup"><span data-stu-id="661c3-p108">If successful, this method returns a `200 OK` response code and a collection of [person](../resources/person.md) objects in the response body. The response can contain one person object or a collection of person objects.</span></span>

## <a name="examples"></a><span data-ttu-id="661c3-160">Примеры</span><span class="sxs-lookup"><span data-stu-id="661c3-160">Examples</span></span>

#### <a name="request"></a><span data-ttu-id="661c3-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="661c3-161">Request</span></span>

<span data-ttu-id="661c3-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="661c3-162">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_person_collection"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/people
```

#### <a name="response"></a><span data-ttu-id="661c3-163">Ответ</span><span class="sxs-lookup"><span data-stu-id="661c3-163">Response</span></span>

<span data-ttu-id="661c3-164">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="661c3-164">The following is an example of the response.</span></span>

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

<span data-ttu-id="661c3-165">Другие примеры см. в статье [Получение релевантной информации о людях](../../../concepts/people_example.md).</span><span class="sxs-lookup"><span data-stu-id="661c3-165">For more examples, see the article [Get relevant information about people](../../../concepts/people_example.md).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List people",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
