# <a name="get-person"></a><span data-ttu-id="a0126-101">Вывод сведений о человеке</span><span class="sxs-lookup"><span data-stu-id="a0126-101">Get person</span></span>

<span data-ttu-id="a0126-102">Получение свойств и связей объекта [person](../resources/person.md).</span><span class="sxs-lookup"><span data-stu-id="a0126-102">Retrieve the properties and relationships of a [person](../resources/person.md) object.</span></span>

<span data-ttu-id="a0126-p101">Для получения этих сведений используйте API службы "Люди". Примеры см. в разделе [Примеры](#examples) и статье о том, как [получить релевантную информацию о людях](../../../concepts/people_example.md).</span><span class="sxs-lookup"><span data-stu-id="a0126-p101">You can get this information via the People API. For examples, see the [Examples](#examples) section and the article [Get relevant information about people](../../../concepts/people_example.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a0126-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a0126-105">Permissions</span></span>
<span data-ttu-id="a0126-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a0126-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>
 

|<span data-ttu-id="a0126-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a0126-108">Permission type</span></span>      | <span data-ttu-id="a0126-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a0126-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a0126-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a0126-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a0126-111">People.Read, People.Read.All</span><span class="sxs-lookup"><span data-stu-id="a0126-111">People.Read, People.Read.All</span></span>    |
|<span data-ttu-id="a0126-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a0126-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0126-113">People.Read</span><span class="sxs-lookup"><span data-stu-id="a0126-113">People.Read</span></span>    |
|<span data-ttu-id="a0126-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a0126-114">Application</span></span> | <span data-ttu-id="a0126-115">People.Read.All</span><span class="sxs-lookup"><span data-stu-id="a0126-115">People.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a0126-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a0126-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/people/{id}
GET /users/{id | userPrincipalName}/people/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a0126-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a0126-117">Optional query parameters</span></span>
<span data-ttu-id="a0126-118">Этот метод поддерживает следующие [параметры запроса OData](../../../concepts/people_example.md) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a0126-118">This method supports the [OData Query Parameters](../../../concepts/people_example.md) to help customize the response.</span></span>

|<span data-ttu-id="a0126-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a0126-119">Name</span></span>|<span data-ttu-id="a0126-120">Значение</span><span class="sxs-lookup"><span data-stu-id="a0126-120">Value</span></span>|<span data-ttu-id="a0126-121">Описание</span><span class="sxs-lookup"><span data-stu-id="a0126-121">Description</span></span>| 
|:---------------|:--------|:-------| 
|<span data-ttu-id="a0126-122">$filter</span><span class="sxs-lookup"><span data-stu-id="a0126-122">$filter</span></span>|<span data-ttu-id="a0126-123">string</span><span class="sxs-lookup"><span data-stu-id="a0126-123">string</span></span>|<span data-ttu-id="a0126-124">Позволяет возвращать в отклике только тех людей, чьи записи содержат указанные критерии.</span><span class="sxs-lookup"><span data-stu-id="a0126-124">Limits the response to only those people whose record contains the specified criteria.</span></span>| 
|<span data-ttu-id="a0126-125">$orderby</span><span class="sxs-lookup"><span data-stu-id="a0126-125">$orderby</span></span>|<span data-ttu-id="a0126-126">строка</span><span class="sxs-lookup"><span data-stu-id="a0126-126">string</span></span>|<span data-ttu-id="a0126-127">По умолчанию люди в ответе сортируются по степени соответствия запросу.</span><span class="sxs-lookup"><span data-stu-id="a0126-127">By default, the people in the response are sorted by their relevance to your query. You can change the order of the people in the response using the $orderby parameter.</span></span> <span data-ttu-id="a0126-128">Этот порядок можно изменить с помощью параметра *$orderby*.</span><span class="sxs-lookup"><span data-stu-id="a0126-128">By default, the people in the response are sorted by their relevance to your query. You can change the order of the people in the response using the *$orderby* parameter.</span></span>| 
|<span data-ttu-id="a0126-129">$search</span><span class="sxs-lookup"><span data-stu-id="a0126-129">$search</span></span>|<span data-ttu-id="a0126-130">string</span><span class="sxs-lookup"><span data-stu-id="a0126-130">string</span></span>|<span data-ttu-id="a0126-131">Поиск пользователей по имени или псевдониму.</span><span class="sxs-lookup"><span data-stu-id="a0126-131">Search for people by name or alias. Supports fuzzy matching.</span></span> <span data-ttu-id="a0126-132">Поддерживается нечеткое соответствие.</span><span class="sxs-lookup"><span data-stu-id="a0126-132">Supports Fuzzy matching</span></span>| 
|<span data-ttu-id="a0126-133">$select</span><span class="sxs-lookup"><span data-stu-id="a0126-133">$select</span></span>|<span data-ttu-id="a0126-134">string</span><span class="sxs-lookup"><span data-stu-id="a0126-134">string</span></span>|<span data-ttu-id="a0126-p105">Список разделенных запятыми свойств, которые необходимо включить в отклик. Для оптимизации производительности выбирайте только необходимые свойства.</span><span class="sxs-lookup"><span data-stu-id="a0126-p105">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>| 
|<span data-ttu-id="a0126-137">$skip</span><span class="sxs-lookup"><span data-stu-id="a0126-137">$skip</span></span>|<span data-ttu-id="a0126-138">int</span><span class="sxs-lookup"><span data-stu-id="a0126-138">int</span></span>|<span data-ttu-id="a0126-p106">Пропуск первых n результатов; эту функцию удобно использовать при разбиении результатов на страницы. Эта возможность не поддерживается при использовании параметра *$search*.</span><span class="sxs-lookup"><span data-stu-id="a0126-p106">Skip the first n results, useful for paging. This is not supported when using *$search*.</span></span>| 
|<span data-ttu-id="a0126-141">$top</span><span class="sxs-lookup"><span data-stu-id="a0126-141">$top</span></span>|<span data-ttu-id="a0126-142">int</span><span class="sxs-lookup"><span data-stu-id="a0126-142">int</span></span>|<span data-ttu-id="a0126-143">Количество возвращаемых результатов.</span><span class="sxs-lookup"><span data-stu-id="a0126-143">Number of results to be returned.</span></span>| 

## <a name="request-headers"></a><span data-ttu-id="a0126-144">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a0126-144">Request headers</span></span>
| <span data-ttu-id="a0126-145">Имя</span><span class="sxs-lookup"><span data-stu-id="a0126-145">Name</span></span>      |<span data-ttu-id="a0126-146">Описание</span><span class="sxs-lookup"><span data-stu-id="a0126-146">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a0126-147">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a0126-147">Authorization</span></span>  | <span data-ttu-id="a0126-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a0126-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a0126-150">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a0126-150">Request body</span></span>
<span data-ttu-id="a0126-151">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a0126-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a0126-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="a0126-152">Response</span></span>
<span data-ttu-id="a0126-153">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [person](../resources/person.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a0126-153">If successful, this method returns a `200 OK` response code and a [ListItemVersion](../resources/person.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a0126-154">Примеры</span><span class="sxs-lookup"><span data-stu-id="a0126-154">Examples</span></span>
#### <a name="request-1"></a><span data-ttu-id="a0126-155">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="a0126-155">Request 1</span></span>
<span data-ttu-id="a0126-156">Ниже приведен пример запроса, который возвращает пользователя с этим идентификатором в организации.</span><span class="sxs-lookup"><span data-stu-id="a0126-156">The following is an example of the request that gets the person who has this ID in the user's organization.</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_person_by_id"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/people/e3d0513b-449e-4198-ba6f-bd97ae7cae85
```

#### <a name="response-1"></a><span data-ttu-id="a0126-157">Ответ 1</span><span class="sxs-lookup"><span data-stu-id="a0126-157">Response 1</span></span>
<span data-ttu-id="a0126-158">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a0126-158">Here is an example of the response.</span></span>

><span data-ttu-id="a0126-159">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a0126-159">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a0126-160">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a0126-160">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_person_by_id",
  "truncated": true,
  "@odata.type": "microsoft.graph.person"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 629

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
```

#### <a name="request-2"></a><span data-ttu-id="a0126-161">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="a0126-161">Request 2</span></span>
<span data-ttu-id="a0126-162">Ниже приведен пример запроса, который возвращает пользователя с этим идентификатором в организации и ограничивает ответ выбранными свойствами.</span><span class="sxs-lookup"><span data-stu-id="a0126-162">The following is an example of the request that gets the person who has this ID in the user's organization and restricts the response to the selected properties.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_person_by_id_with_select"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/people/e3d0513b-449e-4198-ba6f-bd97ae7cae85?$select=displayName
```
#### <a name="response-2"></a><span data-ttu-id="a0126-163">Ответ 2</span><span class="sxs-lookup"><span data-stu-id="a0126-163">Response 2</span></span>
<span data-ttu-id="a0126-164">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a0126-164">Here is an example of the response.</span></span>

><span data-ttu-id="a0126-165">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a0126-165">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a0126-166">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a0126-166">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_person_by_id_with_select",
  "truncated": true,
  "@odata.type": "microsoft.graph.person"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 305

{
  "id": "e3d0513b-449e-4198-ba6f-bd97ae7cae85",
  "displayName": "Isaiah Langer"
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
