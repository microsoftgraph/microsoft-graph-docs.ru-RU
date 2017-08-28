# <a name="list-pages"></a><span data-ttu-id="a7d04-101">Перечисление страниц</span><span class="sxs-lookup"><span data-stu-id="a7d04-101">List pages</span></span>

<span data-ttu-id="a7d04-102">Получение списка объектов [page](../resources/page.md) из указанного раздела.</span><span class="sxs-lookup"><span data-stu-id="a7d04-102">Retrieve a list of [page](../resources/page.md) objects from the specified section.</span></span>
## <a name="permissions"></a><span data-ttu-id="a7d04-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a7d04-103">Permissions</span></span>
<span data-ttu-id="a7d04-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a7d04-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a7d04-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a7d04-106">Permission type</span></span>      | <span data-ttu-id="a7d04-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a7d04-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a7d04-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a7d04-108">Delegated (work or school account)</span></span> | <span data-ttu-id="a7d04-109">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7d04-109">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="a7d04-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a7d04-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7d04-111">Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a7d04-111">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="a7d04-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a7d04-112">Application</span></span> | <span data-ttu-id="a7d04-113">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7d04-113">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a7d04-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a7d04-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sections/{id}/pages
GET /users/{id | userPrincipalName}/onenote/sections/{id}/pages
GET /groups/{id}/onenote/sections/{id}/pages
GET /sites/{id}/onenote/sections/{id}/pages
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a7d04-115">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a7d04-115">Optional query parameters</span></span>
<span data-ttu-id="a7d04-116">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a7d04-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="a7d04-p102">Запрос страниц по умолчанию возвращает первые 20 страниц, упорядоченные по атрибуту `lastModifiedTime desc`. Если запрос по умолчанию возвращает более 20 страниц, ответ содержит URL-адрес `@odata.nextLink`, который можно использовать для перехода на следующую страницу результатов. Максимальное количество страниц, возвращаемых по запросу `top`, — 100.</span><span class="sxs-lookup"><span data-stu-id="a7d04-p102">The default query for pages returns the top 20 pages ordered by `lastModifiedTime desc`. If the default query returns more than 20 pages, the response contains an `@odata.nextLink` that you can use to page through the result set. The maximum number of pages returned for a `top` request is 100.</span></span>

<span data-ttu-id="a7d04-p103">Ответ по умолчанию разворачивает `parentSection` и выбирает свойства `id`, `name` и `self` раздела. Допустимые значения `expand` для страниц: `parentNotebook` и `parentSection`.</span><span class="sxs-lookup"><span data-stu-id="a7d04-p103">The default response expands `parentSection` and selects the section's `id`, `name`, and `self` properties. Valid `expand` values for pages are `parentNotebook` and `parentSection`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a7d04-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a7d04-122">Request headers</span></span>
| <span data-ttu-id="a7d04-123">Имя</span><span class="sxs-lookup"><span data-stu-id="a7d04-123">Name</span></span>       | <span data-ttu-id="a7d04-124">Тип</span><span class="sxs-lookup"><span data-stu-id="a7d04-124">Type</span></span> | <span data-ttu-id="a7d04-125">Описание</span><span class="sxs-lookup"><span data-stu-id="a7d04-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a7d04-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="a7d04-126">Authorization</span></span>  | <span data-ttu-id="a7d04-127">string</span><span class="sxs-lookup"><span data-stu-id="a7d04-127">string</span></span>  | <span data-ttu-id="a7d04-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a7d04-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a7d04-130">Accept</span><span class="sxs-lookup"><span data-stu-id="a7d04-130">Accept</span></span> | <span data-ttu-id="a7d04-131">строка</span><span class="sxs-lookup"><span data-stu-id="a7d04-131">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="a7d04-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a7d04-132">Request body</span></span>
<span data-ttu-id="a7d04-133">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a7d04-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a7d04-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="a7d04-134">Response</span></span>

<span data-ttu-id="a7d04-135">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию объектов [page](../resources/page.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a7d04-135">If successful, this method returns a `200 OK` response code and a collection of [page](../resources/page.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a7d04-136">Пример</span><span class="sxs-lookup"><span data-stu-id="a7d04-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a7d04-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="a7d04-137">Request</span></span>
<span data-ttu-id="a7d04-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a7d04-138">Here is an example of the request.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/sections/{id}/pages
```
##### <a name="response"></a><span data-ttu-id="a7d04-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7d04-139">Response</span></span>
<span data-ttu-id="a7d04-p105">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a7d04-p105">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 393

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List pages",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->