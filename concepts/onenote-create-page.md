# <a name="create-onenote-pages"></a><span data-ttu-id="24ade-101">Создание страниц OneNote</span><span class="sxs-lookup"><span data-stu-id="24ade-101">Create OneNote pages</span></span>

<span data-ttu-id="24ade-102">**Относится к:** обычные записные книжки в OneDrive | корпоративные записные книжки в Office 365</span><span class="sxs-lookup"><span data-stu-id="24ade-102">**Applies to**: Consumer notebooks on OneDrive | Enterprise notebooks on Office 365</span></span>

<span data-ttu-id="24ade-103">Чтобы создать страницу OneNote, отправьте запрос POST в конечную точку *pages*.</span><span class="sxs-lookup"><span data-stu-id="24ade-103">To create a OneNote page, you send a POST request to a *pages* endpoint.</span></span> <span data-ttu-id="24ade-104">Пример:</span><span class="sxs-lookup"><span data-stu-id="24ade-104">For example:</span></span>

`POST ../notes/sections/{id}/pages`

<br/>

<span data-ttu-id="24ade-105">Отправьте в тексте сообщения HTML-код, определяющий страницу.</span><span class="sxs-lookup"><span data-stu-id="24ade-105">Send the HTML that defines the page in the message body.</span></span> <span data-ttu-id="24ade-106">Если запрос выполнен успешно, Microsoft Graph возвращает код состояния HTTP 201.</span><span class="sxs-lookup"><span data-stu-id="24ade-106">If the request is successful, Microsoft Graph returns a 201 HTTP status code.</span></span>


> <span data-ttu-id="24ade-107">**Примечание.** Сведения о запросах POST, которые вы можете отправлять для создания разделов, групп разделов и записных книжек, см. в [интерактивном справочнике по REST](http://dev.onenote.com/docs).</span><span class="sxs-lookup"><span data-stu-id="24ade-107">**Note:** To learn about the POST requests you can send to create sections, section groups, and notebooks, see our [interactive REST reference](http://dev.onenote.com/docs).</span></span>


<a name="request-uri"></a>

## <a name="construct-the-request-uri"></a><span data-ttu-id="24ade-108">Создание URI запроса</span><span class="sxs-lookup"><span data-stu-id="24ade-108">Construct the request URI</span></span>

<span data-ttu-id="24ade-109">Чтобы создать URI запроса POST, начните с корневого URL-адреса службы:</span><span class="sxs-lookup"><span data-stu-id="24ade-109">To construct the POST request URI, start with the service root URL:</span></span>

`https://graph.microsoft.com/v1.0/me/onenote`

<br/>

<span data-ttu-id="24ade-110">Затем добавьте конечную точку *pages*:</span><span class="sxs-lookup"><span data-stu-id="24ade-110">Then append the *pages* endpoint:</span></span>

- <span data-ttu-id="24ade-111">**Создание страницы в любом разделе (по его названию)**</span><span class="sxs-lookup"><span data-stu-id="24ade-111">**Create a page in any section (specified by section name)**</span></span><br/><br/>`.../pages?sectionName=DefaultSection`

- <span data-ttu-id="24ade-112">**Создание страницы в любом разделе (по его идентификатору)**</span><span class="sxs-lookup"><span data-stu-id="24ade-112">**Create a page in any section (specified by ID)**</span></span><br/><br/>`.../sections/{section-id}/pages` 

<span data-ttu-id="24ade-113">При создании страниц в личной записной книжке пользователя Microsoft Graph также предоставляет конечные точки, с помощью которых можно создавать страницы в записной книжке по умолчанию:</span><span class="sxs-lookup"><span data-stu-id="24ade-113">If you're creating pages in the user's personal notebook, Microsoft Graph also provides endpoints you can use to create pages in the default notebook:</span></span>

- <span data-ttu-id="24ade-114">**Создание страницы в стандартном разделе стандартной записной книжки**</span><span class="sxs-lookup"><span data-stu-id="24ade-114">**Create a page in the default section of the default notebook**</span></span><br/><br/>`../pages` 



<span data-ttu-id="24ade-115">Полный URI запроса будет выглядеть так, как в одном из следующих примеров:</span><span class="sxs-lookup"><span data-stu-id="24ade-115">Your full request URI will look like one of these examples:</span></span>

- `https://graph.microsoft.com/v1.0/me/onenote/sections/{id}/pages`
- `https://graph.microsoft.com/v1.0/me/onenote/pages?sectionName=Homework`

<span data-ttu-id="24ade-116">См. дополнительные сведения о [корневом URL-адресе службы](../api-reference/v1.0/resources/onenote-api-overview.md#root-url).</span><span class="sxs-lookup"><span data-stu-id="24ade-116">Learn more about the [service root URL](../api-reference/v1.0/resources/onenote-api-overview.md#root-url).</span></span>

<a name="post-pages-section-name"></a>

### <a name="using-the-sectionname-url-parameter"></a><span data-ttu-id="24ade-117">Использование параметра *sectionName* URL-адреса</span><span class="sxs-lookup"><span data-stu-id="24ade-117">Using the *sectionName* URL parameter</span></span>

<span data-ttu-id="24ade-118">При создании страницы в именованном разделе записной книжки по умолчанию с помощью параметра *sectionName* действуют следующие правила:</span><span class="sxs-lookup"><span data-stu-id="24ade-118">The following rules apply when using the *sectionName* parameter to create a page in a named section in the default notebook:</span></span>

- <span data-ttu-id="24ade-119">Можно ссылаться только на разделы верхнего уровня (не внутри групп разделов).</span><span class="sxs-lookup"><span data-stu-id="24ade-119">Only top-level sections can be referenced (not sections within section groups).</span></span>

- <span data-ttu-id="24ade-120">Если в стандартной записной книжке нет раздела с указанным названием, API создает его.</span><span class="sxs-lookup"><span data-stu-id="24ade-120">If a section with the specified name doesn't exist in the default notebook, the API creates it.</span></span> <span data-ttu-id="24ade-121">В названиях разделов не допускаются следующие символы: `? * \ / : < > | & # " % ~`</span><span class="sxs-lookup"><span data-stu-id="24ade-121">These characters are not allowed for section names: `? * \ / : < > | & # " % ~`</span></span>

- <span data-ttu-id="24ade-122">При сопоставлении названий разделов регистр не учитывается, но он сохраняется при их создании.</span><span class="sxs-lookup"><span data-stu-id="24ade-122">Section names are case-insensitive for matching, but case is preserved when sections are created.</span></span> <span data-ttu-id="24ade-123">Например, если указать название "Мой новый раздел", то оно будет отображаться и дальше, но в последующих запросах можно использовать имя "мой новый раздел".</span><span class="sxs-lookup"><span data-stu-id="24ade-123">So "My New Section" will display like that, but "my new section" would also match on subsequent posts.</span></span>

- <span data-ttu-id="24ade-124">В названиях разделов следует использовать кодировку URL.</span><span class="sxs-lookup"><span data-stu-id="24ade-124">Section names must be URL-encoded.</span></span> <span data-ttu-id="24ade-125">Например, пробелы следует кодировать как *%20*.</span><span class="sxs-lookup"><span data-stu-id="24ade-125">For example, spaces must be encoded as *%20*.</span></span>

- <span data-ttu-id="24ade-126">Параметр *sectionName* действителен только с маршрутом `../notes/pages` (не `../notes/sections/{id}/pages`).</span><span class="sxs-lookup"><span data-stu-id="24ade-126">The *sectionName* parameter is valid only with the `../notes/pages` route (not `../notes/sections/{id}/pages`).</span></span>

<span data-ttu-id="24ade-127">Разделы создаются только в случае их отсутствия, поэтому этот вызов можно использовать для каждой страницы, создаваемой приложением.</span><span class="sxs-lookup"><span data-stu-id="24ade-127">Because sections are created if they don't exist, it's safe to use this call with every page your app creates.</span></span> <span data-ttu-id="24ade-128">Пользователи могут переименовывать разделы, но при этом API создаст новый раздел с указанным вами названием.</span><span class="sxs-lookup"><span data-stu-id="24ade-128">Users might rename sections, but the API will create a new section with the section name that you supply.</span></span> 

> <span data-ttu-id="24ade-129">**Примечание.** Возвращаемые интерфейсом API ссылки на страницы в переименованном разделе по-прежнему будут указывать на старые страницы.</span><span class="sxs-lookup"><span data-stu-id="24ade-129">**Note:** The links returned by the API for pages in a renamed section will still reach those older pages.</span></span> 


<a name="message-body"></a>

## <a name="construct-the-message-body"></a><span data-ttu-id="24ade-130">Составление текста сообщения</span><span class="sxs-lookup"><span data-stu-id="24ade-130">Construct the message body</span></span>

<span data-ttu-id="24ade-131">HTML-код, определяющий содержимое страницы, называют *входным HTML-кодом*.</span><span class="sxs-lookup"><span data-stu-id="24ade-131">The HTML that defines page content is called *input HTML*.</span></span> <span data-ttu-id="24ade-132">Входной HTML-код поддерживают [часть стандартных атрибутов HTML и CSS](#supported-html-and-css-for-onenote-pages), а также настраиваемые атрибуты.</span><span class="sxs-lookup"><span data-stu-id="24ade-132">Input HTML supports a [subset of standard HTML and CSS](#supported-html-and-css-for-onenote-pages), with the addition of custom attributes.</span></span> <span data-ttu-id="24ade-133">(Настраиваемые атрибуты, например **data-id** и **data-render-src**, описываются в статье [Входной и выходной HTML-код](onenote_input_output_html.md).)</span><span class="sxs-lookup"><span data-stu-id="24ade-133">(Custom attributes, like **data-id** and **data-render-src**, are described in [Input and output HTML](onenote_input_output_html.md).)</span></span> 

<span data-ttu-id="24ade-134">Отправьте входной HTML-код в тексте сообщения запроса POST.</span><span class="sxs-lookup"><span data-stu-id="24ade-134">Send the input HTML in the message body of the POST request.</span></span> <span data-ttu-id="24ade-135">Вы можете отправить HTML-код прямо в тексте сообщения, используя тип контента `application/xhtml+xml` или `text/html`, или в части Presentation составного запроса.</span><span class="sxs-lookup"><span data-stu-id="24ade-135">You can send the input HTML directly in the message body using the  `application/xhtml+xml` or `text/html` content type, or you can send it in the "Presentation" part of a multipart request.</span></span> 

<span data-ttu-id="24ade-136">В приведенном ниже примере входной HTML-код отправляется прямо в тексте сообщения.</span><span class="sxs-lookup"><span data-stu-id="24ade-136">The following example sends the input HTML directly in the message body.</span></span>

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
    <img src="http://..." alt="an image on the page" width="500" />
  </body>
</html>
```

<br/>

<span data-ttu-id="24ade-137">Если вы отправляете двоичные данные, необходимо использовать [составной запрос](#example-request).</span><span class="sxs-lookup"><span data-stu-id="24ade-137">If you're sending binary data, you must use a [multipart request](#example-request).</span></span> 

> <span data-ttu-id="24ade-138">**Примечание.** Чтобы упростить программирование и обеспечение согласованности в приложении, вы можете использовать составные запросы для создания всех страниц.</span><span class="sxs-lookup"><span data-stu-id="24ade-138">**Note:** To simplify programming and consistency in your app, you can use multipart requests to create all pages.</span></span> <span data-ttu-id="24ade-139">Рекомендуем использовать библиотеку для создания составных сообщений.</span><span class="sxs-lookup"><span data-stu-id="24ade-139">It's a good idea to use a library to construct multipart messages.</span></span> <span data-ttu-id="24ade-140">Это снижает риск создания полезных данных в неправильном формате.</span><span class="sxs-lookup"><span data-stu-id="24ade-140">This reduces the risk of creating malformed payloads.</span></span>


<a name="input-html-rules"></a>

### <a name="requirements-and-limitations-for-input-html-in-post-pages-requests"></a><span data-ttu-id="24ade-141">Требования и ограничения для входного HTML-кода в запросах POST для страниц</span><span class="sxs-lookup"><span data-stu-id="24ade-141">Requirements and limitations for input HTML in POST pages requests</span></span>

<span data-ttu-id="24ade-142">Отправляя входной HTML-код, учитывайте следующие требования и ограничения:</span><span class="sxs-lookup"><span data-stu-id="24ade-142">When sending input HTML, be aware of these general requirements and limitations:</span></span>  

- <span data-ttu-id="24ade-143">Входной HTML-код должен быть правильно оформленным XHTML-кодом с кодировкой UTF-8.</span><span class="sxs-lookup"><span data-stu-id="24ade-143">Input HTML should be UTF-8 encoded and well-formed XHTML.</span></span> <span data-ttu-id="24ade-144">Всем открывающим тегам контейнеров должны соответствовать закрывающие теги.</span><span class="sxs-lookup"><span data-stu-id="24ade-144">All container start tags require matching closing tags.</span></span> <span data-ttu-id="24ade-145">Все значения атрибутов должны быть окружены двойными или одинарными кавычками.</span><span class="sxs-lookup"><span data-stu-id="24ade-145">All attribute values must be surrounded by double- or single-quote marks.</span></span>  <!--docs say MUST be encoded-->

- <span data-ttu-id="24ade-146">Код JavaScript, вложенные файлы и CSS удаляются.</span><span class="sxs-lookup"><span data-stu-id="24ade-146">JavaScript code, included files, and CSS are removed.</span></span> 

- <span data-ttu-id="24ade-147">HTML-формы полностью удаляются.</span><span class="sxs-lookup"><span data-stu-id="24ade-147">HTML forms are removed in their entirety.</span></span>  

- <span data-ttu-id="24ade-148">Microsoft Graph поддерживает [подмножество элементов HTML](#supported-html-and-css-for-onenote-pages).</span><span class="sxs-lookup"><span data-stu-id="24ade-148">Microsoft Graph supports a [subset of HTML elements](#supported-html-and-css-for-onenote-pages).</span></span> 

- <span data-ttu-id="24ade-149">Microsoft Graph поддерживает отдельные стандартные атрибуты HTML и ряд настраиваемых атрибутов, таких как атрибут **data-id**, используемый для обновления страниц.</span><span class="sxs-lookup"><span data-stu-id="24ade-149">Microsoft Graph supports a subset of common HTML attributes and a set of custom attributes, such as the **data-id** attribute used for updating pages.</span></span> <span data-ttu-id="24ade-150">Поддерживаемые атрибуты описываются в статье [Входной и выходной HTML-код](onenote_input_output_html.md).</span><span class="sxs-lookup"><span data-stu-id="24ade-150">For supported attributes, see [Input and output HTML](onenote_input_output_html.md).</span></span>


<a name="supported-html"></a>

### <a name="supported-html-and-css-for-onenote-pages"></a><span data-ttu-id="24ade-151">Поддерживаемые атрибуты HTML и CSS для страниц OneNote</span><span class="sxs-lookup"><span data-stu-id="24ade-151">Supported HTML and CSS for OneNote pages</span></span>

<span data-ttu-id="24ade-152">Поддерживаются не все элементы, атрибуты и свойства (в HTML4, XHTML, CSS, HTML5 и т. д).</span><span class="sxs-lookup"><span data-stu-id="24ade-152">Not all elements, attributes, and properties are supported (in HTML4, XHTML, CSS, HTML5, etc.).</span></span> <span data-ttu-id="24ade-153">Microsoft Graph принимает ограниченный набор элементов HTML, более соответствующий особенностям работы с OneNote.</span><span class="sxs-lookup"><span data-stu-id="24ade-153">Instead, Microsoft Graph accepts a limited set of HTML that better fits how people use OneNote.</span></span> <span data-ttu-id="24ade-154">Дополнительные сведения см. на странице [Поддержка HTML-тегов для страниц](http://dev.onenote.com/docs#/introduction/html-tag-support-for-pages).</span><span class="sxs-lookup"><span data-stu-id="24ade-154">For more information, see [HTML tag support for pages](http://dev.onenote.com/docs#/introduction/html-tag-support-for-pages).</span></span> <span data-ttu-id="24ade-155">Если тег не указан на этой странице, скорее всего, он будет игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="24ade-155">If a tag's not listed there, it'll probably be ignored.</span></span>

<!--Microsoft Graph only accepts UTF-8 data. Be sure that all requests are encoded that way, and your content-type headers indicate that as well. xx our examples don't show this-->

<span data-ttu-id="24ade-156">Ниже перечислены базовые типы элементов, которые поддерживает Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="24ade-156">The following list shows the basic element types that Microsoft Graph supports:</span></span>

- <span data-ttu-id="24ade-157">`<head>` и `<body>`</span><span class="sxs-lookup"><span data-stu-id="24ade-157">`<head>` and `<body>`</span></span></p>
- <span data-ttu-id="24ade-158">`<title>` и `<meta>`, которые задают заголовок и дату создания страницы</span><span class="sxs-lookup"><span data-stu-id="24ade-158">`<title>` and `<meta>` that set the page title and creation date</span></span></p>
- <span data-ttu-id="24ade-159">`<h1>`–`<h6>` для заголовков разделов</span><span class="sxs-lookup"><span data-stu-id="24ade-159">`<h1>` through `<h6>` for section headings</span></span></p>
- <span data-ttu-id="24ade-160">`<p>` для абзацев</span><span class="sxs-lookup"><span data-stu-id="24ade-160">`<p>` for paragraphs</span></span></p>
- <span data-ttu-id="24ade-161">`<ul>`, `<ol>` и `<li>` для списков и их элементов</span><span class="sxs-lookup"><span data-stu-id="24ade-161">`<ul>`, `<ol>`, and `<li>` for lists and list items</span></span></p>
- <span data-ttu-id="24ade-162">`<table>`, `<tr>` и `<td>`, включая вложенные таблицы</span><span class="sxs-lookup"><span data-stu-id="24ade-162">`<table>`, `<tr>` and `<td>`, including nested tables</span></span></p>
- <span data-ttu-id="24ade-163">`<pre>` для предварительно отформатированного текста (с сохранением пробелов и разрывов строк)</span><span class="sxs-lookup"><span data-stu-id="24ade-163">`<pre>` for preformatted text (preserves white space and line breaks)</span></span></p>
- <span data-ttu-id="24ade-164">`<b>` и `<i>` для полужирного текста и курсива</span><span class="sxs-lookup"><span data-stu-id="24ade-164">`<b>` and `<i>` for bold and italic character styles</span></span></p>

<span data-ttu-id="24ade-165">Microsoft Graph сохраняет семантическое содержимое и базовую структуру входного HTML-кода при создании страниц, но преобразует входной HTML-код для использования поддерживаемого набора элементов HTML и CSS.</span><span class="sxs-lookup"><span data-stu-id="24ade-165">Microsoft Graph preserves the semantic content and basic structure of the input HTML when it creates pages, but it converts the input HTML to use the supported set of HTML and CSS.</span></span> <span data-ttu-id="24ade-166">Функции, отсутствующие в OneNote, преобразовывать не во что, поэтому они могут не распознаваться в исходном HTML-коде.</span><span class="sxs-lookup"><span data-stu-id="24ade-166">Features that don't exist in OneNote have nothing to be translated to, so they might not be recognized in the source HTML.</span></span> 


<a name="example"></a>

## <a name="example-request"></a><span data-ttu-id="24ade-167">Пример запроса</span><span class="sxs-lookup"><span data-stu-id="24ade-167">Example request</span></span>

<span data-ttu-id="24ade-168">Этот пример составного запроса создает страницу, содержащую изображения и внедренный файл.</span><span class="sxs-lookup"><span data-stu-id="24ade-168">This example multipart request creates a page that contains images and an embedded file.</span></span> <span data-ttu-id="24ade-169">Обязательная часть **Presentation** содержит входной HTML-код, определяющий страницу.</span><span class="sxs-lookup"><span data-stu-id="24ade-169">The required **Presentation** part contains the input HTML that defines the page.</span></span> <span data-ttu-id="24ade-170">Часть **imageBlock1** содержит двоичные данные изображения, а **fileBlock1** — двоичные данные файла.</span><span class="sxs-lookup"><span data-stu-id="24ade-170">The **imageBlock1** part contains the binary image data, and **fileBlock1** contains the binary file data.</span></span> <span data-ttu-id="24ade-171">Части данных также могут содержать HTML-код. В этом случае Microsoft Graph [отображает HTML-код в виде изображения](onenote_images_files.md#add-an-image-using-binary-data) на странице OneNote.</span><span class="sxs-lookup"><span data-stu-id="24ade-171">Data parts can also contain HTML, in which case Microsoft Graph [renders the HTML as an image](onenote_images_files.md#add-an-image-using-binary-data) on the OneNote page.</span></span> 

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
    <img src="http://..." alt="an image on the page" width="500" />
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

<span data-ttu-id="24ade-172">Дополнительные примеры создания страниц, содержащих изображения и другие файлы, см. в статье [Добавление изображений и файлов](onenote_images_files.md), наших [руководствах](https://docs.microsoft.com/en-us/previous-versions/office/office-365-api/how-to/onenote-tutorial) и [примерах](https://github.com/onenotedev).</span><span class="sxs-lookup"><span data-stu-id="24ade-172">For more examples that show how to create pages that contain images and other files, see [Add images and files](onenote_images_files.md), our [tutorials](https://docs.microsoft.com/en-us/previous-versions/office/office-365-api/how-to/onenote-tutorial), and our [samples](https://github.com/onenotedev).</span></span> <span data-ttu-id="24ade-173">Кроме того, узнайте, как [создавать элементы с абсолютным положением](onenote-abs-pos.md), [использовать теги примечаний](onenote-note-tags.md), а также [извлекать данные](onenote-extract-data.md) из визитных карточек, рецептов из Интернета и описаний продуктов.</span><span class="sxs-lookup"><span data-stu-id="24ade-173">Also, learn how to [create absolute positioned elements](onenote-abs-pos.md), [use note tags](onenote-note-tags.md), and [extract data](onenote-extract-data.md) for business card captures and online recipe and product listings.</span></span>

<span data-ttu-id="24ade-174">Microsoft Graph требует строгого соответствия некоторым форматам, таким как символы новой строки CRLF в тексте составного сообщения.</span><span class="sxs-lookup"><span data-stu-id="24ade-174">Microsoft Graph is strict about some formats, such as CRLF newlines in a multipart message body.</span></span> <span data-ttu-id="24ade-175">Чтобы снизить риск создания полезных данных в неправильном формате, следует использовать библиотеку для создания составных сообщений.</span><span class="sxs-lookup"><span data-stu-id="24ade-175">To reduce the risk of creating malformed payloads, you should use a library to construct multipart messages.</span></span> 

<span data-ttu-id="24ade-176">Если появится состояние 400 (неправильный формат полезных данных), проверьте форматирование символов новой строки и пробелов, а также наличие проблем с кодировкой.</span><span class="sxs-lookup"><span data-stu-id="24ade-176">If you do receive a 400 status for a malformed payload, check the formatting of newlines and whitespaces, and check for encoding issues.</span></span> <span data-ttu-id="24ade-177">Например, попробуйте использовать параметр `charset=utf-8` (пример: `Content-Type: text/html; charset=utf-8`).</span><span class="sxs-lookup"><span data-stu-id="24ade-177">For example, try using `charset=utf-8` (example: `Content-Type: text/html; charset=utf-8`).</span></span>

<span data-ttu-id="24ade-178">См. [требования и ограничения для входного HTML-кода](#requirements-and-limitations-for-input-html-in-post-pages-requests) и [ограничения размера запросов POST](onenote_images_files.md#size-limitations-for-post-pages-requests).</span><span class="sxs-lookup"><span data-stu-id="24ade-178">See [requirements and limitations for input HTML](#requirements-and-limitations-for-input-html-in-post-pages-requests) and [size limits for POST requests](onenote_images_files.md#size-limitations-for-post-pages-requests).</span></span>


<a name="request-response-info"></a>

## <a name="request-and-response-information-for-post-pages-requests"></a><span data-ttu-id="24ade-179">Информация о запросах *POST для страниц* и соответствующих ответах</span><span class="sxs-lookup"><span data-stu-id="24ade-179">Request and response information for *POST pages* requests</span></span>

| <span data-ttu-id="24ade-180">Данные запроса</span><span class="sxs-lookup"><span data-stu-id="24ade-180">Request data</span></span> | <span data-ttu-id="24ade-181">Описание</span><span class="sxs-lookup"><span data-stu-id="24ade-181">Description</span></span> |  
|------|------|  
| <span data-ttu-id="24ade-182">Протокол</span><span class="sxs-lookup"><span data-stu-id="24ade-182">Protocol</span></span> | <span data-ttu-id="24ade-183">Все запросы используют протокол SSL/TLS для HTTPS.</span><span class="sxs-lookup"><span data-stu-id="24ade-183">All requests use the SSL/TLS HTTPS protocol.</span></span> |  
| <span data-ttu-id="24ade-184">Заголовок Authorization</span><span class="sxs-lookup"><span data-stu-id="24ade-184">Authorization header</span></span> | <p><span data-ttu-id="24ade-185">`Bearer {token}`, где `{token}` — действительный маркер доступа OAuth 2.0 для зарегистрированного приложения.</span><span class="sxs-lookup"><span data-stu-id="24ade-185">`Bearer {token}`, where `{token}` is a valid OAuth 2.0 access token for your registered app.</span></span></p><p><span data-ttu-id="24ade-186">Если он отсутствует или является недействительным, запрос завершится ошибкой с кодом состояния 401.</span><span class="sxs-lookup"><span data-stu-id="24ade-186">If missing or invalid, the request fails with a 401 status code.</span></span> <span data-ttu-id="24ade-187">См. статью [Проверка подлинности и разрешения](permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="24ade-187">See [Authentication and permissions](permissions_reference.md).</span></span></p> |  
| <span data-ttu-id="24ade-188">Заголовок Content-Type</span><span class="sxs-lookup"><span data-stu-id="24ade-188">Content-Type header</span></span> | <p><span data-ttu-id="24ade-189">`text/html` или `application/xhtml+xml` для HTML-содержимого, отправляемого либо непосредственно в тексте сообщения, либо в обязательной части Presentation составных запросов.</span><span class="sxs-lookup"><span data-stu-id="24ade-189">`text/html` or `application/xhtml+xml` for the HTML content, whether it's sent directly in the message body or in the required "Presentation" part of multipart requests.</span></span></p><p><span data-ttu-id="24ade-190">Составные запросы необходимы при отправке двоичных данных и используют тип контента `multipart/form-data; boundary=part-boundary`, где `{part-boundary}` — это строка, обозначающая начало и конец каждой части данных.</span><span class="sxs-lookup"><span data-stu-id="24ade-190">Multipart requests are required when sending binary data, and use the `multipart/form-data; boundary=part-boundary` content type, where `{part-boundary}` is a string that signals the start and end of each data part.</span></span></p> |  
| <span data-ttu-id="24ade-191">Заголовок Accept</span><span class="sxs-lookup"><span data-stu-id="24ade-191">Accept header</span></span> | `application/json` | 

<br/>

| <span data-ttu-id="24ade-192">Данные ответа</span><span class="sxs-lookup"><span data-stu-id="24ade-192">Response data</span></span> | <span data-ttu-id="24ade-193">Описание</span><span class="sxs-lookup"><span data-stu-id="24ade-193">Description</span></span> |  
|------|------|  
| <span data-ttu-id="24ade-194">Код успешного завершения</span><span class="sxs-lookup"><span data-stu-id="24ade-194">Success code</span></span> | <span data-ttu-id="24ade-195">Код состояния HTTP 201</span><span class="sxs-lookup"><span data-stu-id="24ade-195">A 201 HTTP status code.</span></span> |  
| <span data-ttu-id="24ade-196">Текст ответа</span><span class="sxs-lookup"><span data-stu-id="24ade-196">Response body</span></span> | <span data-ttu-id="24ade-197">Представление OData новой страницы в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="24ade-197">A OData representation of the new page in JSON format.</span></span> |  
| <span data-ttu-id="24ade-198">Ошибки</span><span class="sxs-lookup"><span data-stu-id="24ade-198">Errors</span></span> | <span data-ttu-id="24ade-199">Если запрос завершается с ошибкой, API возвращает ошибки в объекте **@api.diagnostics** в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="24ade-199">If the request fails, the API returns errors in the **@api.diagnostics** object in the response body.</span></span> |  
| <span data-ttu-id="24ade-200">Заголовок Location</span><span class="sxs-lookup"><span data-stu-id="24ade-200">Location header</span></span> | <span data-ttu-id="24ade-201">URL-адрес ресурса новой страницы.</span><span class="sxs-lookup"><span data-stu-id="24ade-201">The resource URL for the new page.</span></span> |  
| <span data-ttu-id="24ade-202">Заголовок X-CorrelationId</span><span class="sxs-lookup"><span data-stu-id="24ade-202">X-CorrelationId header</span></span> | <span data-ttu-id="24ade-203">GUID, уникальный идентификатор запроса.</span><span class="sxs-lookup"><span data-stu-id="24ade-203">A GUID that uniquely identifies the request.</span></span> <span data-ttu-id="24ade-204">Это значение можно использовать вместе со значением заголовка Date при устранении неполадок совместно со службой поддержки Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="24ade-204">You can use this value along with the value of the Date header when working with Microsoft support to troubleshoot issues.</span></span> |  


<a name="root-url"></a>

### <a name="constructing-the-microsoft-graph-service-root-url"></a><span data-ttu-id="24ade-205">Составление корневого URL-адреса службы Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="24ade-205">Constructing the Microsoft Graph service root URL</span></span>

<span data-ttu-id="24ade-206">В корневом URL-адресе службы Microsoft Graph используется следующий формат для всех вызовов Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="24ade-206">The Microsoft Graph service root URL uses the following format for all calls to Microsoft Graph:</span></span>

`https://graph.microsoft.com/{version}/me/onenote/`  

<span data-ttu-id="24ade-207">Сегмент `version` URL-адреса представляет нужную версию Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="24ade-207">The `version` segment in the URL represents the version of Microsoft Graph that you want to use.</span></span> <span data-ttu-id="24ade-208">Используйте значение `v1.0` для стабильного кода в рабочей среде.</span><span class="sxs-lookup"><span data-stu-id="24ade-208">Use `v1.0` for stable production code.</span></span> <span data-ttu-id="24ade-209">Используйте значение `beta`, чтобы опробовать функцию, находящуюся на стадии разработки.</span><span class="sxs-lookup"><span data-stu-id="24ade-209">Use `beta` to try out a feature that's in development.</span></span> <span data-ttu-id="24ade-210">Функции бета-версии могут меняться, поэтому не следует использовать их в производственном коде.</span><span class="sxs-lookup"><span data-stu-id="24ade-210">Features and functionality in beta may change, so you shouldn't use it in your production code.</span></span> 

<span data-ttu-id="24ade-211">Используйте значение `me` для содержимого OneNote, доступного текущему пользователю (если он является владельцем или с ним поделились этим содержимым).</span><span class="sxs-lookup"><span data-stu-id="24ade-211">Use `me` for OneNote content that the current user can access (owned and shared).</span></span> <span data-ttu-id="24ade-212">Используйте значение `users/{id}` для содержимого OneNote, которым указанный (в URL-адресе) пользователь поделился с текущим пользователем.</span><span class="sxs-lookup"><span data-stu-id="24ade-212">Use `users/{id}` for OneNote content that the specified user (in the URL) has shared with the current user.</span></span> <span data-ttu-id="24ade-213">Используйте [Microsoft Graph](https://graph.microsoft.com/v1.0/users) для получения идентификаторов пользователей.</span><span class="sxs-lookup"><span data-stu-id="24ade-213">Use [Microsoft Graph](https://graph.microsoft.com/v1.0/users) to get user IDs.</span></span> 


<a name="permissions"></a>

## <a name="permissions"></a><span data-ttu-id="24ade-214">Разрешения</span><span class="sxs-lookup"><span data-stu-id="24ade-214">Permissions</span></span>

<span data-ttu-id="24ade-215">Для создания страниц OneNote необходимо запрашивать соответствующие разрешения.</span><span class="sxs-lookup"><span data-stu-id="24ade-215">To create OneNote pages, you'll need to request appropriate permissions.</span></span> <span data-ttu-id="24ade-216">Выберите минимальный уровень разрешений, необходимый для работы вашего приложения.</span><span class="sxs-lookup"><span data-stu-id="24ade-216">Choose the lowest level of permissions that your app needs to do its work.</span></span>

<span data-ttu-id="24ade-217">Варианты:</span><span class="sxs-lookup"><span data-stu-id="24ade-217">Choose from:</span></span>

- <span data-ttu-id="24ade-218">Notes.Create</span><span class="sxs-lookup"><span data-stu-id="24ade-218">Notes.Create</span></span>
- <span data-ttu-id="24ade-219">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="24ade-219">Notes.ReadWrite</span></span>
- <span data-ttu-id="24ade-220">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24ade-220">Notes.ReadWrite.All</span></span>

<span data-ttu-id="24ade-221">Дополнительные сведения о разрешениях и принципе их работы см. в [справочнике по разрешениям Microsoft Graph](permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="24ade-221">For more information about permission scopes and how they work, see [Microsoft Graph permissions reference](permissions_reference.md).</span></span>




<a name="see-also"></a>

## <a name="see-also"></a><span data-ttu-id="24ade-222">См. также</span><span class="sxs-lookup"><span data-stu-id="24ade-222">See also</span></span>

- [<span data-ttu-id="24ade-223">Добавление изображений и файлов</span><span class="sxs-lookup"><span data-stu-id="24ade-223">Add images and files</span></span>](onenote_images_files.md)
- [<span data-ttu-id="24ade-224">Создание элементов с абсолютным положением</span><span class="sxs-lookup"><span data-stu-id="24ade-224">Create absolute positioned elements</span></span>](onenote-abs-pos.md)  
- [<span data-ttu-id="24ade-225">Извлечение данных</span><span class="sxs-lookup"><span data-stu-id="24ade-225">Extract data</span></span>](onenote-extract-data.md)
- [<span data-ttu-id="24ade-226">Использование тегов заметок</span><span class="sxs-lookup"><span data-stu-id="24ade-226">Use note tags</span></span>](onenote-note-tags.md)
- [<span data-ttu-id="24ade-227">Интеграция с OneNote</span><span class="sxs-lookup"><span data-stu-id="24ade-227">Integrate with OneNote</span></span>](integrate_with_onenote.md)
- [<span data-ttu-id="24ade-228">Блог разработчиков OneNote</span><span class="sxs-lookup"><span data-stu-id="24ade-228">OneNote Developer Blog</span></span>](http://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="24ade-229">Вопросы разработки OneNote на сайте Stack Overflow</span><span class="sxs-lookup"><span data-stu-id="24ade-229">OneNote development questions on Stack Overflow</span></span>](http://go.microsoft.com/fwlink/?LinkID=390182)
- [<span data-ttu-id="24ade-230">Репозитории GitHub OneNote</span><span class="sxs-lookup"><span data-stu-id="24ade-230">OneNote GitHub repos</span></span>](http://go.microsoft.com/fwlink/?LinkID=390178)  


