# <a name="get-page"></a><span data-ttu-id="01456-101">Получение страницы</span><span class="sxs-lookup"><span data-stu-id="01456-101">Get page</span></span>

<span data-ttu-id="01456-102">Получение свойств и связей объекта [page](../resources/page.md).</span><span class="sxs-lookup"><span data-stu-id="01456-102">Retrieve the properties and relationships of a [page](../resources/page.md) object.</span></span>

<span data-ttu-id="01456-103">**Получение сведений о странице**</span><span class="sxs-lookup"><span data-stu-id="01456-103">**Getting page information**</span></span>

<span data-ttu-id="01456-104">Доступ к метаданным страницы по ее идентификатору:</span><span class="sxs-lookup"><span data-stu-id="01456-104">Access a page's metadata by page identifier:</span></span>

```
GET /me/onenote/pages/{id}
```

<span data-ttu-id="01456-105">**Получение содержимого страницы**</span><span class="sxs-lookup"><span data-stu-id="01456-105">**Getting page content**</span></span>

<span data-ttu-id="01456-106">Чтобы получить содержимое HTML страницы, вы можете использовать конечную точку `content` страницы:</span><span class="sxs-lookup"><span data-stu-id="01456-106">You can use the page's `content` endpoint to get the HTML content of a page:</span></span>

```
GET /me/onenote/pages/{id}/content[?includeIDs=true]
GET /me/onenote/pages/{id}/$value[?includeIDs=true]
```

<span data-ttu-id="01456-107">Параметр запроса `includeIDs=true` используется для [обновления страниц](../api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="01456-107">The `includeIDs=true` query option is used to [update pages](../api/page_update.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="01456-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="01456-108">Permissions</span></span>
<span data-ttu-id="01456-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="01456-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="01456-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="01456-111">Permission type</span></span>      | <span data-ttu-id="01456-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="01456-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="01456-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01456-113">Delegated (work or school account)</span></span> | <span data-ttu-id="01456-114">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01456-114">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="01456-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01456-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01456-116">Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="01456-116">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="01456-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="01456-117">Application</span></span> | <span data-ttu-id="01456-118">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01456-118">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="01456-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01456-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/pages/{id}
GET /users/{id | userPrincipalName}/onenote/pages/{id}
GET /groups/{id}/onenote/pages/{id}
GET /sites/{id}/onenote/pages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="01456-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="01456-120">Optional query parameters</span></span>
<span data-ttu-id="01456-121">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) `select` и `expand` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="01456-121">This method supports the `select` and `expand` [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="01456-p102">Отклик, возвращаемый по умолчанию, разворачивает `parentSection` и выбирает свойства `id`, `name` и `self` раздела. Допустимые значения `expand` для страниц: `parentNotebook` и `parentSection`.</span><span class="sxs-lookup"><span data-stu-id="01456-p102">The default response expands `parentSection` and selects the section's `id`, `name`, and `self` properties. Valid `expand` values for pages are `parentNotebook` and `parentSection`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="01456-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="01456-124">Request headers</span></span>
| <span data-ttu-id="01456-125">Имя</span><span class="sxs-lookup"><span data-stu-id="01456-125">Name</span></span>       | <span data-ttu-id="01456-126">Тип</span><span class="sxs-lookup"><span data-stu-id="01456-126">Type</span></span> | <span data-ttu-id="01456-127">Описание</span><span class="sxs-lookup"><span data-stu-id="01456-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="01456-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="01456-128">Authorization</span></span>  | <span data-ttu-id="01456-129">string</span><span class="sxs-lookup"><span data-stu-id="01456-129">string</span></span>  | <span data-ttu-id="01456-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="01456-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="01456-132">Accept</span><span class="sxs-lookup"><span data-stu-id="01456-132">Accept</span></span> | <span data-ttu-id="01456-133">строка</span><span class="sxs-lookup"><span data-stu-id="01456-133">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="01456-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="01456-134">Request body</span></span>
<span data-ttu-id="01456-135">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="01456-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="01456-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="01456-136">Response</span></span>

<span data-ttu-id="01456-137">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [page](../resources/page.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="01456-137">If successful, this method returns a `200 OK` response code and the [page](../resources/page.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="01456-138">Пример</span><span class="sxs-lookup"><span data-stu-id="01456-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="01456-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="01456-139">Request</span></span>
<span data-ttu-id="01456-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="01456-140">Here is an example of the request.</span></span>
 <!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/pages/{id}
```
##### <a name="response"></a><span data-ttu-id="01456-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="01456-141">Response</span></span>
<span data-ttu-id="01456-p104">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="01456-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
 <!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 312

{
  "title": "title-value",
  "createdByAppId": "createdByAppId-value",
  "links": {
    "oneNoteClientUrl": {
      "href": "href-value"
    },
    "oneNoteWebUrl": {
      "href": "href-value"
    }
  },
  "contentUrl": "contentUrl-value",
  "content": "content-value",
  "lastModifiedDateTime": "2016-10-19T10:37:00Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get page",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
