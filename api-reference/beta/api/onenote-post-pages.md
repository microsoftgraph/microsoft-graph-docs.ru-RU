---
title: Создание страницы
description: Создайте новую страницу OneNote в разделе по умолчанию записной книжки по умолчанию.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 828fc09e3b7cdb281b682df93b3d6f94f264330d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48004643"
---
# <a name="create-page"></a><span data-ttu-id="b89fb-103">Создание страницы</span><span class="sxs-lookup"><span data-stu-id="b89fb-103">Create page</span></span>

<span data-ttu-id="b89fb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b89fb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b89fb-105">Создайте новую страницу OneNote в разделе по умолчанию записной книжки по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b89fb-105">Create a new OneNote page in the default section of the default notebook.</span></span>

<span data-ttu-id="b89fb-106">Чтобы создать страницу в другом разделе записной книжки, используемой по умолчанию, можно использовать `sectionName` параметр запроса.</span><span class="sxs-lookup"><span data-stu-id="b89fb-106">To create a page in a different section in the default notebook, you can use the `sectionName` query parameter.</span></span>  <span data-ttu-id="b89fb-107">Пример: `../onenote/pages?sectionName=My%20section`.</span><span class="sxs-lookup"><span data-stu-id="b89fb-107">Example: `../onenote/pages?sectionName=My%20section`</span></span>

<span data-ttu-id="b89fb-108">Эта `POST /onenote/pages` операция используется только для создания страниц в записной книжке текущего пользователя по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b89fb-108">The `POST /onenote/pages` operation is used only to create pages in the current user's default notebook.</span></span> <span data-ttu-id="b89fb-109">Если вы нацелены на другие записные книжки, вы можете [создавать страницы в указанном разделе](../api/section-post-pages.md).</span><span class="sxs-lookup"><span data-stu-id="b89fb-109">If you're targeting other notebooks, you can [create pages in a specified section](../api/section-post-pages.md).</span></span>      

> <span data-ttu-id="b89fb-110">**Примечание:** Существует предельное число страниц, которые можно добавить в раздел с помощью этого API.</span><span class="sxs-lookup"><span data-stu-id="b89fb-110">**Note:** There is a limit to the number of pages that can be added to a section using this API.</span></span> <span data-ttu-id="b89fb-111">Дополнительные сведения см. в статье [Создание страниц OneNote](/graph/onenote-create-page) для всех ограничений с помощью этого API.</span><span class="sxs-lookup"><span data-stu-id="b89fb-111">For details, see [Create OneNote pages](/graph/onenote-create-page) for all limitations with this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="b89fb-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b89fb-112">Permissions</span></span>
<span data-ttu-id="b89fb-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b89fb-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b89fb-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b89fb-115">Permission type</span></span>      | <span data-ttu-id="b89fb-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b89fb-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b89fb-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b89fb-117">Delegated (work or school account)</span></span> | <span data-ttu-id="b89fb-118">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b89fb-118">Notes.Create, Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="b89fb-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b89fb-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b89fb-120">Notes.Create, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b89fb-120">Notes.Create, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="b89fb-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b89fb-121">Application</span></span> | <span data-ttu-id="b89fb-122">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b89fb-122">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b89fb-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b89fb-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
POST /me/onenote/pages
POST /users/{id | userPrincipalName}/onenote/pages
POST /groups/{id}/onenote/pages
POST /sites/{id}/onenote/pages
```

## <a name="request-headers"></a><span data-ttu-id="b89fb-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b89fb-124">Request headers</span></span>  
| <span data-ttu-id="b89fb-125">Имя</span><span class="sxs-lookup"><span data-stu-id="b89fb-125">Name</span></span>       | <span data-ttu-id="b89fb-126">Тип</span><span class="sxs-lookup"><span data-stu-id="b89fb-126">Type</span></span> | <span data-ttu-id="b89fb-127">Описание</span><span class="sxs-lookup"><span data-stu-id="b89fb-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b89fb-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="b89fb-128">Authorization</span></span>  | <span data-ttu-id="b89fb-129">string</span><span class="sxs-lookup"><span data-stu-id="b89fb-129">string</span></span>  | <span data-ttu-id="b89fb-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b89fb-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b89fb-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b89fb-132">Content-Type</span></span> | <span data-ttu-id="b89fb-133">string</span><span class="sxs-lookup"><span data-stu-id="b89fb-133">string</span></span> | <span data-ttu-id="b89fb-p106">`text/html` или `application/xhtml+xml` для содержимого HTML, в том числе для необходимой части Presentation составных запросов. В составных запросах используется тип содержимого `multipart/form-data; boundary=your-boundary`.</span><span class="sxs-lookup"><span data-stu-id="b89fb-p106">`text/html` or `application/xhtml+xml` for the HTML content, including for the required "Presentation" part of multipart requests. Multipart requests use the `multipart/form-data; boundary=your-boundary` content type.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b89fb-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b89fb-136">Request body</span></span>
<span data-ttu-id="b89fb-137">В теле запроса добавьте HTML-контент для страницы.</span><span class="sxs-lookup"><span data-stu-id="b89fb-137">In the request body, supply the HTML content for the page.</span></span>

<span data-ttu-id="b89fb-p107">Текст может содержать HTML-код, размещенный прямо в тексте запроса, либо формат составного сообщения, как показано в примере. Если вы отправляете двоичные данные, необходимо отправить составной запрос.</span><span class="sxs-lookup"><span data-stu-id="b89fb-p107">The body can contain HTML placed directly in the request body, or it can contain a multipart message format as shown in the example. If you're sending binary data, then you must send a multipart request.</span></span>

## <a name="response"></a><span data-ttu-id="b89fb-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="b89fb-140">Response</span></span>

<span data-ttu-id="b89fb-141">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [оненотепаже](../resources/onenotepage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b89fb-141">If successful, this method returns a `201 Created` response code and the new [onenotepage](../resources/onenotepage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b89fb-142">Пример</span><span class="sxs-lookup"><span data-stu-id="b89fb-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b89fb-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="b89fb-143">Request</span></span>
<span data-ttu-id="b89fb-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b89fb-144">Here is an example of the request.</span></span>

<span data-ttu-id="b89fb-145">В `../onenote/pages` пути можно использовать `sectionName` параметр запроса, чтобы создать страницу в определенном разделе записной книжки по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b89fb-145">In the `../onenote/pages` path, you can use the `sectionName` query parameter to create a page in a specific section in the default notebook.</span></span> <span data-ttu-id="b89fb-146">Пример: `../onenote/pages?sectionName=My%20section`.</span><span class="sxs-lookup"><span data-stu-id="b89fb-146">Example: `../onenote/pages?sectionName=My%20section`.</span></span> <span data-ttu-id="b89fb-147">Если раздел не существует (или был переименован), API создаст новый раздел.</span><span class="sxs-lookup"><span data-stu-id="b89fb-147">If the section doesn't exist (or was renamed), the API will create a new section.</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/me/onenote/pages
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
##### <a name="response"></a><span data-ttu-id="b89fb-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="b89fb-148">Response</span></span>
<span data-ttu-id="b89fb-p109">Ниже приведен пример отклика. Примечание. Показанный здесь объект ответа усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b89fb-p109">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call. </span></span><!-- { "blockType": "ignored" } -->
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
<!--
{
  "type": "#page.annotation",
  "description": "Create Page",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


