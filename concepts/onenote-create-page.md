---
title: Создание страниц OneNote
description: " Корпоративная записная книжка в Microsoft 365"
author: jewan-microsoft
localization_priority: Priority
ms.prod: onenote
ms.openlocfilehash: 815c42257449dde122958cc4ab3f9293387c0cb3
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472792"
---
# <a name="create-onenote-pages"></a><span data-ttu-id="e3824-103">Создание страниц OneNote</span><span class="sxs-lookup"><span data-stu-id="e3824-103">Create OneNote pages</span></span>

<span data-ttu-id="e3824-104">**Область применения:** Пользовательские записные книжки в OneDrive | Корпоративные записные книжки в Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="e3824-104">**Applies to**: Consumer notebooks on OneDrive | Enterprise notebooks on Microsoft 365</span></span>

<span data-ttu-id="e3824-105">Чтобы создать страницу OneNote, отправьте запрос POST в конечную точку *pages*.</span><span class="sxs-lookup"><span data-stu-id="e3824-105">To create a OneNote page, you send a POST request to a *pages* endpoint.</span></span> <span data-ttu-id="e3824-106">Пример:</span><span class="sxs-lookup"><span data-stu-id="e3824-106">For example:</span></span>

`POST ../notes/sections/{id}/pages`

<br/>

<span data-ttu-id="e3824-107">Отправьте в тексте сообщения HTML-код, определяющий страницу.</span><span class="sxs-lookup"><span data-stu-id="e3824-107">Send the HTML that defines the page in the message body.</span></span> <span data-ttu-id="e3824-108">Если запрос выполнен успешно, Microsoft Graph возвращает код состояния HTTP 201.</span><span class="sxs-lookup"><span data-stu-id="e3824-108">If the request is successful, Microsoft Graph returns a 201 HTTP status code.</span></span>


> <span data-ttu-id="e3824-109">**Примечание.** Сведения о запросах POST, которые вы можете отправлять для создания разделов, групп разделов и записных книжек, см. в [интерактивном справочнике по REST](https://dev.onenote.com/docs).</span><span class="sxs-lookup"><span data-stu-id="e3824-109">**Note:** To learn about the POST requests you can send to create sections, section groups, and notebooks, see our [interactive REST reference](https://dev.onenote.com/docs).</span></span>


<a name="request-uri"></a>

## <a name="construct-the-request-uri"></a><span data-ttu-id="e3824-110">Создание URI запроса</span><span class="sxs-lookup"><span data-stu-id="e3824-110">Construct the request URI</span></span>

<span data-ttu-id="e3824-111">Чтобы создать URI запроса POST, начните с корневого URL-адреса службы:</span><span class="sxs-lookup"><span data-stu-id="e3824-111">To construct the POST request URI, start with the service root URL:</span></span>

`https://graph.microsoft.com/v1.0/me/onenote`

<br/>

<span data-ttu-id="e3824-112">Затем добавьте конечную точку *pages*:</span><span class="sxs-lookup"><span data-stu-id="e3824-112">Then append the *pages* endpoint:</span></span>

- <span data-ttu-id="e3824-113">**Создание страницы в любом разделе (по его названию)**</span><span class="sxs-lookup"><span data-stu-id="e3824-113">**Create a page in any section (specified by section name)**</span></span><br/><br/>`.../pages?sectionName=DefaultSection`

- <span data-ttu-id="e3824-114">**Создание страницы в любом разделе (по его идентификатору)**</span><span class="sxs-lookup"><span data-stu-id="e3824-114">**Create a page in any section (specified by ID)**</span></span><br/><br/>`.../sections/{section-id}/pages` 

<span data-ttu-id="e3824-115">При создании страниц в личной записной книжке пользователя Microsoft Graph также предоставляет конечные точки, с помощью которых можно создавать страницы в записной книжке по умолчанию:</span><span class="sxs-lookup"><span data-stu-id="e3824-115">If you're creating pages in the user's personal notebook, Microsoft Graph also provides endpoints you can use to create pages in the default notebook:</span></span>

- <span data-ttu-id="e3824-116">**Создание страницы в стандартном разделе стандартной записной книжки**</span><span class="sxs-lookup"><span data-stu-id="e3824-116">**Create a page in the default section of the default notebook**</span></span><br/><br/>`../pages` 



<span data-ttu-id="e3824-117">Полный URI запроса будет выглядеть так, как в одном из следующих примеров:</span><span class="sxs-lookup"><span data-stu-id="e3824-117">Your full request URI will look like one of these examples:</span></span>

- `https://graph.microsoft.com/v1.0/me/onenote/sections/{id}/pages`
- `https://graph.microsoft.com/v1.0/me/onenote/pages?sectionName=Homework`

<span data-ttu-id="e3824-118">См. дополнительные сведения о [корневом URL-адресе службы](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0#root-url).</span><span class="sxs-lookup"><span data-stu-id="e3824-118">Learn more about the [service root URL](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0#root-url).</span></span>

<a name="post-pages-section-name"></a>

### <a name="using-the-sectionname-url-parameter"></a><span data-ttu-id="e3824-119">Использование параметра *sectionName* URL-адреса</span><span class="sxs-lookup"><span data-stu-id="e3824-119">Using the *sectionName* URL parameter</span></span>

<span data-ttu-id="e3824-120">При создании страницы в именованном разделе записной книжки по умолчанию с помощью параметра *sectionName* действуют следующие правила:</span><span class="sxs-lookup"><span data-stu-id="e3824-120">The following rules apply when using the *sectionName* parameter to create a page in a named section in the default notebook:</span></span>

- <span data-ttu-id="e3824-121">Можно ссылаться только на разделы верхнего уровня (не внутри групп разделов).</span><span class="sxs-lookup"><span data-stu-id="e3824-121">Only top-level sections can be referenced (not sections within section groups).</span></span>

- <span data-ttu-id="e3824-122">Если в стандартной записной книжке нет раздела с указанным названием, API создает его.</span><span class="sxs-lookup"><span data-stu-id="e3824-122">If a section with the specified name doesn't exist in the default notebook, the API creates it.</span></span> <span data-ttu-id="e3824-123">В названиях разделов не допускаются следующие символы: `? * \ / : < > | & # " % ~`</span><span class="sxs-lookup"><span data-stu-id="e3824-123">These characters are not allowed for section names: `? * \ / : < > | & # " % ~`</span></span>

- <span data-ttu-id="e3824-124">При сопоставлении названий разделов регистр не учитывается, но он сохраняется при их создании.</span><span class="sxs-lookup"><span data-stu-id="e3824-124">Section names are case-insensitive for matching, but case is preserved when sections are created.</span></span> <span data-ttu-id="e3824-125">Например, если указать название "Мой новый раздел", то оно будет отображаться и дальше, но в последующих запросах можно использовать имя "мой новый раздел".</span><span class="sxs-lookup"><span data-stu-id="e3824-125">So "My New Section" will display like that, but "my new section" would also match on subsequent posts.</span></span>

- <span data-ttu-id="e3824-126">В названиях разделов следует использовать кодировку URL.</span><span class="sxs-lookup"><span data-stu-id="e3824-126">Section names must be URL-encoded.</span></span> <span data-ttu-id="e3824-127">Например, пробелы следует кодировать как *%20*.</span><span class="sxs-lookup"><span data-stu-id="e3824-127">For example, spaces must be encoded as *%20*.</span></span>

- <span data-ttu-id="e3824-128">Параметр *sectionName* действителен только с маршрутом `../notes/pages` (не `../notes/sections/{id}/pages`).</span><span class="sxs-lookup"><span data-stu-id="e3824-128">The *sectionName* parameter is valid only with the `../notes/pages` route (not `../notes/sections/{id}/pages`).</span></span>

<span data-ttu-id="e3824-129">Разделы создаются только в случае их отсутствия, поэтому этот вызов можно использовать для каждой страницы, создаваемой приложением.</span><span class="sxs-lookup"><span data-stu-id="e3824-129">Because sections are created if they don't exist, it's safe to use this call with every page your app creates.</span></span> <span data-ttu-id="e3824-130">Пользователи могут переименовывать разделы, но при этом API создаст новый раздел с указанным вами названием.</span><span class="sxs-lookup"><span data-stu-id="e3824-130">Users might rename sections, but the API will create a new section with the section name that you supply.</span></span> 

> <span data-ttu-id="e3824-131">**Примечание.** Возвращаемые интерфейсом API ссылки на страницы в переименованном разделе по-прежнему будут указывать на старые страницы.</span><span class="sxs-lookup"><span data-stu-id="e3824-131">**Note:** The links returned by the API for pages in a renamed section will still reach those older pages.</span></span> 


<a name="message-body"></a>

## <a name="construct-the-message-body"></a><span data-ttu-id="e3824-132">Составление текста сообщения</span><span class="sxs-lookup"><span data-stu-id="e3824-132">Construct the message body</span></span>

<span data-ttu-id="e3824-133">HTML-код, определяющий содержимое страницы, называют *входным HTML-кодом*.</span><span class="sxs-lookup"><span data-stu-id="e3824-133">The HTML that defines page content is called *input HTML*.</span></span> <span data-ttu-id="e3824-134">Входной HTML-код поддерживает [часть стандартных атрибутов HTML и CSS](#supported-html-and-css-for-onenote-pages), а также настраиваемые атрибуты.</span><span class="sxs-lookup"><span data-stu-id="e3824-134">Input HTML supports a [subset of standard HTML and CSS](#supported-html-and-css-for-onenote-pages), with the addition of custom attributes.</span></span> <span data-ttu-id="e3824-135">(Настраиваемые атрибуты, например **data-id** и **data-render-src**, описываются в статье [Входной и выходной HTML-код](onenote-input-output-html.md).)</span><span class="sxs-lookup"><span data-stu-id="e3824-135">(Custom attributes, like **data-id** and **data-render-src**, are described in [Input and output HTML](onenote-input-output-html.md).)</span></span> 

<span data-ttu-id="e3824-136">Отправьте входной HTML-код в тексте сообщения запроса POST.</span><span class="sxs-lookup"><span data-stu-id="e3824-136">Send the input HTML in the message body of the POST request.</span></span> <span data-ttu-id="e3824-137">Вы можете отправить HTML-код прямо в тексте сообщения, используя тип контента `application/xhtml+xml` или `text/html`, или в части Presentation составного запроса.</span><span class="sxs-lookup"><span data-stu-id="e3824-137">You can send the input HTML directly in the message body using the  `application/xhtml+xml` or `text/html` content type, or you can send it in the "Presentation" part of a multipart request.</span></span> 

<span data-ttu-id="e3824-138">В приведенном ниже примере входной HTML-код отправляется прямо в тексте сообщения.</span><span class="sxs-lookup"><span data-stu-id="e3824-138">The following example sends the input HTML directly in the message body.</span></span>

```html
POST https://graph.microsoft.com/v1.0/me/onenote/pages
Authorization: Bearer {token}
Content-Type: application/xhtml+xml

<!DOCTYPE html>
<html>
  <head>
    <title>A page with a block of HTML</title>
    <meta name="created" content="2015-07-22T09:00:00-08:00" />
  </head>
  <body>
    <p>This page contains some <i>formatted</i> <b>text</b> and an image.</p>
    <img src="https://..." alt="an image on the page" width="500" />
  </body>
</html>
```

<br/>

<span data-ttu-id="e3824-139">Если вы отправляете двоичные данные, необходимо использовать [составной запрос](#example-request).</span><span class="sxs-lookup"><span data-stu-id="e3824-139">If you're sending binary data, you must use a [multipart request](#example-request).</span></span> 

> <span data-ttu-id="e3824-140">**Примечание.** Чтобы упростить программирование и обеспечение согласованности в приложении, вы можете использовать составные запросы для создания всех страниц.</span><span class="sxs-lookup"><span data-stu-id="e3824-140">**Note:** To simplify programming and consistency in your app, you can use multipart requests to create all pages.</span></span> <span data-ttu-id="e3824-141">Рекомендуем использовать библиотеку для создания составных сообщений.</span><span class="sxs-lookup"><span data-stu-id="e3824-141">It's a good idea to use a library to construct multipart messages.</span></span> <span data-ttu-id="e3824-142">Это снижает риск создания полезных данных в неправильном формате.</span><span class="sxs-lookup"><span data-stu-id="e3824-142">This reduces the risk of creating malformed payloads.</span></span>


<a name="input-html-rules"></a>

### <a name="requirements-and-limitations-for-input-html-in-post-pages-requests"></a><span data-ttu-id="e3824-143">Требования и ограничения для входного HTML-кода в запросах POST для страниц</span><span class="sxs-lookup"><span data-stu-id="e3824-143">Requirements and limitations for input HTML in POST pages requests</span></span>

<span data-ttu-id="e3824-144">Отправляя входной HTML-код, учитывайте следующие требования и ограничения:</span><span class="sxs-lookup"><span data-stu-id="e3824-144">When sending input HTML, be aware of these general requirements and limitations:</span></span>  

- <span data-ttu-id="e3824-145">Входной HTML-код должен быть правильно оформленным XHTML-кодом с кодировкой UTF-8.</span><span class="sxs-lookup"><span data-stu-id="e3824-145">Input HTML should be UTF-8 encoded and well-formed XHTML.</span></span> <span data-ttu-id="e3824-146">Всем открывающим тегам контейнеров должны соответствовать закрывающие теги.</span><span class="sxs-lookup"><span data-stu-id="e3824-146">All container start tags require matching closing tags.</span></span> <span data-ttu-id="e3824-147">Все значения атрибутов должны быть заключены в двойные или одинарные кавычки.</span><span class="sxs-lookup"><span data-stu-id="e3824-147">All attribute values must be surrounded by double- or single-quote marks.</span></span>  <!--docs say MUST be encoded-->

- <span data-ttu-id="e3824-148">Код JavaScript, вложенные файлы и CSS удаляются.</span><span class="sxs-lookup"><span data-stu-id="e3824-148">JavaScript code, included files, and CSS are removed.</span></span> 

- <span data-ttu-id="e3824-149">HTML-формы полностью удаляются.</span><span class="sxs-lookup"><span data-stu-id="e3824-149">HTML forms are removed in their entirety.</span></span>  

- <span data-ttu-id="e3824-150">Microsoft Graph поддерживает [подмножество элементов HTML](#supported-html-and-css-for-onenote-pages).</span><span class="sxs-lookup"><span data-stu-id="e3824-150">Microsoft Graph supports a [subset of HTML elements](#supported-html-and-css-for-onenote-pages).</span></span> 

- <span data-ttu-id="e3824-151">Microsoft Graph поддерживает отдельные стандартные атрибуты HTML и ряд настраиваемых атрибутов, таких как атрибут **data-id**, используемый для обновления страниц.</span><span class="sxs-lookup"><span data-stu-id="e3824-151">Microsoft Graph supports a subset of common HTML attributes and a set of custom attributes, such as the **data-id** attribute used for updating pages.</span></span> <span data-ttu-id="e3824-152">Поддерживаемые атрибуты описываются в статье [Входной и выходной HTML-код](onenote-input-output-html.md).</span><span class="sxs-lookup"><span data-stu-id="e3824-152">For supported attributes, see [Input and output HTML](onenote-input-output-html.md).</span></span>


<a name="supported-html"></a>

### <a name="supported-html-and-css-for-onenote-pages"></a><span data-ttu-id="e3824-153">Поддерживаемые атрибуты HTML и CSS для страниц OneNote</span><span class="sxs-lookup"><span data-stu-id="e3824-153">Supported HTML and CSS for OneNote pages</span></span>

<span data-ttu-id="e3824-154">Поддерживаются не все элементы, атрибуты и свойства (в HTML4, XHTML, CSS, HTML5 и т. д).</span><span class="sxs-lookup"><span data-stu-id="e3824-154">Not all elements, attributes, and properties are supported (in HTML4, XHTML, CSS, HTML5, etc.).</span></span> <span data-ttu-id="e3824-155">Microsoft Graph принимает ограниченный набор элементов HTML, более соответствующий особенностям работы с OneNote.</span><span class="sxs-lookup"><span data-stu-id="e3824-155">Instead, Microsoft Graph accepts a limited set of HTML that better fits how people use OneNote.</span></span> <span data-ttu-id="e3824-156">Дополнительные сведения см. на странице [Поддержка HTML-тегов для страниц](https://dev.onenote.com/docs#/introduction/html-tag-support-for-pages).</span><span class="sxs-lookup"><span data-stu-id="e3824-156">For more information, see [HTML tag support for pages](https://dev.onenote.com/docs#/introduction/html-tag-support-for-pages).</span></span> <span data-ttu-id="e3824-157">Если тег не указан на этой странице, скорее всего, он будет игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="e3824-157">If a tag's not listed there, it'll probably be ignored.</span></span>

<!--Microsoft Graph only accepts UTF-8 data. Be sure that all requests are encoded that way, and your content-type headers indicate that as well. xx our examples don't show this-->

<span data-ttu-id="e3824-158">Ниже перечислены базовые типы элементов, которые поддерживает Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="e3824-158">The following list shows the basic element types that Microsoft Graph supports:</span></span>

- <span data-ttu-id="e3824-159">`<head>` и `<body>`</span><span class="sxs-lookup"><span data-stu-id="e3824-159">`<head>` and `<body>`</span></span></p>
- <span data-ttu-id="e3824-160">`<title>` и `<meta>`, которые задают заголовок и дату создания страницы</span><span class="sxs-lookup"><span data-stu-id="e3824-160">`<title>` and `<meta>` that set the page title and creation date</span></span></p>
- <span data-ttu-id="e3824-161">`<h1>` — `<h6>` для заголовков разделов</span><span class="sxs-lookup"><span data-stu-id="e3824-161">`<h1>` through `<h6>` for section headings</span></span></p>
- <span data-ttu-id="e3824-162">`<p>` для абзацев</span><span class="sxs-lookup"><span data-stu-id="e3824-162">`<p>` for paragraphs</span></span></p>
- <span data-ttu-id="e3824-163">`<ul>`, `<ol>` и `<li>` для списков и их элементов</span><span class="sxs-lookup"><span data-stu-id="e3824-163">`<ul>`, `<ol>`, and `<li>` for lists and list items</span></span></p>
- <span data-ttu-id="e3824-164">`<table>`, `<tr>` и `<td>`, включая вложенные таблицы</span><span class="sxs-lookup"><span data-stu-id="e3824-164">`<table>`, `<tr>` and `<td>`, including nested tables</span></span></p>
- <span data-ttu-id="e3824-165">`<pre>` для предварительно отформатированного текста (с сохранением пробелов и разрывов строк)</span><span class="sxs-lookup"><span data-stu-id="e3824-165">`<pre>` for preformatted text (preserves white space and line breaks)</span></span></p>
- <span data-ttu-id="e3824-166">`<b>` и `<i>` для полужирного текста и курсива</span><span class="sxs-lookup"><span data-stu-id="e3824-166">`<b>` and `<i>` for bold and italic character styles</span></span></p>

<span data-ttu-id="e3824-167">Microsoft Graph сохраняет семантическое содержимое и базовую структуру входного HTML-кода при создании страниц, но преобразует входной HTML-код для использования поддерживаемого набора элементов HTML и CSS.</span><span class="sxs-lookup"><span data-stu-id="e3824-167">Microsoft Graph preserves the semantic content and basic structure of the input HTML when it creates pages, but it converts the input HTML to use the supported set of HTML and CSS.</span></span> <span data-ttu-id="e3824-168">Функции, отсутствующие в OneNote, преобразовывать не во что, поэтому они могут не распознаваться в исходном HTML-коде.</span><span class="sxs-lookup"><span data-stu-id="e3824-168">Features that don't exist in OneNote have nothing to be translated to, so they might not be recognized in the source HTML.</span></span> 


<a name="example"></a>

## <a name="example-request"></a><span data-ttu-id="e3824-169">Пример запроса</span><span class="sxs-lookup"><span data-stu-id="e3824-169">Example request</span></span>

<span data-ttu-id="e3824-170">Этот пример составного запроса создает страницу, содержащую изображения и внедренный файл.</span><span class="sxs-lookup"><span data-stu-id="e3824-170">This example multipart request creates a page that contains images and an embedded file.</span></span> <span data-ttu-id="e3824-171">Обязательная часть **Presentation** содержит входной HTML-код, определяющий страницу.</span><span class="sxs-lookup"><span data-stu-id="e3824-171">The required **Presentation** part contains the input HTML that defines the page.</span></span> <span data-ttu-id="e3824-172">Часть **imageBlock1** содержит двоичные данные изображения, а **fileBlock1** — двоичные данные файла.</span><span class="sxs-lookup"><span data-stu-id="e3824-172">The **imageBlock1** part contains the binary image data, and **fileBlock1** contains the binary file data.</span></span> <span data-ttu-id="e3824-173">Части данных также могут содержать HTML-код. В этом случае Microsoft Graph [отображает HTML-код в виде изображения](onenote-images-files.md#add-an-image-using-binary-data) на странице OneNote.</span><span class="sxs-lookup"><span data-stu-id="e3824-173">Data parts can also contain HTML, in which case Microsoft Graph [renders the HTML as an image](onenote-images-files.md#add-an-image-using-binary-data) on the OneNote page.</span></span> 

```html
POST https://graph.microsoft.com/v1.0/me/onenote/pages
Authorization: Bearer {token}
Content-Type: multipart/form-data; boundary=MyPartBoundary198374

--MyPartBoundary198374
Content-Disposition:form-data; name="Presentation"
Content-Type:text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with rendered images and an attached file</title>
    <meta name="created" content="2015-07-22T09:00:00-08:00" />
  </head>
  <body>
    <p>Here's an image from an <i>online source</i>:</p>
    <img src="https://..." alt="an image on the page" width="500" />
    <p>Here's an image uploaded as <b>binary data</b>:</p>
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

<span data-ttu-id="e3824-174">Дополнительные примеры создания страниц, содержащих изображения и другие файлы, см. в статье [Добавление изображений и файлов](onenote-images-files.md), наших [руководствах](/previous-versions/office/office-365-api/how-to/onenote-tutorial) и [примерах](https://github.com/onenotedev).</span><span class="sxs-lookup"><span data-stu-id="e3824-174">For more examples that show how to create pages that contain images and other files, see [Add images and files](onenote-images-files.md), our [tutorials](/previous-versions/office/office-365-api/how-to/onenote-tutorial), and our [samples](https://github.com/onenotedev).</span></span> <span data-ttu-id="e3824-175">Кроме того, узнайте, как [создавать элементы с абсолютным положением](onenote-abs-pos.md), [использовать теги примечаний](onenote-note-tags.md), а также [извлекать данные](onenote-extract-data.md) из визитных карточек, рецептов из Интернета и описаний товаров.</span><span class="sxs-lookup"><span data-stu-id="e3824-175">Also, learn how to [create absolute positioned elements](onenote-abs-pos.md), [use note tags](onenote-note-tags.md), and [extract data](onenote-extract-data.md) for business card captures and online recipe and product listings.</span></span>

<span data-ttu-id="e3824-176">Microsoft Graph требует строгого соответствия некоторым форматам, таким как символы новой строки CRLF в тексте составного сообщения.</span><span class="sxs-lookup"><span data-stu-id="e3824-176">Microsoft Graph is strict about some formats, such as CRLF newlines in a multipart message body.</span></span> <span data-ttu-id="e3824-177">Чтобы снизить риск получения полезных данных в неправильном формате, для создания составных сообщений следует использовать библиотеку.</span><span class="sxs-lookup"><span data-stu-id="e3824-177">To reduce the risk of creating malformed payloads, you should use a library to construct multipart messages.</span></span> 

<span data-ttu-id="e3824-178">Если появится состояние 400 (неправильный формат полезных данных), проверьте форматирование символов новой строки и пробелов, а также наличие проблем с кодировкой.</span><span class="sxs-lookup"><span data-stu-id="e3824-178">If you do receive a 400 status for a malformed payload, check the formatting of newlines and whitespaces, and check for encoding issues.</span></span> <span data-ttu-id="e3824-179">Например, попробуйте использовать параметр `charset=utf-8` (пример: `Content-Type: text/html; charset=utf-8`).</span><span class="sxs-lookup"><span data-stu-id="e3824-179">For example, try using `charset=utf-8` (example: `Content-Type: text/html; charset=utf-8`).</span></span>

<span data-ttu-id="e3824-180">См. [требования и ограничения для входного HTML-кода](#requirements-and-limitations-for-input-html-in-post-pages-requests) и [ограничения размера запросов POST](onenote-images-files.md#size-limitations-for-post-pages-requests).</span><span class="sxs-lookup"><span data-stu-id="e3824-180">See [requirements and limitations for input HTML](#requirements-and-limitations-for-input-html-in-post-pages-requests) and [size limits for POST requests](onenote-images-files.md#size-limitations-for-post-pages-requests).</span></span>


<a name="request-response-info"></a>

## <a name="request-and-response-information-for-post-pages-requests"></a><span data-ttu-id="e3824-181">Информация о запросах *POST для страниц* и соответствующих ответах</span><span class="sxs-lookup"><span data-stu-id="e3824-181">Request and response information for *POST pages* requests</span></span>

| <span data-ttu-id="e3824-182">Данные запроса</span><span class="sxs-lookup"><span data-stu-id="e3824-182">Request data</span></span> | <span data-ttu-id="e3824-183">Описание</span><span class="sxs-lookup"><span data-stu-id="e3824-183">Description</span></span> |  
|------|------|  
| <span data-ttu-id="e3824-184">Протокол</span><span class="sxs-lookup"><span data-stu-id="e3824-184">Protocol</span></span> | <span data-ttu-id="e3824-185">Все запросы используют протокол SSL/TLS для HTTPS.</span><span class="sxs-lookup"><span data-stu-id="e3824-185">All requests use the SSL/TLS HTTPS protocol.</span></span> |  
| <span data-ttu-id="e3824-186">Заголовок Authorization</span><span class="sxs-lookup"><span data-stu-id="e3824-186">Authorization header</span></span> | <p><span data-ttu-id="e3824-187">`Bearer {token}`, где `{token}` — действительный маркер доступа OAuth 2.0 для зарегистрированного приложения.</span><span class="sxs-lookup"><span data-stu-id="e3824-187">`Bearer {token}`, where `{token}` is a valid OAuth 2.0 access token for your registered app.</span></span></p><p><span data-ttu-id="e3824-188">Если он отсутствует или является недействительным, запрос завершится ошибкой с кодом состояния 401.</span><span class="sxs-lookup"><span data-stu-id="e3824-188">If missing or invalid, the request fails with a 401 status code.</span></span> <span data-ttu-id="e3824-189">См. статью [Проверка подлинности и разрешения](permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e3824-189">See [Authentication and permissions](permissions-reference.md).</span></span></p> |  
| <span data-ttu-id="e3824-190">Заголовок Content-Type</span><span class="sxs-lookup"><span data-stu-id="e3824-190">Content-Type header</span></span> | <p><span data-ttu-id="e3824-191">`text/html` или `application/xhtml+xml` для HTML-содержимого, отправляемого либо непосредственно в тексте сообщения, либо в обязательной части Presentation составных запросов.</span><span class="sxs-lookup"><span data-stu-id="e3824-191">`text/html` or `application/xhtml+xml` for the HTML content, whether it's sent directly in the message body or in the required "Presentation" part of multipart requests.</span></span></p><p><span data-ttu-id="e3824-192">Составные запросы необходимы при отправке двоичных данных и используют тип контента `multipart/form-data; boundary=part-boundary`, где `{part-boundary}` — это строка, обозначающая начало и конец каждой части данных.</span><span class="sxs-lookup"><span data-stu-id="e3824-192">Multipart requests are required when sending binary data, and use the `multipart/form-data; boundary=part-boundary` content type, where `{part-boundary}` is a string that signals the start and end of each data part.</span></span></p> |  
| <span data-ttu-id="e3824-193">Заголовок Accept</span><span class="sxs-lookup"><span data-stu-id="e3824-193">Accept header</span></span> | `application/json` | 

<br/>

| <span data-ttu-id="e3824-194">Данные ответа</span><span class="sxs-lookup"><span data-stu-id="e3824-194">Response data</span></span> | <span data-ttu-id="e3824-195">Описание</span><span class="sxs-lookup"><span data-stu-id="e3824-195">Description</span></span> |  
|------|------|  
| <span data-ttu-id="e3824-196">Код успешного завершения</span><span class="sxs-lookup"><span data-stu-id="e3824-196">Success code</span></span> | <span data-ttu-id="e3824-197">Код состояния HTTP 201</span><span class="sxs-lookup"><span data-stu-id="e3824-197">A 201 HTTP status code.</span></span> |  
| <span data-ttu-id="e3824-198">Текст ответа</span><span class="sxs-lookup"><span data-stu-id="e3824-198">Response body</span></span> | <span data-ttu-id="e3824-199">Представление OData новой страницы в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e3824-199">A OData representation of the new page in JSON format.</span></span> |  
| <span data-ttu-id="e3824-200">Ошибки</span><span class="sxs-lookup"><span data-stu-id="e3824-200">Errors</span></span> | <span data-ttu-id="e3824-201">Если запрос завершается сбоем, API возвращает ошибки в объекте **\@api.diagnostics** в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e3824-201">If the request fails, the API returns errors in the **\@api.diagnostics** object in the response body.</span></span> |  
| <span data-ttu-id="e3824-202">Заголовок Location</span><span class="sxs-lookup"><span data-stu-id="e3824-202">Location header</span></span> | <span data-ttu-id="e3824-203">URL-адрес ресурса новой страницы.</span><span class="sxs-lookup"><span data-stu-id="e3824-203">The resource URL for the new page.</span></span> |  
| <span data-ttu-id="e3824-204">Заголовок X-CorrelationId</span><span class="sxs-lookup"><span data-stu-id="e3824-204">X-CorrelationId header</span></span> | <span data-ttu-id="e3824-205">GUID, уникальный идентификатор запроса.</span><span class="sxs-lookup"><span data-stu-id="e3824-205">A GUID that uniquely identifies the request.</span></span> <span data-ttu-id="e3824-206">Это значение можно использовать вместе со значением заголовка Date при устранении неполадок совместно со службой поддержки Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="e3824-206">You can use this value along with the value of the Date header when working with Microsoft support to troubleshoot issues.</span></span> |  


<a name="root-url"></a>

### <a name="constructing-the-microsoft-graph-service-root-url"></a><span data-ttu-id="e3824-207">Составление корневого URL-адреса службы Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="e3824-207">Constructing the Microsoft Graph service root URL</span></span>

<span data-ttu-id="e3824-208">В корневом URL-адресе службы Microsoft Graph используется следующий формат для всех вызовов Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="e3824-208">The Microsoft Graph service root URL uses the following format for all calls to Microsoft Graph:</span></span>

`https://graph.microsoft.com/{version}/me/onenote/`  

<span data-ttu-id="e3824-209">Сегмент `version` URL-адреса представляет нужную версию Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="e3824-209">The `version` segment in the URL represents the version of Microsoft Graph that you want to use.</span></span> <span data-ttu-id="e3824-210">Используйте значение `v1.0` для стабильного кода в рабочей среде.</span><span class="sxs-lookup"><span data-stu-id="e3824-210">Use `v1.0` for stable production code.</span></span> <span data-ttu-id="e3824-211">Используйте значение `beta`, чтобы опробовать функцию, находящуюся на стадии разработки.</span><span class="sxs-lookup"><span data-stu-id="e3824-211">Use `beta` to try out a feature that's in development.</span></span> <span data-ttu-id="e3824-212">Функции бета-версии могут меняться, поэтому не следует использовать их в производственном коде.</span><span class="sxs-lookup"><span data-stu-id="e3824-212">Features and functionality in beta may change, so you shouldn't use it in your production code.</span></span> 

<span data-ttu-id="e3824-213">Используйте значение `me` для содержимого OneNote, доступного текущему пользователю (если он является владельцем или с ним поделились этим содержимым).</span><span class="sxs-lookup"><span data-stu-id="e3824-213">Use `me` for OneNote content that the current user can access (owned and shared).</span></span> <span data-ttu-id="e3824-214">Используйте значение `users/{id}` для содержимого OneNote, которым указанный (в URL-адресе) пользователь поделился с текущим пользователем.</span><span class="sxs-lookup"><span data-stu-id="e3824-214">Use `users/{id}` for OneNote content that the specified user (in the URL) has shared with the current user.</span></span> <span data-ttu-id="e3824-215">Используйте [Microsoft Graph](https://graph.microsoft.com/v1.0/users) для получения идентификаторов пользователей.</span><span class="sxs-lookup"><span data-stu-id="e3824-215">Use [Microsoft Graph](https://graph.microsoft.com/v1.0/users) to get user IDs.</span></span> 

<a name="limitations"></a>

## <a name="onenote-section-size-limitations"></a><span data-ttu-id="e3824-216">Ограничения размера раздела OneNote</span><span class="sxs-lookup"><span data-stu-id="e3824-216">OneNote section size limitations</span></span>
<span data-ttu-id="e3824-217">Существует ограничение на количество страниц, которые можно добавить в раздел с помощью API OneNote.</span><span class="sxs-lookup"><span data-stu-id="e3824-217">There is a limit to the number of pages that you can add to a section using the OneNote API.</span></span> <span data-ttu-id="e3824-218">Когда этот предел достигнут для раздела и предпринята попытка создать новую страницу в этом разделе, вы увидите ответ с кодом состояния HTTP `507` и сообщением «Превышено максимально допустимое количество страниц в разделе».</span><span class="sxs-lookup"><span data-stu-id="e3824-218">When this limit is reached for a section and an attempt is made to create a new page in that section, you will see a response with HTTP status code `507` and message "Exceeded the maximum number of pages allowed per section".</span></span> <span data-ttu-id="e3824-219">Дополнительные сведения об этом коде ошибки см. В разделе [Коды ошибок OneNote](onenote-error-codes.md).</span><span class="sxs-lookup"><span data-stu-id="e3824-219">For more information about this error code, see [OneNote error codes](onenote-error-codes.md).</span></span>

<span data-ttu-id="e3824-220">Вы можете использовать один из следующих обходных путей:</span><span class="sxs-lookup"><span data-stu-id="e3824-220">You can use one of the following workarounds:</span></span>
- <span data-ttu-id="e3824-221">Создайте новый раздел и добавьте туда новые страницы.</span><span class="sxs-lookup"><span data-stu-id="e3824-221">Create a new section and add new pages there.</span></span>
- <span data-ttu-id="e3824-222">Удалите неиспользуемые страницы из существующего раздела, который достиг ограничения страницы.</span><span class="sxs-lookup"><span data-stu-id="e3824-222">Delete unused pages of an existing section that has reached the page limit.</span></span>

<a name="permissions"></a>

## <a name="permissions"></a><span data-ttu-id="e3824-223">Permissions</span><span class="sxs-lookup"><span data-stu-id="e3824-223">Permissions</span></span>

<span data-ttu-id="e3824-224">Для создания страниц OneNote необходимо запрашивать соответствующие разрешения.</span><span class="sxs-lookup"><span data-stu-id="e3824-224">To create OneNote pages, you'll need to request appropriate permissions.</span></span> <span data-ttu-id="e3824-225">Выберите минимальный уровень разрешений, необходимый для работы вашего приложения.</span><span class="sxs-lookup"><span data-stu-id="e3824-225">Choose the lowest level of permissions that your app needs to do its work.</span></span>

<span data-ttu-id="e3824-226">Варианты:</span><span class="sxs-lookup"><span data-stu-id="e3824-226">Choose from:</span></span>

- <span data-ttu-id="e3824-227">Notes.Create</span><span class="sxs-lookup"><span data-stu-id="e3824-227">Notes.Create</span></span>
- <span data-ttu-id="e3824-228">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e3824-228">Notes.ReadWrite</span></span>
- <span data-ttu-id="e3824-229">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3824-229">Notes.ReadWrite.All</span></span>

<span data-ttu-id="e3824-230">Дополнительные сведения об областях разрешений и принципе их использования см. в [справочнике по разрешениям Microsoft Graph](permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e3824-230">For more information about permission scopes and how they work, see [Microsoft Graph permissions reference](permissions-reference.md).</span></span>




<a name="see-also"></a>

## <a name="see-also"></a><span data-ttu-id="e3824-231">См. также</span><span class="sxs-lookup"><span data-stu-id="e3824-231">See also</span></span>

- [<span data-ttu-id="e3824-232">Добавление изображений и файлов</span><span class="sxs-lookup"><span data-stu-id="e3824-232">Add images and files</span></span>](onenote-images-files.md)
- [<span data-ttu-id="e3824-233">Создание элементов с абсолютным положением</span><span class="sxs-lookup"><span data-stu-id="e3824-233">Create absolute positioned elements</span></span>](onenote-abs-pos.md)  
- [<span data-ttu-id="e3824-234">Извлечение данных</span><span class="sxs-lookup"><span data-stu-id="e3824-234">Extract data</span></span>](onenote-extract-data.md)
- [<span data-ttu-id="e3824-235">Использование тегов заметок</span><span class="sxs-lookup"><span data-stu-id="e3824-235">Use note tags</span></span>](onenote-note-tags.md)
- [<span data-ttu-id="e3824-236">Интеграция с OneNote</span><span class="sxs-lookup"><span data-stu-id="e3824-236">Integrate with OneNote</span></span>](integrate-with-onenote.md)
- [<span data-ttu-id="e3824-237">Блог разработчиков OneNote</span><span class="sxs-lookup"><span data-stu-id="e3824-237">OneNote Developer Blog</span></span>](https://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="e3824-238">Вопросы разработки OneNote на сайте «Вопросы и ответы Майкрософт»</span><span class="sxs-lookup"><span data-stu-id="e3824-238">OneNote development questions on Microsoft Q&A</span></span>](https://docs.microsoft.com/answers/topics/microsoft-graph-notes.html)
- [<span data-ttu-id="e3824-239">Репозитории GitHub OneNote</span><span class="sxs-lookup"><span data-stu-id="e3824-239">OneNote GitHub repos</span></span>](https://go.microsoft.com/fwlink/?LinkID=390178)