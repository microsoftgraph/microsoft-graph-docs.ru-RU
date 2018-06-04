
# <a name="add-images-videos-and-files-to-onenote-pages"></a><span data-ttu-id="6592e-101">Добавление изображений, видео и файлов на страницы OneNote</span><span class="sxs-lookup"><span data-stu-id="6592e-101">Add images, videos, and files to OneNote pages</span></span>

<span data-ttu-id="6592e-102">*__Относится к:__ пользовательские записные книжки в OneDrive | корпоративные записные книжки в Office 365*</span><span class="sxs-lookup"><span data-stu-id="6592e-102">*__Applies to:__ Consumer notebooks on OneDrive | Enterprise notebooks on Office 365*</span></span>

<span data-ttu-id="6592e-103">С помощью элементов **img**, **object** и **iframe** вы можете добавлять изображения, видео и файлы на страницу OneNote при ее [создании](onenote-create-page.md) или [обновлении](onenote_update_page.md).</span><span class="sxs-lookup"><span data-stu-id="6592e-103">You can use **img**, **object**, and **iframe** elements to add images, videos, and files to a OneNote page when you're [creating](onenote-create-page.md) or [updating](onenote_update_page.md) the page.</span></span> 

- <span data-ttu-id="6592e-104">Элемент **img** используется для отрисовки изображения на странице.</span><span class="sxs-lookup"><span data-stu-id="6592e-104">Use **img** to render an image on the page.</span></span>
- <span data-ttu-id="6592e-105">Элемент **iframe** используется для внедрения видео в страницу.</span><span class="sxs-lookup"><span data-stu-id="6592e-105">Use **iframe** to embed a video on the page.</span></span>
- <span data-ttu-id="6592e-106">Элемент **object** используется для добавления вложенного файла на страницу.</span><span class="sxs-lookup"><span data-stu-id="6592e-106">Use **object** to add a file attachment to the page.</span></span>


<a name="images"></a>
## <a name="adding-images"></a><span data-ttu-id="6592e-107">Добавление изображений</span><span class="sxs-lookup"><span data-stu-id="6592e-107">Adding images</span></span>

<span data-ttu-id="6592e-108">Изображения можно добавлять по URL-адресу или путем отправки необработанных данных.</span><span class="sxs-lookup"><span data-stu-id="6592e-108">Images can be added by URL reference or by sending raw data.</span></span> <span data-ttu-id="6592e-109">Microsoft Graph поддерживает перечисленные ниже способы добавления изображений, логотипов и фотографий на страницы OneNote.</span><span class="sxs-lookup"><span data-stu-id="6592e-109">Microsoft Graph supports the following methods of adding images, logos, and photos to OneNote pages.</span></span> 

[<span data-ttu-id="6592e-110">Добавление общедоступного изображения из Интернета</span><span class="sxs-lookup"><span data-stu-id="6592e-110">Add a public image from the web</span></span>](#add-a-public-image-from-the-web)  
<span data-ttu-id="6592e-111">Используйте элемент `img` с параметром `src="http://image-url"` и укажите URL-адрес общедоступного изображения.</span><span class="sxs-lookup"><span data-stu-id="6592e-111">Use `img` with `src="http://image-url"` and specify the URL of a publicly accessible image.</span></span> <span data-ttu-id="6592e-112">Отрисовывает изображение на странице OneNote.</span><span class="sxs-lookup"><span data-stu-id="6592e-112">Renders the image on the OneNote page.</span></span></p>
[<span data-ttu-id="6592e-113">Добавление изображения с помощью двоичных данных</span><span class="sxs-lookup"><span data-stu-id="6592e-113">Add an image using binary data</span></span>](#add-an-image-using-binary-data)</p>
<span data-ttu-id="6592e-114">Используйте элемент `img` с параметром `src="name:image-block-name"` и отправьте файл изображения в части данных составного запроса.</span><span class="sxs-lookup"><span data-stu-id="6592e-114">Use `img` with `src="name:image-block-name"` and send the image file in a data part of a multipart request.</span></span> <span data-ttu-id="6592e-115">Отрисовывает изображение на странице OneNote.</span><span class="sxs-lookup"><span data-stu-id="6592e-115">Renders the image on the OneNote page.</span></span></p>
[<span data-ttu-id="6592e-116">Добавление моментального снимка веб-страницы</span><span class="sxs-lookup"><span data-stu-id="6592e-116">Add a webpage snapshot</span></span>](#add-a-webpage-snapshot)</p>
<span data-ttu-id="6592e-117">Используйте элемент `img` с параметром `data-render-src="http://webpage-url"` и укажите URL-адрес веб-страницы.</span><span class="sxs-lookup"><span data-stu-id="6592e-117">Use `img` with `data-render-src="http://webpage-url"` and specify the URL of a webpage.</span></span> <span data-ttu-id="6592e-118">Отрисовывает моментальный снимок всей веб-страницы на странице OneNote.</span><span class="sxs-lookup"><span data-stu-id="6592e-118">Renders a snapshot of the whole webpage on the OneNote page.</span></span></p>
[<span data-ttu-id="6592e-119">Добавление изображения, созданного из HTML-кода</span><span class="sxs-lookup"><span data-stu-id="6592e-119">Add an image rendered from HTML</span></span>](#add-an-image-rendered-from-html)</p>
<span data-ttu-id="6592e-120">Используйте элемент `img` с параметром `data-render-src="name:html-block-name"` и отправьте HTML-код в части данных составного запроса.</span><span class="sxs-lookup"><span data-stu-id="6592e-120">Use `img` with `data-render-src="name:html-block-name"` and send HTML in the data part of a multipart request.</span></span> <span data-ttu-id="6592e-121">Отрисовывает HTML в виде изображения на странице OneNote.</span><span class="sxs-lookup"><span data-stu-id="6592e-121">Renders the HTML as an image on the OneNote page.</span></span></p>
[<span data-ttu-id="6592e-122">Добавление изображений содержимого PDF-файлов</span><span class="sxs-lookup"><span data-stu-id="6592e-122">Add images of PDF file contents</span></span>](#add-images-of-pdf-file-contents)</p>
<span data-ttu-id="6592e-123">Используйте элемент `<img data-render-src="name:part-name" />` и отправьте PDF-файл в части данных составного запроса.</span><span class="sxs-lookup"><span data-stu-id="6592e-123">Use `<img data-render-src="name:part-name" />` and send the PDF file in the data part of a multipart request.</span></span> <span data-ttu-id="6592e-124">Отрисовывает каждую PDF-страницу в виде отдельного изображения на странице OneNote.</span><span class="sxs-lookup"><span data-stu-id="6592e-124">Renders each PDF page as a separate image on the OneNote page.</span></span></p>
[<span data-ttu-id="6592e-125">Добавление файла изображения в качестве вложения</span><span class="sxs-lookup"><span data-stu-id="6592e-125">Add an image file as a file attachment</span></span>](#add-an-image-file-as-an-attachment)</p>
<span data-ttu-id="6592e-126">Используйте элемент `object` с параметром `data="name:file-block-name" data-attachment="file-name.file-ext" type="media-type"` и отправьте файл изображения в части данных составного запроса.</span><span class="sxs-lookup"><span data-stu-id="6592e-126">Use `object` with `data="name:file-block-name" data-attachment="file-name.file-ext" type="media-type"` and send an image file in the data part of a multipart request.</span></span> <span data-ttu-id="6592e-127">Добавляет вложенный файл на страницу OneNote и отображает значок файла.</span><span class="sxs-lookup"><span data-stu-id="6592e-127">Adds a file attachment to the OneNote page and displays a file icon.</span></span></p>

> <span data-ttu-id="6592e-128">**Примечание.** Чтобы получить изображения со страницы OneNote, сначала отправьте [запрос GET на получение содержимого страницы](onenote-get-content.md#page-html-content).</span><span class="sxs-lookup"><span data-stu-id="6592e-128">**Note:** To get images on a OneNote page, first send a [GET request for the page content](onenote-get-content.md#page-html-content).</span></span> <span data-ttu-id="6592e-129">Будут возвращены URL-адреса ресурсов изображения на странице.</span><span class="sxs-lookup"><span data-stu-id="6592e-129">This returns the URLs to the image resources on the page.</span></span> <span data-ttu-id="6592e-130">Затем разделите [запросы GET на получение ресурсов изображений](onenote-get-content.md#image-or-other-file-resource).</span><span class="sxs-lookup"><span data-stu-id="6592e-130">Then you separate [GET requests to the image resources](onenote-get-content.md#image-or-other-file-resource).</span></span>


<span data-ttu-id="6592e-131">**Атрибуты изображения**</span><span class="sxs-lookup"><span data-stu-id="6592e-131">**Image attributes**</span></span> 

<span data-ttu-id="6592e-132">Элемент **img** при необходимости может включать атрибуты **alt**, **height** и **width**, а также атрибуты стиля **max-width** и **max-height**.</span><span class="sxs-lookup"><span data-stu-id="6592e-132">An **img** element can optionally include **alt**, **height**, and **width** attributes, and the style attributes **max-width** and **max-height**.</span></span>

<span data-ttu-id="6592e-133">**Типы мультимедиа для изображений**</span><span class="sxs-lookup"><span data-stu-id="6592e-133">**Image media types**</span></span>

<span data-ttu-id="6592e-134">Microsoft Graph поддерживает типы изображений TIFF, PNG, GIF, JPEG и BMP.</span><span class="sxs-lookup"><span data-stu-id="6592e-134">Microsoft Graph supports TIFF, PNG, GIF, JPEG, and BMP image types.</span></span> <span data-ttu-id="6592e-135">Чтобы сохранить изображение другого формата, которое желательно не преобразовывать, [отправьте двоичные данные](#add-an-image-using-binary-data) в составном запросе.</span><span class="sxs-lookup"><span data-stu-id="6592e-135">To capture an image that uses a different format that you don't want to convert, [send the binary data](#add-an-image-using-binary-data) in a multipart request.</span></span> <span data-ttu-id="6592e-136">Использовать Base64 или другую кодировку для двоичных данных не нужно.</span><span class="sxs-lookup"><span data-stu-id="6592e-136">You don't need to use Base64 or otherwise encode the binary data that you send.</span></span>

> <span data-ttu-id="6592e-137">**Примечание.** API обнаруживает исходный тип входного изображения и возвращает его в виде атрибута **data-fullres-src-type** [выходного HTML-кода](onenote_input_output_html.md#output-html).</span><span class="sxs-lookup"><span data-stu-id="6592e-137">**Note:** The OneNote APIs automatically detect the input image type, and returns it as the **data-fullres-src-type** in the output HTML.</span></span> <span data-ttu-id="6592e-138">API также возвращает тип оптимизированного изображения в атрибуте **data-src-type**.</span><span class="sxs-lookup"><span data-stu-id="6592e-138">The API also returns the image type of the optimized image in **data-src-type**.</span></span>
 
<span data-ttu-id="6592e-139">Ознакомьтесь с [ограничениями](#size-limitations-for-post-pages-requests) на создание страниц, содержащих файлы мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="6592e-139">See [limitations](#size-limitations-for-post-pages-requests) that apply when creating pages that contain media.</span></span>


<a name="image-img-url-src"></a>
### <a name="add-a-public-image-from-the-web"></a><span data-ttu-id="6592e-140">Добавление общедоступного изображения из Интернета</span><span class="sxs-lookup"><span data-stu-id="6592e-140">Add a public image from the web</span></span>

<span data-ttu-id="6592e-141">Во входных данных HTML запроса добавьте параметр `<img src="http://..." />` и укажите URL-адрес общедоступного изображения в атрибуте **src**.</span><span class="sxs-lookup"><span data-stu-id="6592e-141">In the input HTML of your request, include  `<img src="http://..." />` and specify the URL of a publicly accessible image for the **src** attribute.</span></span>

```
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
    <img src="http://..." width="300"/>
  </body>
</html>

--MyAppPartBoundary--  
```

<a name="image-img-binary-src"></a>
### <a name="add-an-image-using-binary-data"></a><span data-ttu-id="6592e-142">Добавление изображения с помощью двоичных данных</span><span class="sxs-lookup"><span data-stu-id="6592e-142">Add an image using binary data</span></span>

<span data-ttu-id="6592e-143">Во входных данных HTML в части **Presentation** запроса добавьте параметр `<img src="name:part-name" />`, где *part-name* — это уникальный идентификатор той части [составного запроса](onenote-create-page.md#example-request), которая содержит двоичные данные изображения.</span><span class="sxs-lookup"><span data-stu-id="6592e-143">In the input HTML of your request's **Presentation** part, include  `<img src="name:part-name" />`, where *part-name* is the unique identifier for the data part in your [multipart request](onenote-create-page.md#example-request) that contains the binary image data.</span></span> <span data-ttu-id="6592e-144">Просто отправьте двоичные данные, не используя Base64 или другую кодировку.</span><span class="sxs-lookup"><span data-stu-id="6592e-144">The image data is the binary file data; don't use Base64 or otherwise encode it.</span></span>

```
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
### <a name="add-a-webpage-snapshot"></a><span data-ttu-id="6592e-145">Добавление моментального снимка веб-страницы</span><span class="sxs-lookup"><span data-stu-id="6592e-145">Add a webpage snapshot</span></span>

<span data-ttu-id="6592e-146">С помощью Microsoft Graph можно создавать моментальные снимки целых веб-страниц и вставлять их в новые страницы.</span><span class="sxs-lookup"><span data-stu-id="6592e-146">You can use Microsoft Graph to snapshot entire webpages and insert them into new pages.</span></span> <span data-ttu-id="6592e-147">Этот способ полезен для архивации веб-страниц или сохранения сложных веб-страниц, которые содержат функции, не поддерживаемые приложением OneNote (например, CSS).</span><span class="sxs-lookup"><span data-stu-id="6592e-147">This method is useful to archive webpages or capture complex webpages that have features that OneNote doesn't support (like some CSS).</span></span>  

<span data-ttu-id="6592e-148">Во входном HTML-коде запроса добавьте параметр `<img src="http://..." />` и укажите URL-адрес нужной веб-страницы в атрибуте **src**.</span><span class="sxs-lookup"><span data-stu-id="6592e-148">In the input HTML of your request, include  `<img src="http://..." />` and specify the URL of the webpage you want to insert for the **src** attribute.</span></span>

```
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
    <img data-render-src="http://www.onenote.com" width="200"/>
  </body>
</html>

--MyAppPartBoundary--  
```


<a name="image-img-binary-data-render-src"></a>
### <a name="add-an-image-rendered-from-html"></a><span data-ttu-id="6592e-149">Добавление изображения, созданного из HTML-кода</span><span class="sxs-lookup"><span data-stu-id="6592e-149">Add an image rendered from HTML</span></span>
<span data-ttu-id="6592e-150">При передаче HTML-кода в виде блока данных убедитесь в отсутствии активного содержимого, для которого могут потребоваться учетные данные пользователя или предварительно загруженный подключаемый модуль браузера.</span><span class="sxs-lookup"><span data-stu-id="6592e-150">When you pass the HTML as a data-block, be sure there is no active content that would require user credentials, or a pre-loaded browser plug-in.</span></span> <span data-ttu-id="6592e-151">Подсистема, которую Microsoft Graph использует для преобразования HTML-страницы в изображение, не может выполнить вход за пользователя и не включает такие подключаемые модули, как Adobe Flash, Apple QuickTime и т. д.</span><span class="sxs-lookup"><span data-stu-id="6592e-151">The engine that Microsoft Graph uses to render the HTML page into an image has no ability to log in a user, and doesn't include plug-ins like Adobe Flash, Apple QuickTime, and so-on.</span></span> <span data-ttu-id="6592e-152">Это также означает, что динамически загружаемое содержимое (например, через скрипт AJAX) не будет отображаться, если для получения данных необходимы учетные данные пользователя или файлы cookie.</span><span class="sxs-lookup"><span data-stu-id="6592e-152">That also means that dynamically-loaded content, like might come with an AJAX script, won't appear if getting the data requires user login credentials or cookies.</span></span>

<span data-ttu-id="6592e-153">Во входных данных HTML в части **Presentation** запроса добавьте параметр `<img data-render-src="name:part-name" />`, где *part-name* — это уникальный идентификатор той части [составного запроса](onenote-create-page.md#example-request), которая содержит HTML-код.</span><span class="sxs-lookup"><span data-stu-id="6592e-153">In the input HTML of your request's **Presentation** part, include  `<img data-render-src="name:part-name" />`, where *part-name* is the unique identifier for the data part in your [multipart request](onenote-create-page.md#example-request) that contains the HTML.</span></span>

```
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
<img src="http://cdn.onenote.net/1664161560_Images/OneNote.ico" />
</body>
</html>

--MyAppPartBoundary--  
```


<a name="image-object"></a>
### <a name="add-an-image-file-as-an-attachment"></a><span data-ttu-id="6592e-154">Добавление файла изображения в качестве вложения</span><span class="sxs-lookup"><span data-stu-id="6592e-154">Add an image file as an attachment</span></span>

<span data-ttu-id="6592e-155">Во входных данных HTML в части **Presentation** запроса добавьте параметр `<object data="name:part-name" data-attachment="file-name.file-ext" type="media-type/media-subtype" />`, где *part-name* — это уникальный идентификатор той части [составного запроса](onenote-create-page.md#example-request), которая содержит двоичные данные изображения.</span><span class="sxs-lookup"><span data-stu-id="6592e-155">In the input HTML of your request's **Presentation** part, include  `<object data="name:part-name" data-attachment="file-name.file-ext" type="media-type/media-subtype" />`, where *part-name* is the unique identifier for the data part in your [multipart request](onenote-create-page.md#example-request) that contains the binary image data.</span></span> <span data-ttu-id="6592e-156">Просто отправьте двоичные данные, не используя Base64 или другую кодировку.</span><span class="sxs-lookup"><span data-stu-id="6592e-156">The image data is the binary file data; don't use Base64 or otherwise encode it.</span></span>

```
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

<span data-ttu-id="6592e-157">Узнайте больше о [типах файлов мультимедиа](#file-media-types).</span><span class="sxs-lookup"><span data-stu-id="6592e-157">Learn more about [file media types](#file-media-types).</span></span>



<a name="videos"></a>
## <a name="adding-videos"></a><span data-ttu-id="6592e-158">Добавление видео</span><span class="sxs-lookup"><span data-stu-id="6592e-158">Adding videos</span></span>

<span data-ttu-id="6592e-159">Вы можете внедрять видео в страницы OneNote с помощью команды `<iframe data-original-src="http://..." />` во входном HTML-коде.</span><span class="sxs-lookup"><span data-stu-id="6592e-159">You can embed videos in OneNote pages using `<iframe data-original-src="http://..." />` in the input HTML.</span></span> 

<span data-ttu-id="6592e-160">**Поддерживаемые сайты с видео**</span><span class="sxs-lookup"><span data-stu-id="6592e-160">**Supported video sites**</span></span>

- <span data-ttu-id="6592e-161">Dailymotion</span><span class="sxs-lookup"><span data-stu-id="6592e-161">Dailymotion</span></span>
- <span data-ttu-id="6592e-162">Office Mix</span><span class="sxs-lookup"><span data-stu-id="6592e-162">Office Mix</span></span>
- <span data-ttu-id="6592e-163">Sway</span><span class="sxs-lookup"><span data-stu-id="6592e-163">Sway</span></span>
- <span data-ttu-id="6592e-164">Sketchfab</span><span class="sxs-lookup"><span data-stu-id="6592e-164">Sketchfab</span></span>
- <span data-ttu-id="6592e-165">TED</span><span class="sxs-lookup"><span data-stu-id="6592e-165">TED</span></span>
- <span data-ttu-id="6592e-166">YouTube</span><span class="sxs-lookup"><span data-stu-id="6592e-166">YouTube</span></span>
- <span data-ttu-id="6592e-167">Vimeo</span><span class="sxs-lookup"><span data-stu-id="6592e-167">Vimeo</span></span>
- <span data-ttu-id="6592e-168">Vine</span><span class="sxs-lookup"><span data-stu-id="6592e-168">Vine</span></span>

<span data-ttu-id="6592e-169">**Атрибуты iframe**</span><span class="sxs-lookup"><span data-stu-id="6592e-169">**iframe attributes**</span></span>

<span data-ttu-id="6592e-170">**data-original-src**</span><span class="sxs-lookup"><span data-stu-id="6592e-170">**data-original-src**</span></span></p>
<span data-ttu-id="6592e-171">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6592e-171">Required.</span></span> <span data-ttu-id="6592e-172">URL-адрес видео.</span><span class="sxs-lookup"><span data-stu-id="6592e-172">The URL of the video source.</span></span><br /><span data-ttu-id="6592e-173">Пример: `data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8"`</span><span class="sxs-lookup"><span data-stu-id="6592e-173">Example: `data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8"`</span></span></p>
<span data-ttu-id="6592e-174">**width**</span><span class="sxs-lookup"><span data-stu-id="6592e-174">**width**</span></span></p>
<span data-ttu-id="6592e-175">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="6592e-175">Optional.</span></span> <span data-ttu-id="6592e-176">Ширина элемента iframe, содержащего видео.</span><span class="sxs-lookup"><span data-stu-id="6592e-176">The width of the iframe that contains the video.</span></span> <span data-ttu-id="6592e-177">Значение по умолчанию: 480.</span><span class="sxs-lookup"><span data-stu-id="6592e-177">Default is 480.</span></span><br /><span data-ttu-id="6592e-178">Пример: `width="300"`</span><span class="sxs-lookup"><span data-stu-id="6592e-178">Example: `width="300"`</span></span></p>
<span data-ttu-id="6592e-179">**height**</span><span class="sxs-lookup"><span data-stu-id="6592e-179">**height**</span></span></p>
<span data-ttu-id="6592e-180">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="6592e-180">Optional.</span></span> <span data-ttu-id="6592e-181">Высота элемента iframe, содержащего видео.</span><span class="sxs-lookup"><span data-stu-id="6592e-181">The height of the iframe that contains the video.</span></span> <span data-ttu-id="6592e-182">Значение по умолчанию: 360.</span><span class="sxs-lookup"><span data-stu-id="6592e-182">Default is 360.</span></span><br /><span data-ttu-id="6592e-183">Пример: `height="300"`</span><span class="sxs-lookup"><span data-stu-id="6592e-183">Example: `height="300"`</span></span></p>

<span data-ttu-id="6592e-184">**Пример**</span><span class="sxs-lookup"><span data-stu-id="6592e-184">**Example**</span></span>

<span data-ttu-id="6592e-185">Во входном HTML-коде запроса добавьте параметр `<iframe data-original-src="http://..." />` и укажите URL-адрес видео в атрибуте **data-original-src**.</span><span class="sxs-lookup"><span data-stu-id="6592e-185">In the input HTML of your request, include `<iframe data-original-src="http://..." />` and specify the URL of the video for the **data-original-src** attribute.</span></span>

```
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


<a name="files"></a>
## <a name="adding-files"></a><span data-ttu-id="6592e-186">Добавление файлов</span><span class="sxs-lookup"><span data-stu-id="6592e-186">Adding installation files</span></span>

<span data-ttu-id="6592e-187">Вы можете добавлять вложенные файлы в страницы OneNote с помощью элемента **object** во входном HTML-коде.</span><span class="sxs-lookup"><span data-stu-id="6592e-187">You can add file attachments to OneNote pages using an **object** element in the input HTML.</span></span> <span data-ttu-id="6592e-188">Если вам нужно добавить PDF-файл, вы можете использовать элемент **img** для отрисовки страниц PDF-файла в виде изображений.</span><span class="sxs-lookup"><span data-stu-id="6592e-188">If you're adding a PDF file, you can use an **img** element to render the PDF pages as images.</span></span> 

[<span data-ttu-id="6592e-189">Добавление вложенного файла</span><span class="sxs-lookup"><span data-stu-id="6592e-189">Add a file attachment</span></span>](#add-a-file-attachment)</p>
<span data-ttu-id="6592e-190">Используйте элемент `<object .../>` и отправьте файл в части данных составного запроса.</span><span class="sxs-lookup"><span data-stu-id="6592e-190">Use `<object .../>` and send the file in a data part of a multipart request.</span></span> <span data-ttu-id="6592e-191">Добавляет вложенный файл и отображает значок файла на странице OneNote.</span><span class="sxs-lookup"><span data-stu-id="6592e-191">Adds a file attachment that displays a file icon on the OneNote page.</span></span></p>
[<span data-ttu-id="6592e-192">Добавление изображений содержимого PDF-файлов</span><span class="sxs-lookup"><span data-stu-id="6592e-192">Add images of PDF file contents</span></span>](#add-images-of-pdf-file-contents)</p>
<span data-ttu-id="6592e-193">Используйте элемент `<img data-render-src="name:part-name" />` и отправьте PDF-файл в части данных составного запроса.</span><span class="sxs-lookup"><span data-stu-id="6592e-193">Use `<img data-render-src="name:part-name" />` and send a PDF file in the data part of a multipart request.</span></span> <span data-ttu-id="6592e-194">Отрисовывает каждую PDF-страницу в виде отдельного изображения на странице OneNote.</span><span class="sxs-lookup"><span data-stu-id="6592e-194">Renders each PDF page as a separate image on the OneNote page.</span></span></p>

<span data-ttu-id="6592e-195">**Атрибуты файлов**</span><span class="sxs-lookup"><span data-stu-id="6592e-195">**File attributes**</span></span>

<span data-ttu-id="6592e-196">Ниже перечислены обязательные атрибуты элемента **object**.</span><span class="sxs-lookup"><span data-stu-id="6592e-196">The **object** element requires the following attributes.</span></span>

<span data-ttu-id="6592e-197">**data-attachment**</span><span class="sxs-lookup"><span data-stu-id="6592e-197">**data-attachment**</span></span></p>
<span data-ttu-id="6592e-198">Имя и расширения файла, который нужно отобразить на странице OneNote.</span><span class="sxs-lookup"><span data-stu-id="6592e-198">The file name and extension to display on the OneNote page.</span></span><br /><span data-ttu-id="6592e-199">Пример: `data-attachment="filename.docx"`</span><span class="sxs-lookup"><span data-stu-id="6592e-199">Example: `data-attachment="filename.docx"`</span></span></p>
<span data-ttu-id="6592e-200">**data**</span><span class="sxs-lookup"><span data-stu-id="6592e-200">**Data**</span></span></p>
<span data-ttu-id="6592e-201">Имя части body в составном запросе, содержащем двоичные данные файла.</span><span class="sxs-lookup"><span data-stu-id="6592e-201">The name of the body part in the multipart request that contains the binary file data.</span></span> <span data-ttu-id="6592e-202">Microsoft Graph не поддерживает передачу URL-адресов через этот атрибут.</span><span class="sxs-lookup"><span data-stu-id="6592e-202">Microsoft Graph does not support passing a URL reference here.</span></span><br /><span data-ttu-id="6592e-203">Пример: `data="name:part-name"`</span><span class="sxs-lookup"><span data-stu-id="6592e-203">Example: `data="name:part-name"`</span></span></p>
<span data-ttu-id="6592e-204">**type**</span><span class="sxs-lookup"><span data-stu-id="6592e-204">**type**</span></span></p>
<span data-ttu-id="6592e-205">MIME-тип файла, который используется для определения значка файла для страницы и приложения, запускаемого, когда пользователь активирует файл на устройстве из OneNote.</span><span class="sxs-lookup"><span data-stu-id="6592e-205">type="standardMimeType" indicates the file MIME type. This is used to select the file icon on the page, and also determines which application starts when the user activates the file on the device from OneNote.</span></span><br /><span data-ttu-id="6592e-206">Пример: `type="application/pdf"`</span><span class="sxs-lookup"><span data-stu-id="6592e-206">Example: `type="application/pdf"`</span></span></p>


<a name="file-media-types"></a>

### <a name="file-media-types"></a><span data-ttu-id="6592e-207">MIME-типы файлов</span><span class="sxs-lookup"><span data-stu-id="6592e-207">File media types</span></span>  
<span data-ttu-id="6592e-208">Microsoft Graph использует предопределенный значок для типа вложенного файла или универсальный значок, если API не распознает тип файла.</span><span class="sxs-lookup"><span data-stu-id="6592e-208">Microsoft Graph uses predefined file-types icon for attached files, or a generic icon when the API doesn't recognize the file type.</span></span> <span data-ttu-id="6592e-209">В приведенной ниже таблице показаны распространенные типы файлов, которые распознает этот API.</span><span class="sxs-lookup"><span data-stu-id="6592e-209">The following table shows some common file types that are recognized by the API.</span></span>

- <span data-ttu-id="6592e-210">application/pdf</span><span class="sxs-lookup"><span data-stu-id="6592e-210">application/pdf</span></span>  
- <span data-ttu-id="6592e-211">application/vnd.openxmlformats-officedocument.wordprocessingml.document</span><span class="sxs-lookup"><span data-stu-id="6592e-211">application/vnd.openxmlformats-officedocument.wordprocessingml.document</span></span>  
- <span data-ttu-id="6592e-212">application/vnd.openxmlformats-officedocument.presentationml.presentation</span><span class="sxs-lookup"><span data-stu-id="6592e-212">application/vnd.openxmlformats-officedocument.presentationml.presentation</span></span>
- <span data-ttu-id="6592e-213">application/vnd.openxmlformats-officedocument.spreadsheetml.sheet</span><span class="sxs-lookup"><span data-stu-id="6592e-213">application/vnd.openxmlformats-officedocument.spreadsheetml.sheet</span></span>
- <span data-ttu-id="6592e-214">image/png</span><span class="sxs-lookup"><span data-stu-id="6592e-214">image/png</span></span>
- <span data-ttu-id="6592e-215">image/jpeg</span><span class="sxs-lookup"><span data-stu-id="6592e-215">image/jpeg</span></span>
- <span data-ttu-id="6592e-216">image/gif</span><span class="sxs-lookup"><span data-stu-id="6592e-216">image/gif</span></span>
- <span data-ttu-id="6592e-217">audio/wav</span><span class="sxs-lookup"><span data-stu-id="6592e-217">audio/wav</span></span>
- <span data-ttu-id="6592e-218">video/mp4</span><span class="sxs-lookup"><span data-stu-id="6592e-218">video/mp4</span></span>
- <span data-ttu-id="6592e-219">application/msword</span><span class="sxs-lookup"><span data-stu-id="6592e-219">application/msword</span></span>
- <span data-ttu-id="6592e-220">application/mspowerpoint</span><span class="sxs-lookup"><span data-stu-id="6592e-220">application/mspowerpoint</span></span>
- <span data-ttu-id="6592e-221">application/excel</span><span class="sxs-lookup"><span data-stu-id="6592e-221">application/excel</span></span>

<span data-ttu-id="6592e-222">Ознакомьтесь с [ограничениями](#size-limitations-for-post-pages-requests) на создание страниц, содержащих файлы мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="6592e-222">See [limitations](#size-limitations-for-post-pages-requests) that apply when creating pages that contain media.</span></span>


<a name="file-object"></a>
### <a name="add-a-file-attachment"></a><span data-ttu-id="6592e-223">Добавление вложенного файла</span><span class="sxs-lookup"><span data-stu-id="6592e-223">Add a file attachment</span></span>

<span data-ttu-id="6592e-224">Во входных данных HTML в части **Presentation** запроса добавьте параметр `<object data="name:part-name" data-attachment="file-name.file-ext" type="media-type/media-subtype" />`, где *part-name* — это уникальный идентификатор той части [составного запроса](onenote-create-page.md#example-request), которая содержит двоичные данные файла.</span><span class="sxs-lookup"><span data-stu-id="6592e-224">In the input HTML of your request's **Presentation** part, include  `<object data="name:part-name" data-attachment="file-name.file-ext" type="media-type/media-subtype" />`, where *part-name* is the unique identifier for the data part in your [multipart request](onenote-create-page.md#example-request) that contains the binary file data.</span></span> <span data-ttu-id="6592e-225">Просто отправьте двоичные данные, не используя Base64 или другую кодировку.</span><span class="sxs-lookup"><span data-stu-id="6592e-225">The image data is the binary file data; don't use Base64 or otherwise encode it.</span></span>

```
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
### <a name="add-images-of-pdf-file-contents"></a><span data-ttu-id="6592e-226">Добавление изображений содержимого PDF-файлов</span><span class="sxs-lookup"><span data-stu-id="6592e-226">Add images of PDF file contents</span></span>

<span data-ttu-id="6592e-227">Во входных данных HTML в части **Presentation** запроса добавьте параметр `<img data-render-src="name:part-name" ... />`, где *part-name* — это уникальный идентификатор той части [составного запроса](onenote-create-page.md#example-request), которая содержит двоичные данные файла.</span><span class="sxs-lookup"><span data-stu-id="6592e-227">In the input HTML of your request's **Presentation** part, include  `<img data-render-src="name:part-name" ... />`, where *part-name* is the unique identifier for the data part in your [multipart request](onenote-create-page.md#example-request) that contains the binary file data.</span></span> <span data-ttu-id="6592e-228">Просто отправьте двоичные данные, не используя Base64 или другую кодировку.</span><span class="sxs-lookup"><span data-stu-id="6592e-228">The image data is the binary file data; don't use Base64 or otherwise encode it.</span></span>

```
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
## <a name="size-limitations-for-post-pages-requests"></a><span data-ttu-id="6592e-229">Ограничения на размер запросов POST для страниц</span><span class="sxs-lookup"><span data-stu-id="6592e-229">Size limitations for POST pages requests</span></span>

<span data-ttu-id="6592e-230">При отправке изображений и файлов учитывайте следующие ограничения: <!--TODO: check these--></span><span class="sxs-lookup"><span data-stu-id="6592e-230">When sending image and file data, be aware of these limitations: <!--TODO: check these--></span></span>

- <span data-ttu-id="6592e-231">Общий максимальный размер данных в запросе POST (включая изображения, файлы и другие данные) составляет приблизительно 70 МБ.</span><span class="sxs-lookup"><span data-stu-id="6592e-231">The total POST size limit is ~70 MB, including images, files, and other data.</span></span> <span data-ttu-id="6592e-232">Фактическое ограничение зависит от кодировки в нижестоящих системах, поэтому не существует фиксированного ограничения в байтах.</span><span class="sxs-lookup"><span data-stu-id="6592e-232">The actual limit is affected by downstream encoding, so there's no fixed byte-count limit.</span></span> <span data-ttu-id="6592e-233">Запросы, превышающие это ограничение, могут возвращать ненадежные результаты.</span><span class="sxs-lookup"><span data-stu-id="6592e-233">Requests that exceed the limit may produce unreliable results.</span></span>

- <span data-ttu-id="6592e-234">Ограничение для каждой части данных (включая заголовки) составляет 25 МБ.</span><span class="sxs-lookup"><span data-stu-id="6592e-234">The limit for each data part is 25 MB, including the part headers.</span></span> <span data-ttu-id="6592e-235">Microsoft Graph отклоняет части данных, превышающие это ограничение.</span><span class="sxs-lookup"><span data-stu-id="6592e-235">Data parts that exceed the limit are rejected by Microsoft Graph.</span></span> 

- <span data-ttu-id="6592e-236">Максимальное количество изображений на странице составляет 150.</span><span class="sxs-lookup"><span data-stu-id="6592e-236">The maximum number of images per page is 150.</span></span> <span data-ttu-id="6592e-237">При использовании атрибута `src="http://..."` API игнорирует теги **img** после достижения этого предела.</span><span class="sxs-lookup"><span data-stu-id="6592e-237">Image limit is 150 per page. When using the **src="internetURL"`src="http://..."` attribute, the API ignores <img>** tags beyond the limit.</span></span>

- <span data-ttu-id="6592e-238">Каждый запрос POST может включать до 6 частей данных, включая обязательную часть **Presentation**.</span><span class="sxs-lookup"><span data-stu-id="6592e-238">The maximum number of data parts is 6 per POST, including the required **Presentation** part.</span></span>

- <span data-ttu-id="6592e-239">Каждый запрос может содержать до пяти элементов **img** с атрибутом **data-render-src** и один элемент **object** с атрибутом **data-render-src**. Остальные ссылки на изображения и файлы игнорируются.</span><span class="sxs-lookup"><span data-stu-id="6592e-239">Each request can contain up to five **img** elements that use **data-render-src** and one **object** elements that uses **data-render-src**. Additional image and file references are ignored.</span></span>

- <span data-ttu-id="6592e-240">Один запрос POST может включать до 30 изображений, независимо от того, какой метод используется для их отправки в API.</span><span class="sxs-lookup"><span data-stu-id="6592e-240">The maximum number of images in a single POST is 30, no matter which method you use to send them to the API.</span></span> <span data-ttu-id="6592e-241">Остальные изображения игнорируются.</span><span class="sxs-lookup"><span data-stu-id="6592e-241">Additional images are ignored.</span></span> <span data-ttu-id="6592e-242">Если вам нужно сохранить веб-страницу с большим количеством изображений, рекомендуем [сохранить ее в виде моментального снимка](#add-a-webpage-snapshot).</span><span class="sxs-lookup"><span data-stu-id="6592e-242">If you want to capture a webpage that contains a lot of images, consider [capturing the whole page as a snapshot](#add-a-webpage-snapshot).</span></span>


## <a name="when-to-use-html-versus-data-render-src"></a><span data-ttu-id="6592e-243">Когда использовать HTML, а когда — *data-render-src*</span><span class="sxs-lookup"><span data-stu-id="6592e-243">When to use HTML versus *data-render-src*</span></span> 
<span data-ttu-id="6592e-244">Если вы выбираете между вставкой HTML на страницу OneNote и использованием атрибута **data-render-src**, учитывайте следующее:</span><span class="sxs-lookup"><span data-stu-id="6592e-244">When trying to decide between directly putting HTML onto the OneNote page, versus using the data-render-src rendering, consider the following:</span></span>

- <span data-ttu-id="6592e-245">Сложный HTML, вероятно, лучше отправлять в механизм визуализации с помощью **data-render-src**, а не пытаться изменить HTML так, чтобы его принял Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="6592e-245">Complex HTML is probably best sent to the rendering engine via data-render-src, rather than attempting to modify the HTML to fit into what the oncshort API can accept. This is also true when your HTML includes tags not yet supported (see ).</span></span> <span data-ttu-id="6592e-246">Это также относится к тем случаям, когда HTML-код включает неподдерживаемые теги.</span><span class="sxs-lookup"><span data-stu-id="6592e-246">This is also true when your HTML includes tags that aren't supported supported.</span></span>

- <span data-ttu-id="6592e-247">Как правило, точную отрисовку страниц для сохранения макета и внешнего вида страницы лучше обеспечивает механизм визуализации с использованием атрибута **data-render-src**.</span><span class="sxs-lookup"><span data-stu-id="6592e-247">Accurate page rendering to preserve the layout and look of the page is probably best done with the rendering engine via **data-render-src**.</span></span>

- <span data-ttu-id="6592e-248">Чтобы текст был доступен для непосредственного редактирования, обычно лучше вставлять HTML-код непосредственно на страницу.</span><span class="sxs-lookup"><span data-stu-id="6592e-248">Directly-editable text is often best done with inserting the HTML directly onto the page. The rendered images are scanned by an optical character recognition (OCR) system, but it's just not the same.</span></span> <span data-ttu-id="6592e-249">Отрисованные изображения сканирует система оптического распознавания символов (OCR), но результаты могут отличаться.</span><span class="sxs-lookup"><span data-stu-id="6592e-249">Directly-editable text is often best done with inserting the HTML directly onto the page. The rendered images are scanned by an optical character recognition (OCR) system, but it's just not the same.</span></span>

- <span data-ttu-id="6592e-250">Моментальный снимок для журнала или архива лучше всего создавать с помощью метода data-render-src.</span><span class="sxs-lookup"><span data-stu-id="6592e-250">Snapshot-in-time for historical or archival purposes is usually best done with the data-render-src method.</span></span>

- <span data-ttu-id="6592e-251">Разметка дизайна веб-страницы для централизованного исправления — по-настоящему сильная сторона атрибута **data-render-src**.</span><span class="sxs-lookup"><span data-stu-id="6592e-251">Marking-up a web page design for revisions is one place the **data-render-src** truly shines.</span></span> <span data-ttu-id="6592e-252">С помощью возможностей рукописного ввода OneNote вы можете рисовать на изображении, чтобы обозначать изменения или выделять важные части.</span><span class="sxs-lookup"><span data-stu-id="6592e-252">Using OneNote's inking capabilities, you can draw on the image to indicate changes or call out important areas.</span></span> <span data-ttu-id="6592e-253">Сохранение веб-страницы в виде изображения значительно упрощает эту задачу.</span><span class="sxs-lookup"><span data-stu-id="6592e-253">Having the web page as an image makes that a lot easier.</span></span>

- <span data-ttu-id="6592e-254">Очень крупные изображения или изображения в форматах, которые OneNote не принимает напрямую, иногда легче преобразовать в эскизы и другие форматы с помощью атрибута **data-render-src**, а не собственного кода.</span><span class="sxs-lookup"><span data-stu-id="6592e-254">Very large images, or images in formats that OneNote doesn't directly accept can sometimes be thumbnailed and converted with the data-render-src method more easily than by doing it in your own code.</span></span> <span data-ttu-id="6592e-255">Даже если изображение также доступно в сети, внедрение данных в запрос POST иногда позволяет быстрее сделать сохраненную страницу доступной пользователю OneNote за счет уменьшения общего количества циклов, необходимых для создания страницы OneNote.</span><span class="sxs-lookup"><span data-stu-id="6592e-255">You can also send the image data for up to 150 images directly inside the oncshort API POST. This is common when the images are from a mobile device camera, or if your app is running on a hardware device like a scanner or camera. Even if the image is also available on the Internet, embedding the data in your POST can sometimes make the captured page available to OneNote user sooner, by reducing the total number of round-trips needed to build the OneNote page.</span></span>

<span data-ttu-id="6592e-256">Иногда лучший способ определить, какой метод лучше подойдет пользователям — опробовать оба варианта во время разработки приложения.</span><span class="sxs-lookup"><span data-stu-id="6592e-256">Sometimes, the best way to determine which method will work best for your users is to try it both ways as you develop your app.</span></span>


<a name="permissions"></a>
## <a name="permissions"></a><span data-ttu-id="6592e-257">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6592e-257">Permissions</span></span>

<span data-ttu-id="6592e-258">Для создания и обновления страниц OneNote необходимо запрашивать соответствующие разрешения.</span><span class="sxs-lookup"><span data-stu-id="6592e-258">To create or update OneNote pages, you'll need to request appropriate permissions.</span></span> <span data-ttu-id="6592e-259">Выберите минимальный уровень, необходимый для работы вашего приложения.</span><span class="sxs-lookup"><span data-stu-id="6592e-259">Choose the lowest level that your app needs to do its work.</span></span>

<span data-ttu-id="6592e-260">**Разрешения для _запросов POST со страницами_**</span><span class="sxs-lookup"><span data-stu-id="6592e-260">**Permissions for _POST pages_**</span></span>

- <span data-ttu-id="6592e-261">Notes.Create</span><span class="sxs-lookup"><span data-stu-id="6592e-261">Notes.Create</span></span>
- <span data-ttu-id="6592e-262">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6592e-262">Notes.ReadWrite</span></span>
- <span data-ttu-id="6592e-263">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6592e-263">Notes.ReadWrite.All</span></span> 

<span data-ttu-id="6592e-264">**Разрешения для _запросов PATCH со страницами_**</span><span class="sxs-lookup"><span data-stu-id="6592e-264">**Permissions for _PATCH pages_**</span></span>

- <span data-ttu-id="6592e-265">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6592e-265">Notes.ReadWrite</span></span>
- <span data-ttu-id="6592e-266">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6592e-266">Notes.ReadWrite.All</span></span>

<span data-ttu-id="6592e-267">Дополнительную информацию о разрешениях и принципе их работы см. в разделе [Разрешения OneNote](permissions_reference.md#notes-permissions).</span><span class="sxs-lookup"><span data-stu-id="6592e-267">For more information about how permission scopes work, see [OneNote permission scopes](permissions_reference.md#notes-permissions).</span></span>


<a name="see-also"></a>
## <a name="additional-resources"></a><span data-ttu-id="6592e-268">Дополнительные ресурсы</span><span class="sxs-lookup"><span data-stu-id="6592e-268">Additional resources</span></span>

- [<span data-ttu-id="6592e-269">Интеграция с OneNote</span><span class="sxs-lookup"><span data-stu-id="6592e-269">Integrate with OneNote</span></span>](integrate_with_onenote.md)
- [<span data-ttu-id="6592e-270">Блог разработчиков OneNote</span><span class="sxs-lookup"><span data-stu-id="6592e-270">OneNote Developer Blog</span></span>](http://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="6592e-271">Вопросы о разработке OneNote на сайте Stack Overflow</span><span class="sxs-lookup"><span data-stu-id="6592e-271">OneNote development questions on Stack Overflow</span></span>](http://go.microsoft.com/fwlink/?LinkID=390182)
- [<span data-ttu-id="6592e-272">Репозитории GitHub OneNote</span><span class="sxs-lookup"><span data-stu-id="6592e-272">OneNote GitHub repos</span></span>](http://go.microsoft.com/fwlink/?LinkID=390178)  
