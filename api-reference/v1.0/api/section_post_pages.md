# <a name="create-page"></a><span data-ttu-id="1da87-101">Создание страницы</span><span class="sxs-lookup"><span data-stu-id="1da87-101">Create page</span></span>

<span data-ttu-id="1da87-102">Создание объекта [page](../resources/page.md) в указанном разделе.</span><span class="sxs-lookup"><span data-stu-id="1da87-102">Create a new [page](../resources/page.md) in the specified section.</span></span>

## <a name="permissions"></a><span data-ttu-id="1da87-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1da87-103">Permissions</span></span>
<span data-ttu-id="1da87-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1da87-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1da87-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1da87-106">Permission type</span></span>      | <span data-ttu-id="1da87-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1da87-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1da87-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1da87-108">Delegated (work or school account)</span></span> | <span data-ttu-id="1da87-109">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1da87-109">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="1da87-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1da87-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1da87-111">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1da87-111">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="1da87-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1da87-112">Application</span></span> | <span data-ttu-id="1da87-113">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1da87-113">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1da87-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1da87-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/pages
POST /users/{id | userPrincipalName}/onenote/sections/{id}/pages
POST /groups/{id}/onenote/sections/{id}/pages
POST /sites/{id}/onenote/sections/{id}/pages
```
## <a name="request-headers"></a><span data-ttu-id="1da87-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1da87-115">Request headers</span></span>
| <span data-ttu-id="1da87-116">Имя</span><span class="sxs-lookup"><span data-stu-id="1da87-116">Name</span></span>       | <span data-ttu-id="1da87-117">Тип</span><span class="sxs-lookup"><span data-stu-id="1da87-117">Type</span></span> | <span data-ttu-id="1da87-118">Описание</span><span class="sxs-lookup"><span data-stu-id="1da87-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1da87-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="1da87-119">Authorization</span></span>  | <span data-ttu-id="1da87-120">string</span><span class="sxs-lookup"><span data-stu-id="1da87-120">string</span></span>  | <span data-ttu-id="1da87-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1da87-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1da87-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1da87-123">Content-Type</span></span> | <span data-ttu-id="1da87-124">string</span><span class="sxs-lookup"><span data-stu-id="1da87-124">string</span></span> | <span data-ttu-id="1da87-p103">`text/html` или `application/xhtml+xml` для содержимого HTML, в том числе для необходимой части Presentation составных запросов. В составных запросах используется тип содержимого `multipart/form-data; boundary=your-boundary`.</span><span class="sxs-lookup"><span data-stu-id="1da87-p103">`text/html` or `application/xhtml+xml` for the HTML content, including for the required "Presentation" part of multipart requests. Multipart requests use the `multipart/form-data; boundary=your-boundary` content type.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1da87-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1da87-127">Request body</span></span>
<span data-ttu-id="1da87-128">В тексте запроса укажите HTML-содержимое страницы.</span><span class="sxs-lookup"><span data-stu-id="1da87-128">In the request body, supply the page HTML content.</span></span>

<span data-ttu-id="1da87-p104">Текст может содержать HTML-код, размещенный прямо в тексте запроса, либо формат составного сообщения, как показано в примере. Если вы отправляете двоичные данные, необходимо отправить составной запрос.</span><span class="sxs-lookup"><span data-stu-id="1da87-p104">The body can contain HTML placed directly in the request body, or it can contain a multipart message format as shown in the example. If you're sending binary data, then you must send a multipart request.</span></span>

## <a name="response"></a><span data-ttu-id="1da87-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="1da87-131">Response</span></span>

<span data-ttu-id="1da87-132">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и новый объект [page](../resources/page.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="1da87-132">If successful, this method returns `201 Created` response code and the new [page](../resources/page.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1da87-133">Пример</span><span class="sxs-lookup"><span data-stu-id="1da87-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1da87-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="1da87-134">Request</span></span>
<span data-ttu-id="1da87-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1da87-135">Here is an example of the request.</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/sections/{id}/pages
Content-length: 312
Content-type: multipart/form-data; boundary=MyPartBoundary198374

--MyPartBoundary198374
Content-Disposition:form-data; name="Presentation"
Content-Type:text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with <i>rendered</i> images and an <b>attached</b> file</title>
    <meta name="created" content="2015-07-22T09:00:00-08:00" />
  </head>
  <body>
    <p>Here's an image from an online source:</p>
    <img src="http://..." alt="an image on the page" width="500" />
    <p>Here's an image uploaded as binary data:</p>
    <img src="name:imageBlock1" alt="an image on the page" width="300" />
    <p>Here's a file attachment:</p>
    <object data-attachment="FileName.pdf" data="name:fileBlock1" type="application/pdf" />
  </body>
</html>

--MyPartBoundary198374
Content-Disposition:form-data; name="imageBlock1"
Content-Type:image/jpeg

... binary image data ...

--MyPartBoundary198374
Content-Disposition:form-data; name="fileBlock1"
Content-Type:application/pdf

... binary file data ...

--MyPartBoundary198374--
```
##### <a name="response"></a><span data-ttu-id="1da87-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="1da87-136">Response</span></span>
<span data-ttu-id="1da87-p105">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1da87-p105">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "lastModifiedDateTime": "2016-10-19T10:37:00Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Page",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
