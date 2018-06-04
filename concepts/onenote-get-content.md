# <a name="get-onenote-content-and-structure-with-microsoft-graph"></a><span data-ttu-id="3ca58-101">Получение содержимого и структуры OneNote с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="3ca58-101">Get OneNote content and structure with Microsoft Graph</span></span>

<span data-ttu-id="3ca58-102">*__Относится к:__ пользовательские записные книжки в OneDrive | корпоративные записные книжки в Office 365*</span><span class="sxs-lookup"><span data-stu-id="3ca58-102">*__Applies to:__ Consumer notebooks on OneDrive | Enterprise notebooks on Office 365*</span></span>

<span data-ttu-id="3ca58-103">Чтобы получить содержимое и структуру OneNote, необходимо отправить запрос GET к целевой конечной точке.</span><span class="sxs-lookup"><span data-stu-id="3ca58-103">To get OneNote content and structure, you send a GET request to the target endpoint.</span></span> <span data-ttu-id="3ca58-104">Пример:</span><span class="sxs-lookup"><span data-stu-id="3ca58-104">For example:</span></span>

`GET ../onenote/pages/{id}`</p>

<span data-ttu-id="3ca58-105">Если запрос выполнен успешно, Microsoft Graph возвращает код состояния HTTP 200 и запрашиваемые объекты или содержимое.</span><span class="sxs-lookup"><span data-stu-id="3ca58-105">If the request is successful, Microsoft Graph returns a 200 HTTP status code and the entities or content that you requested.</span></span> <span data-ttu-id="3ca58-106">Объекты OneNote возвращаются в виде объектов JSON, соответствующих спецификации OData версии 4.0.</span><span class="sxs-lookup"><span data-stu-id="3ca58-106">OneNote entities are returned as JSON objects that conform to the OData version 4.0 specification.</span></span>

<span data-ttu-id="3ca58-107">С помощью параметров строки запроса вы можете фильтровать запросы и повышать производительность.</span><span class="sxs-lookup"><span data-stu-id="3ca58-107">By using query string options, you can filter your queries and improve performance.</span></span>


<a name="request-uri"></a>
## <a name="construct-the-request-uri"></a><span data-ttu-id="3ca58-108">Создание URI запроса</span><span class="sxs-lookup"><span data-stu-id="3ca58-108">Construct the request</span></span>

<span data-ttu-id="3ca58-109">Чтобы создать URI запроса, начните с корневого URL-адреса службы:</span><span class="sxs-lookup"><span data-stu-id="3ca58-109">To construct the request URI, start with the service root URL:</span></span>

`https://graph.microsoft.com/v1.0/me/onenote`

<span data-ttu-id="3ca58-110">Затем добавьте конечную точку нужного ресурса.</span><span class="sxs-lookup"><span data-stu-id="3ca58-110">Then append the endpoint of the resource you want to retrieve.</span></span> <span data-ttu-id="3ca58-111">([Пути к ресурсам](#resource-paths-for-get-requests) показаны в следующем разделе.)</span><span class="sxs-lookup"><span data-stu-id="3ca58-111">([Resource paths](#resource-paths-for-get-requests) are shown in the next section.)</span></span>


<span data-ttu-id="3ca58-112">Полный URI запроса будет выглядеть так, как в одном из следующих примеров:</span><span class="sxs-lookup"><span data-stu-id="3ca58-112">Your full request URI will look like one of these examples:</span></span>
- `https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}/sections`</p>
- `https://graph.microsoft.com/v1.0/me/onenote/notes/pages`</p>
- `https://graph.microsoft.com/v1.0/me/onenote/pages?select=title,self`</p>

> <span data-ttu-id="3ca58-113">**Примечание.** Узнайте больше о [корневом URL-адресе службы](../api-reference/v1.0/resources/onenote-api-overview.md#root-url).</span><span class="sxs-lookup"><span data-stu-id="3ca58-113">**Note:** Learn more about the [service root URL](../api-reference/v1.0/resources/onenote-api-overview.md#root-url).</span></span>

<a name="resource-paths"></a>
## <a name="resource-paths-for-get-requests"></a><span data-ttu-id="3ca58-114">Пути к ресурсам для запросов GET</span><span class="sxs-lookup"><span data-stu-id="3ca58-114">Resource paths for GET requests</span></span>

<span data-ttu-id="3ca58-115">Используйте приведенные ниже пути к ресурсам, чтобы получать страницы, разделы, группы разделов, записные книжки, а также ресурсы изображений или файлов.</span><span class="sxs-lookup"><span data-stu-id="3ca58-115">Use the following resource paths to get pages, sections, section groups, notebooks, and image or file resources.</span></span>

<span data-ttu-id="3ca58-116">[Коллекция Page](#page-collection)&nbsp;&nbsp;|&nbsp;&nbsp;[Объект Page](#page-entity)&nbsp;&nbsp;|&nbsp;&nbsp;[Предварительный просмотр страницы](#page-preview)&nbsp;&nbsp;|&nbsp;&nbsp;[HTML-содержимое страницы](#page-html-content)&nbsp;&nbsp;|&nbsp;&nbsp; [Коллекция Section](#section-collection)&nbsp;&nbsp;|&nbsp;&nbsp;[Объект Section](#section-entity)&nbsp;&nbsp;|&nbsp;&nbsp;[Коллекция SectionGroup](#sectiongroup-collection)&nbsp;&nbsp;|&nbsp;&nbsp; [Объект SectionGroup](#sectiongroup-entity)&nbsp;&nbsp;|&nbsp;&nbsp;[Коллекция Notebook](#notebook-collection)&nbsp;&nbsp;|&nbsp;&nbsp;[Объект Notebook](#notebook-entity)&nbsp;&nbsp;|&nbsp;&nbsp; [Ресурс изображения или другого файла](#image-or-other-file-resource)</span><span class="sxs-lookup"><span data-stu-id="3ca58-116">[Page collection](#page-collection)&nbsp;&nbsp;|&nbsp;&nbsp;[Page entity](#page-entity)&nbsp;&nbsp;|&nbsp;&nbsp;[Page preview](#page-preview)&nbsp;&nbsp;|&nbsp;&nbsp;[Page HTML content](#page-html-content)&nbsp;&nbsp;|&nbsp;&nbsp; [Section collection](#section-collection)&nbsp;&nbsp;|&nbsp;&nbsp;[Section entity](#section-entity)&nbsp;&nbsp;|&nbsp;&nbsp;[SectionGroup collection](#sectiongroup-collection)&nbsp;&nbsp;|&nbsp;&nbsp; [SectionGroup entity](#sectiongroup-entity)&nbsp;&nbsp;|&nbsp;&nbsp;[Notebook collection](#notebook-collection)&nbsp;&nbsp;|&nbsp;&nbsp;[Notebook entity](#notebook-entity)&nbsp;&nbsp;|&nbsp;&nbsp; [Image or other file resource](#image-or-other-file-resource)</span></span>

<a name="get-pages"></a>
### <a name="page-collection"></a><span data-ttu-id="3ca58-117">Коллекция Page</span><span class="sxs-lookup"><span data-stu-id="3ca58-117">Page collection</span></span>

<span data-ttu-id="3ca58-118">Получение страниц (метаданных) из всех записных книжек</span><span class="sxs-lookup"><span data-stu-id="3ca58-118">Get pages (metadata) across all notebooks</span></span>

`../pages[?filter,orderby,select,expand,top,skip,search,count]`

<span data-ttu-id="3ca58-119">Получение страниц (метаданных) из определенного раздела</span><span class="sxs-lookup"><span data-stu-id="3ca58-119">Get pages (metadata) from a specific section</span></span>

`../sections/{section-id}/pages[?filter,orderby,select,expand,top,skip,search,count,pagelevel]`

 
<span data-ttu-id="3ca58-120">Параметр строки запроса `search` доступен только для пользовательских записных книжек.</span><span class="sxs-lookup"><span data-stu-id="3ca58-120">The `search` query string option is available for consumer notebooks only.</span></span>

<span data-ttu-id="3ca58-121">По умолчанию для страниц используется порядок сортировки `lastModifiedTime desc`.</span><span class="sxs-lookup"><span data-stu-id="3ca58-121">The default sort order is `lastModifiedTime desc`.</span></span>

<span data-ttu-id="3ca58-122">Запрос по умолчанию разворачивает родительский раздел и выбирает свойства `id`, `name` и `self` этого раздела.</span><span class="sxs-lookup"><span data-stu-id="3ca58-122">The default query expands the parent section and selects the section's `id`, `name`, and `self` properties.</span></span>

<span data-ttu-id="3ca58-123">По умолчанию в ответ на запросы *GET для страниц* возвращаются только первые 20 записей.</span><span class="sxs-lookup"><span data-stu-id="3ca58-123">By default, only the top 20 entries are returned for *GET pages* requests.</span></span> <span data-ttu-id="3ca58-124">В ответах на запросы, в которых не указан параметр **top**, возвращается ссылка **@odata.nextLink**, с помощью которой можно получить следующие 20 записей.</span><span class="sxs-lookup"><span data-stu-id="3ca58-124">GET requests for pages that retrieve the default number of entries (that is, they don’t specify a top expression) return an @odata.nextLink link in the response that you can use to get the next 20 entries.</span></span>

<span data-ttu-id="3ca58-125">Для коллекции страниц в разделе используйте параметр **pagelevel**, чтобы возвращать уровень отступа страниц и их порядок в разделе.</span><span class="sxs-lookup"><span data-stu-id="3ca58-125">For the pages collection in a section, use **pagelevel** to return the indentation level of pages and their order within the section.</span></span> 

<span data-ttu-id="3ca58-126">**Пример:**  `GET ../sections/{section-id}/pages?pagelevel=true`.</span><span class="sxs-lookup"><span data-stu-id="3ca58-126">Example</span></span>

- - -

<a name="get-page"></a> 
### <a name="page-entity"></a><span data-ttu-id="3ca58-127">Объект Page</span><span class="sxs-lookup"><span data-stu-id="3ca58-127">Page entity</span></span>

<span data-ttu-id="3ca58-128">Получение метаданных определенной страницы.</span><span class="sxs-lookup"><span data-stu-id="3ca58-128">Get the metadata for a folder.</span></span> 

`../pages/{page-id}[?select,expand,pagelevel]` 


<span data-ttu-id="3ca58-129">Запросы страниц могут разворачивать свойства **parentNotebook** и **parentSection**.</span><span class="sxs-lookup"><span data-stu-id="3ca58-129">Pages can expand the **parentNotebook** and **parentSection** properties.</span></span>

<span data-ttu-id="3ca58-130">Запрос по умолчанию разворачивает родительский раздел и выбирает свойства `id`, `name` и `self` этого раздела.</span><span class="sxs-lookup"><span data-stu-id="3ca58-130">The default query expands the parent section and selects the section's `id`, `name`, and `self` properties.</span></span>

<span data-ttu-id="3ca58-131">С помощью параметра **pagelevel** можно вернуть уровень отступа страницы и ее порядковый номер в родительском разделе.</span><span class="sxs-lookup"><span data-stu-id="3ca58-131">Use **pagelevel** to return the indentation level of the page and its order within its parent section.</span></span> <span data-ttu-id="3ca58-132">Пример: `GET ../pages/{page-id}?pagelevel=true`.</span><span class="sxs-lookup"><span data-stu-id="3ca58-132">Example:`GET ../pages/{page-id}?pagelevel=true` "\:"</span></span>

- - -

<a name="get-page-preview"></a> 
### <a name="page-preview"></a><span data-ttu-id="3ca58-133">Предварительный просмотр страницы</span><span class="sxs-lookup"><span data-stu-id="3ca58-133">Page preview</span></span>

<span data-ttu-id="3ca58-134">Получение образца текста и изображений на странице</span><span class="sxs-lookup"><span data-stu-id="3ca58-134">Get text and image preview content for a page</span></span>

`../pages/{page-id}/preview`


<span data-ttu-id="3ca58-135">Ответ JSON содержит образец содержимого, с помощью которого пользователи могут узнать, что находится на странице.</span><span class="sxs-lookup"><span data-stu-id="3ca58-135">The JSON response contains the preview content, which you can use to help users identify what's in the page.</span></span>

```json
{
  "@odata.context":"https://www.onenote.com/api/v1.0/$metadata#Microsoft.OneNote.Api.PagePreview",
  "previewText":"text-snippet",
  "links":{
    "previewImageUrl":{
      "href":"https://www.onenote.com/api/v1.0/resources/{id}/content?publicAuth=true&mimeType=image/png"
    }
  }
}
```

<span data-ttu-id="3ca58-136">Свойство **previewText** содержит фрагмент текста со страницы.</span><span class="sxs-lookup"><span data-stu-id="3ca58-136">The **previewText** property contains a text snippet from the page.</span></span> <span data-ttu-id="3ca58-137">Microsoft Graph возвращает полные фразы длиной до 300 символов.</span><span class="sxs-lookup"><span data-stu-id="3ca58-137">Microsoft Graph returns complete phrases, up to a maximum of 300 characters.</span></span> 

<span data-ttu-id="3ca58-138">Если на странице есть изображение, подходящее для предварительного просмотра, то свойство **href** объекта **previewImageUrl** будет содержать ссылку на общедоступный [ресурс изображения](#image-or-other-file-resource) с предварительной проверкой подлинности.</span><span class="sxs-lookup"><span data-stu-id="3ca58-138">If the page has an image that can be used to build a preview UI, the **href** property in the **previewImageUrl** object contains a link to a public, pre-authenticated [image resource](#image-or-other-file-resource).</span></span> <span data-ttu-id="3ca58-139">Эту ссылку можно использовать в коде HTML.</span><span class="sxs-lookup"><span data-stu-id="3ca58-139">You can use this link in HTML,</span></span>

<span data-ttu-id="3ca58-140">**Пример:** `<img src="https://www.onenote.com/api/v1.0/resources/{id}/content?publicAuth=true&mimeType=image/png" />`.</span><span class="sxs-lookup"><span data-stu-id="3ca58-140">Example</span></span> <span data-ttu-id="3ca58-141">В противном случае свойство **href** содержит значение null.</span><span class="sxs-lookup"><span data-stu-id="3ca58-141">Otherwise, **href** returns null.</span></span>

- - -

<a name="get-page-content"></a> 
### <a name="page-html-content"></a><span data-ttu-id="3ca58-142">HTML-содержимое страницы</span><span class="sxs-lookup"><span data-stu-id="3ca58-142">Page HTML content</span></span>

<span data-ttu-id="3ca58-143">Получение HTML-содержимого страницы `../pages/{page-id}/content[?includeIDs,preAuthenticated]`</span><span class="sxs-lookup"><span data-stu-id="3ca58-143">Get the HTML content of a page `../pages/{page-id}/content[?includeIDs,preAuthenticated]`</span></span>

<span data-ttu-id="3ca58-144">(*дополнительные сведения о [возвращаемом HTML-содержимом](onenote_input_output_html.md)*)</span><span class="sxs-lookup"><span data-stu-id="3ca58-144">(*learn more about [returned HTML content](onenote_input_output_html.md)*)</span></span> 

 
<span data-ttu-id="3ca58-145">Указав в строке запроса параметр **includeIDs=true**, можно получить созданные идентификаторы, используемые для [обновления страницы](onenote_update_page.md).</span><span class="sxs-lookup"><span data-stu-id="3ca58-145">Use the **includeIDs=true** query string option to get generated IDs used to [update the page](onenote_update_page.md).</span></span>

<span data-ttu-id="3ca58-146">Указав в строке запроса параметр **preAuthenticated=true**, можно получить общедоступные URL-адреса [ресурсов изображений](#image-or-other-file-resource) на странице.</span><span class="sxs-lookup"><span data-stu-id="3ca58-146">Use the **preAuthenticated=true** query string option to get public URLs to the [image resources](#image-or-other-file-resource) that are on the page.</span></span> <span data-ttu-id="3ca58-147">Общедоступные URL-адреса действительны в течение одного часа.</span><span class="sxs-lookup"><span data-stu-id="3ca58-147">The public URLs that are returned are valid for one hour.</span></span> 

- - -

<a name="get-sections"></a>
### <a name="section-collection"></a><span data-ttu-id="3ca58-148">Коллекция Section</span><span class="sxs-lookup"><span data-stu-id="3ca58-148">Section collection</span></span>

<span data-ttu-id="3ca58-149">Получение всех разделов всех записных книжек, принадлежащих пользователю, включая разделы из вложенных групп разделов `../sections[?filter,orderby,select,top,skip,expand,count]`</span><span class="sxs-lookup"><span data-stu-id="3ca58-149">Get all sections from all notebooks that are owned by the user, including sections in nested section groups `../sections[?filter,orderby,select,top,skip,expand,count]`</span></span> 

<span data-ttu-id="3ca58-150">Получение всех разделов, вложенных непосредственно в определенную группу разделов</span><span class="sxs-lookup"><span data-stu-id="3ca58-150">Get all sections that are directly under a specific section group</span></span>

`../sectionGroups/{sectiongroup-id}/sections[?filter,orderby,select,top,skip,expand,count]` 

<span data-ttu-id="3ca58-151">Получение всех разделов, вложенных непосредственно в определенную записную книжку `../notebooks/{notebook-id}/sections[?filter,orderby,select,top,skip,expand,count]`</span><span class="sxs-lookup"><span data-stu-id="3ca58-151">Get all sections that are directly under a specific notebook `../notebooks/{notebook-id}/sections[?filter,orderby,select,top,skip,expand,count]`</span></span> 

 
<span data-ttu-id="3ca58-152">Запросы разделов могут разворачивать свойства **parentNotebook** и **parentSectionGroup**.</span><span class="sxs-lookup"><span data-stu-id="3ca58-152">Sections can expand the **parentNotebook** and **parentSectionGroup** properties.</span></span>

<span data-ttu-id="3ca58-153">По умолчанию для разделов используется порядок сортировки `name asc`.</span><span class="sxs-lookup"><span data-stu-id="3ca58-153">The default sort order is `name asc`.</span></span>

<span data-ttu-id="3ca58-154">Запрос по умолчанию разворачивает родительскую записную книжку и родительскую группу разделов и выбирает их свойства `id`, `name` и `self`.</span><span class="sxs-lookup"><span data-stu-id="3ca58-154">The default query expands the parent notebook and parent section group and selects their `id`, `name`, and `self` properties.</span></span>

- - -

<a name="get-section"></a>
### <a name="section-entity"></a><span data-ttu-id="3ca58-155">Объект Section</span><span class="sxs-lookup"><span data-stu-id="3ca58-155">Section entity</span></span>

<span data-ttu-id="3ca58-156">Получение определенного раздела</span><span class="sxs-lookup"><span data-stu-id="3ca58-156">Get a specific entity</span></span>

`../sections/{section-id}[?select,expand]` 

 
<span data-ttu-id="3ca58-157">Запросы разделов могут разворачивать свойства **parentNotebook** и **parentSectionGroup**.</span><span class="sxs-lookup"><span data-stu-id="3ca58-157">Sections can expand the **parentNotebook** and **parentSectionGroup** properties.</span></span>

<span data-ttu-id="3ca58-158">Запрос по умолчанию разворачивает родительскую записную книжку и родительскую группу разделов и выбирает их свойства `id`, `name` и `self`.</span><span class="sxs-lookup"><span data-stu-id="3ca58-158">The default query expands the parent notebook and parent section group and selects their `id`, `name`, and `self` properties.</span></span>

- - -

<a name="get-section-groups"></a>
### <a name="sectiongroup-collection"></a><span data-ttu-id="3ca58-159">Коллекция SectionGroup</span><span class="sxs-lookup"><span data-stu-id="3ca58-159">SectionGroup collection</span></span>

<span data-ttu-id="3ca58-160">Получение всех групп разделов из всех записных книжек, принадлежащих пользователю, включая вложенные</span><span class="sxs-lookup"><span data-stu-id="3ca58-160">Get all section groups from all notebooks that are owned by the user, including nested section groups</span></span>

`../sectionGroups[?filter,orderby,select,top,skip,expand,count]` 

<span data-ttu-id="3ca58-161">Получение всех групп разделов, вложенных непосредственно в определенную записную книжку</span><span class="sxs-lookup"><span data-stu-id="3ca58-161">Get all section groups that are directly under a specific notebook</span></span> 

`../notebooks/{notebook-id}/sectionGroups[?filter,orderby,select,top,skip,expand,count]` 

<span data-ttu-id="3ca58-162">Запросы групп разделов могут разворачивать свойства **sections**, **sectionGroups**, **parentNotebook** и **parentSectionGroup**.</span><span class="sxs-lookup"><span data-stu-id="3ca58-162">Section groups can expand the **sections**, **sectionGroups**, **parentNotebook**, and **parentSectionGroup** properties.</span></span>

<span data-ttu-id="3ca58-163">По умолчанию для групп разделов используется порядок сортировки `name asc`.</span><span class="sxs-lookup"><span data-stu-id="3ca58-163">The default sort order for section groups is `name asc`.</span></span>

<span data-ttu-id="3ca58-164">Запрос по умолчанию разворачивает родительскую записную книжку и родительскую группу разделов и выбирает их свойства `id`, `name` и `self`.</span><span class="sxs-lookup"><span data-stu-id="3ca58-164">The default query expands the parent notebook and parent section group and selects their `id`, `name`, and `self` properties.</span></span>

- - -

<a name="get-section-group"></a>
### <a name="sectiongroup-entity"></a><span data-ttu-id="3ca58-165">Объект SectionGroup</span><span class="sxs-lookup"><span data-stu-id="3ca58-165">SectionGroup entity</span></span>

<span data-ttu-id="3ca58-166">Получение определенной группы разделов</span><span class="sxs-lookup"><span data-stu-id="3ca58-166">Get a specific section group and expand its sections and section groups.</span></span>

`../sectionGroups/{sectiongroup-id}[?select,expand]` 


<span data-ttu-id="3ca58-167">Запросы групп разделов могут разворачивать свойства **sections**, **sectionGroups**, **parentNotebook** и **parentSectionGroup**.</span><span class="sxs-lookup"><span data-stu-id="3ca58-167">Section groups can expand the **sections**, **sectionGroups**, **parentNotebook**, and **parentSectionGroup** properties.</span></span>

<span data-ttu-id="3ca58-168">Запрос по умолчанию разворачивает родительскую записную книжку и родительскую группу разделов и выбирает их свойства `id`, `name` и `self`.</span><span class="sxs-lookup"><span data-stu-id="3ca58-168">The default query expands the parent notebook and parent section group and selects their `id`, `name`, and `self` properties.</span></span>

- - -

<a name="get-notebooks"></a>
### <a name="notebook-collection"></a><span data-ttu-id="3ca58-169">Коллекция Notebook</span><span class="sxs-lookup"><span data-stu-id="3ca58-169">notebook collection</span></span>

<span data-ttu-id="3ca58-170">Получение всех записных книжек, принадлежащих пользователю</span><span class="sxs-lookup"><span data-stu-id="3ca58-170">Get all the notebooks that are owned by the user</span></span> 

`../notebooks[?filter,orderby,select,top,skip,expand,count]` 

 
<span data-ttu-id="3ca58-171">Запросы записных книжек могут разворачивать свойства **sections** и **sectionGroups**.</span><span class="sxs-lookup"><span data-stu-id="3ca58-171">Notebooks can expand the **sections** and **sectionGroups** properties.</span></span>

<span data-ttu-id="3ca58-172">По умолчанию для записных книжек используется порядок сортировки `name asc`.</span><span class="sxs-lookup"><span data-stu-id="3ca58-172">The default sort order is `name asc`.</span></span> 

- - -

<a name="get-notebook"></a>
### <a name="notebook-entity"></a><span data-ttu-id="3ca58-173">Объект Notebook</span><span class="sxs-lookup"><span data-stu-id="3ca58-173">Notebook entity</span></span>

<span data-ttu-id="3ca58-174">Получение определенной записной книжки `../notebooks/{notebook-id}[?select,expand]`</span><span class="sxs-lookup"><span data-stu-id="3ca58-174">Get a specific notebook `../notebooks/{notebook-id}[?select,expand]`</span></span> 


<span data-ttu-id="3ca58-175">Запросы записных книжек могут разворачивать свойства **sections** и **sectionGroups**.</span><span class="sxs-lookup"><span data-stu-id="3ca58-175">Notebooks can expand the **sections** and **sectionGroups** properties.</span></span>

- - -

<a name="get-resource"></a>
### <a name="image-or-other-file-resource"></a><span data-ttu-id="3ca58-176">Ресурс изображения или другого файла</span><span class="sxs-lookup"><span data-stu-id="3ca58-176">Image or other file resource</span></span>

<span data-ttu-id="3ca58-177">Получение двоичных данных определенного ресурса</span><span class="sxs-lookup"><span data-stu-id="3ca58-177">Get the binary data of a specific resource by sending a GET request to the resource's  endpoint:</span></span> 

`../resources/{resource-id}/$value` 


<span data-ttu-id="3ca58-178">URI ресурса файла можно найти в [выходном HTML-коде](onenote_input_output_html.md) страницы.</span><span class="sxs-lookup"><span data-stu-id="3ca58-178">You can find the file's resource URI in the page's [output HTML](onenote_input_output_html.md).</span></span>

<span data-ttu-id="3ca58-179">Например, тег **img** содержит конечные точки для исходного изображения в атрибуте **data-fullres-src** и оптимизированное изображение в атрибуте **src**.</span><span class="sxs-lookup"><span data-stu-id="3ca58-179">In the page HTML, an **** tag includes endpoints for the original image resource in the **** attribute and the optimized image in the **** attribute:</span></span> 

<span data-ttu-id="3ca58-180">**Пример:**</span><span class="sxs-lookup"><span data-stu-id="3ca58-180">**Example**</span></span>

```
<img 
    src="https://www.onenote.com/api/v1.0/me/notes/resources/{image-id}/$value"  
    data-src-type="image/png"
    data-fullres-src="https://www.onenote.com/api/v1.0/resources/{image-id}/$value"  
    data-fullres-src-type="image/png" ... />
```

<span data-ttu-id="3ca58-181">Тег **object** содержит конечную точку файлового ресурса в атрибуте **data**.</span><span class="sxs-lookup"><span data-stu-id="3ca58-181">And an **object** tag includes the endpoint for the file resource in the **data** attribute.</span></span> 

<span data-ttu-id="3ca58-182">**Пример:**</span><span class="sxs-lookup"><span data-stu-id="3ca58-182">**Example**</span></span>

```
<object
    data="http://www.onenote.com/api/v1.0/me/notes/resources/{file-id}/$value"
    data-attachment="fileName.pdf" 
    type="application/pdf" ... />
```

<span data-ttu-id="3ca58-183">Чтобы получить общедоступные URL-адреса изображений на странице с предварительной проверкой подлинности, включите параметр **preAuthenticated=true** в строку запроса при [получении содержимого страницы](#page-html-content) (**пример**: `GET ../pages/{page-id}/content?preAuthenticated=true`).</span><span class="sxs-lookup"><span data-stu-id="3ca58-183">To get public URLs to the image resources on a page, include preAuthenticated=true in the query string when you retrieve the page content (example: ).</span></span> <span data-ttu-id="3ca58-184">Возвращаемые в [выходном HTML-коде](onenote_input_output_html.md#output-html-examples-for-images) общедоступные URL-адреса действительны в течение одного часа.</span><span class="sxs-lookup"><span data-stu-id="3ca58-184">The public URLs that are returned are valid for one hour.</span></span> <span data-ttu-id="3ca58-185">Без этого флага полученные изображения не отображаются непосредственно в браузере, так как они являются личными и для их получения необходимо пройти проверку подлинности, как и для другого содержимого страницы.</span><span class="sxs-lookup"><span data-stu-id="3ca58-185">By default, images won't render directly in a browser because they are private and require authorization to retrieve them, like the rest of the page contents.</span></span> 

> <span data-ttu-id="3ca58-186">**Примечание.** Получение коллекции ресурсов не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ca58-186">**Note:** Getting a collection of resources is not supported.</span></span> 

<span data-ttu-id="3ca58-187">При получении файлового ресурса не требуется включать в запрос тип контента **Accept**.</span><span class="sxs-lookup"><span data-stu-id="3ca58-187">When you get a file resource, you don't need to include an **Accept** content type in the request.</span></span>

<span data-ttu-id="3ca58-188">Дополнительные сведения о запросах GET см. в следующих статьях:</span><span class="sxs-lookup"><span data-stu-id="3ca58-188">For more information about GET requests, see:</span></span> 
- [<span data-ttu-id="3ca58-189">GET Pages</span><span class="sxs-lookup"><span data-stu-id="3ca58-189">Get pages</span></span>](../api-reference/v1.0/api/page_get.md)
- [<span data-ttu-id="3ca58-190">GET Sections</span><span class="sxs-lookup"><span data-stu-id="3ca58-190">GET sections</span></span>](../api-reference/v1.0/api/section_get.md)
- [<span data-ttu-id="3ca58-191">GET SectionGroups</span><span class="sxs-lookup"><span data-stu-id="3ca58-191">GET sectiongroups</span></span>](../api-reference/v1.0/api/sectiongroup_get.md)
- [<span data-ttu-id="3ca58-192">GET Notebooks</span><span class="sxs-lookup"><span data-stu-id="3ca58-192">GET notebooks</span></span>](../api-reference/v1.0/api/notebook_get.md) 

<span data-ttu-id="3ca58-193">Все эти статьи входят в справочные материалы по REST API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="3ca58-193">in the Microsoft Graph API REST reference.</span></span>


<a name="example"></a>
## <a name="example-get-requests"></a><span data-ttu-id="3ca58-194">Примеры запросов GET</span><span class="sxs-lookup"><span data-stu-id="3ca58-194">Example GET requests</span></span>
<span data-ttu-id="3ca58-195">Вы можете запрашивать объекты OneNote и содержимое страницы поиска, чтобы получать только нужные вам сведения.</span><span class="sxs-lookup"><span data-stu-id="3ca58-195">You can query for OneNote entities and search page content to get just the information you need.</span></span> <span data-ttu-id="3ca58-196">Ниже показаны некоторые способы использования [поддерживаемых параметров строки](#supported-odata-query-string-options) в запросах GET к Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="3ca58-196">The following examples show some ways you can use [supported query string options](#supported-odata-query-string-options) in GET requests to Microsoft Graph.</span></span> 

<span data-ttu-id="3ca58-197">**Помните:**</span><span class="sxs-lookup"><span data-stu-id="3ca58-197">**Remember:**</span></span>

- <span data-ttu-id="3ca58-198">Все запросы GET начинаются с [корневого URL-адреса службы](../api-reference/v1.0/resources/onenote-api-overview.md#root-url).</span><span class="sxs-lookup"><span data-stu-id="3ca58-198">All GET requests start with the service root URL, for example:</span></span>

  <span data-ttu-id="3ca58-199">**Примеры:**</span><span class="sxs-lookup"><span data-stu-id="3ca58-199">**Examples**</span></span> 
  - `https://www.onenote.com/api/v1.0/me/notes`
  - `https://www.onenote.com/api/v1.0/myOrganization/siteCollections/{id}/sites/{id}/notes/`

- <span data-ttu-id="3ca58-200">Пробелы в строке запроса URL следует кодировать как %20.</span><span class="sxs-lookup"><span data-stu-id="3ca58-200">Spaces in the URL query string must be replaced with  the %20 encoding. Example:  filter=isDefault%20eq%20true</span></span>

<span data-ttu-id="3ca58-201">Пример: `filter=title%20eq%20'biology'`</span><span class="sxs-lookup"><span data-stu-id="3ca58-201">Example: `filter=title%20eq%20'biology'`</span></span>

- <span data-ttu-id="3ca58-202">Имена свойств и сравнения строк OData чувствительны к регистру.</span><span class="sxs-lookup"><span data-stu-id="3ca58-202">Property names and OData string comparisons are case sensitive.</span></span> <span data-ttu-id="3ca58-203">Рекомендуем использовать функцию OData **tolower** для сравнения строк.</span><span class="sxs-lookup"><span data-stu-id="3ca58-203">Property names and OData string comparisons are case sensitive. We recommend using the OData **tolower** function for string comparisons. Example: filter=tolower(name) eq 'spring'</span></span>

   <span data-ttu-id="3ca58-204">Пример: `filter=tolower(name) eq 'spring'`</span><span class="sxs-lookup"><span data-stu-id="3ca58-204">Example: `filter=tolower(name) eq 'spring'`</span></span>
 

<span data-ttu-id="3ca58-205">**search и filter**</span><span class="sxs-lookup"><span data-stu-id="3ca58-205">**search & filter**</span></span>  

<span data-ttu-id="3ca58-206">Получение всех страниц с термином *recipe*, созданных определенным приложением.</span><span class="sxs-lookup"><span data-stu-id="3ca58-206">Get all pages that contain the term *recipe* that were created by a specific app.</span></span>  <span data-ttu-id="3ca58-207">(Параметр `search` доступен только для пользовательских записных книжек.)</span><span class="sxs-lookup"><span data-stu-id="3ca58-207">(`search` is available for consumer notebooks only)</span></span>

```
[GET] ../pages?search=recipe&filter=createdByAppId eq 'WLID-000000004C12821A'
```
 
<span data-ttu-id="3ca58-208">**search и select**</span><span class="sxs-lookup"><span data-stu-id="3ca58-208">**search & select**</span></span>  

<span data-ttu-id="3ca58-209">Получение заголовка, клиентских ссылок OneNote и ссылки **contentUrl** для всех страниц, содержащих термин *golgi app*.</span><span class="sxs-lookup"><span data-stu-id="3ca58-209">Get the title, oncshort client links, and contentUrl link for all pages that contain the term golgi app.</span></span>  <span data-ttu-id="3ca58-210">(Параметр `search` доступен только для пользовательских записных книжек.)</span><span class="sxs-lookup"><span data-stu-id="3ca58-210">(`search` is available for consumer notebooks only)</span></span>

```
[GET] ../pages?search=golgi app&select=title,links,contentUrl
```
 
<span data-ttu-id="3ca58-211">**expand**</span><span class="sxs-lookup"><span data-stu-id="3ca58-211">**expand**</span></span>  

<span data-ttu-id="3ca58-212">Получение всех записных книжек, а также разворачивание их разделов и групп разделов.</span><span class="sxs-lookup"><span data-stu-id="3ca58-212">Get all notebooks and expand their sections and section groups.</span></span>  

```
[GET] ../notebooks?expand=sections,sectionGroups
```
 
<span data-ttu-id="3ca58-213">Получение определенной группы разделов и разворачивание ее разделов и групп разделов.</span><span class="sxs-lookup"><span data-stu-id="3ca58-213">Get a specific section group and expand its sections and section groups.</span></span>  

```
[GET] ../sectionGroups/{sectiongroup-id}?expand=sections,sectionGroups
```

<span data-ttu-id="3ca58-214">Получение страницы и разворачивание ее родительского раздела и родительской записной книжки.</span><span class="sxs-lookup"><span data-stu-id="3ca58-214">Get a page and expand its parent section and parent notebook.</span></span>

```
[GET] ../pages/{page-id}?expand=parentSection,parentNotebook
```

<span data-ttu-id="3ca58-215">**expand** (несколько уровней)</span><span class="sxs-lookup"><span data-stu-id="3ca58-215">expand (multiple levels)</span></span>  

<span data-ttu-id="3ca58-216">Получение всех записных книжек и разворачивание их разделов и групп, а также разворачивание всех разделов в каждой группе.</span><span class="sxs-lookup"><span data-stu-id="3ca58-216">Get all notebooks and expand their sections and section groups, and expand all sections in each section group.</span></span>  

```
[GET] ../notebooks?expand=sections,sectionGroups(expand=sections)
```
 
><span data-ttu-id="3ca58-217">Разворачивание родительских элементов или разворачивание дочерних элементов создает циклическую ссылку и не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ca58-217">Expanding parents of child entities or expanding children of parent entities creates a circular reference and  is not supported.</span></span>

 
<span data-ttu-id="3ca58-218">**expand и select** (несколько уровней)</span><span class="sxs-lookup"><span data-stu-id="3ca58-218">expand & select (multiple levels)</span></span>  

<span data-ttu-id="3ca58-219">Получение имени и ссылки **self** для определенной группы разделов, а также получение имени и ссылок **self** для всех ее разделов.</span><span class="sxs-lookup"><span data-stu-id="3ca58-219">Get the name and **self** link for a specific section group, and get the name and self links for all its sections.</span></span>  

```
[GET] ../sectionGroups/{sectiongroup-id}?expand=sections(select=name,self)&select=name,self
```
 
<span data-ttu-id="3ca58-220">Получение имени и ссылки **self** для всех разделов, а также получение имени и времени создания родительской записной книжки каждого раздела.</span><span class="sxs-lookup"><span data-stu-id="3ca58-220">Get the name and **self** link for all sections, and get the name and created time of its parent notebook.</span></span>  

```
[GET] ../sections?expand=parentNotebook(select=name,createdTime)&select=name,self
```
 
<span data-ttu-id="3ca58-221">Получение названий и идентификаторов всех страниц, а также получение названия родительского раздела и родительской записной книжки.</span><span class="sxs-lookup"><span data-stu-id="3ca58-221">Get the title and ID for all pages, and get the name of the parent section and parent notebook.</span></span>

```
[GET] ../pages?select=id,title&expand=parentSection(select=name),parentNotebook(select=name)
```

<span data-ttu-id="3ca58-222">**expand и levels** (несколько уровней)</span><span class="sxs-lookup"><span data-stu-id="3ca58-222">expand & levels (multiple levels)</span></span>  

<span data-ttu-id="3ca58-223">Получение всех записных книжек, разделов и групп разделов.</span><span class="sxs-lookup"><span data-stu-id="3ca58-223">Get all notebooks, sections, and section groups.</span></span>  

```
[GET] ../notebooks?expand=sections,sectionGroups(expand=sections,sectionGroups(levels=max;expand=sections))
```
 
<span data-ttu-id="3ca58-224">**filter**</span><span class="sxs-lookup"><span data-stu-id="3ca58-224">**filter**</span></span>  

<span data-ttu-id="3ca58-225">Получение всех разделов, созданных в октябре 2014 г.</span><span class="sxs-lookup"><span data-stu-id="3ca58-225">Get all sections that were created in October 2014.</span></span>

```
[GET] ../sections?filter=createdTime ge 2014-10-01 and createdTime le 2014-10-31
```

<span data-ttu-id="3ca58-226">Получение страниц, созданных определенным приложением с 1 января 2015 г.</span><span class="sxs-lookup"><span data-stu-id="3ca58-226">Get the pages that were created by a specific app since January 1, 2015.</span></span>

```
[GET] ../pages?filter=createdByAppId eq 'WLID-0000000048118631' and createdTime ge 2015-01-01
```

<span data-ttu-id="3ca58-227">**filter и expand**</span><span class="sxs-lookup"><span data-stu-id="3ca58-227">**filter & expand**</span></span>  

<span data-ttu-id="3ca58-228">Получение всех страниц определенной записной книжки.</span><span class="sxs-lookup"><span data-stu-id="3ca58-228">Get all pages in a specific notebook.</span></span> <span data-ttu-id="3ca58-229">По умолчанию API возвращает 20 записей.</span><span class="sxs-lookup"><span data-stu-id="3ca58-229">The API returns 20 entries by default.</span></span>

```
[GET] ../pages?filter=parentNotebook/id eq '{notebook-id}'&expand=parentNotebook
```

<span data-ttu-id="3ca58-230">Получение имени и ссылки **pagesUrl** для всех разделов в записной книжке *School*.</span><span class="sxs-lookup"><span data-stu-id="3ca58-230">Get the name and pagesUrl link for all sections in the user's default  notebook.</span></span> <span data-ttu-id="3ca58-231">При сравнении строк OData учитывается регистр, поэтому рекомендуем использовать функцию **tolower**.</span><span class="sxs-lookup"><span data-stu-id="3ca58-231">Get the name and **pagesUrl** link for all sections from the School notebook.  OData string comparisons are case sensitive, so use the tolower function as a best practice.</span></span>

```
[GET] ../notebooks?filter=tolower(name) eq 'school'&expand=sections(select=name,pagesUrl)
```

<span data-ttu-id="3ca58-232">**filter, select и orderby**</span><span class="sxs-lookup"><span data-stu-id="3ca58-232">**filter & select & orderby**</span></span>   

<span data-ttu-id="3ca58-233">Получение имени и ссылки **pagesUrl** для всех разделов, имена которых содержат термин *spring*.</span><span class="sxs-lookup"><span data-stu-id="3ca58-233">Get the name and **pagesUrl** link for  all sections that contain the term *spring* in the section name. Order sections by last modified date.</span></span> <span data-ttu-id="3ca58-234">Упорядочивание разделов по дате последнего изменения.</span><span class="sxs-lookup"><span data-stu-id="3ca58-234">Order sections by last modified date.</span></span>

```
[GET] ../sections?filter=contains(tolower(name),'spring')&select=name,pagesUrl&orderby=lastModifiedTime desc
```
 
<span data-ttu-id="3ca58-235">**orderby**</span><span class="sxs-lookup"><span data-stu-id="3ca58-235">**orderby**</span></span>  

<span data-ttu-id="3ca58-236">Получение первых 20 страниц, отсортированных по свойству **createdByAppId** и времени создания (по убыванию).</span><span class="sxs-lookup"><span data-stu-id="3ca58-236">Get the first  20 pages ordered by **createdByAppId** property and then by most recent created time. The API returns 20 pages by default.</span></span> <span data-ttu-id="3ca58-237">По умолчанию API возвращает 20 записей.</span><span class="sxs-lookup"><span data-stu-id="3ca58-237">The API returns 20 entries by default.</span></span>

```
[GET] ../pages?orderby=createdByAppId,createdTime desc
```

<span data-ttu-id="3ca58-238">**search, filter и top**</span><span class="sxs-lookup"><span data-stu-id="3ca58-238">**search & filter & top**</span></span>  

<span data-ttu-id="3ca58-239">Получение пяти последних страниц, созданных с 1 января 2015 г. и содержащих фразу *cell division*.</span><span class="sxs-lookup"><span data-stu-id="3ca58-239">Get the five  newest pages  created since January 1, 2015 that contain the phrase *cell division. The API returns 20 pages by default with a maximum of 100. The default sort order for pages lastModifiedTime desc*.</span></span> <span data-ttu-id="3ca58-240">По умолчанию API возвращает 20 записей. Максимальное количество записей — 100.</span><span class="sxs-lookup"><span data-stu-id="3ca58-240">Get pages 51 to 100. The API returns 20 entries by default with a maximum of 100.</span></span> <span data-ttu-id="3ca58-241">По умолчанию для страниц используется порядок сортировки `lastModifiedTime desc`.</span><span class="sxs-lookup"><span data-stu-id="3ca58-241">The default sort order is `lastModifiedTime desc`.</span></span> <span data-ttu-id="3ca58-242">(Параметр `search` доступен только для пользовательских записных книжек.)</span><span class="sxs-lookup"><span data-stu-id="3ca58-242">(`search` is available for consumer notebooks only)</span></span>

```
[GET] ../pages?search="cell division"&filter=createdTime ge 2015-01-01&top=5
```

<span data-ttu-id="3ca58-243">**search, filter, top и skip**</span><span class="sxs-lookup"><span data-stu-id="3ca58-243">**search & filter & top & skip**</span></span>  

<span data-ttu-id="3ca58-244">Получение следующих пяти страниц из набора результатов.</span><span class="sxs-lookup"><span data-stu-id="3ca58-244">Get the next five  pages  in the result set.</span></span> <span data-ttu-id="3ca58-245">(Параметр `search` доступен только для пользовательских записных книжек.)</span><span class="sxs-lookup"><span data-stu-id="3ca58-245">(`search` is available for consumer notebooks only)</span></span>

```
[GET] ../pages?search=biology&filter=createdTime ge 2015-01-01&top=5&skip=5
```

<span data-ttu-id="3ca58-246">И следующих пяти.</span><span class="sxs-lookup"><span data-stu-id="3ca58-246">And the next five.</span></span> <span data-ttu-id="3ca58-247">(Параметр `search` доступен только для пользовательских записных книжек.)</span><span class="sxs-lookup"><span data-stu-id="3ca58-247">(`search` is available for consumer notebooks only)</span></span>

```
[GET] ../pages?search=biology&filter=createdTime ge 2015-01-01&top=5&skip=10
```

> <span data-ttu-id="3ca58-248">**Примечание.** Если параметры **search** и **filter** применяются к одному запросу, результаты включают только те объекты, которые соответствуют обоим условиям.</span><span class="sxs-lookup"><span data-stu-id="3ca58-248">If both **search** and **filter** are applied to the same request, the results include only those entities that match both criteria.</span></span>
 
<span data-ttu-id="3ca58-249">**select**</span><span class="sxs-lookup"><span data-stu-id="3ca58-249">**select**</span></span>  

<span data-ttu-id="3ca58-250">Получение имени, времени создания и ссылки **self** для всех разделов в записных книжках пользователя.</span><span class="sxs-lookup"><span data-stu-id="3ca58-250">Get the name, created time, and **self** link for all sections in the user's notebooks.</span></span>

```
[GET] ../sections?select=name,createdTime,self
```

<span data-ttu-id="3ca58-251">Получение заголовка, времени создания и клиентских ссылок OneNote для определенной страницы.</span><span class="sxs-lookup"><span data-stu-id="3ca58-251">Get the title, created time, and oncshort client links for a specific page.</span></span>

```
[GET] ../pages/{page-id}?select=title,createdTime,links
```

<span data-ttu-id="3ca58-252">**select, expand и filter** (несколько уровней)</span><span class="sxs-lookup"><span data-stu-id="3ca58-252">select & expand & filter (multiple levels)</span></span>  

<span data-ttu-id="3ca58-253">Получение имени и ссылки **pagesUrl** для всех разделов в записной книжке пользователя по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="3ca58-253">Get the name and **pagesUrl** link for all sections in the user's default  notebook.</span></span>

```
[GET] ../notebooks?select=name&expand=sections(select=name,pagesUrl)&filter=isDefault eq true
```

<span data-ttu-id="3ca58-254">**top, select и orderby**</span><span class="sxs-lookup"><span data-stu-id="3ca58-254">**top & select & orderby**</span></span>  

<span data-ttu-id="3ca58-255">Получение названия и ссылки **self** для первых 50 страниц, упорядоченных по названию в алфавитном порядке.</span><span class="sxs-lookup"><span data-stu-id="3ca58-255">Get the title and **self** link for the first 50 pages, ordered alphabetically by title. The API returns 20 entries by default with a maximum of 100. The default sort order for pages lastModifiedTime desc.</span></span> <span data-ttu-id="3ca58-256">По умолчанию API возвращает 20 записей. Максимальное количество записей — 100.</span><span class="sxs-lookup"><span data-stu-id="3ca58-256">Get pages 51 to 100. The API returns 20 entries by default with a maximum of 100.</span></span> <span data-ttu-id="3ca58-257">По умолчанию для страниц используется порядок сортировки `lastModifiedTime desc`.</span><span class="sxs-lookup"><span data-stu-id="3ca58-257">The default sort order is `lastModifiedTime desc`.</span></span>

```
[GET] ../pages?top=50&select=title,self&orderby=title
```

<span data-ttu-id="3ca58-258">**skip, top, select и orderby**</span><span class="sxs-lookup"><span data-stu-id="3ca58-258">**skip & top & select & orderby**</span></span>  

<span data-ttu-id="3ca58-p123">Получение страниц с 51 по 100. По умолчанию API возвращает 20 записей, а максимальное количество составляет 100.</span><span class="sxs-lookup"><span data-stu-id="3ca58-p123">Get pages 51 to 100. The API returns 20 entries by default with a maximum of 100.</span></span>

```
[GET] ../pages?skip=50&top=50&select=title,self&orderby=title
```

> <span data-ttu-id="3ca58-261">**Примечание.** Запросы GET для страниц, которые получают количество записей по умолчанию (то есть в них не указывается выражение **top**), возвращают в ответе ссылку **@odata.nextLink**, с помощью которой можно получить следующие 20 записей.</span><span class="sxs-lookup"><span data-stu-id="3ca58-261">GET requests for **pages** that retrieve the default number of entries (that is, they don’t specify a **top** expression) return an @odata.nextLink link in the response that you can use to get the next 20 entries.</span></span>
 

<a name="query-options"></a>
## <a name="supported-odata-query-string-options"></a><span data-ttu-id="3ca58-262">Поддерживаемые параметры строки запроса OData</span><span class="sxs-lookup"><span data-stu-id="3ca58-262">Supported OData query string options</span></span>

<span data-ttu-id="3ca58-263">Вы можете настраивать запросы GET к Microsoft Graph, используя параметры строки запроса OData, и получать только нужную информацию.</span><span class="sxs-lookup"><span data-stu-id="3ca58-263">When sending GET requests to the onnvshort API, you can use OData query string options to customize your query and get just the information you need. They can also improve performance by reducing the number of calls to the service and the size of the response payload.</span></span> <span data-ttu-id="3ca58-264">Они также могут повышать производительность, уменьшая количество вызовов службы и размер полезных данных ответа.</span><span class="sxs-lookup"><span data-stu-id="3ca58-264">When sending GET requests to the onnvshort API, you can use OData query string options to customize your query and get just the information you need. They can also improve performance by reducing the number of calls to the service and the size of the response payload.</span></span>

> <span data-ttu-id="3ca58-265">**Примечание.** Для удобства чтения в примерах из этой статьи не используется код %20, которым нужно заменять пробелы в строке запроса URL: `filter=isDefault%20eq%20true`</span><span class="sxs-lookup"><span data-stu-id="3ca58-265">For readability, the examples in this article don't use the  %20`filter=isDefault%20eq%20true` percent-encoding required for spaces in the URL query string. Example:  filter=isDefault%20eq%20true</span></span>
 
| <span data-ttu-id="3ca58-266">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="3ca58-266">Query option</span></span> | <span data-ttu-id="3ca58-267">Пример и описание</span><span class="sxs-lookup"><span data-stu-id="3ca58-267">Example and description</span></span> |  
|------|------|  
| <span data-ttu-id="3ca58-268">count</span><span class="sxs-lookup"><span data-stu-id="3ca58-268">count</span></span> | <p>`count=true`</p><p><span data-ttu-id="3ca58-269">Количество объектов в коллекции.</span><span class="sxs-lookup"><span data-stu-id="3ca58-269">The count of entities in the collection.</span></span> <span data-ttu-id="3ca58-270">Значение возвращается в свойстве ответа **@odata.count**.</span><span class="sxs-lookup"><span data-stu-id="3ca58-270">The count of entities in the collection. The value is returned in the **@odata.count** property in the response.</span></span></p> |  
| <span data-ttu-id="3ca58-271">expand</span><span class="sxs-lookup"><span data-stu-id="3ca58-271">expand</span></span> | <p>`expand=sections,sectionGroups`</p><p><span data-ttu-id="3ca58-272">Свойства навигации, которые следует вернуть в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3ca58-272">The navigation properties to return inline  in the response. The following properties are supported for expand expressions:</span></span> <span data-ttu-id="3ca58-273">Для выражений **expand** поддерживаются следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="3ca58-273">The navigation properties to return inline  in the response. The following properties are supported for **expand** expressions:</span></span><br /> <span data-ttu-id="3ca58-274">— страницы: **parentNotebook**, **parentSection**;</span><span class="sxs-lookup"><span data-stu-id="3ca58-274">Pages: 
**parentNotebook**, **parentSection**</span></span><br /> <span data-ttu-id="3ca58-275">— разделы: **parentNotebook**, **parentSectionGroup**;</span><span class="sxs-lookup"><span data-stu-id="3ca58-275">Sections: 
**parentNotebook**, **parentSectionGroup**</span></span><br /> <span data-ttu-id="3ca58-276">— группы разделов: **sections**, **sectionGroups**, **parentNotebook**, **parentSectionGroup**;</span><span class="sxs-lookup"><span data-stu-id="3ca58-276">Section groups: 
**sections**, **sectionGroups**, **parentNotebook**, **parentSectionGroup**</span></span><br /> <span data-ttu-id="3ca58-277">— записные книжки: **sections**, **sectionGroups**.</span><span class="sxs-lookup"><span data-stu-id="3ca58-277">Notebooks: **sections**, **sectionGroups**</span></span></p><p><span data-ttu-id="3ca58-278">По умолчанию GET-запросы страниц разворачивают объект **parentSection** и выбирают свойства **id**, **name** и **self** этого раздела.</span><span class="sxs-lookup"><span data-stu-id="3ca58-278">By default, GET requests for pages expands **parentSection** and select the section's **id**, **name**, and **self** properties. Default GET requests for sections and section groups expand both parentNotebook and parentSectionGroup, and select the parents' id, name, and self properties.</span></span> <span data-ttu-id="3ca58-279">По умолчанию GET-запросы разделов и их групп разворачивают свойства **parentNotebook** и **parentSectionGroup**, а также выбирают свойства **id**, **name** и **self** родительского объекта.</span><span class="sxs-lookup"><span data-stu-id="3ca58-279">By default, GET requests for sections and section groups expand both **parentNotebook** and **parentSectionGroup**, and select the parents' **id**, **name**, and **self** properties.</span></span> </p><p><span data-ttu-id="3ca58-280">Может использоваться для одного объекта или коллекции.</span><span class="sxs-lookup"><span data-stu-id="3ca58-280">Can be used  for a single  entity or a collection. Separate  multiple properties with commas. Property names are case sensitive.</span></span> <span data-ttu-id="3ca58-281">Свойства следует разделять запятыми.</span><span class="sxs-lookup"><span data-stu-id="3ca58-281">Separate multiple properties with commas.</span></span> <span data-ttu-id="3ca58-282">В именах свойств учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="3ca58-282">The column names are case sensitive.</span></span></p> |   
| <span data-ttu-id="3ca58-283">filter</span><span class="sxs-lookup"><span data-stu-id="3ca58-283">filter</span></span> | <p>`filter=isDefault eq true`</p><p><span data-ttu-id="3ca58-284">Логическое выражение, указывающее, следует ли включать запись в набор результатов.</span><span class="sxs-lookup"><span data-stu-id="3ca58-284">A Boolean expression for whether to include an entry in the result set.</span></span> <span data-ttu-id="3ca58-285">Поддерживаются следующие функции и операторы OData:</span><span class="sxs-lookup"><span data-stu-id="3ca58-285">Supports the following OData operators and functions:</span></span><br /> <span data-ttu-id="3ca58-286">— операторы сравнения: **eq**, **ne**, **gt**, **ge**, **lt**, **le**;</span><span class="sxs-lookup"><span data-stu-id="3ca58-286">Comparison operators: eq, ne, gt, ge, lt, le</span></span><br /> <span data-ttu-id="3ca58-287">— логические операторы: **and**, **or**, **not**;</span><span class="sxs-lookup"><span data-stu-id="3ca58-287">- Logical operators: **and**, **or**, **not**</span></span><br /> <span data-ttu-id="3ca58-288">— строковые функции: **contains**, **endswith**, **startswith**, **length**, **indexof**, **substring**, **tolower**, **toupper**, **trim**, **concat**.</span><span class="sxs-lookup"><span data-stu-id="3ca58-288">- String functions: **contains**, **endswith**, **startswith**, **length**, **indexof**, **substring**, **tolower**, **toupper**, **trim**, **concat**</span></span></p><p><span data-ttu-id="3ca58-289">В именах [свойств](#onenote-entity-properties) и сравнениях строк OData учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="3ca58-289">[Property](#onenote-entity-properties) names and OData string comparisons are case sensitive.</span></span> <span data-ttu-id="3ca58-290">Рекомендуем использовать функцию OData **tolower** для сравнения строк.</span><span class="sxs-lookup"><span data-stu-id="3ca58-290">Property names and OData string comparisons are case sensitive. We recommend using the OData **tolower** function for string comparisons. Example: filter=tolower(name) eq 'spring'</span></span> <span data-ttu-id="3ca58-291">Пример: `filter=tolower(name) eq 'spring'`</span><span class="sxs-lookup"><span data-stu-id="3ca58-291">Example: `filter=tolower(name) eq 'spring'`</span></span></p> |  
| <span data-ttu-id="3ca58-292">orderby</span><span class="sxs-lookup"><span data-stu-id="3ca58-292">orderby</span></span> | <p>`orderby=title,createdTime desc`</p><p><span data-ttu-id="3ca58-293">[Свойства](#onenote-entity-properties), по которым нужно выполнить сортировку, с необязательным параметром **asc** (по умолчанию) или **desc**.</span><span class="sxs-lookup"><span data-stu-id="3ca58-293">The [properties](#onenote-entity-properties) to sort by, with an optional **asc** (default) or **desc** sort order. You can sort by any property of the entity in the requested collection.</span></span> <span data-ttu-id="3ca58-294">Выполнять сортировку можно по любому свойству объекта в запрашиваемой коллекции.</span><span class="sxs-lookup"><span data-stu-id="3ca58-294">The properties to sort by, with an optional asc (default) or desc sort order. You can sort by any property of the entity in the requested collection.</span></span></p><p><span data-ttu-id="3ca58-295">По умолчанию для записных книжек, разделов и их групп используется порядок сортировки `name asc`, а для страниц — `lastModifiedTime desc` (начиная с последней измененной страницы).</span><span class="sxs-lookup"><span data-stu-id="3ca58-295">The default sort order for notebooks, section groups, and sections is name asc`name asc`, and for pages is lastModifiedTime desc`lastModifiedTime desc` (last modified page first).</span></span></p><p><span data-ttu-id="3ca58-296">Разделяйте свойства запятыми и указывайте их в порядке применения.</span><span class="sxs-lookup"><span data-stu-id="3ca58-296">Separate  multiple properties with commas, and list them in the order that you want them applied. Property names are case sensitive.</span></span> <span data-ttu-id="3ca58-297">В именах свойств учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="3ca58-297">The column names are case sensitive.</span></span></p> |  
| <span data-ttu-id="3ca58-298">search</span><span class="sxs-lookup"><span data-stu-id="3ca58-298">search</span></span> | <p>`search=cell div`</p><p><span data-ttu-id="3ca58-299">Доступен только для пользовательских записных книжек.</span><span class="sxs-lookup"><span data-stu-id="3ca58-299">Available for consumer notebooks only.</span></span></p><p><span data-ttu-id="3ca58-300">Термин или фраза, которую нужно найти в заголовке, тексте страницы, замещающем тексте изображений и распознанном тексте.</span><span class="sxs-lookup"><span data-stu-id="3ca58-300">
The term or phrase to search for in the page title, page body, image alt text, and image OCR text. By default, search queries return results sorted by relevance.</span></span> <span data-ttu-id="3ca58-301">По умолчанию поисковые запросы возвращают результаты, отсортированные по релевантности.</span><span class="sxs-lookup"><span data-stu-id="3ca58-301">By default, search queries return results sorted by relevance.</span></span></p><p><span data-ttu-id="3ca58-302">OneNote использует полнотекстовый поиск Bing для поддержки поиска фраз, выделения корней, игнорирования орфографических ошибок, релевантности и ранжирования, разбиения слов, разных языков и других функций полнотекстового поиска.</span><span class="sxs-lookup"><span data-stu-id="3ca58-302">onnvshort uses Bing full text search to support phrase search, stemming, spelling forgiveness, relevance and ranking, word breaking, multiple languages, and other full-text search features. Search strings are case insensitive.</span></span> <span data-ttu-id="3ca58-303">В строках поиска не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="3ca58-303">Search strings are case insensitive.</span></span></p><p><span data-ttu-id="3ca58-304">Применяется только к страницам записных книжек, принадлежащих пользователю (не тех, которыми с ним поделились другие).</span><span class="sxs-lookup"><span data-stu-id="3ca58-304">Applies only to pages in notebooks owned by the user (not shared with the user).</span></span> <span data-ttu-id="3ca58-305">Индексированное содержимое является личным и доступно только владельцу.</span><span class="sxs-lookup"><span data-stu-id="3ca58-305">Indexed content is private and can only be accessed by the owner.</span></span> <span data-ttu-id="3ca58-306">Страницы, защищенные паролем, не индексируются.</span><span class="sxs-lookup"><span data-stu-id="3ca58-306">Password-protected pages are not indexed.</span></span> <span data-ttu-id="3ca58-307">Применяется только к конечной точке `pages`.</span><span class="sxs-lookup"><span data-stu-id="3ca58-307">Applies only to the `pages` endpoint.</span></span></p> |  
| <span data-ttu-id="3ca58-308">select</span><span class="sxs-lookup"><span data-stu-id="3ca58-308">select</span></span> | <p>`select=id,title`</p><p><span data-ttu-id="3ca58-309">Возвращаемые [свойства](#onenote-entity-properties).</span><span class="sxs-lookup"><span data-stu-id="3ca58-309">The [properties](#onenote-entity-properties) to return.</span></span> <span data-ttu-id="3ca58-310">Может использоваться для одного объекта или коллекции.</span><span class="sxs-lookup"><span data-stu-id="3ca58-310">Can be used  for  a single  entity or for a collection. Separate  multiple properties with commas. Property names are case sensitive.</span></span> <span data-ttu-id="3ca58-311">Свойства следует разделять запятыми.</span><span class="sxs-lookup"><span data-stu-id="3ca58-311">Separate multiple properties with commas.</span></span> <span data-ttu-id="3ca58-312">В именах свойств учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="3ca58-312">The column names are case sensitive.</span></span></p> |  
| <span data-ttu-id="3ca58-313">skip</span><span class="sxs-lookup"><span data-stu-id="3ca58-313">skip</span></span> | <p>`skip=10`</p><p><span data-ttu-id="3ca58-314">Количество записей, которое следует пропустить в наборе результатов.</span><span class="sxs-lookup"><span data-stu-id="3ca58-314">The number of entries  to skip in the result set. Typically used for paging results.</span></span> <span data-ttu-id="3ca58-315">Обычно используется для разбиения результатов на страницы.</span><span class="sxs-lookup"><span data-stu-id="3ca58-315">Typically used for paging results.</span></span></p> |  
| <span data-ttu-id="3ca58-316">top</span><span class="sxs-lookup"><span data-stu-id="3ca58-316">top</span></span> | <p>`top=50`</p><p><span data-ttu-id="3ca58-317">Количество записей, которое следует вернуть в наборе результатов, до 100.</span><span class="sxs-lookup"><span data-stu-id="3ca58-317">The number of entries to return in the result set, up to a maximum of 100. The default value for pages is 20.</span></span> <span data-ttu-id="3ca58-318">Значение по умолчанию — 20.</span><span class="sxs-lookup"><span data-stu-id="3ca58-318">The default value is 20.</span></span></p> |  

<span data-ttu-id="3ca58-319">В Microsoft Graph также доступен параметр строки запроса `pagelevel`, с помощью которого можно получить уровень и порядок страниц в родительском разделе.</span><span class="sxs-lookup"><span data-stu-id="3ca58-319">Microsoft Graph also provides the `pagelevel` query string option you can use to get the level and order of pages within the parent section.</span></span> <span data-ttu-id="3ca58-320">Применяется только к запросам страниц в определенном разделе и запросам определенной страницы.</span><span class="sxs-lookup"><span data-stu-id="3ca58-320">Applies only to queries for pages in a specific section or queries for a specific page.</span></span> 

<span data-ttu-id="3ca58-321">**Пример:**</span><span class="sxs-lookup"><span data-stu-id="3ca58-321">**Example**</span></span> 

- `GET ../sections/{section-id}/pages?pagelevel=true` 
- `GET ../pages/{page-id}?pagelevel=true` 

### <a name="supported-odata-operators-and-functions"></a><span data-ttu-id="3ca58-322">Поддерживаемые операторы и функции OData</span><span class="sxs-lookup"><span data-stu-id="3ca58-322">Supported OData operators and functions</span></span>

<span data-ttu-id="3ca58-323">Microsoft Graph поддерживает указанные ниже функции и операторы OData в выражениях **filter**.</span><span class="sxs-lookup"><span data-stu-id="3ca58-323">Microsoft Graph supports the following OData operators and functions in **filter** expressions.</span></span> <span data-ttu-id="3ca58-324">Используя выражения OData, помните:</span><span class="sxs-lookup"><span data-stu-id="3ca58-324">When using OData expressions, remember:</span></span>  
- <span data-ttu-id="3ca58-325">Пробелы в строке запроса URL необходимо заменять кодом `%20`.</span><span class="sxs-lookup"><span data-stu-id="3ca58-325">Spaces in the URL query string must be replaced with  the %20`%20` encoding. Example:  filter=isDefault%20eq%20true</span></span>

   <span data-ttu-id="3ca58-326">**Пример:** `filter=isDefault%20eq%20true`</span><span class="sxs-lookup"><span data-stu-id="3ca58-326">Example</span></span>
- <span data-ttu-id="3ca58-327">Имена свойств и сравнения строк OData чувствительны к регистру.</span><span class="sxs-lookup"><span data-stu-id="3ca58-327">Property names and OData string comparisons are case sensitive.</span></span> <span data-ttu-id="3ca58-328">Рекомендуем использовать функцию OData **tolower** для сравнения строк.</span><span class="sxs-lookup"><span data-stu-id="3ca58-328">Property names and OData string comparisons are case sensitive. We recommend using the OData **tolower** function for string comparisons. Example: filter=tolower(name) eq 'spring'</span></span>
   
   <span data-ttu-id="3ca58-329">**Пример:** `filter=tolower(name) eq 'spring'`</span><span class="sxs-lookup"><span data-stu-id="3ca58-329">Example</span></span>

| <span data-ttu-id="3ca58-330">Оператор сравнения</span><span class="sxs-lookup"><span data-stu-id="3ca58-330">Comparison operator</span></span> | <span data-ttu-id="3ca58-331">Пример</span><span class="sxs-lookup"><span data-stu-id="3ca58-331">Example</span></span> |  
|------|------|  
| <span data-ttu-id="3ca58-332">eq</span><span class="sxs-lookup"><span data-stu-id="3ca58-332">eq</span></span><br /><span data-ttu-id="3ca58-333">(равно)</span><span class="sxs-lookup"><span data-stu-id="3ca58-333">(equal to)</span></span> | `createdByAppId eq '{app-id}'` |  
| <span data-ttu-id="3ca58-334">ne</span><span class="sxs-lookup"><span data-stu-id="3ca58-334">ne</span></span><br /><span data-ttu-id="3ca58-335">(не равно)</span><span class="sxs-lookup"><span data-stu-id="3ca58-335">(not equal to)</span></span> | `userRole ne 'Owner'` |  
| <span data-ttu-id="3ca58-336">gt</span><span class="sxs-lookup"><span data-stu-id="3ca58-336">gt</span></span><br /><span data-ttu-id="3ca58-337">(больше)</span><span class="sxs-lookup"><span data-stu-id="3ca58-337">(greater than)</span></span> | `createdTime gt 2014-02-23` |  
| <span data-ttu-id="3ca58-338">ge</span><span class="sxs-lookup"><span data-stu-id="3ca58-338">ge</span></span><br /><span data-ttu-id="3ca58-339">(больше или равно)</span><span class="sxs-lookup"><span data-stu-id="3ca58-339">(greater than or equal to)</span></span> | `lastModifiedTime ge 2014-05-05T07:00:00Z` |  
| <span data-ttu-id="3ca58-340">lt</span><span class="sxs-lookup"><span data-stu-id="3ca58-340">lt</span></span><br /><span data-ttu-id="3ca58-341">(меньше)</span><span class="sxs-lookup"><span data-stu-id="3ca58-341">(less than)</span></span> | `createdTime lt 2014-02-23` |  
| <span data-ttu-id="3ca58-342">le</span><span class="sxs-lookup"><span data-stu-id="3ca58-342">le</span></span><br /><span data-ttu-id="3ca58-343">(меньше или равно)</span><span class="sxs-lookup"><span data-stu-id="3ca58-343">(less than or equal to)</span></span> | `lastModifiedTime le 2014-02-23` |  
 
| <span data-ttu-id="3ca58-344">Логический оператор</span><span class="sxs-lookup"><span data-stu-id="3ca58-344">Logical operator</span></span> | <span data-ttu-id="3ca58-345">Пример</span><span class="sxs-lookup"><span data-stu-id="3ca58-345">Example</span></span> |  
|------|------|  
| <span data-ttu-id="3ca58-346">и</span><span class="sxs-lookup"><span data-stu-id="3ca58-346">and</span></span> | `createdTime le 2014-01-30 and createdTime gt 2014-01-23` |  
| <span data-ttu-id="3ca58-347">Кроме того:</span><span class="sxs-lookup"><span data-stu-id="3ca58-347">or</span></span> | `createdByAppId eq '{app-id}' or createdByAppId eq '{app-id}'` |  
| <span data-ttu-id="3ca58-348">
not</span><span class="sxs-lookup"><span data-stu-id="3ca58-348">NOT</span></span> | `not contains(tolower(title),'school')` |  
 
| <span data-ttu-id="3ca58-349">Строкова функция</span><span class="sxs-lookup"><span data-stu-id="3ca58-349">String function</span></span> | <span data-ttu-id="3ca58-350">Пример</span><span class="sxs-lookup"><span data-stu-id="3ca58-350">Example</span></span> |  
|------|------|   
| <span data-ttu-id="3ca58-351">contains</span><span class="sxs-lookup"><span data-stu-id="3ca58-351">contains</span></span> | `contains(tolower(title),'spring')` |  
| <span data-ttu-id="3ca58-352">endswith</span><span class="sxs-lookup"><span data-stu-id="3ca58-352">endswith</span></span> | `endswith(tolower(title),'spring')` |  
| <span data-ttu-id="3ca58-353">startswith</span><span class="sxs-lookup"><span data-stu-id="3ca58-353">startswith</span></span> | `startswith(tolower(title),'spring')` |  
| <span data-ttu-id="3ca58-354">length</span><span class="sxs-lookup"><span data-stu-id="3ca58-354">length</span></span> | `length(title) eq 19` |  
| <span data-ttu-id="3ca58-355">indexof</span><span class="sxs-lookup"><span data-stu-id="3ca58-355">indexof</span></span> | `indexof(tolower(title),'spring') eq 1` |  
| <span data-ttu-id="3ca58-356">substring</span><span class="sxs-lookup"><span data-stu-id="3ca58-356">substring</span></span> | `substring(tolower(title),1) eq 'spring'` |  
| <span data-ttu-id="3ca58-357">tolower</span><span class="sxs-lookup"><span data-stu-id="3ca58-357">tolower</span></span> | `tolower(title) eq 'spring'` |  
| <span data-ttu-id="3ca58-358">toupper</span><span class="sxs-lookup"><span data-stu-id="3ca58-358">toupper</span></span> | `toupper(title) eq 'SPRING'` |  
| <span data-ttu-id="3ca58-359">trim</span><span class="sxs-lookup"><span data-stu-id="3ca58-359">trim</span></span> | `trim(tolower(title)) eq 'spring'` |  
| <span data-ttu-id="3ca58-360">concat</span><span class="sxs-lookup"><span data-stu-id="3ca58-360">concat</span></span> | `concat(title,'- by MyRecipesApp') eq 'Carrot Cake Recipe - by MyRecipesApp'` |  
 

<a name="properties"></a>
## <a name="onenote-entity-properties"></a><span data-ttu-id="3ca58-361">Свойства объектов OneNote</span><span class="sxs-lookup"><span data-stu-id="3ca58-361">OneNote entity properties</span></span>

<span data-ttu-id="3ca58-362">Выражения запроса **filter**, **select**, **expand** и **orderby** могут включать свойства объектов OneNote.</span><span class="sxs-lookup"><span data-stu-id="3ca58-362">The **filter**, **select**, **expand**, and **orderby** query expressions can include properties of OneNote entities.</span></span> 

<span data-ttu-id="3ca58-363">**Пример:**</span><span class="sxs-lookup"><span data-stu-id="3ca58-363">**Example**</span></span>

`../sections?filter=createdTime ge 2015-01-01&select=name,pagesUrl&orderby=lastModifiedTime desc` 

<span data-ttu-id="3ca58-364">Имена свойств в выражениях запроса чувствительны к регистру.</span><span class="sxs-lookup"><span data-stu-id="3ca58-364">Property names are case sensitive in query expressions.</span></span>

<span data-ttu-id="3ca58-365">Список свойств и их типов см. в следующих статьях:</span><span class="sxs-lookup"><span data-stu-id="3ca58-365">For the list of properties and property types, see:</span></span>

- [<span data-ttu-id="3ca58-366">GET Pages</span><span class="sxs-lookup"><span data-stu-id="3ca58-366">Get pages</span></span>](../api-reference/v1.0/api/page_get.md)
- [<span data-ttu-id="3ca58-367">GET Sections</span><span class="sxs-lookup"><span data-stu-id="3ca58-367">GET sections</span></span>](../api-reference/v1.0/api/section_get.md)
- [<span data-ttu-id="3ca58-368">GET SectionGroups</span><span class="sxs-lookup"><span data-stu-id="3ca58-368">GET sectiongroups</span></span>](../api-reference/v1.0/api/sectiongroup_get.md)
- [<span data-ttu-id="3ca58-369">GET Notebooks</span><span class="sxs-lookup"><span data-stu-id="3ca58-369">GET notebooks</span></span>](../api-reference/v1.0/api/notebook_get.md) 

<span data-ttu-id="3ca58-370">Все эти статьи входят в справочные материалы по REST API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="3ca58-370">in the Microsoft Graph API REST reference.</span></span>

<span data-ttu-id="3ca58-371">Параметр строки запроса **expand** можно использовать со следующими свойствами навигации:</span><span class="sxs-lookup"><span data-stu-id="3ca58-371">The **expand** query string option can be used with the following navigation properties:</span></span>

- <span data-ttu-id="3ca58-372">страницы: **parentNotebook**, **parentSection**;</span><span class="sxs-lookup"><span data-stu-id="3ca58-372">Pages: 
**parentNotebook**, **parentSection**</span></span>
- <span data-ttu-id="3ca58-373">разделы: **parentNotebook**, **parentSectionGroup**;</span><span class="sxs-lookup"><span data-stu-id="3ca58-373">Sections: 
**parentNotebook**, **parentSectionGroup**</span></span>
- <span data-ttu-id="3ca58-374">группы разделов: **sections**, **sectionGroups**, **parentNotebook**, **parentSectionGroup**;</span><span class="sxs-lookup"><span data-stu-id="3ca58-374">Section groups: 
**sections**, **sectionGroups**, **parentNotebook**, **parentSectionGroup**</span></span>
- <span data-ttu-id="3ca58-375">записные книжки: **sections**, **sectionGroups**.</span><span class="sxs-lookup"><span data-stu-id="3ca58-375">Notebooks: **sections**, **sectionGroups**</span></span>


<a name="request-response-info"></a>
## <a name="request-and-response-information-for-get-requests"></a><span data-ttu-id="3ca58-376">Информация о запросах *GET* и соответствующих ответах</span><span class="sxs-lookup"><span data-stu-id="3ca58-376">Request and response information for *GET* requests</span></span>

| <span data-ttu-id="3ca58-377">Данные запроса</span><span class="sxs-lookup"><span data-stu-id="3ca58-377">Request data</span></span> | <span data-ttu-id="3ca58-378">Описание</span><span class="sxs-lookup"><span data-stu-id="3ca58-378">Description</span></span> |  
|------|------|  
| <span data-ttu-id="3ca58-379">Протокол</span><span class="sxs-lookup"><span data-stu-id="3ca58-379">Protocol</span></span> | <span data-ttu-id="3ca58-380">Все запросы используют протокол SSL/TLS для HTTPS.</span><span class="sxs-lookup"><span data-stu-id="3ca58-380">All requests use the SSL/TLS HTTPS protocol.</span></span> |  
| <span data-ttu-id="3ca58-381">Заголовок авторизации</span><span class="sxs-lookup"><span data-stu-id="3ca58-381">Authorization header</span></span> | <p><span data-ttu-id="3ca58-382">`Bearer {token}`, где *{token}*  — это действительный маркер доступа OAuth 2.0 для зарегистрированного приложения.</span><span class="sxs-lookup"><span data-stu-id="3ca58-382">`Bearer {token}`, where *{token}* is a valid OAuth 2.0 access token for your registered app.</span></span></p><p><span data-ttu-id="3ca58-383">Если он отсутствует или является недействительным, произойдет сбой запроса с кодом состояния 401.</span><span class="sxs-lookup"><span data-stu-id="3ca58-383">If missing or invalid, the request fails with a 401 status code.</span></span> <span data-ttu-id="3ca58-384">См. статью [Проверка подлинности и разрешения](permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3ca58-384">See [Authentication and permissions](permissions_reference.md).</span></span></p> |  
| <span data-ttu-id="3ca58-385">Заголовок Accept</span><span class="sxs-lookup"><span data-stu-id="3ca58-385">accept header</span></span> | <p><span data-ttu-id="3ca58-386">- `application/json` для объектов OneNote и их наборов</span><span class="sxs-lookup"><span data-stu-id="3ca58-386">- `application/json` for OneNote entities and entity sets</span></span></p><p><span data-ttu-id="3ca58-387">- `text/html` для содержимого страницы</span><span class="sxs-lookup"><span data-stu-id="3ca58-387">- `text/html` for page content</span></span></p> | 

| <span data-ttu-id="3ca58-388">Данные ответа</span><span class="sxs-lookup"><span data-stu-id="3ca58-388">Response data</span></span> | <span data-ttu-id="3ca58-389">Описание</span><span class="sxs-lookup"><span data-stu-id="3ca58-389">Description</span></span> |  
|------|------|  
| <span data-ttu-id="3ca58-390">Код успешного завершения</span><span class="sxs-lookup"><span data-stu-id="3ca58-390">Success code</span></span> | <span data-ttu-id="3ca58-391">Код состояния HTTP 200</span><span class="sxs-lookup"><span data-stu-id="3ca58-391">A 200 (OK) status code.</span></span> |  
| <span data-ttu-id="3ca58-392">Текст ответа</span><span class="sxs-lookup"><span data-stu-id="3ca58-392">Response body</span></span> | <span data-ttu-id="3ca58-393">Представление объекта или набора объектов в формате JSON, HTML-код страницы или двоичные данные файлового ресурса.</span><span class="sxs-lookup"><span data-stu-id="3ca58-393">An OData representation of the entity or entity set in JSON format, the page HTML, or file resource binary data.</span></span>  |  
| <span data-ttu-id="3ca58-394">Ошибки</span><span class="sxs-lookup"><span data-stu-id="3ca58-394">Errors</span></span> | <span data-ttu-id="3ca58-395">Если запрос завершается с ошибкой, API возвращает [ошибки](onenote_error_codes.md) в объекте **@api.diagnostics** в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3ca58-395">If the update request fails, the API returns errors in the **api.diagnostics** object in the response body. The request will fail if:</span></span> |  
| <span data-ttu-id="3ca58-396">Заголовок X-CorrelationId</span><span class="sxs-lookup"><span data-stu-id="3ca58-396">X-CorrelationId header</span></span> | <span data-ttu-id="3ca58-397">GUID, уникальный идентификатор запроса.</span><span class="sxs-lookup"><span data-stu-id="3ca58-397">A GUID that uniquely identifies the request.</span></span> <span data-ttu-id="3ca58-398">Это значение можно использовать вместе со значением заголовка Date при устранении неполадок совместно со службой поддержки Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="3ca58-398">You can use this value along with the value of the Date header when working with Microsoft support to troubleshoot issues.</span></span> |  


<a name="root-url"></a>
### <a name="constructing-the-microsoft-graph-notes-service-root-url"></a><span data-ttu-id="3ca58-399">Составление корневого URL-адреса службы заметок Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="3ca58-399">Constructing the Microsoft Graph notes service root URL</span></span>

<span data-ttu-id="3ca58-400">Для всех вызовов заметок Microsoft Graph используется следующий формат корневого URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="3ca58-400">The Microsoft Graph notes root URL uses the following format for all calls to Microsoft Graph notes.</span></span> <span data-ttu-id="3ca58-401">`https://graph.microsoft.com/{version}/me/onenote/`. Сегмент URL-адреса `version` представляет нужную версию Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="3ca58-401">`https://graph.microsoft.com/{version}/me/onenote/`  The `version` segment in the URL represents the version of Microsoft Graph that you want to use.</span></span> <span data-ttu-id="3ca58-402">Используйте значение `v1.0` для стабильного производственного кода.</span><span class="sxs-lookup"><span data-stu-id="3ca58-402">Use `v1.0` for stable production code.</span></span> <span data-ttu-id="3ca58-403">Используйте значение `beta`, чтобы опробовать функцию, находящуюся на стадии разработки.</span><span class="sxs-lookup"><span data-stu-id="3ca58-403">Use `beta` to try out a feature that's in development.</span></span> <span data-ttu-id="3ca58-404">Функции бета-версии могут меняться, поэтому не следует использовать их в производственном коде.</span><span class="sxs-lookup"><span data-stu-id="3ca58-404">Features and functionality in beta may change, so you shouldn't use it in your production code.</span></span> <span data-ttu-id="3ca58-405">Используйте значение `me` для содержимого OneNote, доступного текущему пользователю (если он является владельцем или с ним поделились этим содержимым).</span><span class="sxs-lookup"><span data-stu-id="3ca58-405">Use `me` for OneNote content that the current user can access (owned and shared).</span></span> <span data-ttu-id="3ca58-406">Используйте значение `users/{id}` для содержимого OneNote, которым указанный (в URL-адресе) пользователь поделился с текущим пользователем.</span><span class="sxs-lookup"><span data-stu-id="3ca58-406">Use `users/{id}` for OneNote content that the specified user (in the URL) has shared with the current user.</span></span> <span data-ttu-id="3ca58-407">Используйте [Microsoft Graph](https://graph.microsoft.com/v1.0/users) для получения идентификаторов пользователей.</span><span class="sxs-lookup"><span data-stu-id="3ca58-407">Use the [Microsoft Graph](https://graph.microsoft.com/v1.0/users) to get user IDs.</span></span> 


<a name="permissions"></a>
## <a name="permissions-for-get-requests"></a><span data-ttu-id="3ca58-408">Разрешения для запросов GET</span><span class="sxs-lookup"><span data-stu-id="3ca58-408">Permissions for GET requests</span></span>

<span data-ttu-id="3ca58-409">Чтобы получить содержимое или структуру OneNote, необходимо запросить соответствующие разрешения.</span><span class="sxs-lookup"><span data-stu-id="3ca58-409">To get OneNote content or structure, you'll need to request appropriate permissions.</span></span> 

<span data-ttu-id="3ca58-410">Указанные ниже разрешения позволяют выполнять запросы GET к Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="3ca58-410">The following scopes allow GET requests to Microsoft Graph.</span></span> <span data-ttu-id="3ca58-411">Выберите минимальный уровень разрешений, необходимый для работы вашего приложения.</span><span class="sxs-lookup"><span data-stu-id="3ca58-411">Choose the lowest level of permissions that your app needs to do its work.</span></span>

<span data-ttu-id="3ca58-412">Варианты:</span><span class="sxs-lookup"><span data-stu-id="3ca58-412">Choose from:</span></span> 
- <span data-ttu-id="3ca58-413">Notes.read</span><span class="sxs-lookup"><span data-stu-id="3ca58-413">Notes.Read</span></span>
- <span data-ttu-id="3ca58-414">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3ca58-414">Notes.ReadWrite</span></span>
- <span data-ttu-id="3ca58-415">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ca58-415">Notes.ReadWrite.All</span></span>


<span data-ttu-id="3ca58-416">Дополнительную информацию о разрешениях и принципе их работы см. в [справочнике по разрешениям Microsoft Graph](permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3ca58-416">For more information about permission scopes and how they work, see [Microsoft Graph permissions reference](permissions_reference.md).</span></span>

<a name="see-also"></a>
## <a name="additional-resources"></a><span data-ttu-id="3ca58-417">Дополнительные ресурсы</span><span class="sxs-lookup"><span data-stu-id="3ca58-417">Additional resources</span></span>

- [<span data-ttu-id="3ca58-418">Входной и выходной код HTML для страниц OneNote</span><span class="sxs-lookup"><span data-stu-id="3ca58-418">Input and output HTML for OneNote pages</span></span>](onenote_input_output_html.md)
- [<span data-ttu-id="3ca58-419">Интеграция с OneNote</span><span class="sxs-lookup"><span data-stu-id="3ca58-419">Integrate with OneNote</span></span>](integrate_with_onenote.md)
- [<span data-ttu-id="3ca58-420">Блог разработчиков OneNote</span><span class="sxs-lookup"><span data-stu-id="3ca58-420">OneNote Developer Blog</span></span>](http://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="3ca58-421">Вопросы о разработке OneNote на сайте Stack Overflow</span><span class="sxs-lookup"><span data-stu-id="3ca58-421">OneNote development questions on Stack Overflow</span></span>](http://go.microsoft.com/fwlink/?LinkID=390182)
- [<span data-ttu-id="3ca58-422">Репозитории GitHub OneNote</span><span class="sxs-lookup"><span data-stu-id="3ca58-422">OneNote GitHub repos</span></span>](http://go.microsoft.com/fwlink/?LinkID=390178)  
