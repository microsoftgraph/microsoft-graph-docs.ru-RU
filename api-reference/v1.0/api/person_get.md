# <a name="get-person"></a><span data-ttu-id="4f624-101">Вывод сведений о человеке</span><span class="sxs-lookup"><span data-stu-id="4f624-101">Get person</span></span>

<span data-ttu-id="4f624-102">Получение свойств и связей объекта [person](../resources/person.md).</span><span class="sxs-lookup"><span data-stu-id="4f624-102">Retrieve the properties and relationships of [plannerAssignedToTaskBoardTaskFormat](../resources/person.md) object.</span></span>

<span data-ttu-id="4f624-p101">Для получения этих сведений используйте API службы "Люди". Примеры представлены в разделе [Примеры](#examples) и статье [Получение релевантных сведений о людях](../../../concepts/people_example.md).</span><span class="sxs-lookup"><span data-stu-id="4f624-p101">You can get this information via the People API. For examples, see the [Examples](#examples) section and the article [Get relevant information about people](../../../concepts/people_example.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4f624-105">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="4f624-105">Prerequisites</span></span>
<span data-ttu-id="4f624-106">Для применения фрагментов этого API требуются следующие **разрешения**: *People.Read*; *People.Read.All*</span><span class="sxs-lookup"><span data-stu-id="4f624-106">The following **permissions** are required to execute portions of this API: *People.Read*; *People.Read.All*</span></span>
 
## <a name="http-request"></a><span data-ttu-id="4f624-107">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4f624-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/people/?$search='{property_value}'
GET /me/people/?$filter={person_property} eq '{property_value}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4f624-108">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4f624-108">Optional query parameters</span></span>
|<span data-ttu-id="4f624-109">Имя</span><span class="sxs-lookup"><span data-stu-id="4f624-109">Name</span></span>|<span data-ttu-id="4f624-110">Значение</span><span class="sxs-lookup"><span data-stu-id="4f624-110">Value</span></span>|<span data-ttu-id="4f624-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4f624-111">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="4f624-112">$filter</span><span class="sxs-lookup"><span data-stu-id="4f624-112">$filter</span></span>|<span data-ttu-id="4f624-113">string</span><span class="sxs-lookup"><span data-stu-id="4f624-113">string</span></span>|<span data-ttu-id="4f624-114">Ограничивает отклик данными тех людей, чьи записи содержат указанные условия.</span><span class="sxs-lookup"><span data-stu-id="4f624-114">Limits the response to only those people whose record contains the specified criteria.</span></span>|
|<span data-ttu-id="4f624-115">$orderby</span><span class="sxs-lookup"><span data-stu-id="4f624-115">$orderby</span></span>|<span data-ttu-id="4f624-116">string</span><span class="sxs-lookup"><span data-stu-id="4f624-116">string</span></span>|<span data-ttu-id="4f624-p102">По умолчанию данные о людях в отклике сортируются по степени соответствия запросу. Этот порядок можно изменить с помощью параметра *$orderby*.</span><span class="sxs-lookup"><span data-stu-id="4f624-p102">By default, the people in the response are sorted by their relevance to your query. You can change the order of the people in the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="4f624-119">$search</span><span class="sxs-lookup"><span data-stu-id="4f624-119">$search</span></span>|<span data-ttu-id="4f624-120">string</span><span class="sxs-lookup"><span data-stu-id="4f624-120">string</span></span>|<span data-ttu-id="4f624-p103">Поиск пользователей по имени или псевдониму. Поддерживается функция нечеткого соответствия.</span><span class="sxs-lookup"><span data-stu-id="4f624-p103">Search for people by name or alias. Supports fuzzy matching.</span></span>|
|<span data-ttu-id="4f624-123">$select</span><span class="sxs-lookup"><span data-stu-id="4f624-123">$select</span></span>|<span data-ttu-id="4f624-124">string</span><span class="sxs-lookup"><span data-stu-id="4f624-124">string</span></span>|<span data-ttu-id="4f624-p104">Разделенный запятыми список свойств, включаемых в ответ. Для оптимальной производительности требуется выбрать подмножество нужных свойств.</span><span class="sxs-lookup"><span data-stu-id="4f624-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>|
|<span data-ttu-id="4f624-127">$skip</span><span class="sxs-lookup"><span data-stu-id="4f624-127">$skip</span></span>|<span data-ttu-id="4f624-128">int</span><span class="sxs-lookup"><span data-stu-id="4f624-128">int</span></span>|<span data-ttu-id="4f624-p105">Пропуск первых n результатов. Эта функция полезна при разбиении на страницы. Не поддерживается, если используется параметр *$search*.</span><span class="sxs-lookup"><span data-stu-id="4f624-p105">Skip the first n results, useful for paging. This is not supported when using *$search*.</span></span>|
|<span data-ttu-id="4f624-131">$top</span><span class="sxs-lookup"><span data-stu-id="4f624-131">$top</span></span>|<span data-ttu-id="4f624-132">int</span><span class="sxs-lookup"><span data-stu-id="4f624-132">int</span></span>|<span data-ttu-id="4f624-133">Число возвращаемых результатов.</span><span class="sxs-lookup"><span data-stu-id="4f624-133">Number of results to be returned.</span></span>|

## <a name="parameters"></a><span data-ttu-id="4f624-134">Параметры</span><span class="sxs-lookup"><span data-stu-id="4f624-134">Parameters</span></span>
| <span data-ttu-id="4f624-135">Параметр</span><span class="sxs-lookup"><span data-stu-id="4f624-135">Parameter</span></span> |<span data-ttu-id="4f624-136">Тип</span><span class="sxs-lookup"><span data-stu-id="4f624-136">Type</span></span>       |<span data-ttu-id="4f624-137">Описание</span><span class="sxs-lookup"><span data-stu-id="4f624-137">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="4f624-138">property_value</span><span class="sxs-lookup"><span data-stu-id="4f624-138">property_value</span></span>|<span data-ttu-id="4f624-139">String</span><span class="sxs-lookup"><span data-stu-id="4f624-139">String</span></span>     |<span data-ttu-id="4f624-p106">Значение сопоставляемого расширенного свойства. Его необходимо указывать, если этот параметр указан для соответствующего сценария в разделе **HTTP-запрос**.</span><span class="sxs-lookup"><span data-stu-id="4f624-p106">The value of the extended property to match. Required where listed in the HTTP request section above.</span></span>|
|<span data-ttu-id="4f624-142">person_property</span><span class="sxs-lookup"><span data-stu-id="4f624-142">person_property</span></span>|<span data-ttu-id="4f624-143">String</span><span class="sxs-lookup"><span data-stu-id="4f624-143">String</span></span>    |<span data-ttu-id="4f624-p107">Соответствие свойству person. Его необходимо указывать, если этот параметр указан для соответствующего сценария в разделе **HTTP-запрос**.</span><span class="sxs-lookup"><span data-stu-id="4f624-p107">The value of the extended property to match. Required where listed in the HTTP request section above.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="4f624-146">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4f624-146">Request headers</span></span>
| <span data-ttu-id="4f624-147">Имя</span><span class="sxs-lookup"><span data-stu-id="4f624-147">Name</span></span>      |<span data-ttu-id="4f624-148">Описание</span><span class="sxs-lookup"><span data-stu-id="4f624-148">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4f624-149">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4f624-149">Authorization</span></span>  | <span data-ttu-id="4f624-p108">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4f624-p108">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4f624-152">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4f624-152">Request body</span></span>
<span data-ttu-id="4f624-153">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4f624-153">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="4f624-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f624-154">Response</span></span>
<span data-ttu-id="4f624-p109">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [person](../resources/person.md) в тексте отклика. Отклик может содержать как один, так и коллекцию экземпляров person.</span><span class="sxs-lookup"><span data-stu-id="4f624-p109">If successful, this method returns a `200 OK` response code and a [person](../resources/person.md) object in the response body. The response can contain one person instance or a collection of person instances.</span></span> 
## <a name="examples"></a><span data-ttu-id="4f624-157">Примеры</span><span class="sxs-lookup"><span data-stu-id="4f624-157">Examples</span></span>
### <a name="perform-a-search"></a><span data-ttu-id="4f624-158">Выполнение поиска</span><span class="sxs-lookup"><span data-stu-id="4f624-158">Perform a search</span></span> 
<span data-ttu-id="4f624-159">В приведенном ниже запросе выполняется поиск пользователя по имени Irene McGowan.</span><span class="sxs-lookup"><span data-stu-id="4f624-159">The following request does a search for a person named Irene McGowan.</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_person"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="Irene McGowan"
```

<span data-ttu-id="4f624-160">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4f624-160">The following example shows the response.</span></span> 

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
### <a name="select-the-fields-to-return-in-a-filtered-response"></a><span data-ttu-id="4f624-161">Выбор полей, которые возвращаются в отфильтрованном отклике</span><span class="sxs-lookup"><span data-stu-id="4f624-161">Select the fields to return in a filtered response</span></span> 
<span data-ttu-id="4f624-162">Можно объединить параметры *$select* и *$filter*, чтобы создать настраиваемый список людей, имеющих отношение к данному пользователю, при этом возвращаются только поля, которые требуются приложению.</span><span class="sxs-lookup"><span data-stu-id="4f624-162">You can combine the *$select* and *$filter* parameters to create a custom list of people relevant to the user and get only the fields that your application needs.</span></span> 

<span data-ttu-id="4f624-p110">В примере ниже возвращаются данные **displayName** и **scoredEmailAddresses** для людей, чье отображаемое имя соответствует указанному. В этом примере возвращаются сведения только о людях, чье отображаемое имя соответствует имени Lorrie Frye.</span><span class="sxs-lookup"><span data-stu-id="4f624-p110">The following example gets the **displayName** and **scoredEmailAddresses** of people whose display name equals the specified name. In this example, only people whose display name equals "Lorrie Frye" are returned.</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_person"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/people/?$select=displayName,scoredEmailAddresses&$filter=displayName eq 'Lorrie Frye'
```

<span data-ttu-id="4f624-165">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4f624-165">The following example shows the response.</span></span> 

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
