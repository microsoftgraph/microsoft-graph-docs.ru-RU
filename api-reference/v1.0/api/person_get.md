# <a name="get-person"></a><span data-ttu-id="ba43d-101">Вывод сведений о человеке</span><span class="sxs-lookup"><span data-stu-id="ba43d-101">Get person</span></span>

<span data-ttu-id="ba43d-102">Получение свойств и связей объекта [person](../resources/person.md).</span><span class="sxs-lookup"><span data-stu-id="ba43d-102">Retrieve the properties and relationships of a [person](../resources/person.md) object.</span></span>

<span data-ttu-id="ba43d-p101">Для получения этих сведений используйте API службы "Люди". Примеры см. в разделе [Примеры](#examples) и статье о том, как [получить релевантную информацию о людях](../../../concepts/people_example.md).</span><span class="sxs-lookup"><span data-stu-id="ba43d-p101">You can get this information via the People API. For examples, see the [Examples](#examples) section and the article [Get relevant information about people](../../../concepts/people_example.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ba43d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ba43d-105">Permissions</span></span>
<span data-ttu-id="ba43d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ba43d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>
 

|<span data-ttu-id="ba43d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ba43d-108">Permission type</span></span>      | <span data-ttu-id="ba43d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ba43d-109">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="ba43d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ba43d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ba43d-111">People.Read, People.Read.All</span><span class="sxs-lookup"><span data-stu-id="ba43d-111">People.Read, People.Read.All</span></span>    | 
|<span data-ttu-id="ba43d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ba43d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba43d-113">People.Read</span><span class="sxs-lookup"><span data-stu-id="ba43d-113">People.Read</span></span>    | 
|<span data-ttu-id="ba43d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ba43d-114">Application</span></span> | <span data-ttu-id="ba43d-115">People.Read.All</span><span class="sxs-lookup"><span data-stu-id="ba43d-115">People.Read.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="ba43d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ba43d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/people/?$search='{property_value}'
GET /me/people/?$filter={person_property} eq '{property_value}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ba43d-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ba43d-117">Optional query parameters</span></span>
|<span data-ttu-id="ba43d-118">Имя</span><span class="sxs-lookup"><span data-stu-id="ba43d-118">Name</span></span>|<span data-ttu-id="ba43d-119">Значение</span><span class="sxs-lookup"><span data-stu-id="ba43d-119">Value</span></span>|<span data-ttu-id="ba43d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ba43d-120">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="ba43d-121">$filter</span><span class="sxs-lookup"><span data-stu-id="ba43d-121">$filter</span></span>|<span data-ttu-id="ba43d-122">string</span><span class="sxs-lookup"><span data-stu-id="ba43d-122">string</span></span>|<span data-ttu-id="ba43d-123">Позволяет возвращать в отклике только тех людей, чьи записи содержат указанные критерии.</span><span class="sxs-lookup"><span data-stu-id="ba43d-123">Limits the response to only those people whose record contains the specified criteria.</span></span>|
|<span data-ttu-id="ba43d-124">$orderby</span><span class="sxs-lookup"><span data-stu-id="ba43d-124">$orderby</span></span>|<span data-ttu-id="ba43d-125">string</span><span class="sxs-lookup"><span data-stu-id="ba43d-125">string</span></span>|<span data-ttu-id="ba43d-p103">По умолчанию данные о людях в отклике сортируются по степени соответствия запросу. Этот порядок можно изменить с помощью параметра *$orderby*.</span><span class="sxs-lookup"><span data-stu-id="ba43d-p103">By default, the people in the response are sorted by their relevance to your query. You can change the order of the people in the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="ba43d-128">$search</span><span class="sxs-lookup"><span data-stu-id="ba43d-128">$search</span></span>|<span data-ttu-id="ba43d-129">string</span><span class="sxs-lookup"><span data-stu-id="ba43d-129">string</span></span>|<span data-ttu-id="ba43d-p104">Поиск пользователей по имени или псевдониму. Поддерживается функция нечеткого соответствия.</span><span class="sxs-lookup"><span data-stu-id="ba43d-p104">Search for people by name or alias. Supports fuzzy matching.</span></span>|
|<span data-ttu-id="ba43d-132">$select</span><span class="sxs-lookup"><span data-stu-id="ba43d-132">$select</span></span>|<span data-ttu-id="ba43d-133">string</span><span class="sxs-lookup"><span data-stu-id="ba43d-133">string</span></span>|<span data-ttu-id="ba43d-p105">Список разделенных запятыми свойств, которые необходимо включить в отклик. Для оптимизации производительности выбирайте только необходимые свойства.</span><span class="sxs-lookup"><span data-stu-id="ba43d-p105">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>|
|<span data-ttu-id="ba43d-136">$skip</span><span class="sxs-lookup"><span data-stu-id="ba43d-136">$skip</span></span>|<span data-ttu-id="ba43d-137">int</span><span class="sxs-lookup"><span data-stu-id="ba43d-137">int</span></span>|<span data-ttu-id="ba43d-p106">Пропуск первых n результатов; эту функцию удобно использовать при разбиении результатов на страницы. Эта возможность не поддерживается при использовании параметра *$search*.</span><span class="sxs-lookup"><span data-stu-id="ba43d-p106">Skip the first n results, useful for paging. This is not supported when using *$search*.</span></span>|
|<span data-ttu-id="ba43d-140">$top</span><span class="sxs-lookup"><span data-stu-id="ba43d-140">$top</span></span>|<span data-ttu-id="ba43d-141">int</span><span class="sxs-lookup"><span data-stu-id="ba43d-141">int</span></span>|<span data-ttu-id="ba43d-142">Число возвращаемых результатов.</span><span class="sxs-lookup"><span data-stu-id="ba43d-142">Number of results to be returned.</span></span>|

## <a name="parameters"></a><span data-ttu-id="ba43d-143">Параметры</span><span class="sxs-lookup"><span data-stu-id="ba43d-143">Parameters</span></span>
| <span data-ttu-id="ba43d-144">Параметр</span><span class="sxs-lookup"><span data-stu-id="ba43d-144">Parameter</span></span> |<span data-ttu-id="ba43d-145">Тип</span><span class="sxs-lookup"><span data-stu-id="ba43d-145">Type</span></span>       |<span data-ttu-id="ba43d-146">Описание</span><span class="sxs-lookup"><span data-stu-id="ba43d-146">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="ba43d-147">property_value</span><span class="sxs-lookup"><span data-stu-id="ba43d-147">property_value</span></span>|<span data-ttu-id="ba43d-148">String</span><span class="sxs-lookup"><span data-stu-id="ba43d-148">String</span></span>     |<span data-ttu-id="ba43d-p107">Значение сопоставляемого расширенного свойства. Его необходимо указывать, если этот параметр указан для соответствующего сценария в разделе **HTTP-запрос**.</span><span class="sxs-lookup"><span data-stu-id="ba43d-p107">The value of the extended property to match. Required where listed in the **HTTP request** section.</span></span>|
|<span data-ttu-id="ba43d-151">person_property</span><span class="sxs-lookup"><span data-stu-id="ba43d-151">person_property</span></span>|<span data-ttu-id="ba43d-152">String</span><span class="sxs-lookup"><span data-stu-id="ba43d-152">String</span></span>    |<span data-ttu-id="ba43d-p108">Соответствие свойству person. Его необходимо указывать, если этот параметр указан для соответствующего сценария в разделе **HTTP-запрос**.</span><span class="sxs-lookup"><span data-stu-id="ba43d-p108">The person property to match. Required where listed in the **HTTP request** section.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="ba43d-155">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ba43d-155">Request headers</span></span>
| <span data-ttu-id="ba43d-156">Имя</span><span class="sxs-lookup"><span data-stu-id="ba43d-156">Name</span></span>      |<span data-ttu-id="ba43d-157">Описание</span><span class="sxs-lookup"><span data-stu-id="ba43d-157">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ba43d-158">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ba43d-158">Authorization</span></span>  | <span data-ttu-id="ba43d-p109">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ba43d-p109">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ba43d-161">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ba43d-161">Request body</span></span>
<span data-ttu-id="ba43d-162">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ba43d-162">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="ba43d-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba43d-163">Response</span></span>
<span data-ttu-id="ba43d-p110">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [person](../resources/person.md) в тексте отклика. Отклик может содержать как один, так и коллекцию экземпляров person.</span><span class="sxs-lookup"><span data-stu-id="ba43d-p110">If successful, this method returns a `200 OK` response code and a [person](../resources/person.md) object in the response body. The response can contain one person instance or a collection of person instances.</span></span> 
## <a name="examples"></a><span data-ttu-id="ba43d-166">Примеры</span><span class="sxs-lookup"><span data-stu-id="ba43d-166">Examples</span></span>
### <a name="perform-a-search"></a><span data-ttu-id="ba43d-167">Выполнение поиска</span><span class="sxs-lookup"><span data-stu-id="ba43d-167">Perform a search</span></span> 
<span data-ttu-id="ba43d-168">В приведенном ниже запросе выполняется поиск пользователя по имени Irene McGowan.</span><span class="sxs-lookup"><span data-stu-id="ba43d-168">The following request does a search for a person named Irene McGowan.</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_person"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="Irene McGowan"
```

<span data-ttu-id="ba43d-169">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ba43d-169">The following example shows the response.</span></span> 

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
           "id": "C0BD1BA1-A84E-4796-9C65-F8A0293741D1",
           "displayName": "Irene McGowan",
           "givenName": "Irene",
           "surname": "McGowan",
           "birthday": "",
           "personNotes": "",
           "isFavorite": false,
           "jobTitle": "Auditor",
           "companyName": null,
           "yomiCompany": "",
           "department": "Finance",
           "officeLocation": "12/1110",
           "profession": "",
           "userPrincipalName": "irenem@contoso.onmicrosoft.com",
           "imAddress": "sip:irenem@contoso.onmicrosoft.com",
           "scoredEmailAddresses": [
               {
                   "address": "irenem@contoso.onmicrosoft.com",
                   "relevanceScore": -16.446060612802224
               }
           ],
           "phones": [
               {
                   "type": "Business",
                   "number": "+1 412 555 0109"
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
### <a name="select-the-fields-to-return-in-a-filtered-response"></a><span data-ttu-id="ba43d-170">Выбор полей, которые возвращаются в отфильтрованном отклике</span><span class="sxs-lookup"><span data-stu-id="ba43d-170">Select the fields to return in a filtered response</span></span> 
<span data-ttu-id="ba43d-171">Сочетая параметры *$select* и *$filter*, вы можете создать настраиваемый список людей, релевантных для пользователя, и получать только те поля, которые необходимы вашему приложению.</span><span class="sxs-lookup"><span data-stu-id="ba43d-171">You can combine the *$select* and *$filter* parameters to create a custom list of people relevant to the user and get only the fields that your application needs.</span></span> 

<span data-ttu-id="ba43d-p111">В примере ниже показано, как получить значения полей **displayName** и **scoredEmailAddresses** для людей, чьи отображаемые имена совпадают с заданными. В этом примере показано, как возвратить людей c отображаемыми именами Lorrie Frye.</span><span class="sxs-lookup"><span data-stu-id="ba43d-p111">The following example gets the **displayName** and **scoredEmailAddresses** of people whose display name equals the specified name. In this example, only people whose display name equals "Lorrie Frye" are returned.</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_person"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/people/?$select=displayName,scoredEmailAddresses&$filter=displayName eq 'Lorrie Frye'
```

<span data-ttu-id="ba43d-174">В примере ниже показан отклик.</span><span class="sxs-lookup"><span data-stu-id="ba43d-174">The following example shows the response.</span></span> 

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
            "scoredEmailAddresses": [
                {
                    "address": "Lorrief@contoso.onmicrosoft.com",
                    "relevanceScore": 8
                }
            ]
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get person",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
