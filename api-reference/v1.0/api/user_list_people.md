# <a name="list-people"></a><span data-ttu-id="9686f-101">Получение списка людей</span><span class="sxs-lookup"><span data-stu-id="9686f-101">List of people</span></span>

<span data-ttu-id="9686f-102">Вы можете получить коллекцию объектов [person](../resources/person.md), упорядоченных по их релевантности для [пользователя](../resources/user.md), которая определяется шаблонами общения и совместной работы пользователя, а также его бизнес-отношениями.</span><span class="sxs-lookup"><span data-stu-id="9686f-102">Retrieve a collection of [person](../resources/person.md) objects ordered by their relevance to the [user](../resources/user.md), which is determined by the user's communication and collaboration patterns and business relationships.</span></span>

<span data-ttu-id="9686f-p101">Вы можете получить эти сведения с помощью API People. Примеры см. в разделе [Примеры](#examples) и статье о том, как [получить релевантную информацию о людях](../../../concepts/people_example.md).</span><span class="sxs-lookup"><span data-stu-id="9686f-p101">You can get this information via the People API. For examples, see the [Examples](#examples) section and the article [Get relevant information about people](../../../concepts/people_example.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9686f-105">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9686f-105">Prerequisites</span></span>
<span data-ttu-id="9686f-106">Для выполнения этого API необходимы следующие **области**: *People.Read* и *People.Read.All*.</span><span class="sxs-lookup"><span data-stu-id="9686f-106">The following **scopes** are required to execute this API: *People.Read* *People.Read.All*</span></span>
 
## <a name="http-request"></a><span data-ttu-id="9686f-107">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9686f-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/people
GET /users/{id | userPrincipalName}/people
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9686f-108">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9686f-108">Optional query parameters</span></span>
|<span data-ttu-id="9686f-109">Имя</span><span class="sxs-lookup"><span data-stu-id="9686f-109">Name</span></span>|<span data-ttu-id="9686f-110">Значение</span><span class="sxs-lookup"><span data-stu-id="9686f-110">Value</span></span>|<span data-ttu-id="9686f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9686f-111">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="9686f-112">$filter</span><span class="sxs-lookup"><span data-stu-id="9686f-112">$filter</span></span>|<span data-ttu-id="9686f-113">string</span><span class="sxs-lookup"><span data-stu-id="9686f-113">string</span></span>|<span data-ttu-id="9686f-114">Позволяет возвращать в отклике только тех людей, чьи записи содержат указанные критерии.</span><span class="sxs-lookup"><span data-stu-id="9686f-114">Limits the response to only those people whose record contains the specified criteria.</span></span>|
|<span data-ttu-id="9686f-115">$orderby</span><span class="sxs-lookup"><span data-stu-id="9686f-115">$orderby</span></span>|<span data-ttu-id="9686f-116">string</span><span class="sxs-lookup"><span data-stu-id="9686f-116">string</span></span>|<span data-ttu-id="9686f-p102">По умолчанию люди в отклике отсортированы по их релевантности вашему запросу. Вы можете изменить порядок людей в отклике, используя параметр *$orderby*.</span><span class="sxs-lookup"><span data-stu-id="9686f-p102">By default, the people in the response are sorted by their relevance to your query. You can change the order of the people in the response by using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="9686f-119">$search</span><span class="sxs-lookup"><span data-stu-id="9686f-119">$search</span></span>|<span data-ttu-id="9686f-120">string</span><span class="sxs-lookup"><span data-stu-id="9686f-120">string</span></span>|<span data-ttu-id="9686f-p103">Поиск пользователей по имени или псевдониму. Поддерживается функция нечеткого соответствия.</span><span class="sxs-lookup"><span data-stu-id="9686f-p103">Search for people by name or alias. Supports fuzzy matching.</span></span>|
|<span data-ttu-id="9686f-123">$select</span><span class="sxs-lookup"><span data-stu-id="9686f-123">$select</span></span>|<span data-ttu-id="9686f-124">string</span><span class="sxs-lookup"><span data-stu-id="9686f-124">string</span></span>|<span data-ttu-id="9686f-p104">Список разделенных запятыми свойств, которые необходимо включить в отклик. Для оптимизации производительности выбирайте только необходимые свойства.</span><span class="sxs-lookup"><span data-stu-id="9686f-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>|
|<span data-ttu-id="9686f-127">$skip</span><span class="sxs-lookup"><span data-stu-id="9686f-127">$skip</span></span>|<span data-ttu-id="9686f-128">int</span><span class="sxs-lookup"><span data-stu-id="9686f-128">int</span></span>|<span data-ttu-id="9686f-p105">Пропуск первых n результатов; эту функцию удобно использовать при разбиении результатов на страницы. Эта возможность не поддерживается при использовании параметра *$search*.</span><span class="sxs-lookup"><span data-stu-id="9686f-p105">Skip the first n results, useful for paging. This is not supported when using *$search*.</span></span>|
|<span data-ttu-id="9686f-131">$top</span><span class="sxs-lookup"><span data-stu-id="9686f-131">$top</span></span>|<span data-ttu-id="9686f-132">int</span><span class="sxs-lookup"><span data-stu-id="9686f-132">int</span></span>|<span data-ttu-id="9686f-133">Количество возвращаемых результатов.</span><span class="sxs-lookup"><span data-stu-id="9686f-133">Number of results to be returned.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="9686f-134">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9686f-134">Request headers</span></span>
| <span data-ttu-id="9686f-135">Имя</span><span class="sxs-lookup"><span data-stu-id="9686f-135">Name</span></span>      |<span data-ttu-id="9686f-136">Описание</span><span class="sxs-lookup"><span data-stu-id="9686f-136">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9686f-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9686f-137">Authorization</span></span>  | <span data-ttu-id="9686f-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9686f-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9686f-140">Accept</span><span class="sxs-lookup"><span data-stu-id="9686f-140">Accept</span></span> | <span data-ttu-id="9686f-141">application/json</span><span class="sxs-lookup"><span data-stu-id="9686f-141">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="9686f-142">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9686f-142">Request body</span></span>
<span data-ttu-id="9686f-143">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9686f-143">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="9686f-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="9686f-144">Response</span></span>
<span data-ttu-id="9686f-p107">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [person](../resources/person.md) в тексте ответа. Отклик может содержать один объект person либо коллекцию объектов person.</span><span class="sxs-lookup"><span data-stu-id="9686f-p107">If successful, this method returns a `200 OK` response code and a collection of [person](../resources/person.md) objects in the response body. The response can contain one person object or a collection of person objects.</span></span> 
## <a name="examples"></a><span data-ttu-id="9686f-147">Примеры</span><span class="sxs-lookup"><span data-stu-id="9686f-147">Examples</span></span>

### <a name="get-a-collection-of-relevant-people"></a><span data-ttu-id="9686f-148">Получение коллекции релевантных людей</span><span class="sxs-lookup"><span data-stu-id="9686f-148">Get a collection of relevant people</span></span> 

<span data-ttu-id="9686f-149">С помощью указанного ниже запроса можно получить людей, наиболее релевантных для пользователя, выполнившего вход в систему (`/me`), на основании его шаблонов общения и совместной работы, а также бизнес-отношений.</span><span class="sxs-lookup"><span data-stu-id="9686f-149">The following request gets the people most relevant to the signed-in user (`/me`), based on communication and collaboration patterns and business relationships.</span></span> 
<!-- {
  "blockType": "request",
  "name": "get_person"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/people/
```

<span data-ttu-id="9686f-p108">В примере ниже показан отклик. По умолчанию в каждом отклике возвращается 10 записей. Вы можете изменить количество возвращаемых записей с помощью параметра запроса *$top*. В этом примере показано, как использовать параметр запроса *$top* для ограничения количества записей (до 3 шт.) в отклике.</span><span class="sxs-lookup"><span data-stu-id="9686f-p108">The following example shows the response. By default, each response returns 10 records. You can change this by using the *$top* query parameter. This example uses *$top* to limit the response to three records.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.person"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "8CE6E1DE-CB84-4BF5-971D-D3ECF452E2B5",
            "displayName": "Lorrie Frye",
            "givenName": "Lorrie",
            "surname": "Frye",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "Paralegal",
            "companyName": null,
            "yomiCompany": "",
            "department": "Legal",
            "officeLocation": "20/1109",
            "profession": "",
            "userPrincipalName": "Lorrief@contoso.onmicrosoft.com",
            "imAddress": "sip:Lorrief@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Lorrief@contoso.onmicrosoft.com",
                    "relevanceScore": 8
                }
            ],
            "phones": [
                {
                    "type": "Business",
                    "number": "+1 980 555 0101"
                }
            ],
            "postalAddresses": [],
            "websites": [],
            "personType": {
                "class": "Person",
                "subclass": "OrganizationUser"
            }
        },
        {
            "id": "5767393D-42BA-4E5C-BEE4-52BB25639CF4",
            "displayName": "Maynard Denman",
            "givenName": "Maynard",
            "surname": "Denman",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "Web Marketing Manager",
            "companyName": null,
            "yomiCompany": "",
            "department": "Sales & Marketing",
            "officeLocation": "20/1101",
            "profession": "",
            "userPrincipalName": "Maynardd@contoso.onmicrosoft.com",
            "imAddress": "sip:Maynardd@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Maynardd@contoso.onmicrosoft.com",
                    "relevanceScore": 8
                }
            ],
            "phones": [
                {
                    "type": "Business",
                    "number": "+1 918 555 0101"
                }
            ],
            "postalAddresses": [],
            "websites": [],
            "personType": {
                "class": "Person",
                "subclass": "OrganizationUser"
            }
        },
        {
            "id": "914B5191-11FA-4C0B-A354-0FA8C8EFD585",
            "displayName": "Darrel Halsey",
            "givenName": "Darrel",
            "surname": "Halsey",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "Attorney",
            "companyName": null,
            "yomiCompany": "",
            "department": "Legal",
            "officeLocation": "14/1102",
            "profession": "",
            "userPrincipalName": "Darrelh@contoso.onmicrosoft.com",
            "imAddress": "sip:Darrelh@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Darrelh@contoso.onmicrosoft.com",
                    "relevanceScore": 8
                }
            ],
            "phones": [
                {
                    "type": "Business",
                    "number": "+1 205 555 0103"
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
### <a name="search-other-users-relevant-people"></a><span data-ttu-id="9686f-154">Поиск людей, релевантных для другого пользователя</span><span class="sxs-lookup"><span data-stu-id="9686f-154">Search other user’s relevant people</span></span>

<span data-ttu-id="9686f-p109">Указанный ниже запрос возвращает людей, наиболее релевантных для другого пользователя в организации пользователя, выполнившего вход в систему. Для выполнения этого запроса требуется разрешение People.Read.All. В этом примере отображаются люди, релевантные для пользователя Roscoe Seidel.</span><span class="sxs-lookup"><span data-stu-id="9686f-p109">The following request gets the people most relevant to another person in the signed-in user's organization. This request requires the People.Read.All permission. In this example, Roscoe Seidel's relevant people are displayed.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_person"
}-->

```http
GET https://graph.microsoft.com/v1.0/users('roscoes@contoso.com')/people/
```

<span data-ttu-id="9686f-p110">В примере ниже показан отклик. По умолчанию в каждом отклике возвращается 10 записей. Вы можете изменить количество возвращаемых записей с помощью параметра *$top*. В этом примере показано, как использовать параметр запроса *$top* для ограничения количества записей (до 3 шт.) в отклике.</span><span class="sxs-lookup"><span data-stu-id="9686f-p110">The following example shows the response. By default, each response returns 10 records. You can change this by using the *$top* parameter. This example uses *$top* to limit the response to three records.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.person"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
     "value": [
        {
            "id": "56155636-703F-47F2-B657-C83F01F49BBC",
            "displayName": "Clifton Clemente",
            "givenName": "Clifton",
            "surname": "Clemente",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "Director",
            "companyName": null,
            "yomiCompany": "",
            "department": "Legal",
            "officeLocation": "19/2106",
            "profession": "",
            "userPrincipalName": "Cliftonc@contoso.onmicrosoft.com",
            "imAddress": "sip:Cliftonc@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Cliftonc@contoso.onmicrosoft.com",
                    "relevanceScore": 20
                }
            ],
            "phones": [
                {
                    "type": "Business",
                    "number": "+1 309 555 0101"
                }
            ],
            "postalAddresses": [],
            "websites": [],
            "personType": {
                "class": "Person",
                "subclass": "OrganizationUser"
            }
        },
        {
            "id": "6BF27D5A-AB4F-4C43-BED0-7DAD9EB0C1C4",
            "displayName": "Sheree Mitchell",
            "givenName": "Sheree",
            "surname": "Mitchell",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "Product Manager",
            "companyName": null,
            "yomiCompany": "",
            "department": "Sales & Marketing",
            "officeLocation": "20/2107",
            "profession": "",
            "userPrincipalName": "Shereem@contoso.onmicrosoft.com",
            "imAddress": "sip:shereem@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Shereem@contoso.onmicrosoft.com",
                    "relevanceScore": 10
                }
            ],
            "phones": [
                {
                    "type": "Business",
                    "number": "+1 918 555 0107"
                }
            ],
            "postalAddresses": [],
            "websites": [],
            "personType": {
                "class": "Person",
                "subclass": "OrganizationUser"
            }
        },
        {
            "id": "B3E5302D-EAF0-4E8B-8C6C-A2AE64B4B163",
            "displayName": "Vincent Matney",
            "givenName": "Vincent",
            "surname": "Matney",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "CVP Engineering",
            "companyName": null,
            "yomiCompany": "",
            "department": "Engineering",
            "officeLocation": "23/2102",
            "profession": "",
            "userPrincipalName": "Vincentm@contoso.onmicrosoft.com",
            "imAddress": "sip:vincentm@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Vincentm@contoso.onmicrosoft.com",
                    "relevanceScore": 10
                }
            ],
            "phones": [
                {
                    "type": "Business",
                    "number": "+1 502 555 0102"
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List people",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
