---
title: Создание страницы
description: Создание объекта page в указанном разделе.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 3617022652bd1e5fc0df0ed3497fb4b5f2e4f576
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915489"
---
# <a name="create-page"></a><span data-ttu-id="ee52b-103">Создание страницы</span><span class="sxs-lookup"><span data-stu-id="ee52b-103">Create page</span></span>

<span data-ttu-id="ee52b-104">Создание объекта [page](../resources/page.md) в указанном разделе.</span><span class="sxs-lookup"><span data-stu-id="ee52b-104">Create a new [page](../resources/page.md) in the specified section.</span></span>

## <a name="permissions"></a><span data-ttu-id="ee52b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ee52b-105">Permissions</span></span>
<span data-ttu-id="ee52b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee52b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee52b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ee52b-108">Permission type</span></span>      | <span data-ttu-id="ee52b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ee52b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ee52b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ee52b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ee52b-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee52b-111">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="ee52b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ee52b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee52b-113">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ee52b-113">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="ee52b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ee52b-114">Application</span></span> | <span data-ttu-id="ee52b-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee52b-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ee52b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ee52b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onenote/sections/{id}/pages
POST /users/{id | userPrincipalName}/onenote/sections/{id}/pages
POST /groups/{id}/onenote/sections/{id}/pages
POST /sites/{id}/onenote/sections/{id}/pages
```
## <a name="request-headers"></a><span data-ttu-id="ee52b-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ee52b-117">Request headers</span></span>
| <span data-ttu-id="ee52b-118">Имя</span><span class="sxs-lookup"><span data-stu-id="ee52b-118">Name</span></span>       | <span data-ttu-id="ee52b-119">Тип</span><span class="sxs-lookup"><span data-stu-id="ee52b-119">Type</span></span> | <span data-ttu-id="ee52b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ee52b-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ee52b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee52b-121">Authorization</span></span>  | <span data-ttu-id="ee52b-122">строка</span><span class="sxs-lookup"><span data-stu-id="ee52b-122">string</span></span>  | <span data-ttu-id="ee52b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ee52b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ee52b-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ee52b-125">Content-Type</span></span> | <span data-ttu-id="ee52b-126">строка</span><span class="sxs-lookup"><span data-stu-id="ee52b-126">string</span></span> | <span data-ttu-id="ee52b-p103">`text/html` или `application/xhtml+xml` для содержимого HTML, в том числе для необходимой части Presentation составных запросов. В составных запросах используется тип содержимого `multipart/form-data; boundary=your-boundary`.</span><span class="sxs-lookup"><span data-stu-id="ee52b-p103">`text/html` or `application/xhtml+xml` for the HTML content, including for the required "Presentation" part of multipart requests. Multipart requests use the `multipart/form-data; boundary=your-boundary` content type.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ee52b-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ee52b-129">Request body</span></span>
<span data-ttu-id="ee52b-130">В тексте запроса укажите HTML-содержимое страницы.</span><span class="sxs-lookup"><span data-stu-id="ee52b-130">In the request body, supply the page HTML content.</span></span>

<span data-ttu-id="ee52b-p104">Текст может содержать HTML-код, размещенный прямо в тексте запроса, либо формат составного сообщения, как показано в примере. Если вы отправляете двоичные данные, необходимо отправить составной запрос.</span><span class="sxs-lookup"><span data-stu-id="ee52b-p104">The body can contain HTML placed directly in the request body, or it can contain a multipart message format as shown in the example. If you're sending binary data, then you must send a multipart request.</span></span>

## <a name="response"></a><span data-ttu-id="ee52b-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee52b-133">Response</span></span>

<span data-ttu-id="ee52b-134">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и новый объект [page](../resources/page.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ee52b-134">If successful, this method returns `201 Created` response code and the new [page](../resources/page.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee52b-135">Пример</span><span class="sxs-lookup"><span data-stu-id="ee52b-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ee52b-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="ee52b-136">Request</span></span>
<span data-ttu-id="ee52b-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ee52b-137">Here is an example of the request.</span></span>

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
##### <a name="response"></a><span data-ttu-id="ee52b-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="ee52b-138">Response</span></span>
<span data-ttu-id="ee52b-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ee52b-139">Here is an example of the response.</span></span> <span data-ttu-id="ee52b-140">Примечание: Для краткости усекается объект ответа, показано ниже.</span><span class="sxs-lookup"><span data-stu-id="ee52b-140">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="ee52b-141">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ee52b-141">All of the properties will be returned from an actual call.</span></span>
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
