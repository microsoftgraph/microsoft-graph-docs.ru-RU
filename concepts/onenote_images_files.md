
# <a name="add-images-videos-and-files-to-onenote-pages"></a><span data-ttu-id="3602f-101">Добавление изображений, видео и файлов на страницы OneNote</span><span class="sxs-lookup"><span data-stu-id="3602f-101">Add images, videos, and files to OneNote pages</span></span>

<span data-ttu-id="3602f-102">**Область применения:** записные книжки клиентов в OneDrive и корпоративные записные книжки в Office 365.</span><span class="sxs-lookup"><span data-stu-id="3602f-102">**Applies to:** Consumer notebooks on OneDrive | Enterprise notebooks on Office 365</span></span>

<span data-ttu-id="3602f-103">С помощью элементов **img**, **object** и **iframe** вы можете добавлять изображения, видео и файлы на страницу OneNote при ее [создании](onenote-create-page.md) или [обновлении](onenote_update_page.md).</span><span class="sxs-lookup"><span data-stu-id="3602f-103">You can use **img**, **object**, and **iframe** elements to add images, videos, and files to a OneNote page when you're [creating](onenote-create-page.md) or [updating](onenote_update_page.md) the page.</span></span> 

- <span data-ttu-id="3602f-104">Элемент **img** используется для отрисовки изображения на странице.</span><span class="sxs-lookup"><span data-stu-id="3602f-104">Use **img** to render an image on the page.</span></span>
- <span data-ttu-id="3602f-105">Элемент **iframe** используется для внедрения видео в страницу.</span><span class="sxs-lookup"><span data-stu-id="3602f-105">Use **iframe** to embed a video on the page.</span></span>
- <span data-ttu-id="3602f-106">Элемент **object** используется для добавления вложенного файла на страницу.</span><span class="sxs-lookup"><span data-stu-id="3602f-106">Use **object** to add a file attachment to the page.</span></span>


<a name="images"></a>

## <a name="adding-images"></a><span data-ttu-id="3602f-107">Добавление изображений</span><span class="sxs-lookup"><span data-stu-id="3602f-107">Adding images</span></span>

<span data-ttu-id="3602f-108">Изображения можно добавлять по URL-адресу или путем отправки необработанных данных.</span><span class="sxs-lookup"><span data-stu-id="3602f-108">Images can be added by URL reference or by sending raw data.</span></span> <span data-ttu-id="3602f-109">Microsoft Graph поддерживает перечисленные ниже способы добавления изображений, логотипов и фотографий на страницы OneNote.</span><span class="sxs-lookup"><span data-stu-id="3602f-109">Microsoft Graph supports the following methods of adding images, logos, and photos to OneNote pages.</span></span> 

[<span data-ttu-id="3602f-110">Добавление общедоступного изображения из Интернета</span><span class="sxs-lookup"><span data-stu-id="3602f-110">Add a public image from the web</span></span>](#add-a-public-image-from-the-web)

<span data-ttu-id="3602f-111">Используйте элемент `img` с параметром `src="http://image-url"` и укажите URL-адрес общедоступного изображения.</span><span class="sxs-lookup"><span data-stu-id="3602f-111">Use `img` with `src="http://image-url"` and specify the URL of a publicly accessible image.</span></span> <span data-ttu-id="3602f-112">Отрисовывает изображение на странице OneNote.</span><span class="sxs-lookup"><span data-stu-id="3602f-112">Renders the image on the OneNote page.</span></span>

[<span data-ttu-id="3602f-113">Добавление изображения с помощью двоичных данных</span><span class="sxs-lookup"><span data-stu-id="3602f-113">Add an image using binary data</span></span>](#add-an-image-using-binary-data)

<span data-ttu-id="3602f-114">Используйте элемент `img` с параметром `src="name:image-block-name"` и отправьте файл изображения в части данных составного запроса.</span><span class="sxs-lookup"><span data-stu-id="3602f-114">Use `img` with `src="name:image-block-name"` and send the image file in a data part of a multipart request.</span></span> <span data-ttu-id="3602f-115">Отрисовывает изображение на странице OneNote.</span><span class="sxs-lookup"><span data-stu-id="3602f-115">Renders the image on the OneNote page.</span></span>

[<span data-ttu-id="3602f-116">Добавление моментального снимка веб-страницы</span><span class="sxs-lookup"><span data-stu-id="3602f-116">Add a webpage snapshot</span></span>](#add-a-webpage-snapshot)

<span data-ttu-id="3602f-117">Используйте элемент `img` с параметром `data-render-src="http://webpage-url"` и укажите URL-адрес веб-страницы.</span><span class="sxs-lookup"><span data-stu-id="3602f-117">Use `img` with `data-render-src="http://webpage-url"` and specify the URL of a webpage.</span></span> <span data-ttu-id="3602f-118">Отрисовывает моментальный снимок всей веб-страницы на странице OneNote.</span><span class="sxs-lookup"><span data-stu-id="3602f-118">Renders a snapshot of the whole webpage on the OneNote page.</span></span>

[<span data-ttu-id="3602f-119">Добавление изображения, созданного из HTML-кода</span><span class="sxs-lookup"><span data-stu-id="3602f-119">Add an image rendered from HTML</span></span>](#add-an-image-rendered-from-html)

<span data-ttu-id="3602f-120">Используйте элемент `img` с параметром `data-render-src="name:html-block-name"` и отправьте HTML-код в части данных составного запроса.</span><span class="sxs-lookup"><span data-stu-id="3602f-120">Use `img` with `data-render-src="name:html-block-name"` and send HTML in the data part of a multipart request.</span></span> <span data-ttu-id="3602f-121">Отрисовывает HTML в виде изображения на странице OneNote.</span><span class="sxs-lookup"><span data-stu-id="3602f-121">Renders the HTML as an image on the OneNote page.</span></span>

[<span data-ttu-id="3602f-122">Добавление изображений содержимого PDF-файлов</span><span class="sxs-lookup"><span data-stu-id="3602f-122">Add images of PDF file contents</span></span>](#add-images-of-pdf-file-contents)

<span data-ttu-id="3602f-123">Используйте элемент `<img data-render-src="name:part-name" />` и отправьте PDF-файл в части данных составного запроса.</span><span class="sxs-lookup"><span data-stu-id="3602f-123">Use `<img data-render-src="name:part-name" />` and send the PDF file in the data part of a multipart request.</span></span> <span data-ttu-id="3602f-124">Отрисовывает каждую PDF-страницу в виде отдельного изображения на странице OneNote.</span><span class="sxs-lookup"><span data-stu-id="3602f-124">Renders each PDF page as a separate image on the OneNote page.</span></span>

[<span data-ttu-id="3602f-125">Добавление файла изображения в качестве вложения</span><span class="sxs-lookup"><span data-stu-id="3602f-125">Add an image file as a file attachment</span></span>](#add-an-image-file-as-an-attachment)

<span data-ttu-id="3602f-126">Используйте элемент `object` с параметром `data="name:file-block-name" data-attachment="file-name.file-ext" type="media-type"` и отправьте файл изображения в части данных составного запроса.</span><span class="sxs-lookup"><span data-stu-id="3602f-126">Use `object` with `data="name:file-block-name" data-attachment="file-name.file-ext" type="media-type"` and send an image file in the data part of a multipart request.</span></span> <span data-ttu-id="3602f-127">Добавляет вложенный файл на страницу OneNote и отображает значок файла.</span><span class="sxs-lookup"><span data-stu-id="3602f-127">Adds a file attachment to the OneNote page and displays a file icon.</span></span>


> <span data-ttu-id="3602f-128">**Примечание.** Чтобы получить изображения со страницы OneNote, сначала отправьте [запрос GET на получение содержимого страницы](onenote-get-content.md#page-html-content).</span><span class="sxs-lookup"><span data-stu-id="3602f-128">**Note:** To get images on a OneNote page, first send a [GET request for the page content](onenote-get-content.md#page-html-content).</span></span> <span data-ttu-id="3602f-129">Будут возвращены URL-адреса ресурсов изображений на странице.</span><span class="sxs-lookup"><span data-stu-id="3602f-129">This returns the URLs to the image resources on the page.</span></span> <span data-ttu-id="3602f-130">Затем разделите [запросы GET на получение ресурсов изображений](onenote-get-content.md#image-or-other-file-resource).</span><span class="sxs-lookup"><span data-stu-id="3602f-130">Then you separate [GET requests to the image resources](onenote-get-content.md#image-or-other-file-resource).</span></span>


#### <a name="image-attributes"></a><span data-ttu-id="3602f-131">Атрибуты изображений</span><span class="sxs-lookup"><span data-stu-id="3602f-131">Image attributes</span></span> 

<span data-ttu-id="3602f-132">Элемент **img** при необходимости может включать атрибуты **alt**, **height** и **width**, а также атрибуты стиля **max-width** и **max-height**.</span><span class="sxs-lookup"><span data-stu-id="3602f-132">An **img** element can optionally include **alt**, **height**, and **width** attributes, and the style attributes **max-width** and **max-height**.</span></span>

#### <a name="image-media-types"></a><span data-ttu-id="3602f-133">Типы мультимедиа для изображений</span><span class="sxs-lookup"><span data-stu-id="3602f-133">Image media types</span></span>

<span data-ttu-id="3602f-134">Microsoft Graph поддерживает типы изображений TIFF, PNG, GIF, JPEG и BMP.</span><span class="sxs-lookup"><span data-stu-id="3602f-134">Microsoft Graph supports TIFF, PNG, GIF, JPEG, and BMP image types.</span></span> <span data-ttu-id="3602f-135">Чтобы сохранить изображение другого формата, которое желательно не преобразовывать, [отправьте двоичные данные](#add-an-image-using-binary-data) в составном запросе.</span><span class="sxs-lookup"><span data-stu-id="3602f-135">To capture an image that uses a different format that you don't want to convert, [send the binary data](#add-an-image-using-binary-data) in a multipart request.</span></span> <span data-ttu-id="3602f-136">Использовать Base64 или другую кодировку для двоичных данных не нужно.</span><span class="sxs-lookup"><span data-stu-id="3602f-136">You don't need to use Base64 or otherwise encode the binary data that you send.</span></span>

> <span data-ttu-id="3602f-137">**Примечание.** API обнаруживает исходный тип входного изображения и возвращает его в виде атрибута **data-fullres-src-type** [выходного HTML-кода](onenote_input_output_html.md#output-html).</span><span class="sxs-lookup"><span data-stu-id="3602f-137">**Note:** The API detects the original input image type, and returns it as the **data-fullres-src-type** attribute in the [output HTML](onenote_input_output_html.md#output-html).</span></span> <span data-ttu-id="3602f-138">API также возвращает тип оптимизированного изображения в атрибуте **data-src-type**.</span><span class="sxs-lookup"><span data-stu-id="3602f-138">The API also returns the image type of the optimized image in **data-src-type**.</span></span>
 
<span data-ttu-id="3602f-139">Ознакомьтесь с [ограничениями](#size-limitations-for-post-pages-requests) на создание страниц, содержащих файлы мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="3602f-139">See [limitations](#size-limitations-for-post-pages-requests) that apply when creating pages that contain media.</span></span>


<a name="image-img-url-src"></a>

### <a name="add-a-public-image-from-the-web"></a><span data-ttu-id="3602f-140">Добавление общедоступного изображения из Интернета</span><span class="sxs-lookup"><span data-stu-id="3602f-140">Add a public image from the web</span></span>

<span data-ttu-id="3602f-141">Во входные данные HTML-кода запроса включите параметр `<img src="http://..." />` и укажите URL-адрес общедоступного изображения в атрибуте **src**.</span><span class="sxs-lookup"><span data-stu-id="3602f-141">In the input HTML of your request, include  `<img src="http://..." />` and specify the URL of a publicly accessible image for the **src** attribute.</span></span>

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
    <img src="http://..." width="300"/>
  </body>
</html>

--MyAppPartBoundary--  
```

<a name="image-img-binary-src"></a>

### <a name="add-an-image-using-binary-data"></a><span data-ttu-id="3602f-142">Добавление изображения с помощью двоичных данных</span><span class="sxs-lookup"><span data-stu-id="3602f-142">Add an image using binary data</span></span>

<span data-ttu-id="3602f-143">Во входной HTML-код из части **Presentation** запроса включите параметр `<img src="name:part-name" />`, где *part-name* — это уникальный идентификатор той части [составного запроса](onenote-create-page.md#example-request), которая содержит двоичные данные изображения.</span><span class="sxs-lookup"><span data-stu-id="3602f-143">In the input HTML of your request's **Presentation** part, include  `<img src="name:part-name" />`, where *part-name* is the unique identifier for the data part in your [multipart request](onenote-create-page.md#example-request) that contains the binary image data.</span></span> <span data-ttu-id="3602f-144">Просто отправьте двоичные данные, не используя Base64 или другую кодировку.</span><span class="sxs-lookup"><span data-stu-id="3602f-144">Just send the binary data, don't use Base64 or otherwise encode it.</span></span>

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

### <a name="add-a-webpage-snapshot"></a><span data-ttu-id="3602f-145">Добавление моментального снимка веб-страницы</span><span class="sxs-lookup"><span data-stu-id="3602f-145">Add a webpage snapshot</span></span>

<span data-ttu-id="3602f-146">С помощью Microsoft Graph можно создавать моментальные снимки целых веб-страниц и вставлять их в новые страницы.</span><span class="sxs-lookup"><span data-stu-id="3602f-146">You can use Microsoft Graph to snapshot entire webpages and insert them into new pages.</span></span> <span data-ttu-id="3602f-147">Этот метод удобен для архивации веб-страниц и сохранения сложных веб-страниц, которые содержат функции, не поддерживаемые OneNote (например, CSS).</span><span class="sxs-lookup"><span data-stu-id="3602f-147">This method is useful to archive webpages or capture complex webpages that have features that OneNote doesn't support (like some CSS).</span></span>  

<span data-ttu-id="3602f-148">Во входной HTML-код запроса включите параметр `<img src="http://..." />` и укажите URL-адрес веб-страницы, которую нужно вставить, в атрибуте **src**.</span><span class="sxs-lookup"><span data-stu-id="3602f-148">In the input HTML of your request, include  `<img src="http://..." />` and specify the URL of the webpage you want to insert for the **src** attribute.</span></span>

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
    <img data-render-src="http://www.onenote.com" width="200"/>
  </body>
</html>

--MyAppPartBoundary--  
```


<a name="image-img-binary-data-render-src"></a>

### <a name="add-an-image-rendered-from-html"></a><span data-ttu-id="3602f-149">Добавление изображения, созданного из HTML-кода</span><span class="sxs-lookup"><span data-stu-id="3602f-149">Add an image rendered from HTML</span></span>

<span data-ttu-id="3602f-150">При передаче HTML-кода в виде блока данных убедитесь в отсутствии активного содержимого, для которого могут потребоваться учетные данные пользователя или предварительно загруженный подключаемый модуль браузера.</span><span class="sxs-lookup"><span data-stu-id="3602f-150">When you pass the HTML as a data-block, be sure there is no active content that would require user credentials, or a pre-loaded browser plug-in.</span></span> <span data-ttu-id="3602f-151">Подсистема, которую Microsoft Graph использует для преобразования HTML-страницы в изображение, не может выполнить вход для пользователя и не включает такие подключаемые модули, как Adobe Flash и Apple QuickTime.</span><span class="sxs-lookup"><span data-stu-id="3602f-151">The engine that Microsoft Graph uses to render the HTML page into an image has no ability to log in a user, and doesn't include plug-ins like Adobe Flash, Apple QuickTime, and so-on.</span></span> <span data-ttu-id="3602f-152">Это также означает, что динамически загружаемое содержимое (например, через скрипт AJAX) не будет отображаться, если для получения данных необходимы учетные данные пользователя или файлы cookie.</span><span class="sxs-lookup"><span data-stu-id="3602f-152">That also means that dynamically-loaded content, like might come with an AJAX script, won't appear if getting the data requires user login credentials or cookies.</span></span>

<span data-ttu-id="3602f-153">Во входной HTML-код из части **Presentation** запроса включите параметр `<img data-render-src="name:part-name" />`, где *part-name* — это уникальный идентификатор той части [составного запроса](onenote-create-page.md#example-request), которая содержит HTML-код.</span><span class="sxs-lookup"><span data-stu-id="3602f-153">In the input HTML of your request's **Presentation** part, include  `<img data-render-src="name:part-name" />`, where *part-name* is the unique identifier for the data part in your [multipart request](onenote-create-page.md#example-request) that contains the HTML.</span></span>


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
<img src="http://cdn.onenote.net/1664161560_Images/OneNote.ico" />
</body>
</html>

--MyAppPartBoundary--  
```


<a name="image-object"></a>

### <a name="add-an-image-file-as-an-attachment"></a><span data-ttu-id="3602f-154">Добавление файла изображения в качестве вложения</span><span class="sxs-lookup"><span data-stu-id="3602f-154">Add an image file as an attachment</span></span>

<span data-ttu-id="3602f-155">Во входной HTML-код из части **Presentation** запроса включите параметр `<object data="name:part-name" data-attachment="file-name.file-ext" type="media-type/media-subtype" />`, где *part-name* — это уникальный идентификатор той части [составного запроса](onenote-create-page.md#example-request), которая содержит двоичные данные изображения.</span><span class="sxs-lookup"><span data-stu-id="3602f-155">In the input HTML of your request's **Presentation** part, include  `<object data="name:part-name" data-attachment="file-name.file-ext" type="media-type/media-subtype" />`, where *part-name* is the unique identifier for the data part in your [multipart request](onenote-create-page.md#example-request) that contains the binary image data.</span></span> <span data-ttu-id="3602f-156">Просто отправьте двоичные данные, не используя Base64 или другую кодировку.</span><span class="sxs-lookup"><span data-stu-id="3602f-156">Just send the binary data, don't use Base64 or otherwise encode it.</span></span>

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

<span data-ttu-id="3602f-157">Узнайте больше о [типах файлов мультимедиа](#file-media-types).</span><span class="sxs-lookup"><span data-stu-id="3602f-157">Learn more about [file media types](#file-media-types).</span></span>



<a name="adding-videos"></a>

## <a name="adding-videos"></a><span data-ttu-id="3602f-158">Добавление видео</span><span class="sxs-lookup"><span data-stu-id="3602f-158">Adding videos</span></span>

<span data-ttu-id="3602f-159">Вы можете внедрять видео в страницы OneNote с помощью команды `<iframe data-original-src="http://..." />` во входном HTML-коде.</span><span class="sxs-lookup"><span data-stu-id="3602f-159">You can embed videos in OneNote pages using `<iframe data-original-src="http://..." />` in the input HTML.</span></span> 

### <a name="supported-video-sites"></a><span data-ttu-id="3602f-160">Поддерживаемые сайты с видео</span><span class="sxs-lookup"><span data-stu-id="3602f-160">Supported video sites</span></span>

- <span data-ttu-id="3602f-161">Dailymotion</span><span class="sxs-lookup"><span data-stu-id="3602f-161">Dailymotion</span></span>
- <span data-ttu-id="3602f-162">Office Mix</span><span class="sxs-lookup"><span data-stu-id="3602f-162">Office Mix</span></span>
- <span data-ttu-id="3602f-163">Sway</span><span class="sxs-lookup"><span data-stu-id="3602f-163">Sway</span></span>
- <span data-ttu-id="3602f-164">Sketchfab</span><span class="sxs-lookup"><span data-stu-id="3602f-164">Sketchfab</span></span>
- <span data-ttu-id="3602f-165">TED</span><span class="sxs-lookup"><span data-stu-id="3602f-165">TED</span></span>
- <span data-ttu-id="3602f-166">YouTube</span><span class="sxs-lookup"><span data-stu-id="3602f-166">YouTube</span></span>
- <span data-ttu-id="3602f-167">Vimeo</span><span class="sxs-lookup"><span data-stu-id="3602f-167">Vimeo</span></span>
- <span data-ttu-id="3602f-168">Vine</span><span class="sxs-lookup"><span data-stu-id="3602f-168">Vine</span></span>

### <a name="iframe-attributes"></a><span data-ttu-id="3602f-169">Атрибуты iframe</span><span class="sxs-lookup"><span data-stu-id="3602f-169">iframe attributes</span></span>

#### <a name="data-original-src"></a><span data-ttu-id="3602f-170">data-original-src</span><span class="sxs-lookup"><span data-stu-id="3602f-170">data-original-src</span></span>

<span data-ttu-id="3602f-171">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3602f-171">Required.</span></span> <span data-ttu-id="3602f-172">URL-адрес видео.</span><span class="sxs-lookup"><span data-stu-id="3602f-172">The URL of the video.</span></span>

<span data-ttu-id="3602f-173">Пример: `data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8"`</span><span class="sxs-lookup"><span data-stu-id="3602f-173">Example: `data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8"`</span></span>

#### <a name="width"></a><span data-ttu-id="3602f-174">width</span><span class="sxs-lookup"><span data-stu-id="3602f-174">width</span></span>

<span data-ttu-id="3602f-175">Необязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="3602f-175">Optional.</span></span> <span data-ttu-id="3602f-176">Ширина элемента iframe, содержащего видео.</span><span class="sxs-lookup"><span data-stu-id="3602f-176">The width of the iframe that contains the video.</span></span> <span data-ttu-id="3602f-177">Значение по умолчанию: 480.</span><span class="sxs-lookup"><span data-stu-id="3602f-177">Default is 480.</span></span>

<span data-ttu-id="3602f-178">Пример: `width="300"`</span><span class="sxs-lookup"><span data-stu-id="3602f-178">Example: `width="300"`</span></span>

#### <a name="height"></a><span data-ttu-id="3602f-179">height</span><span class="sxs-lookup"><span data-stu-id="3602f-179">height</span></span>

<span data-ttu-id="3602f-180">Необязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="3602f-180">Optional.</span></span> <span data-ttu-id="3602f-181">Высота элемента iframe, содержащего видео.</span><span class="sxs-lookup"><span data-stu-id="3602f-181">The height of the iframe that contains the video.</span></span> <span data-ttu-id="3602f-182">Значение по умолчанию: 360.</span><span class="sxs-lookup"><span data-stu-id="3602f-182">Default is 360.</span></span>

<span data-ttu-id="3602f-183">Пример: `height="300"`</span><span class="sxs-lookup"><span data-stu-id="3602f-183">Example: `height="300"`</span></span>

### <a name="example"></a><span data-ttu-id="3602f-184">Пример</span><span class="sxs-lookup"><span data-stu-id="3602f-184">Example</span></span>

<span data-ttu-id="3602f-185">Во входном HTML-коде запроса добавьте параметр `<iframe data-original-src="http://..." />` и укажите URL-адрес видео в атрибуте **data-original-src**.</span><span class="sxs-lookup"><span data-stu-id="3602f-185">In the input HTML of your request, include `<iframe data-original-src="http://..." />` and specify the URL of the video for the **data-original-src** attribute.</span></span>

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

## <a name="adding-files"></a><span data-ttu-id="3602f-186">Добавление файлов</span><span class="sxs-lookup"><span data-stu-id="3602f-186">Adding files</span></span>

<span data-ttu-id="3602f-187">Вы можете добавлять вложенные файлы в страницы OneNote с помощью элемента **object** во входном HTML-коде.</span><span class="sxs-lookup"><span data-stu-id="3602f-187">You can add file attachments to OneNote pages using an **object** element in the input HTML.</span></span> <span data-ttu-id="3602f-188">Если вам нужно добавить PDF-файл, вы можете использовать элемент **img** для отрисовки страниц PDF-файла в виде изображений.</span><span class="sxs-lookup"><span data-stu-id="3602f-188">If you're adding a PDF file, you can use an **img** element to render the PDF pages as images.</span></span> 

[<span data-ttu-id="3602f-189">Добавление вложенного файла</span><span class="sxs-lookup"><span data-stu-id="3602f-189">Add a file attachment</span></span>](#add-a-file-attachment)

<span data-ttu-id="3602f-190">Используйте элемент `<object .../>` и отправьте файл в части данных составного запроса.</span><span class="sxs-lookup"><span data-stu-id="3602f-190">Use `<object .../>` and send the file in a data part of a multipart request.</span></span> <span data-ttu-id="3602f-191">Добавляет вложенный файл и отображает значок файла на странице OneNote.</span><span class="sxs-lookup"><span data-stu-id="3602f-191">Adds a file attachment that displays a file icon on the OneNote page.</span></span>

[<span data-ttu-id="3602f-192">Добавление изображений содержимого PDF-файлов</span><span class="sxs-lookup"><span data-stu-id="3602f-192">Add images of PDF file contents</span></span>](#add-images-of-pdf-file-contents)

<span data-ttu-id="3602f-193">Используйте элемент `<img data-render-src="name:part-name" />` и отправьте PDF-файл в части данных составного запроса.</span><span class="sxs-lookup"><span data-stu-id="3602f-193">Use `<img data-render-src="name:part-name" />` and send a PDF file in the data part of a multipart request.</span></span> <span data-ttu-id="3602f-194">Отрисовывает каждую PDF-страницу в виде отдельного изображения на странице OneNote.</span><span class="sxs-lookup"><span data-stu-id="3602f-194">Renders each PDF page as a separate image on the OneNote page.</span></span>

#### <a name="file-attributes"></a><span data-ttu-id="3602f-195">Атрибуты файлов</span><span class="sxs-lookup"><span data-stu-id="3602f-195">File attributes</span></span>

<span data-ttu-id="3602f-196">Ниже перечислены обязательные атрибуты элемента **object**.</span><span class="sxs-lookup"><span data-stu-id="3602f-196">The **object** element requires the following attributes.</span></span>

<span data-ttu-id="3602f-197">**data-attachment**</span><span class="sxs-lookup"><span data-stu-id="3602f-197">**data-attachment**</span></span>

<span data-ttu-id="3602f-198">Имя и расширения файла, который нужно отобразить на странице OneNote.</span><span class="sxs-lookup"><span data-stu-id="3602f-198">The file name and extension to display on the OneNote page.</span></span>

<span data-ttu-id="3602f-199">Пример: `data-attachment="filename.docx"`</span><span class="sxs-lookup"><span data-stu-id="3602f-199">Example: `data-attachment="filename.docx"`</span></span>

<span data-ttu-id="3602f-200">**data**</span><span class="sxs-lookup"><span data-stu-id="3602f-200">**data**</span></span>

<span data-ttu-id="3602f-201">Имя части body в составном запросе, содержащем двоичные данные файла.</span><span class="sxs-lookup"><span data-stu-id="3602f-201">The name of the body part in the multipart request that contains the binary file data.</span></span> <span data-ttu-id="3602f-202">Microsoft Graph не поддерживает передачу URL-адресов через этот атрибут.</span><span class="sxs-lookup"><span data-stu-id="3602f-202">Microsoft Graph does not support passing a URL reference here.</span></span>

<span data-ttu-id="3602f-203">Пример: `data="name:part-name"`</span><span class="sxs-lookup"><span data-stu-id="3602f-203">Example: `data="name:part-name"`</span></span>

<span data-ttu-id="3602f-204">**type**</span><span class="sxs-lookup"><span data-stu-id="3602f-204">**type**</span></span>

<span data-ttu-id="3602f-205">MIME-тип файла, который используется для определения значка файла для страницы и приложения, запускаемого, когда пользователь активирует файл на устройстве из OneNote.</span><span class="sxs-lookup"><span data-stu-id="3602f-205">The file media type, used to determine the file icon to use on the page, and which application starts when the user activates the file on the device from OneNote.</span></span>

<span data-ttu-id="3602f-206">Пример: `type="application/pdf"`</span><span class="sxs-lookup"><span data-stu-id="3602f-206">Example: `type="application/pdf"`</span></span>


<a name="file-media-types"></a>

#### <a name="file-media-types"></a><span data-ttu-id="3602f-207">MIME-типы файлов</span><span class="sxs-lookup"><span data-stu-id="3602f-207">File media types</span></span>  

<span data-ttu-id="3602f-208">Microsoft Graph использует предопределенный значок для типа вложенного файла или универсальный значок, если API не распознает тип файла.</span><span class="sxs-lookup"><span data-stu-id="3602f-208">Microsoft Graph uses predefined file-types icon for attached files, or a generic icon when the API doesn't recognize the file type.</span></span> <span data-ttu-id="3602f-209">В приведенной ниже таблице показаны распространенные типы файлов, которые распознает этот API.</span><span class="sxs-lookup"><span data-stu-id="3602f-209">The following table shows some common file types that are recognized by the API.</span></span>

- <span data-ttu-id="3602f-210">application/pdf</span><span class="sxs-lookup"><span data-stu-id="3602f-210">application/pdf</span></span>  
- <span data-ttu-id="3602f-211">application/vnd.openxmlformats-officedocument.wordprocessingml.document</span><span class="sxs-lookup"><span data-stu-id="3602f-211">application/vnd.openxmlformats-officedocument.wordprocessingml.document</span></span>  
- <span data-ttu-id="3602f-212">application/vnd.openxmlformats-officedocument.presentationml.presentation</span><span class="sxs-lookup"><span data-stu-id="3602f-212">application/vnd.openxmlformats-officedocument.presentationml.presentation</span></span>
- <span data-ttu-id="3602f-213">application/vnd.openxmlformats-officedocument.spreadsheetml.sheet</span><span class="sxs-lookup"><span data-stu-id="3602f-213">application/vnd.openxmlformats-officedocument.spreadsheetml.sheet</span></span>
- <span data-ttu-id="3602f-214">image/png</span><span class="sxs-lookup"><span data-stu-id="3602f-214">image/png</span></span>
- <span data-ttu-id="3602f-215">image/jpeg</span><span class="sxs-lookup"><span data-stu-id="3602f-215">image/jpeg</span></span>
- <span data-ttu-id="3602f-216">image/gif</span><span class="sxs-lookup"><span data-stu-id="3602f-216">image/gif</span></span>
- <span data-ttu-id="3602f-217">audio/wav</span><span class="sxs-lookup"><span data-stu-id="3602f-217">audio/wav</span></span>
- <span data-ttu-id="3602f-218">video/mp4</span><span class="sxs-lookup"><span data-stu-id="3602f-218">video/mp4</span></span>
- <span data-ttu-id="3602f-219">application/msword</span><span class="sxs-lookup"><span data-stu-id="3602f-219">application/msword</span></span>
- <span data-ttu-id="3602f-220">application/mspowerpoint</span><span class="sxs-lookup"><span data-stu-id="3602f-220">application/mspowerpoint</span></span>
- <span data-ttu-id="3602f-221">application/excel</span><span class="sxs-lookup"><span data-stu-id="3602f-221">application/excel</span></span>

<span data-ttu-id="3602f-222">Ознакомьтесь с [ограничениями](#size-limitations-for-post-pages-requests) на создание страниц, содержащих файлы мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="3602f-222">See [limitations](#size-limitations-for-post-pages-requests) that apply when creating pages that contain media.</span></span>


<a name="file-object"></a>

### <a name="add-a-file-attachment"></a><span data-ttu-id="3602f-223">Добавление вложенного файла</span><span class="sxs-lookup"><span data-stu-id="3602f-223">Add a file attachment</span></span>

<span data-ttu-id="3602f-224">Во входной HTML-код из части **Presentation** запроса включите параметр `<object data="name:part-name" data-attachment="file-name.file-ext" type="media-type/media-subtype" />`, где *part-name* — это уникальный идентификатор той части [составного запроса](onenote-create-page.md#example-request), которая содержит данные двоичного файла.</span><span class="sxs-lookup"><span data-stu-id="3602f-224">In the input HTML of your request's **Presentation** part, include  `<object data="name:part-name" data-attachment="file-name.file-ext" type="media-type/media-subtype" />`, where *part-name* is the unique identifier for the data part in your [multipart request](onenote-create-page.md#example-request) that contains the binary file data.</span></span> <span data-ttu-id="3602f-225">Просто отправьте двоичные данные, не используя Base64 или другую кодировку.</span><span class="sxs-lookup"><span data-stu-id="3602f-225">Just send the binary data, don't use Base64 or otherwise encode it.</span></span>

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

### <a name="add-images-of-pdf-file-contents"></a><span data-ttu-id="3602f-226">Добавление изображений содержимого PDF-файлов</span><span class="sxs-lookup"><span data-stu-id="3602f-226">Add images of PDF file contents</span></span>

<span data-ttu-id="3602f-227">Во входной HTML-код из части **Presentation** запроса включите параметр `<img data-render-src="name:part-name" ... />`, где *part-name* — это уникальный идентификатор той части [составного запроса](onenote-create-page.md#example-request), которая содержит данные двоичного файла.</span><span class="sxs-lookup"><span data-stu-id="3602f-227">In the input HTML of your request's **Presentation** part, include  `<img data-render-src="name:part-name" ... />`, where *part-name* is the unique identifier for the data part in your [multipart request](onenote-create-page.md#example-request) that contains the binary file data.</span></span> <span data-ttu-id="3602f-228">Просто отправьте двоичные данные, не используя Base64 или другую кодировку.</span><span class="sxs-lookup"><span data-stu-id="3602f-228">Just send the binary data, don't use Base64 or otherwise encode it.</span></span>

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

## <a name="size-limitations-for-post-pages-requests"></a><span data-ttu-id="3602f-229">Ограничения на размер запросов POST для страниц</span><span class="sxs-lookup"><span data-stu-id="3602f-229">Size limitations for POST pages requests</span></span>

<span data-ttu-id="3602f-230">При отправке изображений и файлов учитывайте следующие ограничения: <!--TODO: check these--></span><span class="sxs-lookup"><span data-stu-id="3602f-230">When sending image and file data, be aware of these limitations: <!--TODO: check these--></span></span>

- <span data-ttu-id="3602f-231">Общий максимальный размер данных в запросе POST (включая изображения, файлы и другие данные) составляет приблизительно 70 МБ.</span><span class="sxs-lookup"><span data-stu-id="3602f-231">The total POST size limit is ~70 MB, including images, files, and other data.</span></span> <span data-ttu-id="3602f-232">Фактическое ограничение зависит от кодировки в нижестоящих системах, поэтому не существует фиксированного ограничения в байтах.</span><span class="sxs-lookup"><span data-stu-id="3602f-232">The actual limit is affected by downstream encoding, so there's no fixed byte-count limit.</span></span> <span data-ttu-id="3602f-233">Запросы, превышающие это ограничение, могут возвращать ненадежные результаты.</span><span class="sxs-lookup"><span data-stu-id="3602f-233">Requests that exceed the limit may produce unreliable results.</span></span>

- <span data-ttu-id="3602f-234">Ограничение для каждой части данных (включая заголовки) составляет 25 МБ.</span><span class="sxs-lookup"><span data-stu-id="3602f-234">The limit for each data part is 25 MB, including the part headers.</span></span> <span data-ttu-id="3602f-235">Microsoft Graph отклоняет части данных, превышающие это ограничение.</span><span class="sxs-lookup"><span data-stu-id="3602f-235">Data parts that exceed the limit are rejected by Microsoft Graph.</span></span> 

- <span data-ttu-id="3602f-236">Максимальное количество изображений на странице составляет 150.</span><span class="sxs-lookup"><span data-stu-id="3602f-236">The maximum number of images per page is 150.</span></span> <span data-ttu-id="3602f-237">При использовании атрибута `src="http://..."` API игнорирует теги **img** после достижения этого предела.</span><span class="sxs-lookup"><span data-stu-id="3602f-237">When using the `src="http://..."` attribute, the API ignores **img** tags beyond the limit.</span></span>

- <span data-ttu-id="3602f-238">Каждый запрос POST может включать до 6 частей данных, включая обязательную часть **Presentation**.</span><span class="sxs-lookup"><span data-stu-id="3602f-238">The maximum number of data parts is 6 per POST, including the required **Presentation** part.</span></span>

- <span data-ttu-id="3602f-239">Каждый запрос может содержать до пяти элементов **img** с атрибутом **data-render-src** и один элемент **object** с атрибутом **data-render-src**. Остальные ссылки на изображения и файлы игнорируются.</span><span class="sxs-lookup"><span data-stu-id="3602f-239">Each request can contain up to five **img** elements that use **data-render-src** and one **object** elements that uses **data-render-src**. Additional image and file references are ignored.</span></span>

- <span data-ttu-id="3602f-240">Один запрос POST может включать до 30 изображений, независимо от того, какой метод используется для их отправки в API.</span><span class="sxs-lookup"><span data-stu-id="3602f-240">The maximum number of images in a single POST is 30, no matter which method you use to send them to the API.</span></span> <span data-ttu-id="3602f-241">Остальные изображения игнорируются.</span><span class="sxs-lookup"><span data-stu-id="3602f-241">Additional images are ignored.</span></span> <span data-ttu-id="3602f-242">Если вам нужно сохранить веб-страницу с большим количеством изображений, рекомендуем [сохранить ее в виде моментального снимка](#add-a-webpage-snapshot).</span><span class="sxs-lookup"><span data-stu-id="3602f-242">If you want to capture a webpage that contains a lot of images, consider [capturing the whole page as a snapshot](#add-a-webpage-snapshot).</span></span>


## <a name="when-to-use-html-versus-data-render-src"></a><span data-ttu-id="3602f-243">Когда использовать HTML, а когда — data-render-src</span><span class="sxs-lookup"><span data-stu-id="3602f-243">When to use HTML versus data-render-src</span></span> 

<span data-ttu-id="3602f-244">Если вы выбираете между вставкой HTML на страницу OneNote и использованием атрибута **data-render-src**, учитывайте следующее:</span><span class="sxs-lookup"><span data-stu-id="3602f-244">When trying to decide between putting HTML directly onto the OneNote page instead of using the **data-render-src** attribute, consider the following:</span></span>

- <span data-ttu-id="3602f-245">Сложный HTML, вероятно, лучше отправлять в механизм визуализации с помощью **data-render-src**, а не пытаться изменить HTML так, чтобы его принял Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="3602f-245">Complex HTML is probably best sent to the rendering engine via **data-render-src**, rather than attempting to modify the HTML to fit into what Microsoft Graph can accept.</span></span> <span data-ttu-id="3602f-246">Это также относится к тем случаям, когда HTML-код включает неподдерживаемые теги.</span><span class="sxs-lookup"><span data-stu-id="3602f-246">This is also true when your HTML includes tags that aren't supported supported.</span></span>

- <span data-ttu-id="3602f-247">Как правило, точную отрисовку страниц для сохранения макета и внешнего вида страницы лучше обеспечивает механизм визуализации с использованием атрибута **data-render-src**.</span><span class="sxs-lookup"><span data-stu-id="3602f-247">Accurate page rendering to preserve the layout and look of the page is probably best done with the rendering engine via **data-render-src**.</span></span>

- <span data-ttu-id="3602f-p130">Напрямую редактируемый текст часто лучше всего реализовать, вставляя HTML напрямую на страницу. Отрисованные изображения сканируются системой распознавания текста (OCR), но результаты не будут одинаковыми.</span><span class="sxs-lookup"><span data-stu-id="3602f-p130">Directly-editable text is often best done with inserting the HTML directly onto the page. The rendered images are scanned by an optical character recognition (OCR) system, but it's just not the same.</span></span>

- <span data-ttu-id="3602f-250">Моментальный снимок для журнала или архива лучше всего создавать с помощью метода **data-render-src**.</span><span class="sxs-lookup"><span data-stu-id="3602f-250">Snapshot-in-time for historical or archival purposes is usually best done with the data-render-src method.</span></span>

- <span data-ttu-id="3602f-p131">Отметка проекта веб-страницы для редактирования — это задача, где **data-render-src** по-настоящему проявляет себя. Используя возможности рукописного ввода OneNote, можно нарисовать изображение для обозначения изменений или подчеркнуть важные области. Наличие веб-страницы в форме изображения намного упрощает эту задачу.</span><span class="sxs-lookup"><span data-stu-id="3602f-p131">Marking-up a web page design for revisions is one place the **data-render-src** truly shines. Using OneNote's inking capabilities, you can draw on the image to indicate changes or call out important areas. Having the web page as an image makes that a lot easier.</span></span>

- <span data-ttu-id="3602f-254">Очень крупные изображения или изображения в форматах, которые OneNote не принимает напрямую, иногда легче преобразовать в эскизы и другие форматы с помощью атрибута **data-render-src**, а не собственного кода.</span><span class="sxs-lookup"><span data-stu-id="3602f-254">Very large images, or images in formats that OneNote doesn't directly accept can sometimes be thumbnailed and converted with the **data-render-src** attribure more easily than by doing it in your own code.</span></span> <span data-ttu-id="3602f-255">Даже если изображение также доступно в сети, внедрение данных в запрос POST иногда позволяет быстрее сделать сохраненную страницу доступной пользователям OneNote за счет уменьшения общего количества круговых путей, необходимых для создания страницы OneNote.</span><span class="sxs-lookup"><span data-stu-id="3602f-255">Even if the image is also available onlinet, embedding the data in your POST can sometimes make the captured page available to OneNote user sooner, by reducing the total number of round-trips needed to build the OneNote page.</span></span>

<span data-ttu-id="3602f-256">Иногда лучший способ определить, какой метод лучше подойдет пользователям — опробовать оба варианта во время разработки приложения.</span><span class="sxs-lookup"><span data-stu-id="3602f-256">Sometimes, the best way to determine which method will work best for your users is to try it both ways as you develop your app.</span></span>


<a name="permissions"></a>

## <a name="permissions"></a><span data-ttu-id="3602f-257">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3602f-257">Permissions</span></span>

<span data-ttu-id="3602f-258">Для создания и обновления страниц OneNote необходимо запрашивать соответствующие разрешения.</span><span class="sxs-lookup"><span data-stu-id="3602f-258">To create or update OneNote pages, you'll need to request appropriate permissions.</span></span> <span data-ttu-id="3602f-259">Выберите минимальный уровень, необходимый для работы вашего приложения.</span><span class="sxs-lookup"><span data-stu-id="3602f-259">Choose the lowest level that your app needs to do its work.</span></span>

#### <a name="permissions-for-post-pages"></a><span data-ttu-id="3602f-260">Разрешения в случае запросов POST для страниц</span><span class="sxs-lookup"><span data-stu-id="3602f-260">Permissions for POST pages</span></span>

- <span data-ttu-id="3602f-261">Notes.Create</span><span class="sxs-lookup"><span data-stu-id="3602f-261">Notes.Create</span></span>
- <span data-ttu-id="3602f-262">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3602f-262">Notes.ReadWrite</span></span>
- <span data-ttu-id="3602f-263">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3602f-263">Notes.ReadWrite.All</span></span> 

#### <a name="permissions-for-patch-pages"></a><span data-ttu-id="3602f-264">Разрешения в случае запросов PATCH для страниц</span><span class="sxs-lookup"><span data-stu-id="3602f-264">Permissions for PATCH pages</span></span>

- <span data-ttu-id="3602f-265">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3602f-265">Notes.ReadWrite</span></span>
- <span data-ttu-id="3602f-266">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3602f-266">Notes.ReadWrite.All</span></span>

<span data-ttu-id="3602f-267">Дополнительные сведения об областях разрешений и принципах их работы см. в разделе [Разрешения OneNote](permissions_reference.md#notes-permissions).</span><span class="sxs-lookup"><span data-stu-id="3602f-267">For more information about permission scopes and how they work, see [OneNote permission scopes](permissions_reference.md#notes-permissions).</span></span>


<a name="see-also"></a>

## <a name="see-also"></a><span data-ttu-id="3602f-268">См. также</span><span class="sxs-lookup"><span data-stu-id="3602f-268">See also</span></span>

- [<span data-ttu-id="3602f-269">Интеграция с OneNote</span><span class="sxs-lookup"><span data-stu-id="3602f-269">Integrate with OneNote</span></span>](integrate_with_onenote.md)
- [<span data-ttu-id="3602f-270">Блог разработчиков OneNote</span><span class="sxs-lookup"><span data-stu-id="3602f-270">OneNote Developer Blog</span></span>](http://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="3602f-271">Вопросы разработки OneNote на сайте Stack Overflow</span><span class="sxs-lookup"><span data-stu-id="3602f-271">OneNote development questions on Stack Overflow</span></span>](http://go.microsoft.com/fwlink/?LinkID=390182)
- [<span data-ttu-id="3602f-272">Репозитории GitHub OneNote</span><span class="sxs-lookup"><span data-stu-id="3602f-272">OneNote GitHub repos</span></span>](http://go.microsoft.com/fwlink/?LinkID=390178)  
