---
title: Создание страницы
description: Создание страницы OneNote в разделе по умолчанию записной книжки по умолчанию.
ms.openlocfilehash: 07f5eef560145a9aec1206d6966d1c113774444d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025302"
---
# <a name="create-page"></a><span data-ttu-id="25891-103">Создание страницы</span><span class="sxs-lookup"><span data-stu-id="25891-103">Create page</span></span>

<span data-ttu-id="25891-104">Создание страницы OneNote в разделе по умолчанию записной книжки по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="25891-104">Create a new OneNote page in the default section of the default notebook.</span></span>

<span data-ttu-id="25891-p101">Чтобы создать страницу в другом разделе записной книжки, используемой по умолчанию, примените параметр запроса `sectionName`.  Пример: `../onenote/pages?sectionName=My%20section`</span><span class="sxs-lookup"><span data-stu-id="25891-p101">To create a page in a different section in the default notebook, you can use the `sectionName` query parameter.  Example: `../onenote/pages?sectionName=My%20section`</span></span>

<span data-ttu-id="25891-p102">Операция `POST /onenote/pages` используется только для создания страниц в записной книжке текущего пользователя, используемой по умолчанию. Если вы хотите сделать это в других записных книжках, вы можете [создать страницы в определенном разделе](../api/section-post-pages.md).</span><span class="sxs-lookup"><span data-stu-id="25891-p102">The `POST /onenote/pages` operation is used only to create pages in the current user's default notebook. If you're targeting other notebooks, you can [create pages in a specified section](../api/section-post-pages.md).</span></span>           
## <a name="permissions"></a><span data-ttu-id="25891-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="25891-109">Permissions</span></span>
<span data-ttu-id="25891-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25891-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25891-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="25891-112">Permission type</span></span>      | <span data-ttu-id="25891-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="25891-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="25891-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="25891-114">Delegated (work or school account)</span></span> | <span data-ttu-id="25891-115">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25891-115">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="25891-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="25891-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25891-117">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="25891-117">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="25891-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="25891-118">Application</span></span> | <span data-ttu-id="25891-119">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25891-119">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="25891-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="25891-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
POST /me/onenote/pages
POST /users/{id | userPrincipalName}/onenote/pages
POST /groups/{id}/onenote/pages
POST /sites/{id}/onenote/pages
```

## <a name="request-headers"></a><span data-ttu-id="25891-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="25891-121">Request headers</span></span>  
| <span data-ttu-id="25891-122">Имя</span><span class="sxs-lookup"><span data-stu-id="25891-122">Name</span></span>       | <span data-ttu-id="25891-123">Тип</span><span class="sxs-lookup"><span data-stu-id="25891-123">Type</span></span> | <span data-ttu-id="25891-124">Описание</span><span class="sxs-lookup"><span data-stu-id="25891-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="25891-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="25891-125">Authorization</span></span>  | <span data-ttu-id="25891-126">string</span><span class="sxs-lookup"><span data-stu-id="25891-126">string</span></span>  | <span data-ttu-id="25891-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="25891-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="25891-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="25891-129">Content-Type</span></span> | <span data-ttu-id="25891-130">строка</span><span class="sxs-lookup"><span data-stu-id="25891-130">string</span></span> | <span data-ttu-id="25891-p105">`text/html` или `application/xhtml+xml` для содержимого HTML, в том числе для необходимой части Presentation составных запросов. В составных запросах используется тип содержимого `multipart/form-data; boundary=your-boundary`.</span><span class="sxs-lookup"><span data-stu-id="25891-p105">`text/html` or `application/xhtml+xml` for the HTML content, including for the required "Presentation" part of multipart requests. Multipart requests use the `multipart/form-data; boundary=your-boundary` content type.</span></span> |

## <a name="request-body"></a><span data-ttu-id="25891-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="25891-133">Request body</span></span>
<span data-ttu-id="25891-134">В теле запроса укажите содержимое HTML для страницы.</span><span class="sxs-lookup"><span data-stu-id="25891-134">In the request body, supply the HTML content for the page.</span></span>

<span data-ttu-id="25891-p106">Тело может содержать HTML-код, размещенный непосредственно в теле запроса, либо формат составного сообщения, как показано в примере. Если вы отправляете двоичные данные, необходимо отправить составной запрос.</span><span class="sxs-lookup"><span data-stu-id="25891-p106">The body can contain HTML placed directly in the request body, or it can contain a multipart message format as shown in the example. If you're sending binary data, then you must send a multipart request.</span></span>

## <a name="response"></a><span data-ttu-id="25891-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="25891-137">Response</span></span>

<span data-ttu-id="25891-138">При успешном выполнении этот метод возвращает код отклика `201 Created` и новый объект [page](../resources/page.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="25891-138">If successful, this method returns a `201 Created` response code and the new [page](../resources/page.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25891-139">Пример</span><span class="sxs-lookup"><span data-stu-id="25891-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="25891-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="25891-140">Request</span></span>
<span data-ttu-id="25891-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="25891-141">Here is an example of the request.</span></span>

<span data-ttu-id="25891-p107">В случае пути `../onenote/pages`, чтобы создать страницу в определенном разделе записной книжки, используемой по умолчанию, примените параметр запроса `sectionName`. Пример: `../onenote/pages?sectionName=My%20section`. Если раздел не существует (либо был переименован), API создаст другой раздел.</span><span class="sxs-lookup"><span data-stu-id="25891-p107">In the `../onenote/pages` path, you can use the `sectionName` query parameter to create a page in a specific section in the default notebook. Example: `../onenote/pages?sectionName=My%20section`. If the section doesn't exist (or was renamed), the API will create a new section.</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/pages
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
    <img src="https://..." alt="an image on the page" width="500" />
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
##### <a name="response"></a><span data-ttu-id="25891-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="25891-145">Response</span></span>
<span data-ttu-id="25891-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="25891-146">Here is an example of the response.</span></span> <span data-ttu-id="25891-147">Примечание: Для краткости усекается объект ответа, показано ниже.</span><span class="sxs-lookup"><span data-stu-id="25891-147">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="25891-148">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="25891-148">All of the properties will be returned from an actual call.</span></span>
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
  "description": "Create Page",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->