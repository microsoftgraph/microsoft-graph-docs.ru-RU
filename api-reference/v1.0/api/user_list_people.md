# <a name="list-people"></a><span data-ttu-id="fa001-101">Получение списка людей</span><span class="sxs-lookup"><span data-stu-id="fa001-101">List people</span></span>

<span data-ttu-id="fa001-102">Вы можете получить коллекцию объектов [person](../resources/person.md), упорядоченных по их релевантности для [пользователя](../resources/user.md), которая определяется шаблонами общения и совместной работы пользователя, а также его бизнес-отношениями.</span><span class="sxs-lookup"><span data-stu-id="fa001-102">Retrieve a collection of [person](../resources/person.md) objects ordered by their relevance to the [user](../resources/user.md), which is determined by the user's communication and collaboration patterns and business relationships.</span></span>

<span data-ttu-id="fa001-p101">Вы можете получить эти сведения с помощью API People. Примеры см. в разделе [Примеры](#examples) и статье о том, как [получить релевантную информацию о людях](../../../concepts/people_example.md).</span><span class="sxs-lookup"><span data-stu-id="fa001-p101">You can get this information via the People API. For examples, see the [Examples](#examples) section and the article [Get relevant information about people](../../../concepts/people_example.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fa001-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fa001-105">Permissions</span></span>
<span data-ttu-id="fa001-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fa001-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>
 

|<span data-ttu-id="fa001-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fa001-108">Permission type</span></span>      | <span data-ttu-id="fa001-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fa001-109">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="fa001-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fa001-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fa001-111">People.Read, People.Read.All</span><span class="sxs-lookup"><span data-stu-id="fa001-111">People.Read, People.Read.All</span></span>    | 
|<span data-ttu-id="fa001-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fa001-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa001-113">People.Read</span><span class="sxs-lookup"><span data-stu-id="fa001-113">People.Read</span></span>    | 
|<span data-ttu-id="fa001-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fa001-114">Application</span></span> | <span data-ttu-id="fa001-115">People.Read.All</span><span class="sxs-lookup"><span data-stu-id="fa001-115">People.Read.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="fa001-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fa001-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/people
GET /users/{id | userPrincipalName}/people
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fa001-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fa001-117">Optional query parameters</span></span>
|<span data-ttu-id="fa001-118">Имя</span><span class="sxs-lookup"><span data-stu-id="fa001-118">Name</span></span>|<span data-ttu-id="fa001-119">Значение</span><span class="sxs-lookup"><span data-stu-id="fa001-119">Value</span></span>|<span data-ttu-id="fa001-120">Описание</span><span class="sxs-lookup"><span data-stu-id="fa001-120">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="fa001-121">$filter</span><span class="sxs-lookup"><span data-stu-id="fa001-121">$filter</span></span>|<span data-ttu-id="fa001-122">string</span><span class="sxs-lookup"><span data-stu-id="fa001-122">string</span></span>|<span data-ttu-id="fa001-123">Позволяет возвращать в отклике только тех людей, чьи записи содержат указанные критерии.</span><span class="sxs-lookup"><span data-stu-id="fa001-123">Limits the response to only those people whose record contains the specified criteria.</span></span>|
|<span data-ttu-id="fa001-124">$orderby</span><span class="sxs-lookup"><span data-stu-id="fa001-124">$orderby</span></span>|<span data-ttu-id="fa001-125">string</span><span class="sxs-lookup"><span data-stu-id="fa001-125">string</span></span>|<span data-ttu-id="fa001-p103">По умолчанию люди в отклике отсортированы по их релевантности вашему запросу. Вы можете изменить порядок людей в отклике, используя параметр *$orderby*.</span><span class="sxs-lookup"><span data-stu-id="fa001-p103">By default, the people in the response are sorted by their relevance to your query. You can change the order of the people in the response by using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="fa001-128">$search</span><span class="sxs-lookup"><span data-stu-id="fa001-128">$search</span></span>|<span data-ttu-id="fa001-129">string</span><span class="sxs-lookup"><span data-stu-id="fa001-129">string</span></span>|<span data-ttu-id="fa001-p104">Поиск пользователей по имени или псевдониму. Поддерживается функция нечеткого соответствия.</span><span class="sxs-lookup"><span data-stu-id="fa001-p104">Search for people by name or alias. Supports fuzzy matching.</span></span>|
|<span data-ttu-id="fa001-132">$select</span><span class="sxs-lookup"><span data-stu-id="fa001-132">$select</span></span>|<span data-ttu-id="fa001-133">string</span><span class="sxs-lookup"><span data-stu-id="fa001-133">string</span></span>|<span data-ttu-id="fa001-p105">Список разделенных запятыми свойств, которые необходимо включить в отклик. Для оптимизации производительности выбирайте только необходимые свойства.</span><span class="sxs-lookup"><span data-stu-id="fa001-p105">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>|
|<span data-ttu-id="fa001-136">$skip</span><span class="sxs-lookup"><span data-stu-id="fa001-136">$skip</span></span>|<span data-ttu-id="fa001-137">int</span><span class="sxs-lookup"><span data-stu-id="fa001-137">int</span></span>|<span data-ttu-id="fa001-p106">Пропуск первых n результатов; эту функцию удобно использовать при разбиении результатов на страницы. Эта возможность не поддерживается при использовании параметра *$search*.</span><span class="sxs-lookup"><span data-stu-id="fa001-p106">Skip the first n results, useful for paging. This is not supported when using *$search*.</span></span>|
|<span data-ttu-id="fa001-140">$top</span><span class="sxs-lookup"><span data-stu-id="fa001-140">$top</span></span>|<span data-ttu-id="fa001-141">int</span><span class="sxs-lookup"><span data-stu-id="fa001-141">int</span></span>|<span data-ttu-id="fa001-142">Количество возвращаемых результатов.</span><span class="sxs-lookup"><span data-stu-id="fa001-142">Number of results to be returned.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="fa001-143">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="fa001-143">Request headers</span></span>
| <span data-ttu-id="fa001-144">Имя</span><span class="sxs-lookup"><span data-stu-id="fa001-144">Name</span></span>      |<span data-ttu-id="fa001-145">Описание</span><span class="sxs-lookup"><span data-stu-id="fa001-145">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fa001-146">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fa001-146">Authorization</span></span>  | <span data-ttu-id="fa001-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fa001-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fa001-149">Accept</span><span class="sxs-lookup"><span data-stu-id="fa001-149">Accept</span></span> | <span data-ttu-id="fa001-150">application/json</span><span class="sxs-lookup"><span data-stu-id="fa001-150">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="fa001-151">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fa001-151">Request body</span></span>
<span data-ttu-id="fa001-152">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fa001-152">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="fa001-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa001-153">Response</span></span>
<span data-ttu-id="fa001-p108">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [person](../resources/person.md) в тексте ответа. Отклик может содержать один объект person либо коллекцию объектов person.</span><span class="sxs-lookup"><span data-stu-id="fa001-p108">If successful, this method returns a `200 OK` response code and a collection of [person](../resources/person.md) objects in the response body. The response can contain one person object or a collection of person objects.</span></span> 
## <a name="examples"></a><span data-ttu-id="fa001-156">Примеры</span><span class="sxs-lookup"><span data-stu-id="fa001-156">Examples</span></span>

### <a name="get-a-collection-of-relevant-people"></a><span data-ttu-id="fa001-157">Получение коллекции релевантных людей</span><span class="sxs-lookup"><span data-stu-id="fa001-157">Get a collection of relevant people</span></span> 

<span data-ttu-id="fa001-158">С помощью указанного ниже запроса можно получить людей, наиболее релевантных для пользователя, выполнившего вход в систему (`/me`), на основании его шаблонов общения и совместной работы, а также бизнес-отношений.</span><span class="sxs-lookup"><span data-stu-id="fa001-158">The following request gets the people most relevant to the signed-in user (`/me`), based on communication and collaboration patterns and business relationships.</span></span> 
<!-- {
  "blockType": "request",
  "name": "get_person"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/people/
```

<span data-ttu-id="fa001-p109">В примере ниже показан отклик. По умолчанию в каждом отклике возвращается 10 записей. Вы можете изменить количество возвращаемых записей с помощью параметра запроса *$top*. В этом примере показано, как использовать параметр запроса *$top* для ограничения количества записей (до 3 шт.) в отклике.</span><span class="sxs-lookup"><span data-stu-id="fa001-p109">The following example shows the response. By default, each response returns 10 records. You can change this by using the *$top* query parameter. This example uses *$top* to limit the response to three records.</span></span>
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
### <a name="search-other-users-relevant-people"></a><span data-ttu-id="fa001-163">Поиск людей, релевантных для другого пользователя</span><span class="sxs-lookup"><span data-stu-id="fa001-163">Search other user’s relevant people</span></span>

<span data-ttu-id="fa001-p110">Указанный ниже запрос возвращает людей, наиболее релевантных для другого пользователя в организации пользователя, выполнившего вход в систему. Для выполнения этого запроса требуется разрешение People.Read.All. В этом примере отображаются люди, релевантные для пользователя Roscoe Seidel.</span><span class="sxs-lookup"><span data-stu-id="fa001-p110">The following request gets the people most relevant to another person in the signed-in user's organization. This request requires the People.Read.All permission. In this example, Roscoe Seidel's relevant people are displayed.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_person"
}-->

```http
GET https://graph.microsoft.com/v1.0/users('roscoes@contoso.com')/people/
```

<span data-ttu-id="fa001-p111">В примере ниже показан отклик. По умолчанию в каждом отклике возвращается 10 записей. Вы можете изменить количество возвращаемых записей с помощью параметра *$top*. В этом примере показано, как использовать параметр запроса *$top* для ограничения количества записей (до 3 шт.) в отклике.</span><span class="sxs-lookup"><span data-stu-id="fa001-p111">The following example shows the response. By default, each response returns 10 records. You can change this by using the *$top* parameter. This example uses *$top* to limit the response to three records.</span></span>

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
