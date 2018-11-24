# <a name="list-pages"></a><span data-ttu-id="c7c93-101">Перечисление страниц</span><span class="sxs-lookup"><span data-stu-id="c7c93-101">List pages</span></span>

<span data-ttu-id="c7c93-102">Получение списка объектов [page](../resources/page.md).</span><span class="sxs-lookup"><span data-stu-id="c7c93-102">Retrieve a list of [page](../resources/page.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="c7c93-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c7c93-103">Permissions</span></span>
<span data-ttu-id="c7c93-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c7c93-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c7c93-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c7c93-106">Permission type</span></span>      | <span data-ttu-id="c7c93-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c7c93-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c7c93-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c7c93-108">Delegated (work or school account)</span></span> | <span data-ttu-id="c7c93-109">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7c93-109">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="c7c93-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c7c93-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7c93-111">Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7c93-111">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="c7c93-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c7c93-112">Application</span></span> | <span data-ttu-id="c7c93-113">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7c93-113">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c7c93-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c7c93-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/pages
GET /users/{id | userPrincipalName}/onenote/pages
GET /groups/{id}/onenote/pages
GET /sites/{id}/onenote/pages
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c7c93-115">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c7c93-115">Optional query parameters</span></span>
<span data-ttu-id="c7c93-116">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c7c93-116">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="c7c93-p102">Запрос страниц по умолчанию возвращает первые 20 страниц, упорядоченные по атрибуту `lastModifiedTime desc`. Если запрос по умолчанию возвращает более 20 страниц, ответ содержит URL-адрес `@odata.nextLink`, который можно использовать для перехода на следующую страницу результатов. Максимальное количество страниц, возвращаемых по запросу `top`, — 100.</span><span class="sxs-lookup"><span data-stu-id="c7c93-p102">The default query for pages returns the top 20 pages ordered by `lastModifiedTime desc`. If the default query returns more than 20 pages, the response contains an `@odata.nextLink` that you can use to page through the result set. The maximum number of pages returned for a `top` request is 100.</span></span>

<span data-ttu-id="c7c93-p103">Ответ по умолчанию разворачивает `parentSection` и выбирает свойства `id`, `displayName` и `self` раздела. Допустимые значения `expand` для страниц: `parentNotebook` и `parentSection`.</span><span class="sxs-lookup"><span data-stu-id="c7c93-p103">The default response expands `parentSection` and selects the section's `id`, `displayName`, and `self` properties. Valid `expand` values for pages are `parentNotebook` and `parentSection`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c7c93-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c7c93-122">Request headers</span></span>
| <span data-ttu-id="c7c93-123">Имя</span><span class="sxs-lookup"><span data-stu-id="c7c93-123">Name</span></span>       | <span data-ttu-id="c7c93-124">Тип</span><span class="sxs-lookup"><span data-stu-id="c7c93-124">Type</span></span> | <span data-ttu-id="c7c93-125">Описание</span><span class="sxs-lookup"><span data-stu-id="c7c93-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c7c93-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7c93-126">Authorization</span></span>  | <span data-ttu-id="c7c93-127">string</span><span class="sxs-lookup"><span data-stu-id="c7c93-127">string</span></span>  | <span data-ttu-id="c7c93-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c7c93-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c7c93-130">Accept</span><span class="sxs-lookup"><span data-stu-id="c7c93-130">Accept</span></span> | <span data-ttu-id="c7c93-131">строка</span><span class="sxs-lookup"><span data-stu-id="c7c93-131">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="c7c93-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c7c93-132">Request body</span></span>
<span data-ttu-id="c7c93-133">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c7c93-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7c93-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="c7c93-134">Response</span></span>

<span data-ttu-id="c7c93-135">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию объектов [page](../resources/page.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c7c93-135">If successful, this method returns a `200 OK` response code and a collection of [page](../resources/page.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c7c93-136">Пример</span><span class="sxs-lookup"><span data-stu-id="c7c93-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c7c93-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7c93-137">Request</span></span>
<span data-ttu-id="c7c93-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c7c93-138">Here is an example of the request.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/pages
```
##### <a name="response"></a><span data-ttu-id="c7c93-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="c7c93-139">Response</span></span>
<span data-ttu-id="c7c93-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c7c93-140">Here is an example of the response.</span></span> <span data-ttu-id="c7c93-141">Примечание: Для краткости усекается объект ответа, показано ниже.</span><span class="sxs-lookup"><span data-stu-id="c7c93-141">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="c7c93-142">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c7c93-142">All of the properties will be returned from an actual call.</span></span>
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