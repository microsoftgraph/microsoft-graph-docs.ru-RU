---
title: Создание страницы
description: Создайте новую страницу OneNote в разделе по умолчанию записной книжки по умолчанию.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 58ec80676455c4804723771e5e71fbab30a9a2c1
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/20/2020
ms.locfileid: "42163418"
---
# <a name="create-page"></a><span data-ttu-id="226ff-103">Создание страницы</span><span class="sxs-lookup"><span data-stu-id="226ff-103">Create page</span></span>

<span data-ttu-id="226ff-104">Создайте новую страницу OneNote в разделе по умолчанию записной книжки по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="226ff-104">Create a new OneNote page in the default section of the default notebook.</span></span>

<span data-ttu-id="226ff-105">Чтобы создать страницу в другом разделе записной книжки, используемой по умолчанию, `sectionName` можно использовать параметр запроса.</span><span class="sxs-lookup"><span data-stu-id="226ff-105">To create a page in a different section in the default notebook, you can use the `sectionName` query parameter.</span></span>  <span data-ttu-id="226ff-106">Пример: `../onenote/pages?sectionName=My%20section`</span><span class="sxs-lookup"><span data-stu-id="226ff-106">Example: `../onenote/pages?sectionName=My%20section`</span></span>

<span data-ttu-id="226ff-107">Эта `POST /onenote/pages` операция используется только для создания страниц в записной книжке текущего пользователя по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="226ff-107">The `POST /onenote/pages` operation is used only to create pages in the current user's default notebook.</span></span> <span data-ttu-id="226ff-108">Если вы нацелены на другие записные книжки, вы можете [создавать страницы в указанном разделе](../api/section-post-pages.md).</span><span class="sxs-lookup"><span data-stu-id="226ff-108">If you're targeting other notebooks, you can [create pages in a specified section](../api/section-post-pages.md).</span></span>  

> <span data-ttu-id="226ff-109">**Примечание:** Существует предельное число страниц, которые можно добавить в раздел с помощью этого API.</span><span class="sxs-lookup"><span data-stu-id="226ff-109">**Note:** There is a limit to the number of pages that can be added to a section using this API.</span></span> <span data-ttu-id="226ff-110">Дополнительные сведения см. в статье [Создание страниц OneNote](/graph/onenote-create-page) для всех ограничений с помощью этого API.</span><span class="sxs-lookup"><span data-stu-id="226ff-110">For details, see [Create OneNote pages](/graph/onenote-create-page) for all limitations with this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="226ff-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="226ff-111">Permissions</span></span>
<span data-ttu-id="226ff-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="226ff-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="226ff-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="226ff-114">Permission type</span></span>      | <span data-ttu-id="226ff-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="226ff-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="226ff-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="226ff-116">Delegated (work or school account)</span></span> | <span data-ttu-id="226ff-117">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="226ff-117">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="226ff-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="226ff-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="226ff-119">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="226ff-119">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="226ff-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="226ff-120">Application</span></span> | <span data-ttu-id="226ff-121">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="226ff-121">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="226ff-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="226ff-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
POST /me/onenote/pages
POST /users/{id | userPrincipalName}/onenote/pages
POST /groups/{id}/onenote/pages
POST /sites/{id}/onenote/pages
```

## <a name="request-headers"></a><span data-ttu-id="226ff-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="226ff-123">Request headers</span></span>  
| <span data-ttu-id="226ff-124">Имя</span><span class="sxs-lookup"><span data-stu-id="226ff-124">Name</span></span>       | <span data-ttu-id="226ff-125">Тип</span><span class="sxs-lookup"><span data-stu-id="226ff-125">Type</span></span> | <span data-ttu-id="226ff-126">Описание</span><span class="sxs-lookup"><span data-stu-id="226ff-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="226ff-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="226ff-127">Authorization</span></span>  | <span data-ttu-id="226ff-128">string</span><span class="sxs-lookup"><span data-stu-id="226ff-128">string</span></span>  | <span data-ttu-id="226ff-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="226ff-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="226ff-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="226ff-131">Content-Type</span></span> | <span data-ttu-id="226ff-132">string</span><span class="sxs-lookup"><span data-stu-id="226ff-132">string</span></span> | <span data-ttu-id="226ff-p106">`text/html` или `application/xhtml+xml` для содержимого HTML, в том числе для необходимой части Presentation составных запросов. В составных запросах используется тип содержимого `multipart/form-data; boundary=your-boundary`.</span><span class="sxs-lookup"><span data-stu-id="226ff-p106">`text/html` or `application/xhtml+xml` for the HTML content, including for the required "Presentation" part of multipart requests. Multipart requests use the `multipart/form-data; boundary=your-boundary` content type.</span></span> |

## <a name="request-body"></a><span data-ttu-id="226ff-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="226ff-135">Request body</span></span>
<span data-ttu-id="226ff-136">В теле запроса добавьте HTML-контент для страницы.</span><span class="sxs-lookup"><span data-stu-id="226ff-136">In the request body, supply the HTML content for the page.</span></span>

<span data-ttu-id="226ff-p107">Текст может содержать HTML-код, размещенный прямо в тексте запроса, либо формат составного сообщения, как показано в примере. Если вы отправляете двоичные данные, необходимо отправить составной запрос.</span><span class="sxs-lookup"><span data-stu-id="226ff-p107">The body can contain HTML placed directly in the request body, or it can contain a multipart message format as shown in the example. If you're sending binary data, then you must send a multipart request.</span></span>

## <a name="response"></a><span data-ttu-id="226ff-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="226ff-139">Response</span></span>

<span data-ttu-id="226ff-140">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [Page](../resources/page.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="226ff-140">If successful, this method returns a `201 Created` response code and the new [page](../resources/page.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="226ff-141">Пример</span><span class="sxs-lookup"><span data-stu-id="226ff-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="226ff-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="226ff-142">Request</span></span>
<span data-ttu-id="226ff-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="226ff-143">Here is an example of the request.</span></span>

<span data-ttu-id="226ff-144">В `../onenote/pages` пути можно использовать параметр `sectionName` запроса, чтобы создать страницу в определенном разделе записной книжки по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="226ff-144">In the `../onenote/pages` path, you can use the `sectionName` query parameter to create a page in a specific section in the default notebook.</span></span> <span data-ttu-id="226ff-145">Пример: `../onenote/pages?sectionName=My%20section`.</span><span class="sxs-lookup"><span data-stu-id="226ff-145">Example: `../onenote/pages?sectionName=My%20section`.</span></span> <span data-ttu-id="226ff-146">Если раздел не существует (или был переименован), API создаст новый раздел.</span><span class="sxs-lookup"><span data-stu-id="226ff-146">If the section doesn't exist (or was renamed), the API will create a new section.</span></span>

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
##### <a name="response"></a><span data-ttu-id="226ff-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="226ff-147">Response</span></span>
<span data-ttu-id="226ff-p109">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="226ff-p109">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call. </span></span><!-- { "blockType": "ignored" } -->
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
