---
title: Добавление изображений, видео и файлов на страницы OneNote
description: " Корпоративные записные книжки в Microsoft 365"
author: jewan-microsoft
localization_priority: Priority
ms.prod: onenote
ms.openlocfilehash: b601495db396d136a1181c81431f70c025475d45
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50474906"
---
# <a name="add-images-videos-and-files-to-onenote-pages"></a><span data-ttu-id="c2de9-103">Добавление изображений, видео и файлов на страницы OneNote</span><span class="sxs-lookup"><span data-stu-id="c2de9-103">Add images, videos, and files to OneNote pages</span></span>

<span data-ttu-id="c2de9-104">**Область применения**: пользовательские записные книжки в OneDrive | корпоративные записные книжки в Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="c2de9-104">**Applies to** Consumer notebooks on OneDrive | Enterprise notebooks on Microsoft 365</span></span>

<span data-ttu-id="c2de9-105">С помощью элементов **img**, **object** и **iframe** вы можете добавлять изображения, видео и файлы на страницу OneNote при ее [создании](onenote-create-page.md) или [обновлении](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="c2de9-105">You can use **img**, **object**, and **iframe** elements to add images, videos, and files to a OneNote page when you're [creating](onenote-create-page.md) or [updating](onenote-update-page.md) the page.</span></span> 

- <span data-ttu-id="c2de9-106">Элемент **img** используется для отрисовки изображения на странице.</span><span class="sxs-lookup"><span data-stu-id="c2de9-106">Use **img** to render an image on the page.</span></span>
- <span data-ttu-id="c2de9-107">Элемент **iframe** используется для внедрения видео в страницу.</span><span class="sxs-lookup"><span data-stu-id="c2de9-107">Use **iframe** to embed a video on the page.</span></span>
- <span data-ttu-id="c2de9-108">Элемент **object** используется для добавления вложенного файла на страницу.</span><span class="sxs-lookup"><span data-stu-id="c2de9-108">Use **object** to add a file attachment to the page.</span></span>


<a name="images"></a>

## <a name="adding-images"></a><span data-ttu-id="c2de9-109">Добавление изображений</span><span class="sxs-lookup"><span data-stu-id="c2de9-109">Adding images</span></span>

<span data-ttu-id="c2de9-110">Изображения можно добавлять по URL-адресу или путем отправки необработанных данных.</span><span class="sxs-lookup"><span data-stu-id="c2de9-110">Images can be added by URL reference or by sending raw data.</span></span> <span data-ttu-id="c2de9-111">Microsoft Graph поддерживает перечисленные ниже способы добавления изображений, логотипов и фотографий на страницы OneNote.</span><span class="sxs-lookup"><span data-stu-id="c2de9-111">Microsoft Graph supports the following methods of adding images, logos, and photos to OneNote pages.</span></span> 

[<span data-ttu-id="c2de9-112">Добавление общедоступного изображения из Интернета</span><span class="sxs-lookup"><span data-stu-id="c2de9-112">Add a public image from the web</span></span>](#add-a-public-image-from-the-web)

<span data-ttu-id="c2de9-113">Используйте элемент `img` с параметром `src="https://image-url"` и укажите URL-адрес общедоступного изображения.</span><span class="sxs-lookup"><span data-stu-id="c2de9-113">Use `img` with `src="https://image-url"` and specify the URL of a publicly accessible image.</span></span> <span data-ttu-id="c2de9-114">Отрисовывает изображение на странице OneNote.</span><span class="sxs-lookup"><span data-stu-id="c2de9-114">Renders the image on the OneNote page.</span></span>

[<span data-ttu-id="c2de9-115">Добавление изображения с помощью двоичных данных</span><span class="sxs-lookup"><span data-stu-id="c2de9-115">Add an image using binary data</span></span>](#add-an-image-using-binary-data)

<span data-ttu-id="c2de9-116">Используйте элемент `img` с параметром `src="name:image-block-name"` и отправьте файл изображения в части данных составного запроса.</span><span class="sxs-lookup"><span data-stu-id="c2de9-116">Use `img` with `src="name:image-block-name"` and send the image file in a data part of a multipart request.</span></span> <span data-ttu-id="c2de9-117">Отрисовывает изображение на странице OneNote.</span><span class="sxs-lookup"><span data-stu-id="c2de9-117">Renders the image on the OneNote page.</span></span>

[<span data-ttu-id="c2de9-118">Добавление моментального снимка веб-страницы</span><span class="sxs-lookup"><span data-stu-id="c2de9-118">Add a webpage snapshot</span></span>](#add-a-webpage-snapshot)

<span data-ttu-id="c2de9-119">Используйте элемент `img` с параметром `data-render-src="https://webpage-url"` и укажите URL-адрес веб-страницы.</span><span class="sxs-lookup"><span data-stu-id="c2de9-119">Use `img` with `data-render-src="https://webpage-url"` and specify the URL of a webpage.</span></span> <span data-ttu-id="c2de9-120">Отрисовывает моментальный снимок всей веб-страницы на странице OneNote.</span><span class="sxs-lookup"><span data-stu-id="c2de9-120">Renders a snapshot of the whole webpage on the OneNote page.</span></span>

[<span data-ttu-id="c2de9-121">Добавление изображения, созданного из HTML-кода</span><span class="sxs-lookup"><span data-stu-id="c2de9-121">Add an image rendered from HTML</span></span>](#add-an-image-rendered-from-html)

<span data-ttu-id="c2de9-122">Используйте элемент `img` с параметром `data-render-src="name:html-block-name"` и отправьте HTML-код в части данных составного запроса.</span><span class="sxs-lookup"><span data-stu-id="c2de9-122">Use `img` with `data-render-src="name:html-block-name"` and send HTML in the data part of a multipart request.</span></span> <span data-ttu-id="c2de9-123">Отрисовывает HTML в виде изображения на странице OneNote.</span><span class="sxs-lookup"><span data-stu-id="c2de9-123">Renders the HTML as an image on the OneNote page.</span></span>

[<span data-ttu-id="c2de9-124">Добавление изображений содержимого PDF-файлов</span><span class="sxs-lookup"><span data-stu-id="c2de9-124">Add images of PDF file contents</span></span>](#add-images-of-pdf-file-contents)

<span data-ttu-id="c2de9-125">Используйте элемент `<img data-render-src="name:part-name" />` и отправьте PDF-файл в части данных составного запроса.</span><span class="sxs-lookup"><span data-stu-id="c2de9-125">Use `<img data-render-src="name:part-name" />` and send the PDF file in the data part of a multipart request.</span></span> <span data-ttu-id="c2de9-126">Отрисовывает каждую PDF-страницу в виде отдельного изображения на странице OneNote.</span><span class="sxs-lookup"><span data-stu-id="c2de9-126">Renders each PDF page as a separate image on the OneNote page.</span></span>

[<span data-ttu-id="c2de9-127">Добавление файла изображения в качестве вложения</span><span class="sxs-lookup"><span data-stu-id="c2de9-127">Add an image file as a file attachment</span></span>](#add-an-image-file-as-an-attachment)

<span data-ttu-id="c2de9-128">Используйте элемент `object` с параметром `data="name:file-block-name" data-attachment="file-name.file-ext" type="media-type"` и отправьте файл изображения в части данных составного запроса.</span><span class="sxs-lookup"><span data-stu-id="c2de9-128">Use `object` with `data="name:file-block-name" data-attachment="file-name.file-ext" type="media-type"` and send an image file in the data part of a multipart request.</span></span> <span data-ttu-id="c2de9-129">Добавляет вложенный файл на страницу OneNote и отображает значок файла.</span><span class="sxs-lookup"><span data-stu-id="c2de9-129">Adds a file attachment to the OneNote page and displays a file icon.</span></span>


> <span data-ttu-id="c2de9-130">**Примечание.** Чтобы получить изображения со страницы OneNote, сначала отправьте [запрос GET на получение содержимого страницы](onenote-get-content.md#page-html-content).</span><span class="sxs-lookup"><span data-stu-id="c2de9-130">**Note:** To get images on a OneNote page, first send a [GET request for the page content](onenote-get-content.md#page-html-content).</span></span> <span data-ttu-id="c2de9-131">Будут возвращены URL-адреса ресурсов изображений на странице.</span><span class="sxs-lookup"><span data-stu-id="c2de9-131">This returns the URLs to the image resources on the page.</span></span> <span data-ttu-id="c2de9-132">Затем разделите [запросы GET на получение ресурсов изображений](onenote-get-content.md#image-or-other-file-resource).</span><span class="sxs-lookup"><span data-stu-id="c2de9-132">You then separate [GET requests to the image resources](onenote-get-content.md#image-or-other-file-resource).</span></span>


#### <a name="image-attributes"></a><span data-ttu-id="c2de9-133">Атрибуты изображений</span><span class="sxs-lookup"><span data-stu-id="c2de9-133">Image attributes</span></span> 

<span data-ttu-id="c2de9-134">Элемент **img** при необходимости может включать атрибуты **alt**, **height** и **width**, а также атрибуты стиля **max-width** и **max-height**.</span><span class="sxs-lookup"><span data-stu-id="c2de9-134">An **img** element can optionally include **alt**, **height**, and **width** attributes, and the style attributes **max-width** and **max-height**.</span></span>

#### <a name="image-media-types"></a><span data-ttu-id="c2de9-135">Типы мультимедиа для изображений</span><span class="sxs-lookup"><span data-stu-id="c2de9-135">Image media types</span></span>

<span data-ttu-id="c2de9-136">Microsoft Graph поддерживает типы изображений TIFF, PNG, GIF, JPEG и BMP.</span><span class="sxs-lookup"><span data-stu-id="c2de9-136">Microsoft Graph supports TIFF, PNG, GIF, JPEG, and BMP image types.</span></span> <span data-ttu-id="c2de9-137">Чтобы сохранить изображение другого формата, которое желательно не преобразовывать, [отправьте двоичные данные](#add-an-image-using-binary-data) в составном запросе.</span><span class="sxs-lookup"><span data-stu-id="c2de9-137">To capture an image that uses a different format that you don't want to convert, [send the binary data](#add-an-image-using-binary-data) in a multipart request.</span></span> <span data-ttu-id="c2de9-138">Использовать Base64 или другую кодировку для двоичных данных не нужно.</span><span class="sxs-lookup"><span data-stu-id="c2de9-138">You don't need to use Base64 or otherwise encode the binary data that you send.</span></span>

> <span data-ttu-id="c2de9-139">**Примечание.** API обнаруживает исходный тип входного изображения и возвращает его в виде атрибута **data-fullres-src-type** [выходного HTML-кода](onenote-input-output-html.md#output-html).</span><span class="sxs-lookup"><span data-stu-id="c2de9-139">**Note:** The API detects the original input image type, and returns it as the **data-fullres-src-type** attribute in the [output HTML](onenote-input-output-html.md#output-html).</span></span> <span data-ttu-id="c2de9-140">API также возвращает тип оптимизированного изображения в атрибуте **data-src-type**.</span><span class="sxs-lookup"><span data-stu-id="c2de9-140">The API also returns the image type of the optimized image in **data-src-type**.</span></span>
 
<span data-ttu-id="c2de9-141">Ознакомьтесь с [ограничениями](#size-limitations-for-post-pages-requests) на создание страниц, содержащих файлы мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="c2de9-141">See [limitations](#size-limitations-for-post-pages-requests) that apply when creating pages that contain media.</span></span>


<a name="image-img-url-src"></a>

### <a name="add-a-public-image-from-the-web"></a><span data-ttu-id="c2de9-142">Добавление общедоступного изображения из Интернета</span><span class="sxs-lookup"><span data-stu-id="c2de9-142">Add a public image from the web</span></span>

<span data-ttu-id="c2de9-143">Во входные данные HTML-кода запроса включите параметр `<img src="https://..." />` и укажите URL-адрес общедоступного изображения в атрибуте **src**.</span><span class="sxs-lookup"><span data-stu-id="c2de9-143">In the input HTML of your request, include `<img src="https://..." />` and specify the URL of a publicly accessible image for the **src** attribute.</span></span>

```html
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with an image: Public URL</title>
    <meta name="created" value="2015-11-11T12:45:00.000-8:00"/>
  </head>
  <body>
    <p>This page displays an image from the web.</p>
    <img src="https://..." width="300"/>
  </body>
</html>

--MyAppPartBoundary--  
```

<a name="image-img-binary-src"></a>

### <a name="add-an-image-using-binary-data"></a><span data-ttu-id="c2de9-144">Добавление изображения с помощью двоичных данных</span><span class="sxs-lookup"><span data-stu-id="c2de9-144">Add an image using binary data</span></span>

<span data-ttu-id="c2de9-145">Во входной HTML-код из части **Presentation** запроса включите параметр `<img src="name:part-name" />`, где *part-name* — это уникальный идентификатор той части [составного запроса](onenote-create-page.md#example-request), которая содержит двоичные данные изображения.</span><span class="sxs-lookup"><span data-stu-id="c2de9-145">In the input HTML of your request's **Presentation** part, include `<img src="name:part-name" />`, where *part-name* is the unique identifier for the data part in your [multipart request](onenote-create-page.md#example-request) that contains the binary image data.</span></span> <span data-ttu-id="c2de9-146">Просто отправьте двоичные данные, не используя Base64 или другую кодировку.</span><span class="sxs-lookup"><span data-stu-id="c2de9-146">Just send the binary data, don't use Base64 or otherwise encode it.</span></span>

```html
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with an image: Image binary data</title>
    <meta name="created" value="2015-11-11T12:45:00.000-8:00"/>
  </head>
  <body>
    <p>This page displays the uploaded image.</p>
    <img src="name:image-block-name" alt="a cool image" width="500"/>
  </body>
</html>

--MyAppPartBoundary
Content-Disposition: form-data; name="MyAppPictureId"
Content-Type: image/jpeg

... image binary data ...

--MyAppPartBoundary--  
```


<a name="image-img-url-data-render-src"></a>

### <a name="add-a-webpage-snapshot"></a><span data-ttu-id="c2de9-147">Добавление моментального снимка веб-страницы</span><span class="sxs-lookup"><span data-stu-id="c2de9-147">Add a webpage snapshot</span></span>

<span data-ttu-id="c2de9-148">С помощью Microsoft Graph можно создавать моментальные снимки целых веб-страниц и вставлять их в новые страницы.</span><span class="sxs-lookup"><span data-stu-id="c2de9-148">You can use Microsoft Graph to snapshot entire webpages and insert them into new pages.</span></span> <span data-ttu-id="c2de9-149">Этот метод удобен для архивации веб-страниц и сохранения сложных веб-страниц, которые содержат функции, не поддерживаемые OneNote (например, CSS).</span><span class="sxs-lookup"><span data-stu-id="c2de9-149">This method is useful to archive webpages or capture complex webpages that have features that OneNote doesn't support (like some CSS).</span></span>  

<span data-ttu-id="c2de9-150">Во входной HTML-код запроса включите параметр `<img src="https://..." />` и укажите URL-адрес веб-страницы, которую нужно вставить, в атрибуте **src**.</span><span class="sxs-lookup"><span data-stu-id="c2de9-150">In the input HTML of your request, include `<img src="https://..." />` and specify the URL of the webpage you want to insert for the **src** attribute.</span></span>

```html
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with an image: Webpage capture</title>
    <meta name="created" value="2015-11-11T12:45:00.000-8:00"/>
  </head>
  <body>
    <p>This page displays an image of the webpage.</p>
    <img data-render-src="https://www.onenote.com" width="200"/>
  </body>
</html>

--MyAppPartBoundary--  
```


<a name="image-img-binary-data-render-src"></a>

### <a name="add-an-image-rendered-from-html"></a><span data-ttu-id="c2de9-151">Добавление изображения, созданного из HTML-кода</span><span class="sxs-lookup"><span data-stu-id="c2de9-151">Add an image rendered from HTML</span></span>

<span data-ttu-id="c2de9-152">При передаче HTML-кода в виде блока данных убедитесь в отсутствии активного содержимого, для которого могут потребоваться учетные данные пользователя или предварительно загруженный подключаемый модуль браузера.</span><span class="sxs-lookup"><span data-stu-id="c2de9-152">When you pass the HTML as a data-block, be sure there is no active content that would require user credentials, or a pre-loaded browser plug-in.</span></span> <span data-ttu-id="c2de9-153">Подсистема, которую Microsoft Graph использует для преобразования HTML-страницы в изображение, не может выполнить вход для пользователя и не включает такие подключаемые модули, как Adobe Flash и Apple QuickTime.</span><span class="sxs-lookup"><span data-stu-id="c2de9-153">The engine that Microsoft Graph uses to render the HTML page into an image has no ability to log in a user, and doesn't include plug-ins like Adobe Flash, Apple QuickTime, and so on.</span></span> <span data-ttu-id="c2de9-154">Это также означает, что динамически загружаемое содержимое (например, через скрипт AJAX) не будет отображаться, если для получения данных необходимы учетные данные пользователя или файлы cookie.</span><span class="sxs-lookup"><span data-stu-id="c2de9-154">That also means that dynamically-loaded content, such as might come with an AJAX script, won't appear if getting the data requires user login credentials or cookies.</span></span>

<span data-ttu-id="c2de9-155">Во входной HTML-код из части **Presentation** запроса включите параметр `<img data-render-src="name:part-name" />`, где *part-name* — это уникальный идентификатор той части [составного запроса](onenote-create-page.md#example-request), которая содержит HTML-код.</span><span class="sxs-lookup"><span data-stu-id="c2de9-155">In the input HTML of your request's **Presentation** part, include `<img data-render-src="name:part-name" />`, where *part-name* is the unique identifier for the data part in your [multipart request](onenote-create-page.md#example-request) that contains the HTML.</span></span>


```html
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with an image: HTML block</title>
    <meta name="created" value="2015-11-11T12:45:00.000-8:00"/>
  </head>
  <body>
    <p>This page displays the block of HTML as an image.</p>
    <img data-render-src="name:html-block-name" alt="a cool image" width="500"/>
  </body>
</html>

--MyAppPartBoundary
Content-Disposition: form-data; name="html-block-name"
Content-Type: text/html

<html>
<body>
<h1>This HTML will render as an image</h1>
<p><b>Don't</b> try to embed another <i>data-render-src</i> type-image inside the HTML part--
it won't work. Instead, use URL-based real images like this:</p>
<img src="https://cdn.onenote.net/1664161560_Images/OneNote.ico" />
</body>
</html>

--MyAppPartBoundary--  
```


<a name="image-object"></a>

### <a name="add-an-image-file-as-an-attachment"></a><span data-ttu-id="c2de9-156">Добавление файла изображения в качестве вложения</span><span class="sxs-lookup"><span data-stu-id="c2de9-156">Add an image file as an attachment</span></span>

<span data-ttu-id="c2de9-157">Во входной HTML-код из части **Presentation** запроса включите параметр `<object data="name:part-name" data-attachment="file-name.file-ext" type="media-type/media-subtype" />`, где *part-name* — это уникальный идентификатор той части [составного запроса](onenote-create-page.md#example-request), которая содержит двоичные данные изображения.</span><span class="sxs-lookup"><span data-stu-id="c2de9-157">In the input HTML of your request's **Presentation** part, include `<object data="name:part-name" data-attachment="file-name.file-ext" type="media-type/media-subtype" />`, where *part-name* is the unique identifier for the data part in your [multipart request](onenote-create-page.md#example-request) that contains the binary image data.</span></span> <span data-ttu-id="c2de9-158">Просто отправьте двоичные данные, не используя Base64 или другую кодировку.</span><span class="sxs-lookup"><span data-stu-id="c2de9-158">Just send the binary data, don't use Base64 or otherwise encode it.</span></span>

```html
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with an image: Binary image data as file attachment</title>
    <meta name="created" value="2015-11-11T12:45:00.000-8:00"/>
  </head>
  <body>
    <p>This page contains the image as a file attachment.</p>
    <object data-attachment="image-file.jpg" data="name:image-block-name" type="image/jpeg" />
  </body>
</html>

--MyAppPartBoundary
Content-Disposition: form-data; name="logo1-file"
Content-Type: image/jpeg

... binary file data ...

--MyAppPartBoundary--
```

<span data-ttu-id="c2de9-159">Узнайте больше о [типах файлов мультимедиа](#file-media-types).</span><span class="sxs-lookup"><span data-stu-id="c2de9-159">Learn more about [file media types](#file-media-types).</span></span>



<a name="adding-videos"></a>

## <a name="adding-videos"></a><span data-ttu-id="c2de9-160">Добавление видео</span><span class="sxs-lookup"><span data-stu-id="c2de9-160">Adding videos</span></span>

<span data-ttu-id="c2de9-161">Вы можете внедрять видео в страницы OneNote с помощью команды `<iframe data-original-src="https://..." />` во входном HTML-коде.</span><span class="sxs-lookup"><span data-stu-id="c2de9-161">You can embed videos in OneNote pages using `<iframe data-original-src="https://..." />` in the input HTML.</span></span> 

### <a name="supported-video-sites"></a><span data-ttu-id="c2de9-162">Поддерживаемые сайты с видео</span><span class="sxs-lookup"><span data-stu-id="c2de9-162">Supported video sites</span></span>

- <span data-ttu-id="c2de9-163">Dailymotion</span><span class="sxs-lookup"><span data-stu-id="c2de9-163">Dailymotion</span></span>
- <span data-ttu-id="c2de9-164">Office Mix</span><span class="sxs-lookup"><span data-stu-id="c2de9-164">Office Mix</span></span>
- <span data-ttu-id="c2de9-165">Sway</span><span class="sxs-lookup"><span data-stu-id="c2de9-165">Sway</span></span>
- <span data-ttu-id="c2de9-166">Sketchfab</span><span class="sxs-lookup"><span data-stu-id="c2de9-166">Sketchfab</span></span>
- <span data-ttu-id="c2de9-167">TED</span><span class="sxs-lookup"><span data-stu-id="c2de9-167">TED</span></span>
- <span data-ttu-id="c2de9-168">YouTube</span><span class="sxs-lookup"><span data-stu-id="c2de9-168">YouTube</span></span>
- <span data-ttu-id="c2de9-169">Vimeo</span><span class="sxs-lookup"><span data-stu-id="c2de9-169">Vimeo</span></span>
- <span data-ttu-id="c2de9-170">Vine</span><span class="sxs-lookup"><span data-stu-id="c2de9-170">Vine</span></span>

### <a name="iframe-attributes"></a><span data-ttu-id="c2de9-171">Атрибуты iframe</span><span class="sxs-lookup"><span data-stu-id="c2de9-171">iframe attributes</span></span>

#### <a name="data-original-src"></a><span data-ttu-id="c2de9-172">data-original-src</span><span class="sxs-lookup"><span data-stu-id="c2de9-172">data-original-src</span></span>

<span data-ttu-id="c2de9-173">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c2de9-173">Required.</span></span> <span data-ttu-id="c2de9-174">URL-адрес видео.</span><span class="sxs-lookup"><span data-stu-id="c2de9-174">The URL of the video.</span></span>

<span data-ttu-id="c2de9-175">Пример: `data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8"`</span><span class="sxs-lookup"><span data-stu-id="c2de9-175">Example: `data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8"`</span></span>

#### <a name="width"></a><span data-ttu-id="c2de9-176">width</span><span class="sxs-lookup"><span data-stu-id="c2de9-176">width</span></span>

<span data-ttu-id="c2de9-177">Необязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="c2de9-177">Optional.</span></span> <span data-ttu-id="c2de9-178">Ширина элемента iframe, содержащего видео.</span><span class="sxs-lookup"><span data-stu-id="c2de9-178">The width of the iframe that contains the video.</span></span> <span data-ttu-id="c2de9-179">Значение по умолчанию: 480.</span><span class="sxs-lookup"><span data-stu-id="c2de9-179">Default is 480.</span></span>

<span data-ttu-id="c2de9-180">Пример: `width="300"`</span><span class="sxs-lookup"><span data-stu-id="c2de9-180">Example: `width="300"`</span></span>

#### <a name="height"></a><span data-ttu-id="c2de9-181">height</span><span class="sxs-lookup"><span data-stu-id="c2de9-181">height</span></span>

<span data-ttu-id="c2de9-182">Необязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="c2de9-182">Optional.</span></span> <span data-ttu-id="c2de9-183">Высота элемента iframe, содержащего видео.</span><span class="sxs-lookup"><span data-stu-id="c2de9-183">The height of the iframe that contains the video.</span></span> <span data-ttu-id="c2de9-184">Значение по умолчанию: 360.</span><span class="sxs-lookup"><span data-stu-id="c2de9-184">Default is 360.</span></span>

<span data-ttu-id="c2de9-185">Пример: `height="300"`</span><span class="sxs-lookup"><span data-stu-id="c2de9-185">Example: `height="300"`</span></span>

### <a name="example"></a><span data-ttu-id="c2de9-186">Пример</span><span class="sxs-lookup"><span data-stu-id="c2de9-186">Example</span></span>

<span data-ttu-id="c2de9-187">Во входном HTML-коде запроса добавьте параметр `<iframe data-original-src="https://..." />` и укажите URL-адрес видео в атрибуте **data-original-src**.</span><span class="sxs-lookup"><span data-stu-id="c2de9-187">In the input HTML of your request, include `<iframe data-original-src="https://..." />` and specify the URL of the video for the **data-original-src** attribute.</span></span>

```html
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
    <head>
        <title>A page with an embedded video</title>
    </head>
    <body>
        <iframe data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8" width="340" height="280"/>
    </body>
</html>

--MyAppPartBoundary--
```


<a name="adding-files"></a>

## <a name="adding-files"></a><span data-ttu-id="c2de9-188">Добавление файлов</span><span class="sxs-lookup"><span data-stu-id="c2de9-188">Adding files</span></span>

<span data-ttu-id="c2de9-189">Вы можете добавлять вложенные файлы в страницы OneNote с помощью элемента **object** во входном HTML-коде.</span><span class="sxs-lookup"><span data-stu-id="c2de9-189">You can add file attachments to OneNote pages using an **object** element in the input HTML.</span></span> <span data-ttu-id="c2de9-190">Если вам нужно добавить PDF-файл, вы можете использовать элемент **img** для отрисовки страниц PDF-файла в виде изображений.</span><span class="sxs-lookup"><span data-stu-id="c2de9-190">If you're adding a PDF file, you can use an **img** element to render the PDF pages as images.</span></span> 

[<span data-ttu-id="c2de9-191">Добавление вложенного файла</span><span class="sxs-lookup"><span data-stu-id="c2de9-191">Add a file attachment</span></span>](#add-a-file-attachment)

<span data-ttu-id="c2de9-192">Используйте элемент `<object .../>` и отправьте файл в части данных составного запроса.</span><span class="sxs-lookup"><span data-stu-id="c2de9-192">Use `<object .../>` and send the file in a data part of a multipart request.</span></span> <span data-ttu-id="c2de9-193">Добавляет вложенный файл и отображает значок файла на странице OneNote.</span><span class="sxs-lookup"><span data-stu-id="c2de9-193">Adds a file attachment that displays a file icon on the OneNote page.</span></span>

[<span data-ttu-id="c2de9-194">Добавление изображений содержимого PDF-файлов</span><span class="sxs-lookup"><span data-stu-id="c2de9-194">Add images of PDF file contents</span></span>](#add-images-of-pdf-file-contents)

<span data-ttu-id="c2de9-195">Используйте элемент `<img data-render-src="name:part-name" />` и отправьте PDF-файл в части данных составного запроса.</span><span class="sxs-lookup"><span data-stu-id="c2de9-195">Use `<img data-render-src="name:part-name" />` and send a PDF file in the data part of a multipart request.</span></span> <span data-ttu-id="c2de9-196">Отрисовывает каждую PDF-страницу в виде отдельного изображения на странице OneNote.</span><span class="sxs-lookup"><span data-stu-id="c2de9-196">Renders each PDF page as a separate image on the OneNote page.</span></span>

#### <a name="file-attributes"></a><span data-ttu-id="c2de9-197">Атрибуты файлов</span><span class="sxs-lookup"><span data-stu-id="c2de9-197">File attributes</span></span>

<span data-ttu-id="c2de9-198">Ниже перечислены обязательные атрибуты элемента **object**.</span><span class="sxs-lookup"><span data-stu-id="c2de9-198">The **object** element requires the following attributes.</span></span>

<span data-ttu-id="c2de9-199">**data-attachment**</span><span class="sxs-lookup"><span data-stu-id="c2de9-199">**data-attachment**</span></span>

<span data-ttu-id="c2de9-200">Имя и расширения файла, который нужно отобразить на странице OneNote.</span><span class="sxs-lookup"><span data-stu-id="c2de9-200">The file name and extension to display on the OneNote page.</span></span>

<span data-ttu-id="c2de9-201">Пример: `data-attachment="filename.docx"`</span><span class="sxs-lookup"><span data-stu-id="c2de9-201">Example: `data-attachment="filename.docx"`</span></span>

<span data-ttu-id="c2de9-202">**data**</span><span class="sxs-lookup"><span data-stu-id="c2de9-202">**data**</span></span>

<span data-ttu-id="c2de9-203">Имя части body в составном запросе, содержащем двоичные данные файла.</span><span class="sxs-lookup"><span data-stu-id="c2de9-203">The name of the body part in the multipart request that contains the binary file data.</span></span> <span data-ttu-id="c2de9-204">Microsoft Graph не поддерживает передачу URL-адресов через этот атрибут.</span><span class="sxs-lookup"><span data-stu-id="c2de9-204">Microsoft Graph does not support passing a URL reference here.</span></span>

<span data-ttu-id="c2de9-205">Пример: `data="name:part-name"`</span><span class="sxs-lookup"><span data-stu-id="c2de9-205">Example: `data="name:part-name"`</span></span>

<span data-ttu-id="c2de9-206">**type**</span><span class="sxs-lookup"><span data-stu-id="c2de9-206">**type**</span></span>

<span data-ttu-id="c2de9-207">MIME-тип файла, который используется для определения значка файла для страницы и приложения, запускаемого, когда пользователь активирует файл на устройстве из OneNote.</span><span class="sxs-lookup"><span data-stu-id="c2de9-207">The file media type, used to determine the file icon to use on the page, and which application starts when the user activates the file on the device from OneNote.</span></span>

<span data-ttu-id="c2de9-208">Пример: `type="application/pdf"`</span><span class="sxs-lookup"><span data-stu-id="c2de9-208">Example: `type="application/pdf"`</span></span>


<a name="file-media-types"></a>

#### <a name="file-media-types"></a><span data-ttu-id="c2de9-209">MIME-типы файлов</span><span class="sxs-lookup"><span data-stu-id="c2de9-209">File media types</span></span>  

<span data-ttu-id="c2de9-210">Microsoft Graph использует предопределенный значок для типа вложенного файла или универсальный значок, если API не распознает тип файла.</span><span class="sxs-lookup"><span data-stu-id="c2de9-210">Microsoft Graph uses predefined file-types icon for attached files, or a generic icon when the API doesn't recognize the file type.</span></span> <span data-ttu-id="c2de9-211">В приведенной ниже таблице показаны распространенные типы файлов, которые распознает этот API.</span><span class="sxs-lookup"><span data-stu-id="c2de9-211">The following table shows some common file types that are recognized by the API.</span></span>

- <span data-ttu-id="c2de9-212">application/pdf</span><span class="sxs-lookup"><span data-stu-id="c2de9-212">application/pdf</span></span>  
- <span data-ttu-id="c2de9-213">application/vnd.openxmlformats-officedocument.wordprocessingml.document</span><span class="sxs-lookup"><span data-stu-id="c2de9-213">application/vnd.openxmlformats-officedocument.wordprocessingml.document</span></span>  
- <span data-ttu-id="c2de9-214">application/vnd.openxmlformats-officedocument.presentationml.presentation</span><span class="sxs-lookup"><span data-stu-id="c2de9-214">application/vnd.openxmlformats-officedocument.presentationml.presentation</span></span>
- <span data-ttu-id="c2de9-215">application/vnd.openxmlformats-officedocument.spreadsheetml.sheet</span><span class="sxs-lookup"><span data-stu-id="c2de9-215">application/vnd.openxmlformats-officedocument.spreadsheetml.sheet</span></span>
- <span data-ttu-id="c2de9-216">image/png</span><span class="sxs-lookup"><span data-stu-id="c2de9-216">image/png</span></span>
- <span data-ttu-id="c2de9-217">image/jpeg</span><span class="sxs-lookup"><span data-stu-id="c2de9-217">image/jpeg</span></span>
- <span data-ttu-id="c2de9-218">image/gif</span><span class="sxs-lookup"><span data-stu-id="c2de9-218">image/gif</span></span>
- <span data-ttu-id="c2de9-219">audio/wav</span><span class="sxs-lookup"><span data-stu-id="c2de9-219">audio/wav</span></span>
- <span data-ttu-id="c2de9-220">video/mp4</span><span class="sxs-lookup"><span data-stu-id="c2de9-220">video/mp4</span></span>
- <span data-ttu-id="c2de9-221">application/msword</span><span class="sxs-lookup"><span data-stu-id="c2de9-221">application/msword</span></span>
- <span data-ttu-id="c2de9-222">application/mspowerpoint</span><span class="sxs-lookup"><span data-stu-id="c2de9-222">application/mspowerpoint</span></span>
- <span data-ttu-id="c2de9-223">application/excel</span><span class="sxs-lookup"><span data-stu-id="c2de9-223">application/excel</span></span>

<span data-ttu-id="c2de9-224">Ознакомьтесь с [ограничениями](#size-limitations-for-post-pages-requests) на создание страниц, содержащих файлы мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="c2de9-224">See [limitations](#size-limitations-for-post-pages-requests) that apply when creating pages that contain media.</span></span>


<a name="file-object"></a>

### <a name="add-a-file-attachment"></a><span data-ttu-id="c2de9-225">Добавление вложенного файла</span><span class="sxs-lookup"><span data-stu-id="c2de9-225">Add a file attachment</span></span>

<span data-ttu-id="c2de9-226">Во входной HTML-код из части **Presentation** запроса включите параметр `<object data="name:part-name" data-attachment="file-name.file-ext" type="media-type/media-subtype" />`, где *part-name* — это уникальный идентификатор той части [составного запроса](onenote-create-page.md#example-request), которая содержит данные двоичного файла.</span><span class="sxs-lookup"><span data-stu-id="c2de9-226">In the input HTML of your request's **Presentation** part, include `<object data="name:part-name" data-attachment="file-name.file-ext" type="media-type/media-subtype" />`, where *part-name* is the unique identifier for the data part in your [multipart request](onenote-create-page.md#example-request) that contains the binary file data.</span></span> <span data-ttu-id="c2de9-227">Просто отправьте двоичные данные, не используя Base64 или другую кодировку.</span><span class="sxs-lookup"><span data-stu-id="c2de9-227">Just send the binary data, don't use Base64 or otherwise encode it.</span></span>

```html
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with an image file attachment</title>
  </head>
  <body>
    <p>This is an image file attachment.</p>
    <object data-attachment="Logo.jpg" data="name:logo1-file" type="image/jpeg" />
  </body>
</html>

--MyAppPartBoundary
Content-Disposition: form-data; name="logo1-file"
Content-Type: image/jpeg

... binary file data ...

--MyAppPartBoundary--
```


<a name="file-binary-data-render-src"></a>

### <a name="add-images-of-pdf-file-contents"></a><span data-ttu-id="c2de9-228">Добавление изображений содержимого PDF-файлов</span><span class="sxs-lookup"><span data-stu-id="c2de9-228">Add images of PDF file contents</span></span>

<span data-ttu-id="c2de9-229">Во входной HTML-код из части **Presentation** запроса включите параметр `<img data-render-src="name:part-name" ... />`, где *part-name* — это уникальный идентификатор той части [составного запроса](onenote-create-page.md#example-request), которая содержит данные двоичного файла.</span><span class="sxs-lookup"><span data-stu-id="c2de9-229">In the input HTML of your request's **Presentation** part, include `<img data-render-src="name:part-name" ... />`, where *part-name* is the unique identifier for the data part in your [multipart request](onenote-create-page.md#example-request) that contains the binary file data.</span></span> <span data-ttu-id="c2de9-230">Просто отправьте двоичные данные, не используя Base64 или другую кодировку.</span><span class="sxs-lookup"><span data-stu-id="c2de9-230">Just send the binary data, don't use Base64 or otherwise encode it.</span></span>

```html
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with images of the pages of a PDF file</title>
  </head>
  <body>
    <p>The pages of this PDF file render as images.</p>
    <img data-render-src="name:file-part" alt="PDF file as images" width="500"/>
  </body>
</html>

--MyAppPartBoundary
Content-Disposition: form-data; name="file-part"
Content-Type: application/pdf

... binary file data ...

--MyAppPartBoundary--  
```


<a name="size-limits"></a>

## <a name="size-limitations-for-post-pages-requests"></a><span data-ttu-id="c2de9-231">Ограничения на размер запросов POST для страниц</span><span class="sxs-lookup"><span data-stu-id="c2de9-231">Size limitations for POST pages requests</span></span>

<span data-ttu-id="c2de9-232">При отправке изображений и файлов учитывайте следующие ограничения:</span><span class="sxs-lookup"><span data-stu-id="c2de9-232">When sending image and file data, be aware of these limitations:</span></span> <!--TODO: check these-->

- <span data-ttu-id="c2de9-233">Для REST API Microsoft Graph применяется ограничение размера запроса 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="c2de9-233">The Microsoft Graph REST API has a 4 MB request limit.</span></span> <span data-ttu-id="c2de9-234">Любое превышение этого значения приведет к ошибке с сообщением "запрос слишком большой (413)".</span><span class="sxs-lookup"><span data-stu-id="c2de9-234">Anything above this will fail with the error message "request too large (413)".</span></span> 

- <span data-ttu-id="c2de9-235">Ограничение запроса для базового интерфейса REST API OneNote выше, но он недоступен через API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c2de9-235">The request limit of the underlying OneNote REST API is higher, but you cannot access it via the Microsoft Graph API.</span></span> 
  - <span data-ttu-id="c2de9-236">Общий максимальный размер данных в запросе POST (включая изображения, файлы и другие данные) составляет приблизительно 70 МБ.</span><span class="sxs-lookup"><span data-stu-id="c2de9-236">The total POST size limit is ~70 MB, including images, files, and other data.</span></span> <span data-ttu-id="c2de9-237">Фактическое ограничение зависит от кодировки в нижестоящих системах, поэтому не существует фиксированного ограничения в байтах.</span><span class="sxs-lookup"><span data-stu-id="c2de9-237">The actual limit is affected by downstream encoding, so there's no fixed byte-count limit.</span></span> <span data-ttu-id="c2de9-238">Запросы, превышающие это ограничение, могут возвращать ненадежные результаты.</span><span class="sxs-lookup"><span data-stu-id="c2de9-238">Requests that exceed the limit might produce unreliable results.</span></span>
  - <span data-ttu-id="c2de9-239">Ограничение для каждой части данных (включая заголовки) составляет 25 МБ.</span><span class="sxs-lookup"><span data-stu-id="c2de9-239">The limit for each data part is 25 MB, including the part headers.</span></span> <span data-ttu-id="c2de9-240">Microsoft Graph отклоняет части данных, превышающие это ограничение.</span><span class="sxs-lookup"><span data-stu-id="c2de9-240">Data parts that exceed the limit are rejected by Microsoft Graph.</span></span> 

- <span data-ttu-id="c2de9-241">Максимальное количество изображений на странице составляет 150.</span><span class="sxs-lookup"><span data-stu-id="c2de9-241">The maximum number of images per page is 150.</span></span> <span data-ttu-id="c2de9-242">При использовании атрибута `src="https://..."` API игнорирует теги **img** после достижения этого предела.</span><span class="sxs-lookup"><span data-stu-id="c2de9-242">When using the `src="https://..."` attribute, the API ignores **img** tags beyond the limit.</span></span>

- <span data-ttu-id="c2de9-243">Каждый запрос POST может включать до 6 частей данных, включая обязательную часть **Presentation**.</span><span class="sxs-lookup"><span data-stu-id="c2de9-243">The maximum number of data parts is 6 per POST, including the required **Presentation** part.</span></span>

- <span data-ttu-id="c2de9-p129">Каждый запрос может содержать до пяти элементов **img** с атрибутом **data-render-src** и один элемент **object** с атрибутом **data-render-src**. Остальные ссылки на изображения и файлы игнорируются.</span><span class="sxs-lookup"><span data-stu-id="c2de9-p129">Each request can contain up to five **img** elements that use **data-render-src** and one **object** elements that uses **data-render-src**. Additional image and file references are ignored.</span></span>

- <span data-ttu-id="c2de9-246">Один запрос POST может включать до 30 изображений, независимо от того, какой метод используется для их отправки в API.</span><span class="sxs-lookup"><span data-stu-id="c2de9-246">The maximum number of images in a single POST is 30, no matter which method you use to send them to the API.</span></span> <span data-ttu-id="c2de9-247">Остальные изображения игнорируются.</span><span class="sxs-lookup"><span data-stu-id="c2de9-247">Additional images are ignored.</span></span> <span data-ttu-id="c2de9-248">Если вам нужно сохранить веб-страницу с большим количеством изображений, рекомендуем [сохранить ее в виде моментального снимка](#add-a-webpage-snapshot).</span><span class="sxs-lookup"><span data-stu-id="c2de9-248">If you want to capture a webpage that contains a lot of images, consider [capturing the whole page as a snapshot](#add-a-webpage-snapshot).</span></span>


## <a name="when-to-use-html-versus-data-render-src"></a><span data-ttu-id="c2de9-249">Когда использовать HTML, а когда — data-render-src</span><span class="sxs-lookup"><span data-stu-id="c2de9-249">When to use HTML versus data-render-src</span></span> 

<span data-ttu-id="c2de9-250">Если вы выбираете между вставкой HTML на страницу OneNote и использованием атрибута **data-render-src**, учитывайте следующее:</span><span class="sxs-lookup"><span data-stu-id="c2de9-250">When trying to decide between putting HTML directly onto the OneNote page instead of using the **data-render-src** attribute, consider the following:</span></span>

- <span data-ttu-id="c2de9-251">Сложный HTML, вероятно, лучше отправлять в механизм визуализации с помощью **data-render-src**, а не пытаться изменить HTML так, чтобы его принял Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c2de9-251">Complex HTML is probably best sent to the rendering engine via **data-render-src**, rather than attempting to modify the HTML to fit into what Microsoft Graph can accept.</span></span> <span data-ttu-id="c2de9-252">Это также относится к тем случаям, когда HTML-код включает неподдерживаемые теги.</span><span class="sxs-lookup"><span data-stu-id="c2de9-252">This is also true when your HTML includes tags that aren't supported supported.</span></span>

- <span data-ttu-id="c2de9-253">Как правило, точную отрисовку страниц для сохранения макета и внешнего вида страницы лучше обеспечивает механизм визуализации с использованием атрибута **data-render-src**.</span><span class="sxs-lookup"><span data-stu-id="c2de9-253">Accurate page rendering to preserve the layout and look of the page is probably best done with the rendering engine via **data-render-src**.</span></span>

- <span data-ttu-id="c2de9-p132">Напрямую редактируемый текст часто лучше всего реализовать, вставляя HTML напрямую на страницу. Отрисованные изображения сканируются системой распознавания текста (OCR), но результаты не будут одинаковыми.</span><span class="sxs-lookup"><span data-stu-id="c2de9-p132">Directly-editable text is often best done with inserting the HTML directly onto the page. The rendered images are scanned by an optical character recognition (OCR) system, but it's just not the same.</span></span>

- <span data-ttu-id="c2de9-256">Моментальный снимок для журнала или архива лучше всего создавать с помощью метода **data-render-src**.</span><span class="sxs-lookup"><span data-stu-id="c2de9-256">Snapshot-in-time for historical or archival purposes is usually best done with the **data-render-src** method.</span></span>

- <span data-ttu-id="c2de9-p133">Отметка проекта веб-страницы для редактирования — это задача, где **data-render-src** по-настоящему проявляет себя. Используя возможности рукописного ввода OneNote, можно нарисовать изображение для обозначения изменений или подчеркнуть важные области. Наличие веб-страницы в форме изображения намного упрощает эту задачу.</span><span class="sxs-lookup"><span data-stu-id="c2de9-p133">Marking-up a web page design for revisions is one place the **data-render-src** truly shines. Using OneNote's inking capabilities, you can draw on the image to indicate changes or call out important areas. Having the web page as an image makes that a lot easier.</span></span>

- <span data-ttu-id="c2de9-260">Очень крупные изображения или изображения в форматах, которые OneNote не принимает напрямую, иногда легче преобразовать в эскизы и другие форматы с помощью атрибута **data-render-src**, а не собственного кода.</span><span class="sxs-lookup"><span data-stu-id="c2de9-260">Very large images, or images in formats that OneNote doesn't directly accept, can sometimes be thumbnailed and converted with the **data-render-src** attribute more easily than by doing it in your own code.</span></span> <span data-ttu-id="c2de9-261">Даже если изображение также доступно в сети, внедрение данных в запрос POST иногда позволяет быстрее сделать сохраненную страницу доступной пользователям OneNote за счет уменьшения общего количества круговых путей, необходимых для создания страницы OneNote.</span><span class="sxs-lookup"><span data-stu-id="c2de9-261">Even if the image is also available online, embedding the data in your POST can sometimes make the captured page available to OneNote users sooner, by reducing the total number of round-trips needed to build the OneNote page.</span></span>

<span data-ttu-id="c2de9-262">Иногда лучший способ определить, какой метод лучше подойдет пользователям — опробовать оба варианта во время разработки приложения.</span><span class="sxs-lookup"><span data-stu-id="c2de9-262">Sometimes, the best way to determine which method will work best for your users is to try it both ways as you develop your app.</span></span>


<a name="permissions"></a>

## <a name="permissions"></a><span data-ttu-id="c2de9-263">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c2de9-263">Permissions</span></span>

<span data-ttu-id="c2de9-264">Для создания и обновления страниц OneNote необходимо запрашивать соответствующие разрешения.</span><span class="sxs-lookup"><span data-stu-id="c2de9-264">To create or update OneNote pages, you'll need to request appropriate permissions.</span></span> <span data-ttu-id="c2de9-265">Выберите минимальный уровень, необходимый для работы вашего приложения.</span><span class="sxs-lookup"><span data-stu-id="c2de9-265">Choose the lowest level that your app needs to do its work.</span></span>

#### <a name="permissions-for-post-pages"></a><span data-ttu-id="c2de9-266">Разрешения в случае запросов POST для страниц</span><span class="sxs-lookup"><span data-stu-id="c2de9-266">Permissions for POST pages</span></span>

- <span data-ttu-id="c2de9-267">Notes.Create</span><span class="sxs-lookup"><span data-stu-id="c2de9-267">Notes.Create</span></span>
- <span data-ttu-id="c2de9-268">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c2de9-268">Notes.ReadWrite</span></span>
- <span data-ttu-id="c2de9-269">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2de9-269">Notes.ReadWrite.All</span></span> 

#### <a name="permissions-for-patch-pages"></a><span data-ttu-id="c2de9-270">Разрешения в случае запросов PATCH для страниц</span><span class="sxs-lookup"><span data-stu-id="c2de9-270">Permissions for PATCH pages</span></span>

- <span data-ttu-id="c2de9-271">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c2de9-271">Notes.ReadWrite</span></span>
- <span data-ttu-id="c2de9-272">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2de9-272">Notes.ReadWrite.All</span></span>

<span data-ttu-id="c2de9-273">Дополнительные сведения об областях разрешений и принципе их работы см. в разделе [Области разрешений OneNote](permissions-reference.md#notes-permissions).</span><span class="sxs-lookup"><span data-stu-id="c2de9-273">For more information about permission scopes and how they work, see [OneNote permission scopes](permissions-reference.md#notes-permissions).</span></span>


<a name="see-also"></a>

## <a name="see-also"></a><span data-ttu-id="c2de9-274">См. также</span><span class="sxs-lookup"><span data-stu-id="c2de9-274">See also</span></span>

- [<span data-ttu-id="c2de9-275">Интеграция с OneNote</span><span class="sxs-lookup"><span data-stu-id="c2de9-275">Integrate with OneNote</span></span>](integrate-with-onenote.md)
- [<span data-ttu-id="c2de9-276">Блог разработчиков OneNote</span><span class="sxs-lookup"><span data-stu-id="c2de9-276">OneNote Developer Blog</span></span>](https://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="c2de9-277">Вопросы разработки OneNote на сайте «Вопросы и ответы Майкрософт»</span><span class="sxs-lookup"><span data-stu-id="c2de9-277">OneNote development questions on Microsoft Q&A</span></span>](https://docs.microsoft.com/answers/topics/microsoft-graph-notes.html)
- [<span data-ttu-id="c2de9-278">Репозитории GitHub OneNote</span><span class="sxs-lookup"><span data-stu-id="c2de9-278">OneNote GitHub repos</span></span>](https://go.microsoft.com/fwlink/?LinkID=390178)  
