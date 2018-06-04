# <a name="update-onenote-page-content"></a><span data-ttu-id="1f7df-101">Обновление содержимого страниц OneNote</span><span class="sxs-lookup"><span data-stu-id="1f7df-101">Update OneNote page content</span></span>

<span data-ttu-id="1f7df-102">*__Относится к:__ пользовательские записные книжки в OneDrive | корпоративные записные книжки в Office 365*</span><span class="sxs-lookup"><span data-stu-id="1f7df-102">*__Applies to:__ Consumer notebooks on OneDrive | Enterprise notebooks on Office 365*</span></span>


<span data-ttu-id="1f7df-103">Чтобы обновить содержимое страницы OneNote, необходимо отправить запрос PATCH в конечную точку *content* страницы:</span><span class="sxs-lookup"><span data-stu-id="1f7df-103">To retrieve the HTML content of a onnvshort page, you send a GET request to  the page's content endpoint:</span></span>

`PATCH ../notes/pages/{id}/content`</p>

<span data-ttu-id="1f7df-104">Отправьте объект изменений JSON в тексте сообщения.</span><span class="sxs-lookup"><span data-stu-id="1f7df-104">Send a JSON change object in the message body.</span></span> <span data-ttu-id="1f7df-105">Если запрос выполнен успешно, Microsoft Graph возвращает код состояния HTTP 204.</span><span class="sxs-lookup"><span data-stu-id="1f7df-105">If the create request is successful, the onnvshort API returns a 201 HTTP status code.</span></span>


<a name="request-uri"></a>
## <a name="construct-the-request-uri"></a><span data-ttu-id="1f7df-106">Создание URI запроса</span><span class="sxs-lookup"><span data-stu-id="1f7df-106">Construct the request</span></span>

<span data-ttu-id="1f7df-107">Чтобы создать URI запроса, начните с корневого URL-адреса службы:</span><span class="sxs-lookup"><span data-stu-id="1f7df-107">To construct the request URI, start with the service root URL:</span></span>

`https://graph.microsoft.com/v1.0/me/onenote`

<span data-ttu-id="1f7df-108">Затем добавьте конечную точку *content* страницы:</span><span class="sxs-lookup"><span data-stu-id="1f7df-108">Then append the page's *content* endpoint:</span></span>

<span data-ttu-id="1f7df-109">**Получение HTML-кода страницы и всех определенных значений *data-id***</span><span class="sxs-lookup"><span data-stu-id="1f7df-109">**Get the page HTML and all defined *data-id* values**</span></span></p>
`../pages/{id}/content`   

<span data-ttu-id="1f7df-110">**Получение HTML-кода страницы, всех определенных значений *data-id* и всех созданных значений *id***</span><span class="sxs-lookup"><span data-stu-id="1f7df-110">**Get the page HTML, all defined *data-id* values, and all generated *id* values**</span></span>  
`../pages/{page-id}/content?includeIDs=true` 

<span data-ttu-id="1f7df-111">Значения **data-id** и **id** используются в качестве идентификаторов **target** для элементов, которые требуется изменить.</span><span class="sxs-lookup"><span data-stu-id="1f7df-111">The **data-id** and **id** values are used as **target** identifiers for the elements you want to update.</span></span>

 
<span data-ttu-id="1f7df-112">Полный URI запроса будет выглядеть так:</span><span class="sxs-lookup"><span data-stu-id="1f7df-112">Your full request URI will look like this:</span></span>

`https://graph.microsoft.com/v1.0/me/onenote/pages/{id}/content`


<span data-ttu-id="1f7df-113">Узнайте больше о [корневом URL-адресе службы](../api-reference/v1.0/resources/onenote-api-overview.md#root-url).</span><span class="sxs-lookup"><span data-stu-id="1f7df-113">Learn more about the [service root URL](../api-reference/v1.0/resources/onenote-api-overview.md#root-url).</span></span>


<a name="message-body"></a>
## <a name="construct-the-message-body"></a><span data-ttu-id="1f7df-114">Составление текста сообщения</span><span class="sxs-lookup"><span data-stu-id="1f7df-114">Construct the message body</span></span>

<span data-ttu-id="1f7df-115">HTML-код страницы OneNote содержит текст, изображения и другое содержимое, структурированные с помощью таких элементов, как **div**, **img** и **ol**.</span><span class="sxs-lookup"><span data-stu-id="1f7df-115">The HTML of a onnvshort page contains text, images, and other content organized into structures such as div, img, and ol elements. To update page HTML, you send a PATCH request to the page's content endpoint:</span></span> <span data-ttu-id="1f7df-116">Для обновления содержимого страницы OneNote необходимо добавлять и заменять элементы HTML на странице.</span><span class="sxs-lookup"><span data-stu-id="1f7df-116">To update OneNote page content, you add and replace HTML elements on the page.</span></span>

<span data-ttu-id="1f7df-117">Изменения отправляются в тексте сообщения в виде массива объектов JSON.</span><span class="sxs-lookup"><span data-stu-id="1f7df-117">Your changes are sent in the message body as an array of JSON change objects.</span></span> <span data-ttu-id="1f7df-118">В каждом объекте указываются целевой элемент, новое содержимое HTML и действия, которые нужно выполнить с содержимым.</span><span class="sxs-lookup"><span data-stu-id="1f7df-118">Your changes are sent in the request body as an array of JSON objects. Each object specifies the target element,  new HTML content, and what to do with the content.</span></span>

<span data-ttu-id="1f7df-p104">Следующий массив определяет два изменения. Первое вставляет изображение над абзацем в качестве элемента того же уровня, а второе добавляет элемент в список в качестве последнего дочернего элемента.</span><span class="sxs-lookup"><span data-stu-id="1f7df-p104">The following array defines two changes. The first inserts an image above a paragraph as a sibling, and the second appends an item to a list as a last child.</span></span>

```json
[
   {
    'target':'#para-id',
    'action':'insert',
    'position':'before',
    'content':'<img src="image-url-or-part-name" alt="Image above the target paragraph" />'
  }, 
  {
    'target':'#list-id',
    'action':'append',
    'content':'<li>Item at the end of the list</li>'
  }
]
```

<span data-ttu-id="1f7df-121">См. [другие примеры](#example-requests).</span><span class="sxs-lookup"><span data-stu-id="1f7df-121">See [more examples](#example-requests).</span></span>


### <a name="attributes-for-json-change-objects"></a><span data-ttu-id="1f7df-122">Атрибуты объектов JSON</span><span class="sxs-lookup"><span data-stu-id="1f7df-122">Attributes for JSON objects</span></span>

<span data-ttu-id="1f7df-123">Для определения объектов JSON в запросах PATCH используются атрибуты **target**, **action**, **position** и **content**.</span><span class="sxs-lookup"><span data-stu-id="1f7df-123">Use the **target**, **action**, **position**, and **content** attributes to define JSON objects for PATCH requests.</span></span>

<span data-ttu-id="1f7df-124">**target**</span><span class="sxs-lookup"><span data-stu-id="1f7df-124">**target**</span></span>  
<span data-ttu-id="1f7df-p105">Обновляемый элемент. Значением должен быть один из следующих идентификаторов:</span><span class="sxs-lookup"><span data-stu-id="1f7df-p105">The element to update. The value must be one of the following identifiers:</span></span>

| <span data-ttu-id="1f7df-127">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="1f7df-127">Identifier</span></span> | <span data-ttu-id="1f7df-128">Описание</span><span class="sxs-lookup"><span data-stu-id="1f7df-128">Description</span></span> |  
|------|------|  
| <span data-ttu-id="1f7df-129">#{data-id}</span><span class="sxs-lookup"><span data-stu-id="1f7df-129">data-id</span></span> | <p><span data-ttu-id="1f7df-130">Этот идентификатор при желании определяется для элементов входного HTML-кода при [создании](onenote-create-page.md) или [обновлении страницы](onenote_update_page.md).</span><span class="sxs-lookup"><span data-stu-id="1f7df-130">This ID is optionally defined on elements in the input HTML when [creating a page](onenote-create-page.md) or [updating a page](onenote_update_page.md).</span></span> <span data-ttu-id="1f7df-131">Добавьте перед этим значением префикс #.</span><span class="sxs-lookup"><span data-stu-id="1f7df-131">Prefix the value with a #.</span></span></p><p> <span data-ttu-id="1f7df-132">Пример: `'target':'#intro'` указывает на элемент `<div data-id="intro" ...>`</span><span class="sxs-lookup"><span data-stu-id="1f7df-132">Example: `'target':'#intro'` targets the element `<div data-id="intro" ...>`</span></span></p> |  
| <span data-ttu-id="1f7df-133">id</span><span class="sxs-lookup"><span data-stu-id="1f7df-133">id</span></span> | <p><span data-ttu-id="1f7df-134">Это [сгенерированный идентификатор](#generated-ids) из Microsoft Graph, необходимый для большинства операций замены.</span><span class="sxs-lookup"><span data-stu-id="1f7df-134">This is the [generated ID](#generated-ids) from Microsoft Graph, and is required for most replace operations.</span></span> <span data-ttu-id="1f7df-135">Не добавляйте перед ним префикс #.</span><span class="sxs-lookup"><span data-stu-id="1f7df-135">Do not prefix with a #.</span></span></p><p> <span data-ttu-id="1f7df-136">Пример: `'target':'div:{33f8a2...}{37}'` указывает на элемент `<div id="div:{33f8a2...}{37}" ...>`</span><span class="sxs-lookup"><span data-stu-id="1f7df-136">Example: `'target':'div:{33f8a2...}{37}'` targets the element `<div id="div:{33f8a2...}{37}" ...>`</span></span></p><p><span data-ttu-id="1f7df-137">Не следует путать эти идентификаторы со значениями **id**, определенными во [входном HTML-коде](onenote_input_output_html.md).</span><span class="sxs-lookup"><span data-stu-id="1f7df-137">Don't confuse these with any **id** values defined in the [input HTML](onenote_input_output_html.md).</span></span> <span data-ttu-id="1f7df-138">Все значения **id**, отправляемые во входном HTML-коде, отклоняются.</span><span class="sxs-lookup"><span data-stu-id="1f7df-138">All **id** values sent in the input HTML are discarded.</span></span></p> |  
| <span data-ttu-id="1f7df-139">body</span><span class="sxs-lookup"><span data-stu-id="1f7df-139">body</span></span> | <span data-ttu-id="1f7df-140">Ключевое слово, указывающее на первый разделитель на странице.</span><span class="sxs-lookup"><span data-stu-id="1f7df-140">The keyword that targets the first div on the page.</span></span> <span data-ttu-id="1f7df-141">Не добавляйте перед ним префикс #.</span><span class="sxs-lookup"><span data-stu-id="1f7df-141">Do not prefix with a #.</span></span> |  
| <span data-ttu-id="1f7df-142">title</span><span class="sxs-lookup"><span data-stu-id="1f7df-142">title</span></span> | <span data-ttu-id="1f7df-143">Ключевое слово, указывающее на заголовок страницы.</span><span class="sxs-lookup"><span data-stu-id="1f7df-143">The keyword that targets the page title.</span></span> <span data-ttu-id="1f7df-144">Не добавляйте перед ним префикс #.</span><span class="sxs-lookup"><span data-stu-id="1f7df-144">Do not prefix with a #.</span></span> |  
 
<span data-ttu-id="1f7df-145">**action**</span><span class="sxs-lookup"><span data-stu-id="1f7df-145">**action**</span></span>  
<span data-ttu-id="1f7df-146">Действие, которое требуется выполнить с целевым элементом.</span><span class="sxs-lookup"><span data-stu-id="1f7df-146">The action to perform on the target element. Possible values are: , , , , or .</span></span> <span data-ttu-id="1f7df-147">См. [поддерживаемые действия для элементов](#supported-elements-and-actions).</span><span class="sxs-lookup"><span data-stu-id="1f7df-147">See [supported actions for elements](#supported-elements-and-actions).</span></span>

| <span data-ttu-id="1f7df-148">Действие</span><span class="sxs-lookup"><span data-stu-id="1f7df-148">Action</span></span> | <span data-ttu-id="1f7df-149">Описание</span><span class="sxs-lookup"><span data-stu-id="1f7df-149">Description</span></span> |  
|------|------|  
| <span data-ttu-id="1f7df-150">append</span><span class="sxs-lookup"><span data-stu-id="1f7df-150">Append</span></span> | <p><span data-ttu-id="1f7df-151">Добавляет указанное содержимое к целевому элементу в качестве первого или последнего дочернего элемента, в зависимости от значения атрибута **position**.</span><span class="sxs-lookup"><span data-stu-id="1f7df-151">**append**Adds the supplied content to the target as a first or last child, as determined by the position attribute.Applies only to body, div, ol, and ul elements.</span></span></p><p><span data-ttu-id="1f7df-152">Применяется только к элементам **body**, **div**, **ol** и **ul**.</span><span class="sxs-lookup"><span data-stu-id="1f7df-152">Applies only to **body**, **div**, **ol**, and **ul** elements.</span></span></p> |  
| <span data-ttu-id="1f7df-153">insert</span><span class="sxs-lookup"><span data-stu-id="1f7df-153">insert</span></span> | <span data-ttu-id="1f7df-154">Добавляет указанное содержимое в качестве элемента того же уровня перед целевым элементом или после него, в зависимости от значения атрибута **position**.</span><span class="sxs-lookup"><span data-stu-id="1f7df-154">**insert**Adds the supplied content as a sibling before or after the target, as determined by the position attribute.</span></span> |  
| <span data-ttu-id="1f7df-155">prepend</span><span class="sxs-lookup"><span data-stu-id="1f7df-155">prepend</span></span> | <p><span data-ttu-id="1f7df-156">Добавляет указанное содержимое к целевому элементу в качестве первого дочернего элемента.</span><span class="sxs-lookup"><span data-stu-id="1f7df-156">Adds the supplied content to the target as a first child.</span></span> <span data-ttu-id="1f7df-157">Сокращение от действия **append** + **before**.</span><span class="sxs-lookup"><span data-stu-id="1f7df-157">Shortcut for **append** + **before**.</span></span></p><p><span data-ttu-id="1f7df-158">Применяется только к элементам **body**, **div**, **ol** и **ul**.</span><span class="sxs-lookup"><span data-stu-id="1f7df-158">Applies only to **body**, **div**, **ol**, and **ul** elements.</span></span></p> |  
| <span data-ttu-id="1f7df-159">replace</span><span class="sxs-lookup"><span data-stu-id="1f7df-159">replace</span></span> | <p><span data-ttu-id="1f7df-160">Заменяет целевой элемент указанным содержимым.</span><span class="sxs-lookup"><span data-stu-id="1f7df-160">Replaces the target with the supplied content.</span></span></p><p><span data-ttu-id="1f7df-161">Для большинства действий **replace** необходимо использовать [сгенерированный идентификатор](#generated-ids) целевого элемента (кроме элементов **img** и **object** внутри разделителя, которые также поддерживают использование **data-id**).</span><span class="sxs-lookup"><span data-stu-id="1f7df-161">Most **replace** actions require using the [generated ID](#generated-ids) for the target (except **img** and **object** elements within a div, which also support using **data-id**).</span></span></p> |  
 
<span data-ttu-id="1f7df-162">**position**</span><span class="sxs-lookup"><span data-stu-id="1f7df-162">**position**</span></span>  
<span data-ttu-id="1f7df-163">Расположение относительно целевого элемента, куда нужно добавить указанное содержимое.</span><span class="sxs-lookup"><span data-stu-id="1f7df-163">The location to add the supplied content, relative to the target element. Possible values are:  (default) or .</span></span> <span data-ttu-id="1f7df-164">Если этот атрибут не указан, по умолчанию используется значение **after**.</span><span class="sxs-lookup"><span data-stu-id="1f7df-164">Defaults to **render** if omitted.</span></span>

| <span data-ttu-id="1f7df-165">Position</span><span class="sxs-lookup"><span data-stu-id="1f7df-165">Position</span></span> | <span data-ttu-id="1f7df-166">Описание</span><span class="sxs-lookup"><span data-stu-id="1f7df-166">Description</span></span> |  
|------|------|  
| <span data-ttu-id="1f7df-167">after (по умолчанию)</span><span class="sxs-lookup"><span data-stu-id="1f7df-167">after (default)</span></span> | <p><span data-ttu-id="1f7df-168">- С действием **append**: последний дочерний элемент целевого элемента.</span><span class="sxs-lookup"><span data-stu-id="1f7df-168">- With **append**: The last child of the target element.</span></span></p><p><span data-ttu-id="1f7df-169">- С действием **insert**: следующий элемент того же уровня, что и целевой элемент.</span><span class="sxs-lookup"><span data-stu-id="1f7df-169">**after** (default)- With append: The last child of the target element.- With insert: The subsequent sibling of the target element.</span></span></p> |
| <span data-ttu-id="1f7df-170">before</span><span class="sxs-lookup"><span data-stu-id="1f7df-170">Before</span></span> | <p><span data-ttu-id="1f7df-171">- С действием **append**: первый дочерний элемент целевого элемента.</span><span class="sxs-lookup"><span data-stu-id="1f7df-171">- With **append**: The first child of the target element.</span></span></p><p><span data-ttu-id="1f7df-172">- С действием **insert**: предыдущий элемент того же уровня, что и целевой элемент.</span><span class="sxs-lookup"><span data-stu-id="1f7df-172">**before**- With append: The first child of the target element.- With insert: The preceding sibling of the target element.</span></span></p> |

<span data-ttu-id="1f7df-173">**content**</span><span class="sxs-lookup"><span data-stu-id="1f7df-173">**content**</span></span>  
<span data-ttu-id="1f7df-174">Строка правильно оформленного HTML-кода, который нужно добавить на страницу, а также двоичные данные изображения или файла.</span><span class="sxs-lookup"><span data-stu-id="1f7df-174">A string of well-formed HTML to add to the page, and any image or file binary data. If the content contains binary data, the request must be sent using the  content type with a "Commands" part.</span></span> <span data-ttu-id="1f7df-175">Если в содержимом есть двоичные данные, необходимо отправить запрос с использованием типа контента `multipart/form-data` с частью Commands (см. [пример](#multipart-request-with-binary-content)).</span><span class="sxs-lookup"><span data-stu-id="1f7df-175">A string of well-formed HTML to add to the page and any image or file binary data. If the content contains binary data, the request must be sent using the multipart/form-data`multipart/form-data` content type with a "Commands" part (see an  [example](#multipart-request-with-binary-content)).</span></span> 
 

<a name="generated-ids"></a>

### <a name="generated-ids"></a><span data-ttu-id="1f7df-176">Сгенерированные идентификаторы</span><span class="sxs-lookup"><span data-stu-id="1f7df-176">Generated IDs</span></span>
<span data-ttu-id="1f7df-177">Microsoft Graph создает значения **id** для тех элементов на странице, которые можно обновить.</span><span class="sxs-lookup"><span data-stu-id="1f7df-177">Microsoft Graph generates **id** values for the elements on the page that can be updated.</span></span> <span data-ttu-id="1f7df-178">Чтобы получить сгенерированные идентификаторы, используйте выражение строки `includeIDs=true` в запросе GET:</span><span class="sxs-lookup"><span data-stu-id="1f7df-178">The onnvshort API generates id`includeIDs=true` values for page elements that can be updated. To get generated IDs, use the includeIDs=true query string expression in your GET request:</span></span>

`GET ../notes/pages/{page-id}/content?includeIDs=true` 

> <span data-ttu-id="1f7df-179">**Примечание.** API отклоняет все значения **id**, определенные во [входном HTML-коде](onenote_input_output_html.md) запросов create-page и update-page.</span><span class="sxs-lookup"><span data-stu-id="1f7df-179">**Note:** The API discards all **id** values that are defined in the [input HTML](onenote_input_output_html.md) of create-page and update-page requests.</span></span>

<span data-ttu-id="1f7df-180">Ниже показаны сгенерированные идентификаторы для абзаца и изображения в [выходном HTML-коде](onenote_input_output_html.md) страницы.</span><span class="sxs-lookup"><span data-stu-id="1f7df-180">The following example shows generated IDs for a paragraph and an image in the [output HTML](onenote_input_output_html.md) of a page.</span></span>

```html
<p id="p:{33f8a242-7c33-4bb2-90c5-8425a68cc5bf}{40}">Some text on the page</p>
<img id="img:{33f8a242-7c33-4bb2-90c5-8425a68cc5bf}{45}" ... />
```

<span data-ttu-id="1f7df-181">Сгенерированные значения **id** могут изменяться после обновления страницы, поэтому вам следует получить текущие значения до создания использующего их PATCH-запроса.</span><span class="sxs-lookup"><span data-stu-id="1f7df-181">Generated **id** values might change after a page update, so you should get the current values before building a PATCH request that uses them.</span></span>
 
<span data-ttu-id="1f7df-182">Вы можете указать целевые элементы, используя значение **data-id** или **id**, как указано ниже.</span><span class="sxs-lookup"><span data-stu-id="1f7df-182">You can specify target elements by using the **data-id** or **id** value, as follows:</span></span>

- <span data-ttu-id="1f7df-183">Для действий **append** и **insert** в качестве целевого значения можно использовать любой идентификатор.</span><span class="sxs-lookup"><span data-stu-id="1f7df-183">For **append** and **insert** actions, you can use either ID as the target value.</span></span>
- <span data-ttu-id="1f7df-184">Для действий **replace** необходимо использовать сгенерированный идентификатор для всех элементов, кроме заголовка, а также изображений и объектов, находящихся внутри разделителя.</span><span class="sxs-lookup"><span data-stu-id="1f7df-184">For **replace** actions, you must use the generated ID for all elements except for the page title and images and objects that are within a div. To replace a title, use the title keyword. To replace images and objects that are within a div, use either data-id or id.</span></span> 
    - <span data-ttu-id="1f7df-185">Чтобы заменить заголовок, используйте ключевое слово **title**.</span><span class="sxs-lookup"><span data-stu-id="1f7df-185">To replace a title, use the **title** keyword.</span></span> 
    - <span data-ttu-id="1f7df-186">Чтобы заменить изображения и объекты, находящиеся внутри разделителя, используйте атрибут **data-id** или **id**.</span><span class="sxs-lookup"><span data-stu-id="1f7df-186">To replace images and objects that are within a div, use either **data-id** or **id**.</span></span>

<span data-ttu-id="1f7df-187">В приведенном ниже примере используется значение **id** целевого элемента.</span><span class="sxs-lookup"><span data-stu-id="1f7df-187">The following example uses the **id** value for the target . Don't use the # prefix with a generated ID.</span></span> <span data-ttu-id="1f7df-188">Не используйте префикс # со сгенерированным идентификатором.</span><span class="sxs-lookup"><span data-stu-id="1f7df-188">The following example uses the id value for the target . Don't use the # prefix with a generated ID.</span></span>

```json
[
   {
    'target':'p:{33f8a242-7c33-4bb2-90c5-8425a68cc5bf}{40}',
    'action':'insert',
    'position':'before',
    'content':'<p>This paragraph goes above the target paragraph.</p>'
  }
]
```

<a name="support-matrix"></a>

## <a name="supported-elements-and-actions"></a><span data-ttu-id="1f7df-189">Поддерживаемые элементы и действия</span><span class="sxs-lookup"><span data-stu-id="1f7df-189">Supported elements and actions</span></span>
<span data-ttu-id="1f7df-190">Многие элементы на странице можно обновлять, но каждый тип элемента поддерживает определенные действия.</span><span class="sxs-lookup"><span data-stu-id="1f7df-190">Many elements on  the page can be updated, but each element type supports specific actions. The following table shows supported target elements and the update actions that they support.</span></span> <span data-ttu-id="1f7df-191">Ниже показаны поддерживаемые целевые элементы и поддерживаемые ими действия по обновлению.</span><span class="sxs-lookup"><span data-stu-id="1f7df-191">Many elements on  the page can be updated, but each element type supports specific actions. The following table shows supported target elements and the update actions that they support.</span></span>

| <span data-ttu-id="1f7df-192">Элемент</span><span class="sxs-lookup"><span data-stu-id="1f7df-192">Element</span></span> | <span data-ttu-id="1f7df-193">Заменить</span><span class="sxs-lookup"><span data-stu-id="1f7df-193">Replace</span></span> | <span data-ttu-id="1f7df-194">Добавление дочернего элемента</span><span class="sxs-lookup"><span data-stu-id="1f7df-194">Append child</span></span> | <span data-ttu-id="1f7df-195">Вставка элемента того же уровня</span><span class="sxs-lookup"><span data-stu-id="1f7df-195">Insert sibling</span></span> |  
|------|------|------|------|  
| <span data-ttu-id="1f7df-196">body</span><span class="sxs-lookup"><span data-stu-id="1f7df-196">body</span></span><br /> <span data-ttu-id="1f7df-197">(делает целевым первый разделитель на странице)</span><span class="sxs-lookup"><span data-stu-id="1f7df-197">body(targets first div on the page)</span></span> | <span data-ttu-id="1f7df-198">нет</span><span class="sxs-lookup"><span data-stu-id="1f7df-198">no</span></span> | <span data-ttu-id="1f7df-199">**да**</span><span class="sxs-lookup"><span data-stu-id="1f7df-199">**yes**</span></span> | <span data-ttu-id="1f7df-200">нет</span><span class="sxs-lookup"><span data-stu-id="1f7df-200">no</span></span> |  
| <span data-ttu-id="1f7df-201">div</span><span class="sxs-lookup"><span data-stu-id="1f7df-201">div</span></span><br /> <span data-ttu-id="1f7df-202">([абсолютное расположение](onenote-abs-pos.md))</span><span class="sxs-lookup"><span data-stu-id="1f7df-202">([absolute positioned](onenote-abs-pos.md))</span></span> | <span data-ttu-id="1f7df-203">нет</span><span class="sxs-lookup"><span data-stu-id="1f7df-203">no</span></span> | <span data-ttu-id="1f7df-204">**да**</span><span class="sxs-lookup"><span data-stu-id="1f7df-204">**yes**</span></span> | <span data-ttu-id="1f7df-205">нет</span><span class="sxs-lookup"><span data-stu-id="1f7df-205">no</span></span> |  
| <span data-ttu-id="1f7df-206">div</span><span class="sxs-lookup"><span data-stu-id="1f7df-206">div</span></span><br /> <span data-ttu-id="1f7df-207">(внутри разделителя)</span><span class="sxs-lookup"><span data-stu-id="1f7df-207">(within a div)</span></span> | <span data-ttu-id="1f7df-208">**да** (только идентификатор)</span><span class="sxs-lookup"><span data-stu-id="1f7df-208">**yes** (id only)</span></span> | <span data-ttu-id="1f7df-209">**да**</span><span class="sxs-lookup"><span data-stu-id="1f7df-209">**Yes**</span></span> | <span data-ttu-id="1f7df-210">**да**</span><span class="sxs-lookup"><span data-stu-id="1f7df-210">**Yes**</span></span> |   
| <span data-ttu-id="1f7df-211">img, object</span><span class="sxs-lookup"><span data-stu-id="1f7df-211">img, object</span></span><br /> <span data-ttu-id="1f7df-212">(внутри разделителя)</span><span class="sxs-lookup"><span data-stu-id="1f7df-212">(within a div)</span></span> | <span data-ttu-id="1f7df-213">**да**</span><span class="sxs-lookup"><span data-stu-id="1f7df-213">**yes**</span></span> | <span data-ttu-id="1f7df-214">нет</span><span class="sxs-lookup"><span data-stu-id="1f7df-214">no</span></span> | <span data-ttu-id="1f7df-215">**да**</span><span class="sxs-lookup"><span data-stu-id="1f7df-215">**yes**</span></span> |   
| <span data-ttu-id="1f7df-216">ol, ul</span><span class="sxs-lookup"><span data-stu-id="1f7df-216">ol, ul</span></span> | <span data-ttu-id="1f7df-217">**да** (только идентификатор)</span><span class="sxs-lookup"><span data-stu-id="1f7df-217">**yes** (id only)</span></span> | <span data-ttu-id="1f7df-218">**да**</span><span class="sxs-lookup"><span data-stu-id="1f7df-218">**Yes**</span></span> | <span data-ttu-id="1f7df-219">**да**</span><span class="sxs-lookup"><span data-stu-id="1f7df-219">**yes**</span></span> |   
| <span data-ttu-id="1f7df-220">table</span><span class="sxs-lookup"><span data-stu-id="1f7df-220">table</span></span> | <span data-ttu-id="1f7df-221">**да** (только идентификатор)</span><span class="sxs-lookup"><span data-stu-id="1f7df-221">**yes** (id only)</span></span> | <span data-ttu-id="1f7df-222">нет</span><span class="sxs-lookup"><span data-stu-id="1f7df-222">no</span></span> | <span data-ttu-id="1f7df-223">**да**</span><span class="sxs-lookup"><span data-stu-id="1f7df-223">**yes**</span></span> |   
| <span data-ttu-id="1f7df-224">p, li, h1-h6</span><span class="sxs-lookup"><span data-stu-id="1f7df-224">p, li, h1-h6</span></span> | <span data-ttu-id="1f7df-225">**да** (только идентификатор)</span><span class="sxs-lookup"><span data-stu-id="1f7df-225">**yes** (id only)</span></span> | <span data-ttu-id="1f7df-226">нет</span><span class="sxs-lookup"><span data-stu-id="1f7df-226">no</span></span> | <span data-ttu-id="1f7df-227">**да**</span><span class="sxs-lookup"><span data-stu-id="1f7df-227">**yes**</span></span> |   
| <span data-ttu-id="1f7df-228">title</span><span class="sxs-lookup"><span data-stu-id="1f7df-228">title</span></span> | <span data-ttu-id="1f7df-229">**да**</span><span class="sxs-lookup"><span data-stu-id="1f7df-229">**yes**</span></span> | <span data-ttu-id="1f7df-230">нет</span><span class="sxs-lookup"><span data-stu-id="1f7df-230">no</span></span> | <span data-ttu-id="1f7df-231">Нет</span><span class="sxs-lookup"><span data-stu-id="1f7df-231">no</span></span> |  
 

<span data-ttu-id="1f7df-232">Указанные ниже элементы не поддерживают никаких действий обновления.</span><span class="sxs-lookup"><span data-stu-id="1f7df-232">The following elements do not support any update actions.</span></span>

- <span data-ttu-id="1f7df-233">img ([абсолютное расположение](onenote-abs-pos.md))</span><span class="sxs-lookup"><span data-stu-id="1f7df-233">img ([absolute positioned](onenote-abs-pos.md))</span></span>
- <span data-ttu-id="1f7df-234">object ([абсолютное расположение](onenote-abs-pos.md))</span><span class="sxs-lookup"><span data-stu-id="1f7df-234">object ([absolute positioned](onenote-abs-pos.md))</span></span>
- <span data-ttu-id="1f7df-235">tr, td</span><span class="sxs-lookup"><span data-stu-id="1f7df-235">tr, td</span></span>
- <span data-ttu-id="1f7df-236">meta</span><span class="sxs-lookup"><span data-stu-id="1f7df-236">meta</span></span>
- <span data-ttu-id="1f7df-237">head</span><span class="sxs-lookup"><span data-stu-id="1f7df-237">head</span></span>
- <span data-ttu-id="1f7df-238">span</span><span class="sxs-lookup"><span data-stu-id="1f7df-238">span</span></span>
- <span data-ttu-id="1f7df-239">a</span><span class="sxs-lookup"><span data-stu-id="1f7df-239">a</span></span>
- <span data-ttu-id="1f7df-240">Теги style</span><span class="sxs-lookup"><span data-stu-id="1f7df-240">style tags</span></span>


<a name="examples"></a>
## <a name="example-requests"></a><span data-ttu-id="1f7df-241">Примеры запросов</span><span class="sxs-lookup"><span data-stu-id="1f7df-241">Example requests</span></span>
<span data-ttu-id="1f7df-242">Запрос на обновление содержит одно или несколько изменений, представленных в виде объектов JSON.</span><span class="sxs-lookup"><span data-stu-id="1f7df-242">An update request contains one or more changes represented as JSON change objects.</span></span> <span data-ttu-id="1f7df-243">Эти объекты могут определять различные целевые элементы на странице, а также различные действия и содержимое для целевых элементов.</span><span class="sxs-lookup"><span data-stu-id="1f7df-243">An update request contains one or more changes represented as JSON objects. These objects can define different targets on the page and different actions and content for the targets.</span></span>

<span data-ttu-id="1f7df-244">Следующие примеры включают объекты JSON, используемые в запросах PATCH, а также готовые запросы PATCH:</span><span class="sxs-lookup"><span data-stu-id="1f7df-244">The following examples include JSON objects used in PATCH requests and complete PATCH requests:</span></span>

<span data-ttu-id="1f7df-245">[Добавление дочерних элементов](#append-child-elements)&nbsp;&nbsp;|&nbsp;&nbsp;[Вставка элементов того же уровня](#insert-sibling-elements)&nbsp;&nbsp;|&nbsp;&nbsp;[Замена элементов](#replace-elements)&nbsp;&nbsp;|&nbsp;&nbsp;[Выполнение запросов PATCH](#complete-patch-request-examples)</span><span class="sxs-lookup"><span data-stu-id="1f7df-245">[Append child elements](#append-child-elements)&nbsp;&nbsp;|&nbsp;&nbsp;[Insert sibling elements](#insert-sibling-elements)&nbsp;&nbsp;|&nbsp;&nbsp;[Replace elements](#replace-elements)&nbsp;&nbsp;|&nbsp;&nbsp;[Complete PATCH requests](#complete-patch-request-examples)</span></span>


<a name="append-examples"></a>

### <a name="append-child-elements"></a><span data-ttu-id="1f7df-246">Добавление дочерних элементов</span><span class="sxs-lookup"><span data-stu-id="1f7df-246">Append  child elements</span></span>
<span data-ttu-id="1f7df-247">Действие **append** добавляет дочерний элемент к элементу **body**, **div** (внутри разделителя), **ol** или **ul**.</span><span class="sxs-lookup"><span data-stu-id="1f7df-247">The **append** action adds a child to a **body**, **div** (within a div), **ol**, or **ul** element. The position attribute determines whether to append the child before or after the target. The default position is after.</span></span> <span data-ttu-id="1f7df-248">Атрибут **position** определяет, где следует добавлять дочерний элемент: до или после целевого элемента.</span><span class="sxs-lookup"><span data-stu-id="1f7df-248">The **position** attribute determines whether to append the child before or after the target.</span></span> <span data-ttu-id="1f7df-249">По умолчанию задано положение **after**.</span><span class="sxs-lookup"><span data-stu-id="1f7df-249">The default position is **after**.</span></span>

#### <a name="append-to-a-div"></a><span data-ttu-id="1f7df-250">Добавление в разделитель</span><span class="sxs-lookup"><span data-stu-id="1f7df-250">Append to a  div</span></span>

<span data-ttu-id="1f7df-251">В приведенном ниже примере в элемент **div1** добавляется два дочерних узла.</span><span class="sxs-lookup"><span data-stu-id="1f7df-251">The following example adds two child nodes  to the **div1** element. It adds an image as the first child and a paragraph as the last child.</span></span> <span data-ttu-id="1f7df-252">Изображение добавляется в качестве первого дочернего элемента, а абзац — в качестве последнего.</span><span class="sxs-lookup"><span data-stu-id="1f7df-252">The following example adds two child nodes  to the div1 element. It adds an image as the first child and a paragraph as the last child.</span></span> 

```json
[
 {
    'target':'#div1',
    'action':'append',
    'position':'before',
    'content':'<img data-id="first-child" src="image-url-or-part-name" />'
  },
  {
    'target':'#div1',
    'action':'append',
    'content':'<p data-id="last-child">New paragraph appended to the div</p>'
  }
]
```
 

#### <a name="append-to-the-body-element"></a><span data-ttu-id="1f7df-253">Добавление к элементу *body*</span><span class="sxs-lookup"><span data-stu-id="1f7df-253">Append to the body element</span></span>

<span data-ttu-id="1f7df-254">Вы можете использовать сокращение **body** для добавления дочернего элемента внутри первого разделителя на любой странице.</span><span class="sxs-lookup"><span data-stu-id="1f7df-254">You can use the body target as a shortcut to append a child element inside the first div on any page.</span></span>

<span data-ttu-id="1f7df-255">В приведенном ниже примере в первый разделитель на странице добавляется два абзаца: один в качестве первого дочернего элемента, а другой — в качестве последнего.</span><span class="sxs-lookup"><span data-stu-id="1f7df-255">The following example adds two paragraphs as the first child and the last child to the first div on the page. Don't use a # with the body target. This example uses the prepend shortcut for append + before.</span></span> <span data-ttu-id="1f7df-256">Не используйте префикс # с целевым элементом **body**.</span><span class="sxs-lookup"><span data-stu-id="1f7df-256">Don't use a # with the **body** target.</span></span> <span data-ttu-id="1f7df-257">В этом примере действие **prepend** используется в качестве сокращения от действия **append** + **before**.</span><span class="sxs-lookup"><span data-stu-id="1f7df-257">This example uses the **prepend** action as a shortcut for **append** + **before**.</span></span>

```json
[
  {
    'target':'body',
    'action':'prepend',
    'content':'<p data-id="first-child">New paragraph as first child in the first div</p>'
  },
  {
    'target':'body',
    'action':'append',
    'content':'<p data-id="last-child">New paragraph as last child in the first div</p>'
  }
]
```
 

#### <a name="append-to-a-list"></a><span data-ttu-id="1f7df-258">Добавление в список</span><span class="sxs-lookup"><span data-stu-id="1f7df-258">Append to a list</span></span>

<span data-ttu-id="1f7df-259">В приведенном ниже примере элемент списка добавляется в качестве последнего дочернего элемента целевого списка.</span><span class="sxs-lookup"><span data-stu-id="1f7df-259">The following example adds a list item as a last child to the target list. The list-style-type property is defined because the item uses a non-default list style.</span></span> <span data-ttu-id="1f7df-260">В нем определяется свойство **list-style-type**, так как для элемента используется нестандартный стиль.</span><span class="sxs-lookup"><span data-stu-id="1f7df-260">The following example adds a list item as a last child to the target list. The **list-style-type** property is defined because the item uses a non-default list style.</span></span>

```json
[
  {
    'target':'#circle-ul',
    'action':'append',
    'content':'<li style="list-style-type:circle">Item at the end of the list</li>'
  }
]
```
 

<a name="insert-examples"></a>

### <a name="insert-sibling-elements"></a><span data-ttu-id="1f7df-261">Вставка элементов того же уровня</span><span class="sxs-lookup"><span data-stu-id="1f7df-261">Insert sibling elements</span></span>
<span data-ttu-id="1f7df-262">Действие **insert** добавляет элемент того же уровня в целевой элемент.</span><span class="sxs-lookup"><span data-stu-id="1f7df-262">The **insert** action adds a sibling to the target element.</span></span> <span data-ttu-id="1f7df-263">Атрибут **position** определяет, где следует вставлять элемент: до или после целевого элемента.</span><span class="sxs-lookup"><span data-stu-id="1f7df-263">The **position** attribute determines whether to insert the sibling before or after the target.</span></span> <span data-ttu-id="1f7df-264">По умолчанию задано положение **after**.</span><span class="sxs-lookup"><span data-stu-id="1f7df-264">The default position is **after**.</span></span> <span data-ttu-id="1f7df-265">См. [элементы, поддерживающие действие **insert**](#supported-elements-and-actions).</span><span class="sxs-lookup"><span data-stu-id="1f7df-265">See [elements that support **insert**](#supported-elements-and-actions).</span></span>

<span data-ttu-id="1f7df-266">**Вставка элементов того же уровня**</span><span class="sxs-lookup"><span data-stu-id="1f7df-266">**Insert siblings**</span></span>

<span data-ttu-id="1f7df-267">В приведенном ниже примере на страницу добавляется два узла того же уровня.</span><span class="sxs-lookup"><span data-stu-id="1f7df-267">The following example adds two sibling nodes to the page.</span></span> <span data-ttu-id="1f7df-268">Над элементом **para1** добавляется изображение, а под элементом **para2** — абзац.</span><span class="sxs-lookup"><span data-stu-id="1f7df-268">The following example adds two sibling nodes to the page. It adds an image above the **para1** element and a paragraph below the **para2** element.</span></span>

```json
[
  {
     'target':'#para1',
     'action':'insert',
     'position':'before',
     'content':'<img src="image-url-or-part-name" alt="Image inserted above the target" />'
  },
  {
    'target':'#para2',
     'action':'insert',
     'content':'<p data-id="next-sibling">Paragraph inserted below the target</p>'
  }
]
```
 

<a name="replace-examples"></a>

### <a name="replace-elements"></a><span data-ttu-id="1f7df-269">Замена элементов</span><span class="sxs-lookup"><span data-stu-id="1f7df-269">Replace elements</span></span>

<span data-ttu-id="1f7df-270">Вы можете использовать **data-id** или сгенерированный **id** в качестве целевого значения для замены элементов **img** и **object** внутри разделителя.</span><span class="sxs-lookup"><span data-stu-id="1f7df-270">You can use either the **data-id** or generated **id** as the target value to replace **img** and **object** elements that are within a div. To replace the page title, use the title keyword. For all other elements that support replace, you must use the generated ID.</span></span> <span data-ttu-id="1f7df-271">Чтобы заменить заголовок, используйте ключевое слово **title**.</span><span class="sxs-lookup"><span data-stu-id="1f7df-271">To replace the page title, use the **title** keyword.</span></span> <span data-ttu-id="1f7df-272">Для всех остальных [элементов, поддерживающих действие **replace**](#supported-elements-and-actions), необходимо использовать сгенерированный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="1f7df-272">For all other [elements that support **replace**](#supported-elements-and-actions), you must use the generated ID.</span></span>

#### <a name="replace-an-image"></a><span data-ttu-id="1f7df-273">Замена изображения</span><span class="sxs-lookup"><span data-stu-id="1f7df-273">Replace an image</span></span>

<span data-ttu-id="1f7df-274">В приведенном ниже примере изображение заменяется разделителем; в качестве целевого элемента используется **data-id** изображения.</span><span class="sxs-lookup"><span data-stu-id="1f7df-274">The following example replaces an image with a div by using the image's **data-id** as the target.</span></span> 

```json
[
  {
    'target':'#img1',
    'action':'replace',
    'content':'<div data-id="new-div"><p>This div replaces the image</p></div>'
  }
]
```
 

#### <a name="update-a-table"></a><span data-ttu-id="1f7df-275">Обновление таблицы</span><span class="sxs-lookup"><span data-stu-id="1f7df-275">Update a table</span></span> 

<span data-ttu-id="1f7df-276">В этом примере показано, как обновить таблицу, используя ее сгенерированный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="1f7df-276">This example shows how to update a table by using its generated ID. Replacing tr and td elements is not supported, but you can replace the entire table.</span></span> <span data-ttu-id="1f7df-277">Замена элементов **tr** и **td** не поддерживается, но вы можете заменить таблицу целиком.</span><span class="sxs-lookup"><span data-stu-id="1f7df-277">This example shows how to update a table by using its generated ID. Replacing **tr** and **td** elements is not supported, but you can replace the entire table.</span></span>

```json
[
  {
    'target':'table:{de3e0977-94e4-4bb0-8fee-0379eaf47486}{11}',
    'action':'replace',
    'content':'<table data-id="football">
      <tr><td><p><b>Brazil</b></p></td><td><p>Germany</p></td></tr>
      <tr><td><p>France</p></td><td><p><b>Italy</b></p></td></tr>
      <tr><td><p>Netherlands</p></td><td><p><b>Spain</b></p></td></tr>
      <tr><td><p>Argentina</p></td><td><p><b>Germany</b></p></td></tr></table>'
  }
]
```
 

#### <a name="change-the-title"></a><span data-ttu-id="1f7df-278">Изменение заголовка</span><span class="sxs-lookup"><span data-stu-id="1f7df-278">Change the title</span></span> 

<span data-ttu-id="1f7df-279">В этом примере показано, как изменить заголовок страницы.</span><span class="sxs-lookup"><span data-stu-id="1f7df-279">This example shows how to change the title of a page.</span></span> <span data-ttu-id="1f7df-280">Чтобы изменить заголовок, используйте ключевое слово **title** в качестве целевого значения.</span><span class="sxs-lookup"><span data-stu-id="1f7df-280">To change the title, use the **title** keyword as the target value.</span></span> <span data-ttu-id="1f7df-281">Не используйте префикс # в целевом заголовке.</span><span class="sxs-lookup"><span data-stu-id="1f7df-281">Don't use a # with the title target.</span></span>

```json
[
  {
    'target':'title',
    'action':'replace',
    'content':'New title'
  }
]
```
 

#### <a name="update-a-to-do-item"></a><span data-ttu-id="1f7df-282">Обновление элемента списка дел</span><span class="sxs-lookup"><span data-stu-id="1f7df-282">Update a to-do item</span></span>

<span data-ttu-id="1f7df-283">В приведенном ниже примере используется действие replace, чтобы перевести флажок в списке дел в состояние "Выполнено".</span><span class="sxs-lookup"><span data-stu-id="1f7df-283">The following example uses the replace action to change a to-do check box item to a completed state.</span></span>

```json
[
  {
    'target':'#task1',
    'action':'replace',
    'content':'<p data-tag="to-do:completed" data-id="task1">First task</p>'
  }
]
```

<span data-ttu-id="1f7df-284">Дополнительные сведения об использовании атрибута [data-tag](onenote-note-tags.md) см. в **этой статье**.</span><span class="sxs-lookup"><span data-stu-id="1f7df-284">See [Use note tags](onenote-note-tags.md) for more about using the **data-tag** attribute.</span></span>


<a name="complete-requests"></a>

### <a name="complete-patch-request-examples"></a><span data-ttu-id="1f7df-285">Примеры выполнения запросов PATCH</span><span class="sxs-lookup"><span data-stu-id="1f7df-285">Complete PATCH request examples</span></span>

<span data-ttu-id="1f7df-286">В следующих примерах показаны готовые запросы PATCH.</span><span class="sxs-lookup"><span data-stu-id="1f7df-286">The following examples show complete PATCH requests.</span></span>

#### <a name="request-with-text-content-only"></a><span data-ttu-id="1f7df-287">Запрос с текстовым содержимым</span><span class="sxs-lookup"><span data-stu-id="1f7df-287">Request with text content only</span></span>  
<span data-ttu-id="1f7df-288">В приведенном ниже примере показан запрос PATCH, в котором используется тип контента **application/json**.</span><span class="sxs-lookup"><span data-stu-id="1f7df-288">The following example shows a PATCH request that uses the   **application/json** content type. You can use this format when your content doesn't contain binary data.</span></span> <span data-ttu-id="1f7df-289">Этот формат можно использовать, если контент не содержит двоичных данных.</span><span class="sxs-lookup"><span data-stu-id="1f7df-289">The following example shows a PATCH request that uses the   application/json content type. You can use this format when your content doesn't contain binary data.</span></span>

```
PATCH https://graph.microsoft.com/v1.0/me/onenote/notebooks/pages/{page-id}/content

Content-Type: application/json
Authorization: Bearer {token}

[
   {
    'target':'#para-id',
    'action':'insert',
    'position':'before',
    'content':'<img src="image-url" alt="New image from a URL" />'
  }, 
  {
    'target':'#list-id',
    'action':'append',
    'content':'<li>Item at the bottom of the list</li>'
  }
]
```
 
<a name="multipart"></a>

#### <a name="multipart-request-with-binary-content"></a><span data-ttu-id="1f7df-290">Составной запрос с двоичным содержимым</span><span class="sxs-lookup"><span data-stu-id="1f7df-290">Multipart request with binary content</span></span> 

<span data-ttu-id="1f7df-291">В приведенном ниже примере показан составной запрос PATCH, включающий двоичные данные.</span><span class="sxs-lookup"><span data-stu-id="1f7df-291">The following example shows a multipart PATCH request that includes binary data.</span></span> <span data-ttu-id="1f7df-292">Составные запросы включают часть Commands, в которой указывается тип контента **application/json** и предоставляется массив объектов изменений JSON.</span><span class="sxs-lookup"><span data-stu-id="1f7df-292">Multipart requests require a "Commands" part that specifies the **application/json** content type and contains the array of JSON change objects.</span></span> <span data-ttu-id="1f7df-293">Другие части данных могут содержать двоичные данные.</span><span class="sxs-lookup"><span data-stu-id="1f7df-293">Other data parts can contain binary data.</span></span> <span data-ttu-id="1f7df-294">Как правило, имена частей представляют собой строки, к которым добавлено текущее время в миллисекундах или случайный GUID.</span><span class="sxs-lookup"><span data-stu-id="1f7df-294">Part names typically are strings appended with the current time in milliseconds or a random GUID.</span></span>

```
PATCH https://graph.microsoft.com/v1.0/me/onenote/notebooks/pages/{page-id}/content

Content-Type: multipart/form-data; boundary=PartBoundary123
Authorization: Bearer {token}

--PartBoundary123
Content-Disposition: form-data; name="Commands"
Content-Type: application/json

[
  {
    'target':'img:{2998967e-69b3-413f-a221-c1a3b5cbe0fc}{42}',
    'action':'replace',
    'content':'<img src="name:image-part-name" alt="New binary image" />'
  }, 
  {
    'target':'#list-id',
    'action':'append',
    'content':'<li>Item at the bottom of the list</li>'
  }
]

--PartBoundary123
Content-Disposition: form-data; name="image-part-name"
Content-Type: image/png

... binary image data ...

--PartBoundary123--
```

<a name="request-response-info"></a>

## <a name="request-and-response-information-for-patch-requests"></a><span data-ttu-id="1f7df-295">Информация о запросах PATCH и соответствующих ответах</span><span class="sxs-lookup"><span data-stu-id="1f7df-295">Request and response information for PATCH requests</span></span>

| <span data-ttu-id="1f7df-296">Данные запроса</span><span class="sxs-lookup"><span data-stu-id="1f7df-296">Request data</span></span> | <span data-ttu-id="1f7df-297">Описание</span><span class="sxs-lookup"><span data-stu-id="1f7df-297">Description</span></span> |  
|------|------|  
| <span data-ttu-id="1f7df-298">Протокол</span><span class="sxs-lookup"><span data-stu-id="1f7df-298">Protocol</span></span> | <span data-ttu-id="1f7df-299">Все запросы используют протокол SSL/TLS для HTTPS.</span><span class="sxs-lookup"><span data-stu-id="1f7df-299">All requests use the SSL/TLS HTTPS protocol.</span></span> |  
| <span data-ttu-id="1f7df-300">Заголовок авторизации</span><span class="sxs-lookup"><span data-stu-id="1f7df-300">Authorization header</span></span> | <p><span data-ttu-id="1f7df-301">`Bearer {token}`, где *{token}*  — это действительный маркер доступа OAuth 2.0 для зарегистрированного приложения.</span><span class="sxs-lookup"><span data-stu-id="1f7df-301">`Bearer {token}`, where *{token}* is a valid OAuth 2.0 access token for your registered app.</span></span></p><p><span data-ttu-id="1f7df-302">Если он отсутствует или является недействительным, произойдет сбой запроса с кодом состояния 401.</span><span class="sxs-lookup"><span data-stu-id="1f7df-302">If missing or invalid, the request fails with a 401 status code.</span></span> <span data-ttu-id="1f7df-303">См. статью [Проверка подлинности и разрешения](permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1f7df-303">See [Authentication and permissions](permissions_reference.md).</span></span></p> |  
| <span data-ttu-id="1f7df-304">Заголовок Content-Type</span><span class="sxs-lookup"><span data-stu-id="1f7df-304">content-type header</span></span> | <p><span data-ttu-id="1f7df-305">`application/json` для массива объектов изменений JSON, отправленного либо непосредственно в тексте сообщения, либо в обязательной части Commands [составных запросов](#multipart-request-with-binary-content).</span><span class="sxs-lookup"><span data-stu-id="1f7df-305">`application/json` for the array of JSON change objects, whether sent directly in the message body or in the required "Commands" part of [multipart requests](#multipart-request-with-binary-content).</span></span></p><p><span data-ttu-id="1f7df-306">Составные запросы необходимы при отправке двоичных данных. В них используется тип контента `multipart/form-data; boundary=part-boundary`, где *{part-boundary}*  — это строка, обозначающая начала и конец каждой части данных.</span><span class="sxs-lookup"><span data-stu-id="1f7df-306">Multipart requests are required when sending binary data, and use the `multipart/form-data; boundary=part-boundary` content type, where *{part-boundary}* is a string that signals the start and end of each data part.</span></span></p> |  
 

| <span data-ttu-id="1f7df-307">Данные ответа</span><span class="sxs-lookup"><span data-stu-id="1f7df-307">Response data</span></span> | <span data-ttu-id="1f7df-308">Описание</span><span class="sxs-lookup"><span data-stu-id="1f7df-308">Description</span></span> |  
|------|------|  
| <span data-ttu-id="1f7df-309">Код успешного завершения</span><span class="sxs-lookup"><span data-stu-id="1f7df-309">Success code</span></span> | <span data-ttu-id="1f7df-p131">Код состояния HTTP 204. Данные JSON не возвращаются по PATCH-запросу.</span><span class="sxs-lookup"><span data-stu-id="1f7df-p131">A 204 HTTP status code. No JSON data is returned for a PATCH request.</span></span> |  
| <span data-ttu-id="1f7df-312">Ошибки</span><span class="sxs-lookup"><span data-stu-id="1f7df-312">Errors</span></span> | <span data-ttu-id="1f7df-313">В статье [Коды ошибок для API OneNote в Microsoft Graph](onenote_error_codes.md) описываются ошибки OneNote, которые может возвращать Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1f7df-313">Read [Error codes for OneNote APIs in Microsoft Graph](onenote_error_codes.md) to learn about OneNote errors that Microsoft Graph can return.</span></span> |  
 
 

<a name="root-url"></a>

### <a name="constructing-the-microsoft-graph-service-root-url"></a><span data-ttu-id="1f7df-314">Составление корневого URL-адреса службы Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1f7df-314">Constructing the Microsoft Graph service root URL</span></span>

<a name="root-url"></a>

## <a name="root-url"></a><span data-ttu-id="1f7df-315">Корневой URL-адрес</span><span class="sxs-lookup"><span data-stu-id="1f7df-315">URL Root</span></span>
<span data-ttu-id="1f7df-316">Для всех вызовов API OneNote используется следующий формат корневого URL-адреса службы OneNote.</span><span class="sxs-lookup"><span data-stu-id="1f7df-316">The OneNote service root URL uses the following format for all calls to the OneNote API.</span></span>
`https://graph.microsoft.com/{version}/me/onenote/`

<span data-ttu-id="1f7df-317">Сегмент `version` URL-адреса представляет нужную версию Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1f7df-317">The `version` segment in the URL represents the version of Microsoft Graph that you want to use.</span></span>
- <span data-ttu-id="1f7df-318">Значение `v1.0` предназначено для стабильного производственного кода.</span><span class="sxs-lookup"><span data-stu-id="1f7df-318">`v1.0` is for stable production code.</span></span>
- <span data-ttu-id="1f7df-319">Используйте значение `beta`, чтобы опробовать функцию, находящуюся на стадии разработки.</span><span class="sxs-lookup"><span data-stu-id="1f7df-319">`beta` is to try out a feature that's in development.</span></span> <span data-ttu-id="1f7df-320">Функции бета-версии могут меняться, поэтому не следует использовать их в производственном коде.</span><span class="sxs-lookup"><span data-stu-id="1f7df-320">Features and functionality in beta may change, so you shouldn't use it in your production code.</span></span>
- <span data-ttu-id="1f7df-321">Значение `me` предназначено для содержимого OneNote, доступного текущему пользователю (если он является владельцем или с ним поделились этим содержимым).</span><span class="sxs-lookup"><span data-stu-id="1f7df-321">`me` is for OneNote content that the current user can access (owned and shared).</span></span>
- <span data-ttu-id="1f7df-322">Значение `users/{id}` предназначено для содержимого OneNote, которым указанный (в URL-адресе) пользователь поделился с текущим пользователем.</span><span class="sxs-lookup"><span data-stu-id="1f7df-322">`users/{id}` is for OneNote content that the specified user (in the URL) has shared with the current user.</span></span> <span data-ttu-id="1f7df-323">Использование [API Graph для Azure AD](https://msdn.microsoft.com/library/azure/ad/graph/api/api-catalog)</span><span class="sxs-lookup"><span data-stu-id="1f7df-323">Use the [Azure AD Graph API](https://msdn.microsoft.com/library/azure/ad/graph/api/api-catalog)</span></span>


> <span data-ttu-id="1f7df-324">**Примечание.** Вы можете получить идентификаторы пользователей, отправив запрос GET к конечной точке `https://graph.microsoft.com/v1.0/users`.</span><span class="sxs-lookup"><span data-stu-id="1f7df-324">**Note:** You can get user ids by making a GET request on `https://graph.microsoft.com/v1.0/users`.</span></span>



<a name="permissions"></a>

## <a name="permissions"></a><span data-ttu-id="1f7df-325">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1f7df-325">Permissions</span></span>

<span data-ttu-id="1f7df-326">Для обновления страниц OneNote необходимо запрашивать соответствующие разрешения.</span><span class="sxs-lookup"><span data-stu-id="1f7df-326">To update OneNote pages, you'll need to request appropriate permissions.</span></span> <span data-ttu-id="1f7df-327">Выберите минимальный уровень разрешений, необходимый для работы вашего приложения.</span><span class="sxs-lookup"><span data-stu-id="1f7df-327">Choose the lowest level of permissions that your app needs to do its work.</span></span>

- <span data-ttu-id="1f7df-328">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1f7df-328">Notes.ReadWrite</span></span>
- <span data-ttu-id="1f7df-329">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f7df-329">Notes.ReadWrite.All</span></span>

<span data-ttu-id="1f7df-330">Дополнительную информацию о разрешениях и принципе их работы см. в разделе [Разрешения OneNote](permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1f7df-330">For more information about how permission scopes work, see [OneNote permission scopes](permissions_reference.md).</span></span>
   

<a name="see-also"></a>

## <a name="additional-resources"></a><span data-ttu-id="1f7df-331">Дополнительные ресурсы</span><span class="sxs-lookup"><span data-stu-id="1f7df-331">Additional resources</span></span>

- [<span data-ttu-id="1f7df-332">Добавление изображений и файлов</span><span class="sxs-lookup"><span data-stu-id="1f7df-332">Add images and files</span></span>](onenote_images_files.md)
- [<span data-ttu-id="1f7df-333">Интеграция с OneNote</span><span class="sxs-lookup"><span data-stu-id="1f7df-333">Integrate with OneNote</span></span>](integrate_with_onenote.md)
- [<span data-ttu-id="1f7df-334">Блог разработчиков OneNote</span><span class="sxs-lookup"><span data-stu-id="1f7df-334">OneNote Developer Blog</span></span>](http://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="1f7df-335">Вопросы о разработке OneNote на сайте Stack Overflow</span><span class="sxs-lookup"><span data-stu-id="1f7df-335">OneNote development questions on Stack Overflow</span></span>](http://go.microsoft.com/fwlink/?LinkID=390182)
- [<span data-ttu-id="1f7df-336">Репозитории GitHub OneNote</span><span class="sxs-lookup"><span data-stu-id="1f7df-336">OneNote GitHub repos</span></span>](http://go.microsoft.com/fwlink/?LinkID=390178)  
