# <a name="update-onenote-page-content"></a><span data-ttu-id="fb41b-101">Обновление содержимого страниц OneNote</span><span class="sxs-lookup"><span data-stu-id="fb41b-101">Update OneNote page content</span></span>

<span data-ttu-id="fb41b-102">**Относится к:** обычные записные книжки в OneDrive | корпоративные записные книжки в Office 365</span><span class="sxs-lookup"><span data-stu-id="fb41b-102">**Applies to:** Consumer notebooks on OneDrive | Enterprise notebooks on Office 365</span></span>


<span data-ttu-id="fb41b-103">Чтобы обновить содержимое страницы OneNote, необходимо отправить запрос PATCH в конечную точку *content* страницы:</span><span class="sxs-lookup"><span data-stu-id="fb41b-103">To update the content of a OneNote page, you send a PATCH request to the page's *content* endpoint:</span></span>

`PATCH ../notes/pages/{id}/content`</p>

<span data-ttu-id="fb41b-104">Отправьте объект изменений JSON в тексте сообщения.</span><span class="sxs-lookup"><span data-stu-id="fb41b-104">Send a JSON change object in the message body.</span></span> <span data-ttu-id="fb41b-105">В случае успешного выполнения запроса Microsoft Graph возвращает код состояния HTTP 204.</span><span class="sxs-lookup"><span data-stu-id="fb41b-105">If the request is successful, the Microsoft Graph returns a 204 HTTP status code.</span></span>


<a name="request-uri"></a>

## <a name="construct-the-request-uri"></a><span data-ttu-id="fb41b-106">Создание URI запроса</span><span class="sxs-lookup"><span data-stu-id="fb41b-106">Construct the request URI</span></span>

<span data-ttu-id="fb41b-107">Чтобы создать URI запроса, начните с корневого URL-адреса службы:</span><span class="sxs-lookup"><span data-stu-id="fb41b-107">To construct the request URI, start with the service root URL:</span></span>

`https://graph.microsoft.com/v1.0/me/onenote`

<br/>

<span data-ttu-id="fb41b-108">Затем добавьте конечную точку *content* страницы:</span><span class="sxs-lookup"><span data-stu-id="fb41b-108">Then append the page's *content* endpoint:</span></span>

- <span data-ttu-id="fb41b-109">**Получение HTML-кода страницы и всех определенных значений *data-id***</span><span class="sxs-lookup"><span data-stu-id="fb41b-109">**Get the page HTML and all defined *data-id* values**</span></span><br/><br/>`../pages/{id}/content`   

- <span data-ttu-id="fb41b-110">**Получение HTML-кода страницы, всех определенных значений *data-id* и всех созданных значений *id***</span><span class="sxs-lookup"><span data-stu-id="fb41b-110">**Get the page HTML, all defined *data-id* values, and all generated *id* values**</span></span><br/><br/>`../pages/{page-id}/content?includeIDs=true` 

<span data-ttu-id="fb41b-111">Значения **data-id** и **id** используются в качестве идентификаторов **target** для элементов, которые требуется изменить.</span><span class="sxs-lookup"><span data-stu-id="fb41b-111">The **data-id** and **id** values are used as **target** identifiers for the elements you want to update.</span></span>

 
<span data-ttu-id="fb41b-112">Полный URI запроса будет выглядеть так:</span><span class="sxs-lookup"><span data-stu-id="fb41b-112">Your full request URI will look like this:</span></span><br/><br/>`https://graph.microsoft.com/v1.0/me/onenote/pages/{id}/content`


<span data-ttu-id="fb41b-113">Узнайте больше о [корневом URL-адресе службы](../api-reference/v1.0/resources/onenote-api-overview.md#root-url).</span><span class="sxs-lookup"><span data-stu-id="fb41b-113">Learn more about the [service root URL](../api-reference/v1.0/resources/onenote-api-overview.md#root-url).</span></span>


<a name="message-body"></a>

## <a name="construct-the-message-body"></a><span data-ttu-id="fb41b-114">Составление текста сообщения</span><span class="sxs-lookup"><span data-stu-id="fb41b-114">Construct the message body</span></span>

<span data-ttu-id="fb41b-115">HTML-код страницы OneNote содержит текст, изображения и другое содержимое, структурированные с помощью таких элементов, как **div**, **img** и **ol**.</span><span class="sxs-lookup"><span data-stu-id="fb41b-115">The HTML of a OneNote page contains text, images, and other content organized into structures such as **div**, **img**, and **ol** elements.</span></span> <span data-ttu-id="fb41b-116">Для обновления содержимого страницы OneNote необходимо добавлять и заменять элементы HTML на странице.</span><span class="sxs-lookup"><span data-stu-id="fb41b-116">To update OneNote page content, you add and replace HTML elements on the page.</span></span>

<span data-ttu-id="fb41b-117">Изменения отправляются в тексте сообщения в виде массива объектов JSON.</span><span class="sxs-lookup"><span data-stu-id="fb41b-117">Your changes are sent in the message body as an array of JSON change objects.</span></span> <span data-ttu-id="fb41b-118">В каждом объекте указываются целевой элемент, новое содержимое HTML и действия, которые нужно выполнить с содержимым.</span><span class="sxs-lookup"><span data-stu-id="fb41b-118">Each object specifies the target element, new HTML content, and what to do with the content.</span></span>

<span data-ttu-id="fb41b-p104">Следующий массив определяет два изменения. Первое вставляет изображение над абзацем в качестве элемента того же уровня, а второе добавляет элемент в список в качестве последнего дочернего элемента.</span><span class="sxs-lookup"><span data-stu-id="fb41b-p104">The following array defines two changes. The first inserts an image above a paragraph as a sibling, and the second appends an item to a list as a last child.</span></span>

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

<span data-ttu-id="fb41b-121">См. [другие примеры](#example-requests).</span><span class="sxs-lookup"><span data-stu-id="fb41b-121">See [more examples](#example-requests).</span></span>


### <a name="attributes-for-json-change-objects"></a><span data-ttu-id="fb41b-122">Атрибуты объектов JSON</span><span class="sxs-lookup"><span data-stu-id="fb41b-122">Attributes for JSON change objects</span></span>

<span data-ttu-id="fb41b-123">Для определения объектов JSON в запросах PATCH используются атрибуты **target**, **action**, **position** и **content**.</span><span class="sxs-lookup"><span data-stu-id="fb41b-123">Use the **target**, **action**, **position**, and **content** attributes to define JSON objects for PATCH requests.</span></span>

#### <a name="target"></a><span data-ttu-id="fb41b-124">target</span><span class="sxs-lookup"><span data-stu-id="fb41b-124">target</span></span>

<span data-ttu-id="fb41b-p105">Обновляемый элемент. Значением должен быть один из следующих идентификаторов:</span><span class="sxs-lookup"><span data-stu-id="fb41b-p105">The element to update. The value must be one of the following identifiers:</span></span>

| <span data-ttu-id="fb41b-127">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="fb41b-127">Identifier</span></span> | <span data-ttu-id="fb41b-128">Описание</span><span class="sxs-lookup"><span data-stu-id="fb41b-128">Description</span></span> |  
|------|------|  
| <span data-ttu-id="fb41b-129">#{data-id}</span><span class="sxs-lookup"><span data-stu-id="fb41b-129">#{data-id}</span></span> | <p><span data-ttu-id="fb41b-130">Этот идентификатор при желании определяется для элементов входного HTML-кода при [создании](onenote-create-page.md) или [обновлении страницы](onenote_update_page.md).</span><span class="sxs-lookup"><span data-stu-id="fb41b-130">This ID is optionally defined on elements in the input HTML when [creating a page](onenote-create-page.md) or [updating a page](onenote_update_page.md).</span></span> <span data-ttu-id="fb41b-131">Добавьте перед этим значением префикс #.</span><span class="sxs-lookup"><span data-stu-id="fb41b-131">Prefix the value with a #.</span></span></p><p> <span data-ttu-id="fb41b-132">Пример:</span><span class="sxs-lookup"><span data-stu-id="fb41b-132">Example:</span></span><br/><span data-ttu-id="fb41b-133">`'target':'#intro'` задает в качестве целевого элемент `<div data-id="intro" ...>`</span><span class="sxs-lookup"><span data-stu-id="fb41b-133">Example: `'target':'#intro'` targets the element `<div data-id="intro" ...>`</span></span></p> |  
| <span data-ttu-id="fb41b-134">id</span><span class="sxs-lookup"><span data-stu-id="fb41b-134">id</span></span> | <p><span data-ttu-id="fb41b-135">Это [сгенерированный идентификатор](#generated-ids) из Microsoft Graph, необходимый для большинства операций замены.</span><span class="sxs-lookup"><span data-stu-id="fb41b-135">This is the [generated ID](#generated-ids) from Microsoft Graph, and is required for most replace operations.</span></span> <span data-ttu-id="fb41b-136">Не добавляйте перед ним префикс #.</span><span class="sxs-lookup"><span data-stu-id="fb41b-136">Do not prefix with a #.</span></span></p><p> <span data-ttu-id="fb41b-137">Пример:</span><span class="sxs-lookup"><span data-stu-id="fb41b-137">Example:</span></span><br/><span data-ttu-id="fb41b-138">`'target':'div:{33f8a2...}{37}'` задает в качестве целевого элемент `<div id="div:{33f8a2...}{37}" ...>`</span><span class="sxs-lookup"><span data-stu-id="fb41b-138">Example: `'target':'div:{33f8a2...}{37}'` targets the element `<div id="div:{33f8a2...}{37}" ...>`</span></span></p><p><span data-ttu-id="fb41b-139">Не путайте эти идентификаторы со значениями **id**, определенными во [входном HTML-коде](onenote_input_output_html.md).</span><span class="sxs-lookup"><span data-stu-id="fb41b-139">Don't confuse these with any **id** values defined in the [input HTML](onenote_input_output_html.md).</span></span> <span data-ttu-id="fb41b-140">Все значения **id**, отправляемые во входном HTML-коде, отклоняются.</span><span class="sxs-lookup"><span data-stu-id="fb41b-140">All **id** values sent in the input HTML are discarded.</span></span></p> |  
| <span data-ttu-id="fb41b-141">body</span><span class="sxs-lookup"><span data-stu-id="fb41b-141">body</span></span> | <span data-ttu-id="fb41b-142">Ключевое слово, указывающее на первый разделитель на странице.</span><span class="sxs-lookup"><span data-stu-id="fb41b-142">The keyword that targets the first div on the page.</span></span> <span data-ttu-id="fb41b-143">Не добавляйте перед ним префикс #.</span><span class="sxs-lookup"><span data-stu-id="fb41b-143">Do not prefix with a #.</span></span> |  
| <span data-ttu-id="fb41b-144">title</span><span class="sxs-lookup"><span data-stu-id="fb41b-144">title</span></span> | <span data-ttu-id="fb41b-145">Ключевое слово, указывающее на заголовок страницы.</span><span class="sxs-lookup"><span data-stu-id="fb41b-145">The keyword that targets the page title.</span></span> <span data-ttu-id="fb41b-146">Не добавляйте перед ним префикс #.</span><span class="sxs-lookup"><span data-stu-id="fb41b-146">Do not prefix with a #.</span></span> |  
 
#### <a name="action"></a><span data-ttu-id="fb41b-147">action</span><span class="sxs-lookup"><span data-stu-id="fb41b-147">action</span></span>

<span data-ttu-id="fb41b-p111">Действие, которое нужно выполнить с целевым элементом. См. [поддерживаемые действия для элементов](#supported-elements-and-actions).</span><span class="sxs-lookup"><span data-stu-id="fb41b-p111">The action to perform on the target element. See [supported actions for elements](#supported-elements-and-actions).</span></span>

| <span data-ttu-id="fb41b-150">Действие</span><span class="sxs-lookup"><span data-stu-id="fb41b-150">Action</span></span> | <span data-ttu-id="fb41b-151">Описание</span><span class="sxs-lookup"><span data-stu-id="fb41b-151">Description</span></span> |  
|------|------|  
| <span data-ttu-id="fb41b-152">append</span><span class="sxs-lookup"><span data-stu-id="fb41b-152">append</span></span> | <p><span data-ttu-id="fb41b-153">Добавляет указанное содержимое к целевому элементу в качестве первого или последнего дочернего элемента, в зависимости от значения атрибута **position**.</span><span class="sxs-lookup"><span data-stu-id="fb41b-153">Adds the supplied content to the target as a first or last child, as determined by the **position** attribute.</span></span></p><p><span data-ttu-id="fb41b-154">Применяется только к элементам **body**, **div**, **ol** и **ul**.</span><span class="sxs-lookup"><span data-stu-id="fb41b-154">Applies only to **body**, **div**, **ol**, and **ul** elements.</span></span></p> |  
| <span data-ttu-id="fb41b-155">insert</span><span class="sxs-lookup"><span data-stu-id="fb41b-155">insert</span></span> | <span data-ttu-id="fb41b-156">Добавляет указанное содержимое в качестве элемента того же уровня перед целевым элементом или после него, в зависимости от значения атрибута **position**.</span><span class="sxs-lookup"><span data-stu-id="fb41b-156">Adds the supplied content as a sibling before or after the target, as determined by the **position** attribute.</span></span> |  
| <span data-ttu-id="fb41b-157">prepend</span><span class="sxs-lookup"><span data-stu-id="fb41b-157">prepend</span></span> | <p><span data-ttu-id="fb41b-158">Добавляет указанное содержимое к целевому элементу в качестве первого дочернего элемента.</span><span class="sxs-lookup"><span data-stu-id="fb41b-158">Adds the supplied content to the target as a first child.</span></span> <span data-ttu-id="fb41b-159">Сокращение от действия **append** + **before**.</span><span class="sxs-lookup"><span data-stu-id="fb41b-159">Shortcut for **append** + **before**.</span></span></p><p><span data-ttu-id="fb41b-160">Применяется только к элементам **body**, **div**, **ol** и **ul**.</span><span class="sxs-lookup"><span data-stu-id="fb41b-160">Applies only to **body**, **div**, **ol**, and **ul** elements.</span></span></p> |  
| <span data-ttu-id="fb41b-161">replace</span><span class="sxs-lookup"><span data-stu-id="fb41b-161">replace</span></span> | <p><span data-ttu-id="fb41b-162">Заменяет целевой элемент указанным содержимым.</span><span class="sxs-lookup"><span data-stu-id="fb41b-162">Replaces the target with the supplied content.</span></span></p><p><span data-ttu-id="fb41b-163">Для большинства действий **replace** необходимо использовать [сгенерированный идентификатор](#generated-ids) целевого элемента (кроме элементов **img** и **object** внутри разделителя, которые также поддерживают использование **data-id**).</span><span class="sxs-lookup"><span data-stu-id="fb41b-163">Most **replace** actions require using the [generated ID](#generated-ids) for the target (except **img** and **object** elements within a div, which also support using **data-id**).</span></span></p> |  
 
#### <a name="position"></a><span data-ttu-id="fb41b-164">position</span><span class="sxs-lookup"><span data-stu-id="fb41b-164">position</span></span>

<span data-ttu-id="fb41b-p113">Место для добавления предоставленного контента относительно целевого элемента. Если атрибут опущен, по умолчанию он принимает значение **after**.</span><span class="sxs-lookup"><span data-stu-id="fb41b-p113">The location to add the supplied content, relative to the target element. Defaults to **after** if omitted.</span></span>

| <span data-ttu-id="fb41b-167">Position</span><span class="sxs-lookup"><span data-stu-id="fb41b-167">Position</span></span> | <span data-ttu-id="fb41b-168">Описание</span><span class="sxs-lookup"><span data-stu-id="fb41b-168">Description</span></span> |  
|------|------|  
| <span data-ttu-id="fb41b-169">after (по умолчанию)</span><span class="sxs-lookup"><span data-stu-id="fb41b-169">after (default)</span></span> |<p><span data-ttu-id="fb41b-170">С действием **append**: последний дочерний элемент целевого элемента.</span><span class="sxs-lookup"><span data-stu-id="fb41b-170">- With **append**: The last child of the target element.</span></span></p><p><span data-ttu-id="fb41b-171">С действием **insert**: следующий элемент того же уровня, что и целевой элемент.</span><span class="sxs-lookup"><span data-stu-id="fb41b-171">- With **insert**: The subsequent sibling of the target element.</span></span></p> |
| <span data-ttu-id="fb41b-172">before</span><span class="sxs-lookup"><span data-stu-id="fb41b-172">before</span></span> | <p><span data-ttu-id="fb41b-173">С действием **append**: первый дочерний элемент целевого элемента.</span><span class="sxs-lookup"><span data-stu-id="fb41b-173">- With **append**: The first child of the target element.</span></span></p><p><span data-ttu-id="fb41b-174">С действием **insert**: предыдущий элемент того же уровня, что и целевой элемент.</span><span class="sxs-lookup"><span data-stu-id="fb41b-174">- With **insert**: The preceding sibling of the target element.</span></span></p> |

#### <a name="content"></a><span data-ttu-id="fb41b-175">content</span><span class="sxs-lookup"><span data-stu-id="fb41b-175">content</span></span>

<span data-ttu-id="fb41b-176">Строка правильно оформленного HTML-кода, который нужно добавить на страницу, а также двоичные данные изображения или файла.</span><span class="sxs-lookup"><span data-stu-id="fb41b-176">A string of well-formed HTML to add to the page, and any image or file binary data.</span></span> <span data-ttu-id="fb41b-177">Если в содержимом есть двоичные данные, необходимо отправить запрос с использованием типа контента `multipart/form-data` с частью Commands (см. [пример](#multipart-request-with-binary-content)).</span><span class="sxs-lookup"><span data-stu-id="fb41b-177">If the content contains binary data, the request must be sent using the `multipart/form-data` content type with a "Commands" part (see an [example](#multipart-request-with-binary-content)).</span></span> 
 

<a name="generated-ids"></a>

### <a name="generated-ids"></a><span data-ttu-id="fb41b-178">Сгенерированные идентификаторы</span><span class="sxs-lookup"><span data-stu-id="fb41b-178">Generated IDs</span></span>
<span data-ttu-id="fb41b-179">Microsoft Graph создает значения **id** для тех элементов на странице, которые можно обновить.</span><span class="sxs-lookup"><span data-stu-id="fb41b-179">Microsoft Graph generates **id** values for the elements on the page that can be updated.</span></span> <span data-ttu-id="fb41b-180">Чтобы получить сгенерированные идентификаторы, используйте выражение строки `includeIDs=true` в запросе GET:</span><span class="sxs-lookup"><span data-stu-id="fb41b-180">To get generated IDs, use the `includeIDs=true` query string expression in your GET request:</span></span>

`GET ../notes/pages/{page-id}/content?includeIDs=true` 

> <span data-ttu-id="fb41b-181">**Примечание.** API отклоняет все значения **id**, определенные во [входном HTML-коде](onenote_input_output_html.md) запросов create-page и update-page.</span><span class="sxs-lookup"><span data-stu-id="fb41b-181">**Note:** The API discards all **id** values that are defined in the [input HTML](onenote_input_output_html.md) of create-page and update-page requests.</span></span>

<span data-ttu-id="fb41b-182">Ниже показаны сгенерированные идентификаторы для абзаца и изображения в [выходном HTML-коде](onenote_input_output_html.md) страницы.</span><span class="sxs-lookup"><span data-stu-id="fb41b-182">The following example shows generated IDs for a paragraph and an image in the [output HTML](onenote_input_output_html.md) of a page.</span></span>

```html
<p id="p:{33f8a242-7c33-4bb2-90c5-8425a68cc5bf}{40}">Some text on the page</p>
<img id="img:{33f8a242-7c33-4bb2-90c5-8425a68cc5bf}{45}" ... />
```

<span data-ttu-id="fb41b-183">Сгенерированные значения **id** могут изменяться после обновления страницы, поэтому вам следует получить текущие значения до создания использующего их PATCH-запроса.</span><span class="sxs-lookup"><span data-stu-id="fb41b-183">Generated **id** values might change after a page update, so you should get the current values before building a PATCH request that uses them.</span></span>
 
<span data-ttu-id="fb41b-184">Вы можете указать целевые элементы, используя значение **data-id** или **id**, как указано ниже.</span><span class="sxs-lookup"><span data-stu-id="fb41b-184">You can specify target elements by using the **data-id** or **id** value, as follows:</span></span>

- <span data-ttu-id="fb41b-185">Для действий **append** и **insert** в качестве целевого значения можно использовать любой идентификатор.</span><span class="sxs-lookup"><span data-stu-id="fb41b-185">For **append** and **insert** actions, you can use either ID as the target value.</span></span>
- <span data-ttu-id="fb41b-186">Для действий **replace** необходимо использовать сгенерированный идентификатор для всех элементов, кроме заголовка, а также изображений и объектов, находящихся внутри разделителя.</span><span class="sxs-lookup"><span data-stu-id="fb41b-186">For **replace** actions, you must use the generated ID for all elements except for the page title and images and objects that are within a div.</span></span> 
    - <span data-ttu-id="fb41b-187">Чтобы заменить заголовок, используйте ключевое слово **title**.</span><span class="sxs-lookup"><span data-stu-id="fb41b-187">To replace a title, use the **title** keyword.</span></span> 
    - <span data-ttu-id="fb41b-188">Чтобы заменить изображения и объекты, находящиеся внутри разделителя, используйте атрибут **data-id** или **id**.</span><span class="sxs-lookup"><span data-stu-id="fb41b-188">To replace images and objects that are within a div, use either **data-id** or **id**.</span></span>

<span data-ttu-id="fb41b-189">В приведенном ниже примере используется значение **id** целевого элемента.</span><span class="sxs-lookup"><span data-stu-id="fb41b-189">The following example uses the **id** value for the target.</span></span> <span data-ttu-id="fb41b-190">Не используйте префикс # со сгенерированным идентификатором.</span><span class="sxs-lookup"><span data-stu-id="fb41b-190">Don't use the # prefix with a generated ID.</span></span>

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

## <a name="supported-elements-and-actions"></a><span data-ttu-id="fb41b-191">Поддерживаемые элементы и действия</span><span class="sxs-lookup"><span data-stu-id="fb41b-191">Supported elements and actions</span></span>

<span data-ttu-id="fb41b-192">Многие элементы на странице можно обновлять, но каждый тип элемента поддерживает определенные действия.</span><span class="sxs-lookup"><span data-stu-id="fb41b-192">Many elements on the page can be updated, but each element type supports specific actions.</span></span> <span data-ttu-id="fb41b-193">Ниже показаны поддерживаемые целевые элементы и поддерживаемые ими действия по обновлению.</span><span class="sxs-lookup"><span data-stu-id="fb41b-193">The following table shows supported target elements and the update actions that they support.</span></span>

| <span data-ttu-id="fb41b-194">Элемент</span><span class="sxs-lookup"><span data-stu-id="fb41b-194">Element</span></span> | <span data-ttu-id="fb41b-195">Заменить</span><span class="sxs-lookup"><span data-stu-id="fb41b-195">Replace</span></span> | <span data-ttu-id="fb41b-196">Добавление дочернего элемента</span><span class="sxs-lookup"><span data-stu-id="fb41b-196">Append child</span></span> | <span data-ttu-id="fb41b-197">Вставка элемента того же уровня</span><span class="sxs-lookup"><span data-stu-id="fb41b-197">Insert sibling</span></span> |  
|------|:------:|:------:|:------:|  
| <span data-ttu-id="fb41b-198">body</span><span class="sxs-lookup"><span data-stu-id="fb41b-198">body</span></span><br /> <span data-ttu-id="fb41b-199">(делает целевым первый разделитель на странице)</span><span class="sxs-lookup"><span data-stu-id="fb41b-199">(targets first div on the page)</span></span> | <span data-ttu-id="fb41b-200">нет</span><span class="sxs-lookup"><span data-stu-id="fb41b-200">no</span></span> | <span data-ttu-id="fb41b-201">**да**</span><span class="sxs-lookup"><span data-stu-id="fb41b-201">**yes**</span></span> | <span data-ttu-id="fb41b-202">нет</span><span class="sxs-lookup"><span data-stu-id="fb41b-202">no</span></span> |  
| <span data-ttu-id="fb41b-203">div</span><span class="sxs-lookup"><span data-stu-id="fb41b-203">div</span></span><br /> <span data-ttu-id="fb41b-204">([абсолютное расположение](onenote-abs-pos.md))</span><span class="sxs-lookup"><span data-stu-id="fb41b-204">([absolute positioned](onenote-abs-pos.md))</span></span> | <span data-ttu-id="fb41b-205">нет</span><span class="sxs-lookup"><span data-stu-id="fb41b-205">no</span></span> | <span data-ttu-id="fb41b-206">**да**</span><span class="sxs-lookup"><span data-stu-id="fb41b-206">**yes**</span></span> | <span data-ttu-id="fb41b-207">нет</span><span class="sxs-lookup"><span data-stu-id="fb41b-207">no</span></span> |  
| <span data-ttu-id="fb41b-208">div</span><span class="sxs-lookup"><span data-stu-id="fb41b-208">div</span></span><br /> <span data-ttu-id="fb41b-209">(внутри разделителя)</span><span class="sxs-lookup"><span data-stu-id="fb41b-209">(within a div)</span></span> | <span data-ttu-id="fb41b-210">**да**</span><span class="sxs-lookup"><span data-stu-id="fb41b-210">**yes**</span></span><br/><span data-ttu-id="fb41b-211">(только идентификатор)</span><span class="sxs-lookup"><span data-stu-id="fb41b-211">yes (id only)</span></span> | <span data-ttu-id="fb41b-212">**да**</span><span class="sxs-lookup"><span data-stu-id="fb41b-212">**yes**</span></span> | <span data-ttu-id="fb41b-213">**да**</span><span class="sxs-lookup"><span data-stu-id="fb41b-213">**yes**</span></span> |   
| <span data-ttu-id="fb41b-214">img, object</span><span class="sxs-lookup"><span data-stu-id="fb41b-214">img, object</span></span><br /> <span data-ttu-id="fb41b-215">(внутри разделителя)</span><span class="sxs-lookup"><span data-stu-id="fb41b-215">(within a div)</span></span> | <span data-ttu-id="fb41b-216">**да**</span><span class="sxs-lookup"><span data-stu-id="fb41b-216">**yes**</span></span> | <span data-ttu-id="fb41b-217">нет</span><span class="sxs-lookup"><span data-stu-id="fb41b-217">no</span></span> | <span data-ttu-id="fb41b-218">**да**</span><span class="sxs-lookup"><span data-stu-id="fb41b-218">**yes**</span></span> |   
| <span data-ttu-id="fb41b-219">ol, ul</span><span class="sxs-lookup"><span data-stu-id="fb41b-219">ol, ul</span></span> | <span data-ttu-id="fb41b-220">**да**</span><span class="sxs-lookup"><span data-stu-id="fb41b-220">**yes**</span></span><br/><span data-ttu-id="fb41b-221">(только идентификатор)</span><span class="sxs-lookup"><span data-stu-id="fb41b-221">yes (id only)</span></span> | <span data-ttu-id="fb41b-222">**да**</span><span class="sxs-lookup"><span data-stu-id="fb41b-222">**yes**</span></span> | <span data-ttu-id="fb41b-223">**да**</span><span class="sxs-lookup"><span data-stu-id="fb41b-223">**yes**</span></span> |   
| <span data-ttu-id="fb41b-224">table</span><span class="sxs-lookup"><span data-stu-id="fb41b-224">table</span></span> | <span data-ttu-id="fb41b-225">**да**</span><span class="sxs-lookup"><span data-stu-id="fb41b-225">**yes**</span></span><br/><span data-ttu-id="fb41b-226">(только идентификатор)</span><span class="sxs-lookup"><span data-stu-id="fb41b-226">yes (id only)</span></span> | <span data-ttu-id="fb41b-227">нет</span><span class="sxs-lookup"><span data-stu-id="fb41b-227">no</span></span> | <span data-ttu-id="fb41b-228">**да**</span><span class="sxs-lookup"><span data-stu-id="fb41b-228">**yes**</span></span> |   
| <span data-ttu-id="fb41b-229">p, li, h1-h6</span><span class="sxs-lookup"><span data-stu-id="fb41b-229">p, li, h1-h6</span></span> | <span data-ttu-id="fb41b-230">**да**</span><span class="sxs-lookup"><span data-stu-id="fb41b-230">**yes**</span></span><br/><span data-ttu-id="fb41b-231">(только идентификатор)</span><span class="sxs-lookup"><span data-stu-id="fb41b-231">yes (id only)</span></span> | <span data-ttu-id="fb41b-232">нет</span><span class="sxs-lookup"><span data-stu-id="fb41b-232">no</span></span> | <span data-ttu-id="fb41b-233">**да**</span><span class="sxs-lookup"><span data-stu-id="fb41b-233">**yes**</span></span> |   
| <span data-ttu-id="fb41b-234">title</span><span class="sxs-lookup"><span data-stu-id="fb41b-234">title</span></span> | <span data-ttu-id="fb41b-235">**да**</span><span class="sxs-lookup"><span data-stu-id="fb41b-235">**yes**</span></span> | <span data-ttu-id="fb41b-236">нет</span><span class="sxs-lookup"><span data-stu-id="fb41b-236">no</span></span> | <span data-ttu-id="fb41b-237">Нет</span><span class="sxs-lookup"><span data-stu-id="fb41b-237">no</span></span> |  
 
<br/>

<span data-ttu-id="fb41b-238">Указанные ниже элементы не поддерживают никаких действий обновления.</span><span class="sxs-lookup"><span data-stu-id="fb41b-238">The following elements do not support any update actions.</span></span>

- <span data-ttu-id="fb41b-239">img ([абсолютное расположение](onenote-abs-pos.md))</span><span class="sxs-lookup"><span data-stu-id="fb41b-239">img ([absolute positioned](onenote-abs-pos.md))</span></span>
- <span data-ttu-id="fb41b-240">object ([абсолютное расположение](onenote-abs-pos.md))</span><span class="sxs-lookup"><span data-stu-id="fb41b-240">object ([absolute positioned](onenote-abs-pos.md))</span></span>
- <span data-ttu-id="fb41b-241">tr, td</span><span class="sxs-lookup"><span data-stu-id="fb41b-241">tr, td</span></span>
- <span data-ttu-id="fb41b-242">meta</span><span class="sxs-lookup"><span data-stu-id="fb41b-242">meta</span></span>
- <span data-ttu-id="fb41b-243">head</span><span class="sxs-lookup"><span data-stu-id="fb41b-243">head</span></span>
- <span data-ttu-id="fb41b-244">span</span><span class="sxs-lookup"><span data-stu-id="fb41b-244">span</span></span>
- <span data-ttu-id="fb41b-245">a</span><span class="sxs-lookup"><span data-stu-id="fb41b-245">a</span></span>
- <span data-ttu-id="fb41b-246">Теги style</span><span class="sxs-lookup"><span data-stu-id="fb41b-246">style tags</span></span>


<a name="examples"></a>

## <a name="example-requests"></a><span data-ttu-id="fb41b-247">Примеры запросов</span><span class="sxs-lookup"><span data-stu-id="fb41b-247">Example requests</span></span>

<span data-ttu-id="fb41b-248">Запрос на обновление содержит одно или несколько изменений, представленных в виде объектов JSON.</span><span class="sxs-lookup"><span data-stu-id="fb41b-248">An update request contains one or more changes represented as JSON change objects.</span></span> <span data-ttu-id="fb41b-249">Эти объекты могут определять различные целевые элементы на странице, а также различные действия и содержимое для целевых элементов.</span><span class="sxs-lookup"><span data-stu-id="fb41b-249">These objects can define different targets on the page and different actions and content for the targets.</span></span>

<span data-ttu-id="fb41b-250">Следующие примеры включают объекты JSON, используемые в запросах PATCH, а также готовые запросы PATCH:</span><span class="sxs-lookup"><span data-stu-id="fb41b-250">The following examples include JSON objects used in PATCH requests and complete PATCH requests:</span></span>

- [<span data-ttu-id="fb41b-251">Добавление дочерних элементов</span><span class="sxs-lookup"><span data-stu-id="fb41b-251">Append child elements</span></span>](#append-child-elements)
- [<span data-ttu-id="fb41b-252">Вставка элементов того же уровня</span><span class="sxs-lookup"><span data-stu-id="fb41b-252">Insert sibling elements</span></span>](#insert-sibling-elements)
- [<span data-ttu-id="fb41b-253">Замена элементов</span><span class="sxs-lookup"><span data-stu-id="fb41b-253">Replace elements</span></span>](#replace-elements)
- [<span data-ttu-id="fb41b-254">Выполнение запросов PATCH</span><span class="sxs-lookup"><span data-stu-id="fb41b-254">Complete PATCH requests</span></span>](#complete-patch-request-examples)


<a name="append-examples"></a>

### <a name="append-child-elements"></a><span data-ttu-id="fb41b-255">Добавление дочерних элементов</span><span class="sxs-lookup"><span data-stu-id="fb41b-255">Append child elements</span></span>

<span data-ttu-id="fb41b-p119">Действие **append** добавляет дочерний элемент в элемент **body**, **div** (в составе разделителя), **ol** или **ul**. Атрибут **position** определяет, следует ли добавить дочерний элемент перед целевым элементом или после него. Расположение по умолчанию — **after**.</span><span class="sxs-lookup"><span data-stu-id="fb41b-p119">The **append** action adds a child to a **body**, **div** (within a div), **ol**, or **ul** element. The **position** attribute determines whether to append the child before or after the target. The default position is **after**.</span></span>

#### <a name="append-to-a-div"></a><span data-ttu-id="fb41b-259">Добавление в разделитель</span><span class="sxs-lookup"><span data-stu-id="fb41b-259">Append to a div</span></span>

<span data-ttu-id="fb41b-260">В приведенном ниже примере в элемент **div1** добавляется два дочерних узла.</span><span class="sxs-lookup"><span data-stu-id="fb41b-260">The following example adds two child nodes to the **div1** element.</span></span> <span data-ttu-id="fb41b-261">Изображение добавляется в качестве первого дочернего элемента, а абзац — в качестве последнего.</span><span class="sxs-lookup"><span data-stu-id="fb41b-261">It adds an image as the first child and a paragraph as the last child.</span></span> 

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
 

#### <a name="append-to-the-body-element"></a><span data-ttu-id="fb41b-262">Добавление к элементу *body*</span><span class="sxs-lookup"><span data-stu-id="fb41b-262">Append to the *body* element</span></span>

<span data-ttu-id="fb41b-263">Вы можете использовать сокращение **body** для добавления дочернего элемента внутри первого разделителя на любой странице.</span><span class="sxs-lookup"><span data-stu-id="fb41b-263">You can use the **body** shortcut to append a child element inside the first div on any page.</span></span>

<span data-ttu-id="fb41b-264">В приведенном ниже примере в первый разделитель на странице добавляется два абзаца: один в качестве первого дочернего элемента, а другой — в качестве последнего.</span><span class="sxs-lookup"><span data-stu-id="fb41b-264">The following example adds two paragraphs as the first child and the last child to the first div on the page.</span></span> <span data-ttu-id="fb41b-265">Не используйте префикс # с целевым элементом **body**.</span><span class="sxs-lookup"><span data-stu-id="fb41b-265">Don't use a # with the **body** target.</span></span> <span data-ttu-id="fb41b-266">В этом примере действие **prepend** используется в качестве сокращения от действия **append** + **before**.</span><span class="sxs-lookup"><span data-stu-id="fb41b-266">This example uses the **prepend** action as a shortcut for **append** + **before**.</span></span>

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
 

#### <a name="append-to-a-list"></a><span data-ttu-id="fb41b-267">Добавление в список</span><span class="sxs-lookup"><span data-stu-id="fb41b-267">Append to a list</span></span>

<span data-ttu-id="fb41b-p122">В следующем примере элемент списка добавляется в качестве последнего дочернего элемента к целевому списку. Свойство **list-style-type** определено, так как элемент использует стиль списка не по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="fb41b-p122">The following example adds a list item as a last child to the target list. The **list-style-type** property is defined because the item uses a non-default list style.</span></span>

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

### <a name="insert-sibling-elements"></a><span data-ttu-id="fb41b-270">Вставка элементов того же уровня</span><span class="sxs-lookup"><span data-stu-id="fb41b-270">Insert sibling elements</span></span>

<span data-ttu-id="fb41b-271">Действие **insert** добавляет элемент того же уровня в целевой элемент.</span><span class="sxs-lookup"><span data-stu-id="fb41b-271">The **insert** action adds a sibling to the target element.</span></span> <span data-ttu-id="fb41b-272">Атрибут **position** определяет, где следует вставлять элемент: до или после целевого элемента.</span><span class="sxs-lookup"><span data-stu-id="fb41b-272">The **position** attribute determines whether to insert the sibling before or after the target.</span></span> <span data-ttu-id="fb41b-273">По умолчанию задано положение **after**.</span><span class="sxs-lookup"><span data-stu-id="fb41b-273">The default position is **after**.</span></span> <span data-ttu-id="fb41b-274">См. [элементы, поддерживающие действие **insert**](#supported-elements-and-actions).</span><span class="sxs-lookup"><span data-stu-id="fb41b-274">See [elements that support **insert**](#supported-elements-and-actions).</span></span>

#### <a name="insert-siblings"></a><span data-ttu-id="fb41b-275">Вставка элементов того же уровня</span><span class="sxs-lookup"><span data-stu-id="fb41b-275">Insert siblings</span></span>

<span data-ttu-id="fb41b-p124">В следующем примере два узла того же уровня добавляются на страницу. Над элементом **para1** добавляется изображение, а под элементом **para2** — абзац.</span><span class="sxs-lookup"><span data-stu-id="fb41b-p124">The following example adds two sibling nodes to the page. It adds an image above the **para1** element and a paragraph below the **para2** element.</span></span>

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

### <a name="replace-elements"></a><span data-ttu-id="fb41b-278">Замена элементов</span><span class="sxs-lookup"><span data-stu-id="fb41b-278">Replace elements</span></span>

<span data-ttu-id="fb41b-279">Вы можете использовать **data-id** или сгенерированный **id** в качестве целевого значения для замены элементов **img** и **object** внутри разделителя.</span><span class="sxs-lookup"><span data-stu-id="fb41b-279">You can use either the **data-id** or generated **id** as the target value to replace **img** and **object** elements that are within a div.</span></span> <span data-ttu-id="fb41b-280">Чтобы заменить заголовок, используйте ключевое слово **title**.</span><span class="sxs-lookup"><span data-stu-id="fb41b-280">To replace the page title, use the **title** keyword.</span></span> <span data-ttu-id="fb41b-281">Для всех остальных [элементов, поддерживающих действие **replace**](#supported-elements-and-actions), необходимо использовать сгенерированный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="fb41b-281">For all other [elements that support **replace**](#supported-elements-and-actions), you must use the generated ID.</span></span>

#### <a name="replace-an-image"></a><span data-ttu-id="fb41b-282">Замена изображения</span><span class="sxs-lookup"><span data-stu-id="fb41b-282">Replace an image</span></span>

<span data-ttu-id="fb41b-283">В приведенном ниже примере изображение заменяется разделителем; в качестве целевого элемента используется **data-id** изображения.</span><span class="sxs-lookup"><span data-stu-id="fb41b-283">The following example replaces an image with a div by using the image's **data-id** as the target.</span></span> 

```json
[
  {
    'target':'#img1',
    'action':'replace',
    'content':'<div data-id="new-div"><p>This div replaces the image</p></div>'
  }
]
```
 

#### <a name="update-a-table"></a><span data-ttu-id="fb41b-284">Обновление таблицы</span><span class="sxs-lookup"><span data-stu-id="fb41b-284">Update a table</span></span> 

<span data-ttu-id="fb41b-p126">Этот пример демонстрирует, как обновить таблицу при помощи ее сгенерированного ИД. Замена элементов **tr** и **td** не поддерживается, но вы можете заменить таблицу целиком.</span><span class="sxs-lookup"><span data-stu-id="fb41b-p126">This example shows how to update a table by using its generated ID. Replacing **tr** and **td** elements is not supported, but you can replace the entire table.</span></span>

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
 

#### <a name="change-the-title"></a><span data-ttu-id="fb41b-287">Изменение заголовка</span><span class="sxs-lookup"><span data-stu-id="fb41b-287">Change the title</span></span> 

<span data-ttu-id="fb41b-288">В этом примере показано, как изменить заголовок страницы.</span><span class="sxs-lookup"><span data-stu-id="fb41b-288">This example shows how to change the title of a page.</span></span> <span data-ttu-id="fb41b-289">Чтобы изменить заголовок, используйте ключевое слово **title** в качестве целевого значения.</span><span class="sxs-lookup"><span data-stu-id="fb41b-289">To change the title, use the **title** keyword as the target value.</span></span> <span data-ttu-id="fb41b-290">Не используйте префикс # в целевом заголовке.</span><span class="sxs-lookup"><span data-stu-id="fb41b-290">Don't use a # with the title target.</span></span>

```json
[
  {
    'target':'title',
    'action':'replace',
    'content':'New title'
  }
]
```
 

#### <a name="update-a-to-do-item"></a><span data-ttu-id="fb41b-291">Обновление элемента списка дел</span><span class="sxs-lookup"><span data-stu-id="fb41b-291">Update a to-do item</span></span>

<span data-ttu-id="fb41b-292">В приведенном ниже примере используется действие replace, чтобы перевести флажок в списке дел в состояние "Выполнено".</span><span class="sxs-lookup"><span data-stu-id="fb41b-292">The following example uses the replace action to change a to-do check box item to a completed state.</span></span>

```json
[
  {
    'target':'#task1',
    'action':'replace',
    'content':'<p data-tag="to-do:completed" data-id="task1">First task</p>'
  }
]
```

<span data-ttu-id="fb41b-293">Дополнительные сведения об использовании атрибута [data-tag](onenote-note-tags.md) см. в **этой статье**.</span><span class="sxs-lookup"><span data-stu-id="fb41b-293">See [Use note tags](onenote-note-tags.md) for more about using the **data-tag** attribute.</span></span>


<a name="complete-requests"></a>

### <a name="complete-patch-request-examples"></a><span data-ttu-id="fb41b-294">Примеры выполнения запросов PATCH</span><span class="sxs-lookup"><span data-stu-id="fb41b-294">Complete PATCH request examples</span></span>

<span data-ttu-id="fb41b-295">В следующих примерах показаны готовые запросы PATCH.</span><span class="sxs-lookup"><span data-stu-id="fb41b-295">The following examples show complete PATCH requests.</span></span>

#### <a name="request-with-text-content-only"></a><span data-ttu-id="fb41b-296">Запрос с текстовым содержимым</span><span class="sxs-lookup"><span data-stu-id="fb41b-296">Request with text content only</span></span>

<span data-ttu-id="fb41b-297">В приведенном ниже примере показан запрос PATCH, в котором используется тип контента **application/json**.</span><span class="sxs-lookup"><span data-stu-id="fb41b-297">The following example shows a PATCH request that uses the **application/json** content type.</span></span> <span data-ttu-id="fb41b-298">Этот формат можно использовать, если контент не содержит двоичных данных.</span><span class="sxs-lookup"><span data-stu-id="fb41b-298">You can use this format when your content doesn't contain binary data.</span></span>

```json
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

#### <a name="multipart-request-with-binary-content"></a><span data-ttu-id="fb41b-299">Составной запрос с двоичным содержимым</span><span class="sxs-lookup"><span data-stu-id="fb41b-299">Multipart request with binary content</span></span> 

<span data-ttu-id="fb41b-300">В приведенном ниже примере показан составной запрос PATCH, включающий двоичные данные.</span><span class="sxs-lookup"><span data-stu-id="fb41b-300">The following example shows a multipart PATCH request that includes binary data.</span></span> <span data-ttu-id="fb41b-301">Составные запросы включают часть Commands, в которой указывается тип контента **application/json** и предоставляется массив объектов изменений JSON.</span><span class="sxs-lookup"><span data-stu-id="fb41b-301">Multipart requests require a "Commands" part that specifies the **application/json** content type and contains the array of JSON change objects.</span></span> <span data-ttu-id="fb41b-302">Другие части данных могут содержать двоичные данные.</span><span class="sxs-lookup"><span data-stu-id="fb41b-302">Other data parts can contain binary data.</span></span> <span data-ttu-id="fb41b-303">Как правило, имена частей представляют собой строки, к которым добавлено текущее время в миллисекундах или случайный GUID.</span><span class="sxs-lookup"><span data-stu-id="fb41b-303">Part names typically are strings appended with the current time in milliseconds or a random GUID.</span></span>

```json
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

## <a name="request-and-response-information-for-patch-requests"></a><span data-ttu-id="fb41b-304">Информация о запросах PATCH и соответствующих ответах</span><span class="sxs-lookup"><span data-stu-id="fb41b-304">Request and response information for PATCH requests</span></span>

| <span data-ttu-id="fb41b-305">Данные запроса</span><span class="sxs-lookup"><span data-stu-id="fb41b-305">Request data</span></span> | <span data-ttu-id="fb41b-306">Описание</span><span class="sxs-lookup"><span data-stu-id="fb41b-306">Description</span></span> |  
|------|------|  
| <span data-ttu-id="fb41b-307">Протокол</span><span class="sxs-lookup"><span data-stu-id="fb41b-307">Protocol</span></span> | <span data-ttu-id="fb41b-308">Все запросы используют протокол SSL/TLS для HTTPS.</span><span class="sxs-lookup"><span data-stu-id="fb41b-308">All requests use the SSL/TLS HTTPS protocol.</span></span> |  
| <span data-ttu-id="fb41b-309">Заголовок Authorization</span><span class="sxs-lookup"><span data-stu-id="fb41b-309">Authorization header</span></span> | <p><span data-ttu-id="fb41b-310">`Bearer {token}`, где `{token}` — действительный маркер доступа OAuth 2.0 для зарегистрированного приложения.</span><span class="sxs-lookup"><span data-stu-id="fb41b-310">`Bearer {token}`, where `{token}` is a valid OAuth 2.0 access token for your registered app.</span></span></p><p><span data-ttu-id="fb41b-311">Если он отсутствует или является недействительным, запрос завершится ошибкой с кодом состояния 401.</span><span class="sxs-lookup"><span data-stu-id="fb41b-311">If missing or invalid, the request fails with a 401 status code.</span></span> <span data-ttu-id="fb41b-312">См. статью [Проверка подлинности и разрешения](permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fb41b-312">See [Authentication and permissions](permissions_reference.md).</span></span></p> |  
| <span data-ttu-id="fb41b-313">Заголовок Content-Type</span><span class="sxs-lookup"><span data-stu-id="fb41b-313">Content-Type header</span></span> | <p><span data-ttu-id="fb41b-314">`application/json` для массива объектов изменений JSON, отправленного либо непосредственно в тексте сообщения, либо в обязательной части Commands [составных запросов](#multipart-request-with-binary-content).</span><span class="sxs-lookup"><span data-stu-id="fb41b-314">`application/json` for the array of JSON change objects, whether sent directly in the message body or in the required "Commands" part of [multipart requests](#multipart-request-with-binary-content).</span></span></p><p><span data-ttu-id="fb41b-315">При отправке двоичных данных необходимы составные запросы и использование типа содержимого `multipart/form-data; boundary=part-boundary`, где `{part-boundary}` представляет собой строку, которая сигнализирует начало и конец каждой части данных.</span><span class="sxs-lookup"><span data-stu-id="fb41b-315">Multipart requests are required when sending binary data, and use the `multipart/form-data; boundary=part-boundary` content type, where `{part-boundary}` is a string that signals the start and end of each data part.</span></span></p> |  

<br/> 

| <span data-ttu-id="fb41b-316">Данные в ответе</span><span class="sxs-lookup"><span data-stu-id="fb41b-316">Response data</span></span> | <span data-ttu-id="fb41b-317">Описание</span><span class="sxs-lookup"><span data-stu-id="fb41b-317">Description</span></span> |  
|------|------|  
| <span data-ttu-id="fb41b-318">Код успешного завершения</span><span class="sxs-lookup"><span data-stu-id="fb41b-318">Success code</span></span> | <span data-ttu-id="fb41b-p131">Код состояния HTTP 204. Данные JSON не возвращаются по PATCH-запросу.</span><span class="sxs-lookup"><span data-stu-id="fb41b-p131">A 204 HTTP status code. No JSON data is returned for a PATCH request.</span></span> |  
| <span data-ttu-id="fb41b-321">Ошибки</span><span class="sxs-lookup"><span data-stu-id="fb41b-321">Errors</span></span> | <span data-ttu-id="fb41b-322">В статье [Коды ошибок для API OneNote в Microsoft Graph](onenote_error_codes.md) описываются ошибки OneNote, которые может возвращать Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="fb41b-322">Read [Error codes for OneNote APIs in Microsoft Graph](onenote_error_codes.md) to learn about OneNote errors that Microsoft Graph can return.</span></span> |  
 
 

<a name="root-url"></a>

### <a name="constructing-the-microsoft-graph-service-root-url"></a><span data-ttu-id="fb41b-323">Составление корневого URL-адреса службы Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="fb41b-323">Constructing the Microsoft Graph service root URL</span></span>

<span data-ttu-id="fb41b-324">Для всех вызовов API OneNote используется следующий формат корневого URL-адреса службы OneNote:</span><span class="sxs-lookup"><span data-stu-id="fb41b-324">The OneNote service root URL uses the following format for all calls to the OneNote API.</span></span>

`https://graph.microsoft.com/{version}/me/onenote/`

<span data-ttu-id="fb41b-325">Сегмент `version` URL-адреса представляет нужную версию Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="fb41b-325">The `version` segment in the URL represents the version of Microsoft Graph that you want to use.</span></span> <span data-ttu-id="fb41b-326">Значение `v1.0` предназначено для стабильного производственного кода.</span><span class="sxs-lookup"><span data-stu-id="fb41b-326">`v1.0` is for stable production code.</span></span> <span data-ttu-id="fb41b-327">Используйте значение `beta`, чтобы опробовать функцию, находящуюся на стадии разработки.</span><span class="sxs-lookup"><span data-stu-id="fb41b-327">`beta` is to try out a feature that's in development.</span></span> <span data-ttu-id="fb41b-328">Функции бета-версии могут меняться, поэтому не следует использовать их в производственном коде.</span><span class="sxs-lookup"><span data-stu-id="fb41b-328">Features and functionality in beta may change, so you shouldn't use it in your production code.</span></span>

<span data-ttu-id="fb41b-329">Значение `me` предназначено для содержимого OneNote, доступного текущему пользователю (если он является владельцем или с ним поделились этим содержимым).</span><span class="sxs-lookup"><span data-stu-id="fb41b-329">`me` is for OneNote content that the current user can access (owned and shared).</span></span> <span data-ttu-id="fb41b-330">Значение `users/{id}` предназначено для содержимого OneNote, которым указанный (в URL-адресе) пользователь поделился с текущим пользователем.</span><span class="sxs-lookup"><span data-stu-id="fb41b-330">`users/{id}` is for OneNote content that the specified user (in the URL) has shared with the current user.</span></span> <span data-ttu-id="fb41b-331">Использование [API Graph для Azure AD](https://msdn.microsoft.com/library/azure/ad/graph/api/api-catalog)</span><span class="sxs-lookup"><span data-stu-id="fb41b-331">Use the [Azure AD Graph API](https://msdn.microsoft.com/library/azure/ad/graph/api/api-catalog)</span></span>


> <span data-ttu-id="fb41b-332">**Примечание.** Вы можете получить идентификаторы пользователей, отправив запрос GET к конечной точке `https://graph.microsoft.com/v1.0/users`.</span><span class="sxs-lookup"><span data-stu-id="fb41b-332">**Note:** You can get user ids by making a GET request on `https://graph.microsoft.com/v1.0/users`.</span></span>



<a name="permissions"></a>

## <a name="permissions"></a><span data-ttu-id="fb41b-333">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fb41b-333">Permissions</span></span>

<span data-ttu-id="fb41b-334">Для обновления страниц OneNote необходимо запрашивать соответствующие разрешения.</span><span class="sxs-lookup"><span data-stu-id="fb41b-334">To update OneNote pages, you'll need to request appropriate permissions.</span></span> <span data-ttu-id="fb41b-335">Выберите минимальный уровень разрешений, необходимый для работы вашего приложения.</span><span class="sxs-lookup"><span data-stu-id="fb41b-335">Choose the lowest level of permissions that your app needs to do its work.</span></span>

- <span data-ttu-id="fb41b-336">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fb41b-336">Notes.ReadWrite</span></span>
- <span data-ttu-id="fb41b-337">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb41b-337">Notes.ReadWrite.All</span></span>

<span data-ttu-id="fb41b-338">Дополнительные сведения об областях разрешений и принципе их работы см. в разделе [Области разрешений OneNote](permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fb41b-338">For more information about permission scopes and how they work, see [OneNote permission scopes](permissions_reference.md).</span></span>
   

<a name="see-also"></a>

## <a name="see-also"></a><span data-ttu-id="fb41b-339">См. также</span><span class="sxs-lookup"><span data-stu-id="fb41b-339">See also</span></span>

- [<span data-ttu-id="fb41b-340">Добавление изображений и файлов</span><span class="sxs-lookup"><span data-stu-id="fb41b-340">Add images and files</span></span>](onenote_images_files.md)
- [<span data-ttu-id="fb41b-341">Интеграция с OneNote</span><span class="sxs-lookup"><span data-stu-id="fb41b-341">Integrate with OneNote</span></span>](integrate_with_onenote.md)
- [<span data-ttu-id="fb41b-342">Блог разработчиков OneNote</span><span class="sxs-lookup"><span data-stu-id="fb41b-342">OneNote Developer Blog</span></span>](http://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="fb41b-343">Вопросы разработки OneNote на сайте Stack Overflow</span><span class="sxs-lookup"><span data-stu-id="fb41b-343">OneNote development questions on Stack Overflow</span></span>](http://go.microsoft.com/fwlink/?LinkID=390182)
- [<span data-ttu-id="fb41b-344">Репозитории GitHub OneNote</span><span class="sxs-lookup"><span data-stu-id="fb41b-344">OneNote GitHub repos</span></span>](http://go.microsoft.com/fwlink/?LinkID=390178)  
