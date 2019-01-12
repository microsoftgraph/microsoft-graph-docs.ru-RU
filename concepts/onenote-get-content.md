---
title: Получение содержимого и структуры OneNote с помощью Microsoft Graph
description: " Корпоративная записная книжка в Office 365"
author: jewan-microsoft
localization_priority: Priority
ms.prod: onenote
ms.openlocfilehash: 883833bccd4663be4d62cbbd46ce7f2a2a471b4b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945036"
---
# <a name="get-onenote-content-and-structure-with-microsoft-graph"></a><span data-ttu-id="916f1-103">Получение содержимого и структуры OneNote с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="916f1-103">Get OneNote content and structure with Microsoft Graph</span></span>

<span data-ttu-id="916f1-104">**Область применения:** пользовательские записные книжки в OneDrive и корпоративные записные книжки в Office 365.</span><span class="sxs-lookup"><span data-stu-id="916f1-104">**Applies to**: Consumer notebooks on OneDrive | Enterprise notebooks on Office 365</span></span>

<span data-ttu-id="916f1-105">Чтобы получить содержимое и структуру OneNote, необходимо отправить запрос GET к целевой конечной точке.</span><span class="sxs-lookup"><span data-stu-id="916f1-105">To get OneNote content and structure, you send a GET request to the target endpoint.</span></span> <span data-ttu-id="916f1-106">Пример:</span><span class="sxs-lookup"><span data-stu-id="916f1-106">For example:</span></span>

`GET ../onenote/pages/{id}`

<span data-ttu-id="916f1-107">Если запрос выполнен успешно, Microsoft Graph возвращает код состояния HTTP 200 и запрашиваемые объекты или содержимое.</span><span class="sxs-lookup"><span data-stu-id="916f1-107">If the request is successful, Microsoft Graph returns a 200 HTTP status code and the entities or content that you requested.</span></span> <span data-ttu-id="916f1-108">Объекты OneNote возвращаются в виде объектов JSON, соответствующих спецификации OData версии 4.0.</span><span class="sxs-lookup"><span data-stu-id="916f1-108">OneNote entities are returned as JSON objects that conform to the OData version 4.0 specification.</span></span>

<span data-ttu-id="916f1-109">С помощью параметров строки запроса вы можете фильтровать запросы и повышать производительность.</span><span class="sxs-lookup"><span data-stu-id="916f1-109">By using query string options, you can filter your queries and improve performance.</span></span>


<a name="request-uri"></a>

## <a name="construct-the-request-uri"></a><span data-ttu-id="916f1-110">Создание URI запроса</span><span class="sxs-lookup"><span data-stu-id="916f1-110">Construct the request URI</span></span>

<span data-ttu-id="916f1-111">Чтобы создать URI запроса, начните с корневого URL-адреса службы:</span><span class="sxs-lookup"><span data-stu-id="916f1-111">To construct the request URI, start with the service root URL:</span></span>

`https://graph.microsoft.com/v1.0/me/onenote`

<br/>

<span data-ttu-id="916f1-112">Затем добавьте конечную точку нужного ресурса.</span><span class="sxs-lookup"><span data-stu-id="916f1-112">Then append the endpoint of the resource you want to retrieve.</span></span> <span data-ttu-id="916f1-113">([Пути к ресурсам](#resource-paths-for-get-requests) показаны в следующем разделе.)</span><span class="sxs-lookup"><span data-stu-id="916f1-113">([Resource paths](#resource-paths-for-get-requests) are shown in the next section.)</span></span>

<span data-ttu-id="916f1-114">Полный URI запроса будет выглядеть так, как в одном из следующих примеров:</span><span class="sxs-lookup"><span data-stu-id="916f1-114">Your full request URI will look like one of these examples:</span></span>

- `https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}/sections`
- `https://graph.microsoft.com/v1.0/me/onenote/notes/pages`
- `https://graph.microsoft.com/v1.0/me/onenote/pages?select=title,self`

> <span data-ttu-id="916f1-115">**Примечание.** Узнайте больше о [корневом URL-адресе службы](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0#root-url).</span><span class="sxs-lookup"><span data-stu-id="916f1-115">**Note:** Learn more about the [service root URL](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0#root-url).</span></span>

<a name="resource-paths"></a>

## <a name="resource-paths-for-get-requests"></a><span data-ttu-id="916f1-116">Пути к ресурсам для запросов GET</span><span class="sxs-lookup"><span data-stu-id="916f1-116">Resource paths for GET requests</span></span>

<span data-ttu-id="916f1-117">Используйте приведенные ниже пути к ресурсам, чтобы получать страницы, разделы, группы разделов, записные книжки, а также изображения или файлы.</span><span class="sxs-lookup"><span data-stu-id="916f1-117">Use the following resource paths to get pages, sections, section groups, notebooks, and image or file resources.</span></span>

- [<span data-ttu-id="916f1-118">Коллекция Page</span><span class="sxs-lookup"><span data-stu-id="916f1-118">Page collection</span></span>](#page-collection)
- [<span data-ttu-id="916f1-119">Объект Page</span><span class="sxs-lookup"><span data-stu-id="916f1-119">Page entity</span></span>](#page-entity)
- [<span data-ttu-id="916f1-120">Предварительный просмотр страницы</span><span class="sxs-lookup"><span data-stu-id="916f1-120">Page preview</span></span>](#page-preview)
- [<span data-ttu-id="916f1-121">HTML-контент страницы</span><span class="sxs-lookup"><span data-stu-id="916f1-121">Page HTML content</span></span>](#page-html-content)
- [<span data-ttu-id="916f1-122">Коллекция Section</span><span class="sxs-lookup"><span data-stu-id="916f1-122">Section collection</span></span>](#section-collection)
- [<span data-ttu-id="916f1-123">Объект Section</span><span class="sxs-lookup"><span data-stu-id="916f1-123">Section entity</span></span>](#section-entity)
- [<span data-ttu-id="916f1-124">Коллекция SectionGroup</span><span class="sxs-lookup"><span data-stu-id="916f1-124">SectionGroup collection</span></span>](#sectiongroup-collection)
- [<span data-ttu-id="916f1-125">Объект SectionGroup</span><span class="sxs-lookup"><span data-stu-id="916f1-125">SectionGroup entity</span></span>](#sectiongroup-entity)
- [<span data-ttu-id="916f1-126">Коллекция Notebook</span><span class="sxs-lookup"><span data-stu-id="916f1-126">Notebook collection</span></span>](#notebook-collection)
- [<span data-ttu-id="916f1-127">Объект Notebook</span><span class="sxs-lookup"><span data-stu-id="916f1-127">Notebook entity</span></span>](#notebook-entity)
- [<span data-ttu-id="916f1-128">Ресурс изображений или других файлов</span><span class="sxs-lookup"><span data-stu-id="916f1-128">Image or other file resource</span></span>](#image-or-other-file-resource)

<a name="get-pages"></a>

### <a name="page-collection"></a><span data-ttu-id="916f1-129">Коллекция Page</span><span class="sxs-lookup"><span data-stu-id="916f1-129">Page collection</span></span>

<span data-ttu-id="916f1-130">Получение страниц (метаданных) из всех записных книжек.</span><span class="sxs-lookup"><span data-stu-id="916f1-130">Get pages (metadata) across all notebooks.</span></span>

`../pages[?filter,orderby,select,expand,top,skip,search,count]`

<br/>

<span data-ttu-id="916f1-131">Получение страниц (метаданных) из определенного раздела.</span><span class="sxs-lookup"><span data-stu-id="916f1-131">Get pages (metadata) from a specific section.</span></span>

`../sections/{section-id}/pages[?filter,orderby,select,expand,top,skip,search,count,pagelevel]`

<br/>
 
<span data-ttu-id="916f1-132">Параметр строки запроса `search` доступен только для пользовательских записных книжек.</span><span class="sxs-lookup"><span data-stu-id="916f1-132">The `search` query string option is available for consumer notebooks only.</span></span>

<span data-ttu-id="916f1-133">По умолчанию для страниц используется порядок сортировки `lastModifiedTime desc`.</span><span class="sxs-lookup"><span data-stu-id="916f1-133">The default sort order for pages is `lastModifiedTime desc`.</span></span>

<span data-ttu-id="916f1-134">Запрос по умолчанию разворачивает родительский раздел и выбирает свойства `id`, `name` и `self` этого раздела.</span><span class="sxs-lookup"><span data-stu-id="916f1-134">The default query expands the parent section and selects the section's `id`, `name`, and `self` properties.</span></span>

<span data-ttu-id="916f1-135">По умолчанию в ответ на запросы *GET для страниц* возвращаются только первые 20 записей.</span><span class="sxs-lookup"><span data-stu-id="916f1-135">By default, only the top 20 entries are returned for *GET pages* requests.</span></span> <span data-ttu-id="916f1-136">В ответах на запросы, в которых не указан параметр **top**, возвращается ссылка `@odata.nextLink`, с помощью которой можно получить следующие 20 записей.</span><span class="sxs-lookup"><span data-stu-id="916f1-136">Requests that don't specify a **top** query string option return an `@odata.nextLink` link in the response that you can use to get the next 20 entries.</span></span>

<span data-ttu-id="916f1-137">Для коллекции страниц в разделе используйте параметр **pagelevel**, чтобы возвращать уровень отступа страниц и их порядок в разделе.</span><span class="sxs-lookup"><span data-stu-id="916f1-137">For the pages collection in a section, use **pagelevel** to return the indentation level of pages and their order within the section.</span></span> 

#### <a name="example"></a><span data-ttu-id="916f1-138">Пример</span><span class="sxs-lookup"><span data-stu-id="916f1-138">Example</span></span>

`GET ../sections/{section-id}/pages?pagelevel=true`



<a name="get-page"></a> 

### <a name="page-entity"></a><span data-ttu-id="916f1-139">Объект Page</span><span class="sxs-lookup"><span data-stu-id="916f1-139">Page entity</span></span>

<span data-ttu-id="916f1-140">Получение метаданных определенной страницы.</span><span class="sxs-lookup"><span data-stu-id="916f1-140">Get the metadata for a specific page.</span></span> 

`../pages/{page-id}[?select,expand,pagelevel]` 

<br/>

<span data-ttu-id="916f1-141">Запросы страниц могут разворачивать свойства **parentNotebook** и **parentSection**.</span><span class="sxs-lookup"><span data-stu-id="916f1-141">Pages can expand the **parentNotebook** and **parentSection** properties.</span></span>

<span data-ttu-id="916f1-142">Запрос по умолчанию разворачивает родительский раздел и выбирает свойства `id`, `name` и `self` этого раздела.</span><span class="sxs-lookup"><span data-stu-id="916f1-142">The default query expands the parent section and selects the section's `id`, `name`, and `self` properties.</span></span>

<span data-ttu-id="916f1-143">С помощью параметра **pagelevel** можно вернуть уровень отступа страницы и ее порядковый номер в родительском разделе.</span><span class="sxs-lookup"><span data-stu-id="916f1-143">Use **pagelevel** to return the indentation level of the page and its order within its parent section.</span></span> 

#### <a name="example"></a><span data-ttu-id="916f1-144">Пример</span><span class="sxs-lookup"><span data-stu-id="916f1-144">Example</span></span>

`GET ../pages/{page-id}?pagelevel=true`



<a name="get-page-preview"></a> 

### <a name="page-preview"></a><span data-ttu-id="916f1-145">Предварительный просмотр страницы</span><span class="sxs-lookup"><span data-stu-id="916f1-145">Page preview</span></span>

<span data-ttu-id="916f1-146">Получение текста и изображений на странице для предварительного просмотра.</span><span class="sxs-lookup"><span data-stu-id="916f1-146">Get text and image preview content for a page.</span></span>

`../pages/{page-id}/preview`

<br/>


<span data-ttu-id="916f1-147">Отклик JSON содержит часть контента для предварительного просмотра, благодаря которому пользователи могут узнать, что находится на странице.</span><span class="sxs-lookup"><span data-stu-id="916f1-147">The JSON response contains the preview content, which you can use to help users identify what's in the page.</span></span>

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

<span data-ttu-id="916f1-148">Свойство **previewText** содержит фрагмент текста со страницы.</span><span class="sxs-lookup"><span data-stu-id="916f1-148">The **previewText** property contains a text snippet from the page.</span></span> <span data-ttu-id="916f1-149">Microsoft Graph возвращает полные фразы длиной до 300 символов.</span><span class="sxs-lookup"><span data-stu-id="916f1-149">Microsoft Graph returns complete phrases, up to a maximum of 300 characters.</span></span> 

<span data-ttu-id="916f1-150">Если на странице есть изображение, подходящее для предварительного просмотра, то свойство **href** объекта **previewImageUrl** будет содержать ссылку на общедоступный [ресурс изображения](#image-or-other-file-resource) с предварительной проверкой подлинности.</span><span class="sxs-lookup"><span data-stu-id="916f1-150">If the page has an image that can be used to build a preview UI, the **href** property in the **previewImageUrl** object contains a link to a public, pre-authenticated [image resource](#image-or-other-file-resource).</span></span> <span data-ttu-id="916f1-151">Эту ссылку можно использовать в коде HTML.</span><span class="sxs-lookup"><span data-stu-id="916f1-151">You can use this link in HTML.</span></span> <span data-ttu-id="916f1-152">Если не сделать этого, свойство **href** возвратит значение NULL.</span><span class="sxs-lookup"><span data-stu-id="916f1-152">Otherwise, **href** returns null.</span></span>

#### <a name="example"></a><span data-ttu-id="916f1-153">Пример</span><span class="sxs-lookup"><span data-stu-id="916f1-153">Example</span></span> 

`<img src="https://www.onenote.com/api/v1.0/resources/{id}/content?publicAuth=true&mimeType=image/png" />`


<a name="get-page-content"></a> 

### <a name="page-html-content"></a><span data-ttu-id="916f1-154">HTML-контент страницы</span><span class="sxs-lookup"><span data-stu-id="916f1-154">Page HTML content</span></span>

<span data-ttu-id="916f1-155">Получение HTML-контента страницы.</span><span class="sxs-lookup"><span data-stu-id="916f1-155">Get the HTML content of a page.</span></span>

`../pages/{page-id}/content[?includeIDs,preAuthenticated]`

<span data-ttu-id="916f1-156">(*Дополнительные сведения о [возвращаемом HTML-контенте](onenote-input-output-html.md)*.)</span><span class="sxs-lookup"><span data-stu-id="916f1-156">(*learn more about [returned HTML content](onenote-input-output-html.md)*)</span></span> 

<br/>

<span data-ttu-id="916f1-157">Указав в строке запроса параметр **includeIDs=true**, можно получить созданные идентификаторы, используемые для [обновления страницы](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="916f1-157">Use the **includeIDs=true** query string option to get generated IDs used to [update the page](onenote-update-page.md).</span></span>

<span data-ttu-id="916f1-158">Указав в строке запроса параметр **preAuthenticated=true**, можно получить общедоступные URL-адреса [ресурсов изображений](#image-or-other-file-resource) на странице.</span><span class="sxs-lookup"><span data-stu-id="916f1-158">Use the **preAuthenticated=true** query string option to get public URLs to the [image resources](#image-or-other-file-resource) that are on the page.</span></span> <span data-ttu-id="916f1-159">Общедоступные URL-адреса действительны в течение одного часа.</span><span class="sxs-lookup"><span data-stu-id="916f1-159">The public URLs are valid for one hour.</span></span> 



<a name="get-sections"></a>

### <a name="section-collection"></a><span data-ttu-id="916f1-160">Коллекция Section</span><span class="sxs-lookup"><span data-stu-id="916f1-160">Section collection</span></span>

<span data-ttu-id="916f1-161">Получение всех разделов всех записных книжек, принадлежащих пользователю, включая разделы из вложенных групп разделов.</span><span class="sxs-lookup"><span data-stu-id="916f1-161">Get all sections from all notebooks that are owned by the user, including sections in nested section groups.</span></span>

`../sections[?filter,orderby,select,top,skip,expand,count]` 

<br/>

<span data-ttu-id="916f1-162">Получение всех разделов, вложенных непосредственно в определенную группу разделов.</span><span class="sxs-lookup"><span data-stu-id="916f1-162">Get all sections that are directly under a specific section group.</span></span>

`../sectionGroups/{sectiongroup-id}/sections[?filter,orderby,select,top,skip,expand,count]` 

<br/>

<span data-ttu-id="916f1-163">Получение всех разделов, вложенных непосредственно в определенную записную книжку.</span><span class="sxs-lookup"><span data-stu-id="916f1-163">Get all sections that are directly under a specific notebook.</span></span>

`../notebooks/{notebook-id}/sections[?filter,orderby,select,top,skip,expand,count]` 

<br/>

<span data-ttu-id="916f1-164">Запросы разделов могут разворачивать свойства **parentNotebook** и **parentSectionGroup**.</span><span class="sxs-lookup"><span data-stu-id="916f1-164">Sections can expand the **parentNotebook** and **parentSectionGroup** properties.</span></span>

<span data-ttu-id="916f1-165">По умолчанию для разделов используется порядок сортировки `name asc`.</span><span class="sxs-lookup"><span data-stu-id="916f1-165">The default sort order for sections is `name asc`.</span></span>

<span data-ttu-id="916f1-166">Запрос по умолчанию разворачивает родительскую записную книжку и родительскую группу разделов и выбирает их свойства `id`, `name` и `self`.</span><span class="sxs-lookup"><span data-stu-id="916f1-166">The default query expands the parent notebook and parent section group and selects their `id`, `name`, and `self` properties.</span></span>



<a name="get-section"></a>

### <a name="section-entity"></a><span data-ttu-id="916f1-167">Объект Section</span><span class="sxs-lookup"><span data-stu-id="916f1-167">Section entity</span></span>

<span data-ttu-id="916f1-168">Получение определенного раздела.</span><span class="sxs-lookup"><span data-stu-id="916f1-168">Get a specific section.</span></span>

`../sections/{section-id}[?select,expand]` 

<br/>

<span data-ttu-id="916f1-169">Запросы разделов могут разворачивать свойства **parentNotebook** и **parentSectionGroup**.</span><span class="sxs-lookup"><span data-stu-id="916f1-169">Sections can expand the **parentNotebook** and **parentSectionGroup** properties.</span></span>

<span data-ttu-id="916f1-170">Запрос по умолчанию разворачивает родительскую записную книжку и родительскую группу разделов и выбирает их свойства `id`, `name` и `self`.</span><span class="sxs-lookup"><span data-stu-id="916f1-170">The default query expands the parent notebook and parent section group and selects their `id`, `name`, and `self` properties.</span></span>



<a name="get-section-groups"></a>

### <a name="sectiongroup-collection"></a><span data-ttu-id="916f1-171">Коллекция SectionGroup</span><span class="sxs-lookup"><span data-stu-id="916f1-171">SectionGroup collection</span></span>

<span data-ttu-id="916f1-172">Получение всех групп разделов из всех записных книжек, принадлежащих пользователю, включая вложенные.</span><span class="sxs-lookup"><span data-stu-id="916f1-172">Get all section groups from all notebooks that are owned by the user, including nested section groups.</span></span>

`../sectionGroups[?filter,orderby,select,top,skip,expand,count]` 

<br/>

<span data-ttu-id="916f1-173">Получение всех групп разделов, вложенных непосредственно в определенную записную книжку.</span><span class="sxs-lookup"><span data-stu-id="916f1-173">Get all section groups that are directly under a specific notebook.</span></span> 

`../notebooks/{notebook-id}/sectionGroups[?filter,orderby,select,top,skip,expand,count]` 

<br/>

<span data-ttu-id="916f1-174">Запросы групп разделов могут разворачивать свойства **sections**, **sectionGroups**, **parentNotebook** и **parentSectionGroup**.</span><span class="sxs-lookup"><span data-stu-id="916f1-174">Section groups can expand the **sections**, **sectionGroups**, **parentNotebook**, and **parentSectionGroup** properties.</span></span>

<span data-ttu-id="916f1-175">По умолчанию для групп разделов используется порядок сортировки `name asc`.</span><span class="sxs-lookup"><span data-stu-id="916f1-175">The default sort order for section groups is `name asc`.</span></span>

<span data-ttu-id="916f1-176">Запрос по умолчанию разворачивает родительскую записную книжку и родительскую группу разделов и выбирает их свойства `id`, `name` и `self`.</span><span class="sxs-lookup"><span data-stu-id="916f1-176">The default query expands the parent notebook and parent section group and selects their `id`, `name`, and `self` properties.</span></span>



<a name="get-section-group"></a>

### <a name="sectiongroup-entity"></a><span data-ttu-id="916f1-177">Объект SectionGroup</span><span class="sxs-lookup"><span data-stu-id="916f1-177">SectionGroup entity</span></span>

<span data-ttu-id="916f1-178">Получение определенной группы разделов.</span><span class="sxs-lookup"><span data-stu-id="916f1-178">Get a specific section group.</span></span>

`../sectionGroups/{sectiongroup-id}[?select,expand]` 

<br/>

<span data-ttu-id="916f1-179">Запросы групп разделов могут разворачивать свойства **sections**, **sectionGroups**, **parentNotebook** и **parentSectionGroup**.</span><span class="sxs-lookup"><span data-stu-id="916f1-179">Section groups can expand the **sections**, **sectionGroups**, **parentNotebook**, and **parentSectionGroup** properties.</span></span>

<span data-ttu-id="916f1-180">Запрос по умолчанию разворачивает родительскую записную книжку и родительскую группу разделов и выбирает их свойства `id`, `name` и `self`.</span><span class="sxs-lookup"><span data-stu-id="916f1-180">The default query expands the parent notebook and parent section group and selects their `id`, `name`, and `self` properties.</span></span>



<a name="get-notebooks"></a>

### <a name="notebook-collection"></a><span data-ttu-id="916f1-181">Коллекция Notebook</span><span class="sxs-lookup"><span data-stu-id="916f1-181">Notebook collection</span></span>

<span data-ttu-id="916f1-182">Получение всех записных книжек, принадлежащих пользователю.</span><span class="sxs-lookup"><span data-stu-id="916f1-182">Get all the notebooks that are owned by the user.</span></span> 

`../notebooks[?filter,orderby,select,top,skip,expand,count]` 

<br/>

<span data-ttu-id="916f1-183">Запросы записных книжек могут разворачивать свойства **sections** и **sectionGroups**.</span><span class="sxs-lookup"><span data-stu-id="916f1-183">Notebooks can expand the **sections** and **sectionGroups** properties.</span></span>

<span data-ttu-id="916f1-184">По умолчанию для записных книжек используется порядок сортировки `name asc`.</span><span class="sxs-lookup"><span data-stu-id="916f1-184">The default sort order for notebooks is `name asc`.</span></span> 



<a name="get-notebook"></a>

### <a name="notebook-entity"></a><span data-ttu-id="916f1-185">Объект Notebook</span><span class="sxs-lookup"><span data-stu-id="916f1-185">Notebook entity</span></span>

<span data-ttu-id="916f1-186">Получение определенной записной книжки.</span><span class="sxs-lookup"><span data-stu-id="916f1-186">Get a specific notebook.</span></span>

`../notebooks/{notebook-id}[?select,expand]` 

<br/>

<span data-ttu-id="916f1-187">Запросы записных книжек могут разворачивать свойства **sections** и **sectionGroups**.</span><span class="sxs-lookup"><span data-stu-id="916f1-187">Notebooks can expand the **sections** and **sectionGroups** properties.</span></span>



<a name="get-resource"></a>

### <a name="image-or-other-file-resource"></a><span data-ttu-id="916f1-188">Ресурс изображений или других файлов</span><span class="sxs-lookup"><span data-stu-id="916f1-188">Image or other file resource</span></span>

<span data-ttu-id="916f1-189">Получение двоичных данных определенного ресурса.</span><span class="sxs-lookup"><span data-stu-id="916f1-189">Get the binary data of a specific resource.</span></span> 

`../resources/{resource-id}/$value` 

<br/>

<span data-ttu-id="916f1-190">URI ресурса файла можно найти в [выходном HTML-коде](onenote-input-output-html.md) страницы.</span><span class="sxs-lookup"><span data-stu-id="916f1-190">You can find the file's resource URI in the page's [output HTML](onenote-input-output-html.md).</span></span>

<span data-ttu-id="916f1-191">Например, тег **img** содержит конечные точки для исходного изображения в атрибуте **data-fullres-src** и оптимизированное изображение в атрибуте **src**.</span><span class="sxs-lookup"><span data-stu-id="916f1-191">For example, an **img** tag includes endpoints for the original image in the **data-fullres-src** attribute and the optimized image in the **src** attribute.</span></span> 

#### <a name="example"></a><span data-ttu-id="916f1-192">Пример</span><span class="sxs-lookup"><span data-stu-id="916f1-192">Example</span></span>

```html
<img 
    src="https://www.onenote.com/api/v1.0/me/notes/resources/{image-id}/$value"  
    data-src-type="image/png"
    data-fullres-src="https://www.onenote.com/api/v1.0/resources/{image-id}/$value"  
    data-fullres-src-type="image/png" ... />
```

<span data-ttu-id="916f1-193">Тег **object** содержит конечную точку файлового ресурса в атрибуте **data**.</span><span class="sxs-lookup"><span data-stu-id="916f1-193">And an **object** tag includes the endpoint for the file resource in the **data** attribute.</span></span> 

#### <a name="example"></a><span data-ttu-id="916f1-194">Пример</span><span class="sxs-lookup"><span data-stu-id="916f1-194">Example</span></span>

```html
<object
    data="https://www.onenote.com/api/v1.0/me/notes/resources/{file-id}/$value"
    data-attachment="fileName.pdf" 
    type="application/pdf" ... />
```

<span data-ttu-id="916f1-195">Чтобы получить общедоступные URL-адреса изображений на странице с предварительной проверкой подлинности, включите параметр `preAuthenticated=true` в строку запроса при [получении содержимого страницы](#page-html-content) (**пример**: `GET ../pages/{page-id}/content?preAuthenticated=true`).</span><span class="sxs-lookup"><span data-stu-id="916f1-195">To get public, pre-authenticated URLs to the image resources on a page, include `preAuthenticated=true` in the query string when you [retrieve the page content](#page-html-content) (**example:**  `GET ../pages/{page-id}/content?preAuthenticated=true`).</span></span> <span data-ttu-id="916f1-196">Возвращаемые в [выходном HTML-коде](onenote-input-output-html.md#output-html-examples-for-images) общедоступные URL-адреса действительны в течение одного часа.</span><span class="sxs-lookup"><span data-stu-id="916f1-196">The public URLs that are returned in the [output HTML](onenote-input-output-html.md#output-html-examples-for-images) are valid for one hour.</span></span> <span data-ttu-id="916f1-197">Без этого флага полученные изображения не отображаются непосредственно в браузере, так как они являются личными и для их получения необходимо пройти проверку подлинности, как и для другого содержимого страницы.</span><span class="sxs-lookup"><span data-stu-id="916f1-197">Without this flag, retrieved images won't render directly in a browser because they are private and require authorization to retrieve them, like the rest of the page contents.</span></span> 

> <span data-ttu-id="916f1-198">**Примечание.** Получение коллекции ресурсов не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="916f1-198">**Note:** Getting a collection of resources is not supported.</span></span> 

<span data-ttu-id="916f1-199">При получении файлового ресурса не требуется включать в запрос тип контента **Accept**.</span><span class="sxs-lookup"><span data-stu-id="916f1-199">When you get a file resource, you don't need to include an **Accept** content type in the request.</span></span>

<span data-ttu-id="916f1-200">Дополнительные сведения о запросах GET см. в следующих статьях документации по API REST Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="916f1-200">For more information about GET requests, see the following resources in the Microsoft Graph API REST reference:</span></span>

- [<span data-ttu-id="916f1-201">Запрос GET для страниц</span><span class="sxs-lookup"><span data-stu-id="916f1-201">GET Pages</span></span>](/graph/api/page-get?view=graph-rest-1.0)
- [<span data-ttu-id="916f1-202">GET Sections</span><span class="sxs-lookup"><span data-stu-id="916f1-202">GET Sections</span></span>](/graph/api/section-get?view=graph-rest-1.0)
- [<span data-ttu-id="916f1-203">GET SectionGroups</span><span class="sxs-lookup"><span data-stu-id="916f1-203">GET SectionGroups</span></span>](/graph/api/sectiongroup-get?view=graph-rest-1.0)
- [<span data-ttu-id="916f1-204">Запрос GET для записных книжек</span><span class="sxs-lookup"><span data-stu-id="916f1-204">GET Notebooks</span></span>](/graph/api/notebook-get?view=graph-rest-1.0) 




<a name="example"></a>

## <a name="example-get-requests"></a><span data-ttu-id="916f1-205">Примеры запросов GET</span><span class="sxs-lookup"><span data-stu-id="916f1-205">Example GET requests</span></span>

<span data-ttu-id="916f1-206">Вы можете запрашивать объекты OneNote и содержимое страницы поиска, чтобы получать только нужные вам сведения.</span><span class="sxs-lookup"><span data-stu-id="916f1-206">You can query for OneNote entities and search page content to get just the information you need.</span></span> <span data-ttu-id="916f1-207">Ниже показаны некоторые способы использования [поддерживаемых параметров строки](#supported-odata-query-string-options) в запросах GET к Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="916f1-207">The following examples show some ways you can use [supported query string options](#supported-odata-query-string-options) in GET requests to Microsoft Graph.</span></span> 

<span data-ttu-id="916f1-208">**Помните:**</span><span class="sxs-lookup"><span data-stu-id="916f1-208">**Remember:**</span></span>

- <span data-ttu-id="916f1-209">Все запросы GET начинаются с [корневого URL-адреса службы](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0#root-url).</span><span class="sxs-lookup"><span data-stu-id="916f1-209">All GET requests start with the [service root URL](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0#root-url).</span></span> <br/><br/><span data-ttu-id="916f1-210">**Примеры**: `https://www.onenote.com/api/v1.0/me/notes` и `https://www.onenote.com/api/v1.0/myOrganization/siteCollections/{id}/sites/{id}/notes/`.</span><span class="sxs-lookup"><span data-stu-id="916f1-210">**Examples**: `https://www.onenote.com/api/v1.0/me/notes` and `https://www.onenote.com/api/v1.0/myOrganization/siteCollections/{id}/sites/{id}/notes/`</span></span>

- <span data-ttu-id="916f1-211">Пробелы в строке запроса URL следует кодировать как %20.</span><span class="sxs-lookup"><span data-stu-id="916f1-211">Spaces in the URL query string must use %20 encoding.</span></span><br/><br/><span data-ttu-id="916f1-212">**Пример**: `filter=title%20eq%20'biology'`.</span><span class="sxs-lookup"><span data-stu-id="916f1-212">**Example**: `filter=title%20eq%20'biology'`</span></span>

- <span data-ttu-id="916f1-213">В случае имен свойств и сравнения строк OData учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="916f1-213">Property names and OData string comparisons are case-sensitive.</span></span> <span data-ttu-id="916f1-214">Рекомендуем использовать функцию OData **tolower** для сравнения строк.</span><span class="sxs-lookup"><span data-stu-id="916f1-214">We recommend using the OData **tolower** function for string comparisons.</span></span><br/><br/><span data-ttu-id="916f1-215">**Пример**: `filter=tolower(name) eq 'spring'`.</span><span class="sxs-lookup"><span data-stu-id="916f1-215">**Example**: `filter=tolower(name) eq 'spring'`</span></span>
 

### <a name="search--filter"></a><span data-ttu-id="916f1-216">search и filter</span><span class="sxs-lookup"><span data-stu-id="916f1-216">search & filter</span></span>  

<span data-ttu-id="916f1-217">Получение всех страниц с термином *recipe*, созданных определенным приложением (`search` доступен только для пользовательских записных книжек).</span><span class="sxs-lookup"><span data-stu-id="916f1-217">Get all pages that contain the term *recipe* that were created by a specific app (`search` is available for consumer notebooks only).</span></span>

```
[GET] ../pages?search=recipe&filter=createdByAppId eq 'WLID-000000004C12821A'
```
 
### <a name="search--select"></a><span data-ttu-id="916f1-218">search и select</span><span class="sxs-lookup"><span data-stu-id="916f1-218">search & select</span></span>  

<span data-ttu-id="916f1-219">Получение заголовка, клиентских ссылок OneNote и ссылки **contentUrl** для всех страниц, содержащих термин *golgi app* (`search` доступен только для пользовательских записных книжек).</span><span class="sxs-lookup"><span data-stu-id="916f1-219">Get the title, OneNote client links, and **contentUrl** link for all pages that contain the term *golgi app* (`search` is available for consumer notebooks only).</span></span>

```
[GET] ../pages?search=golgi app&select=title,links,contentUrl
```
 
### <a name="expand"></a><span data-ttu-id="916f1-220">expand</span><span class="sxs-lookup"><span data-stu-id="916f1-220">expand</span></span> 

<span data-ttu-id="916f1-221">Получение всех записных книжек, а также разворачивание их разделов и групп разделов.</span><span class="sxs-lookup"><span data-stu-id="916f1-221">Get all notebooks and expand their sections and section groups.</span></span>  

```
[GET] ../notebooks?expand=sections,sectionGroups
```

<br/>

<span data-ttu-id="916f1-222">Получение определенной группы разделов и разворачивание ее разделов и групп разделов.</span><span class="sxs-lookup"><span data-stu-id="916f1-222">Get a specific section group and expand its sections and section groups.</span></span>  

```
[GET] ../sectionGroups/{sectiongroup-id}?expand=sections,sectionGroups
```

<br/>

<span data-ttu-id="916f1-223">Получение страницы и разворачивание ее родительского раздела и родительской записной книжки.</span><span class="sxs-lookup"><span data-stu-id="916f1-223">Get a page and expand its parent section and parent notebook.</span></span>

```
[GET] ../pages/{page-id}?expand=parentSection,parentNotebook
```

### <a name="expand-multiple-levels"></a><span data-ttu-id="916f1-224">expand (несколько уровней)</span><span class="sxs-lookup"><span data-stu-id="916f1-224">expand (multiple levels)</span></span>  

<span data-ttu-id="916f1-225">Получение всех записных книжек и разворачивание их разделов и групп разделов, а также разворачивание всех разделов в каждой группе разделов.</span><span class="sxs-lookup"><span data-stu-id="916f1-225">Get all notebooks and expand their sections and section groups, and expand all sections in each section group.</span></span>  

```
[GET] ../notebooks?expand=sections,sectionGroups(expand=sections)
```
 
> <span data-ttu-id="916f1-226">**Примечание.** Разворачивание родительских элементов объектов или разворачивание дочерних элементов объектов создает циклическую ссылку и не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="916f1-226">**Note:** Expanding parents of child entities or expanding children of parent entities creates a circular reference and is not supported.</span></span>

 
### <a name="expand--select-multiple-levels"></a><span data-ttu-id="916f1-227">expand и select (несколько уровней)</span><span class="sxs-lookup"><span data-stu-id="916f1-227">expand & select (multiple levels)</span></span>  

<span data-ttu-id="916f1-228">Получение имени и ссылки **self** для определенной группы разделов, а также получение имени и ссылок **self** для всех ее разделов.</span><span class="sxs-lookup"><span data-stu-id="916f1-228">Get the name and **self** link for a specific section group, and get the name and **self** links for all its sections.</span></span>  

```
[GET] ../sectionGroups/{sectiongroup-id}?expand=sections(select=name,self)&select=name,self
```

<br/>

<span data-ttu-id="916f1-229">Получение имени и ссылки **self** для всех разделов, а также получение имени и времени создания родительской записной книжки каждого раздела.</span><span class="sxs-lookup"><span data-stu-id="916f1-229">Get the name and **self** link for all sections, and get the name and created time of each section's parent notebook.</span></span>  

```
[GET] ../sections?expand=parentNotebook(select=name,createdTime)&select=name,self
```

<br/>
 
<span data-ttu-id="916f1-230">Получение названий и идентификаторов всех страниц, а также получение названия родительского раздела и родительской записной книжки.</span><span class="sxs-lookup"><span data-stu-id="916f1-230">Get the title and ID for all pages, and get the name of the parent section and parent notebook.</span></span>

```
[GET] ../pages?select=id,title&expand=parentSection(select=name),parentNotebook(select=name)
```

### <a name="expand--levels-multiple-levels"></a><span data-ttu-id="916f1-231">expand и levels (несколько уровней)</span><span class="sxs-lookup"><span data-stu-id="916f1-231">expand & levels (multiple levels)</span></span>  

<span data-ttu-id="916f1-232">Получение всех записных книжек, разделов и групп разделов.</span><span class="sxs-lookup"><span data-stu-id="916f1-232">Get all notebooks, sections, and section groups.</span></span>  

```
[GET] ../notebooks?expand=sections,sectionGroups(expand=sections,sectionGroups(levels=max;expand=sections))
```
 
### <a name="filter"></a><span data-ttu-id="916f1-233">filter</span><span class="sxs-lookup"><span data-stu-id="916f1-233">filter</span></span>

<span data-ttu-id="916f1-234">Получение всех разделов, созданных в октябре 2014 г.</span><span class="sxs-lookup"><span data-stu-id="916f1-234">Get all sections that were created in October 2014.</span></span>

```
[GET] ../sections?filter=createdTime ge 2014-10-01 and createdTime le 2014-10-31
```

<br/>

<span data-ttu-id="916f1-235">Получение страниц, созданных определенным приложением с 1 января 2015 г.</span><span class="sxs-lookup"><span data-stu-id="916f1-235">Get the pages that were created by a specific app since January 1, 2015.</span></span>

```
[GET] ../pages?filter=createdByAppId eq 'WLID-0000000048118631' and createdTime ge 2015-01-01
```

### <a name="filter--expand"></a><span data-ttu-id="916f1-236">filter и expand</span><span class="sxs-lookup"><span data-stu-id="916f1-236">filter & expand</span></span>  

<span data-ttu-id="916f1-237">Получение всех страниц определенной записной книжки.</span><span class="sxs-lookup"><span data-stu-id="916f1-237">Get all pages in a specific notebook.</span></span> <span data-ttu-id="916f1-238">По умолчанию API возвращает 20 записей.</span><span class="sxs-lookup"><span data-stu-id="916f1-238">The API returns 20 entries by default.</span></span>

```
[GET] ../pages?filter=parentNotebook/id eq '{notebook-id}'&expand=parentNotebook
```

<br/>

<span data-ttu-id="916f1-239">Получение имени и ссылки **pagesUrl** для всех разделов в записной книжке *School*.</span><span class="sxs-lookup"><span data-stu-id="916f1-239">Get the name and **pagesUrl** link for all sections from the *School* notebook.</span></span> <span data-ttu-id="916f1-240">При сравнении строк OData учитывается регистр, поэтому рекомендуем использовать функцию **tolower**.</span><span class="sxs-lookup"><span data-stu-id="916f1-240">OData string comparisons are case-sensitive, so use the **tolower** function as a best practice.</span></span>

```
[GET] ../notebooks?filter=tolower(name) eq 'school'&expand=sections(select=name,pagesUrl)
```

### <a name="filter--select--orderby"></a><span data-ttu-id="916f1-241">filter, select и orderby</span><span class="sxs-lookup"><span data-stu-id="916f1-241">filter & select & orderby</span></span>   

<span data-ttu-id="916f1-242">Получение имени и ссылки **pagesUrl** для всех разделов, имена которых содержат термин *spring*.</span><span class="sxs-lookup"><span data-stu-id="916f1-242">Get the name and **pagesUrl** link for all sections that contain the term *spring* in the section name.</span></span> <span data-ttu-id="916f1-243">Упорядочивание разделов по дате последнего изменения.</span><span class="sxs-lookup"><span data-stu-id="916f1-243">Order sections by last modified date.</span></span>

```
[GET] ../sections?filter=contains(tolower(name),'spring')&select=name,pagesUrl&orderby=lastModifiedTime desc
```
 
### <a name="orderby"></a><span data-ttu-id="916f1-244">orderby</span><span class="sxs-lookup"><span data-stu-id="916f1-244">orderby</span></span>

<span data-ttu-id="916f1-245">Получение первых 20 страниц, отсортированных по свойству **createdByAppId** и времени создания (по убыванию).</span><span class="sxs-lookup"><span data-stu-id="916f1-245">Get the first 20 pages ordered by **createdByAppId** property and then by most recent created time.</span></span> <span data-ttu-id="916f1-246">По умолчанию API возвращает 20 записей.</span><span class="sxs-lookup"><span data-stu-id="916f1-246">The API returns 20 entries by default.</span></span>

```
[GET] ../pages?orderby=createdByAppId,createdTime desc
```

### <a name="search--filter--top"></a><span data-ttu-id="916f1-247">search, filter и top</span><span class="sxs-lookup"><span data-stu-id="916f1-247">search & filter & top</span></span> 

<span data-ttu-id="916f1-248">Получение пяти последних страниц, созданных с 1 января 2015 г. и содержащих фразу *cell division*.</span><span class="sxs-lookup"><span data-stu-id="916f1-248">Get the five newest pages created since January 1, 2015 that contain the phrase *cell division*.</span></span> <span data-ttu-id="916f1-249">По умолчанию API возвращает 20 записей. Максимальное количество записей — 100.</span><span class="sxs-lookup"><span data-stu-id="916f1-249">The API returns 20 entries by default with a maximum of 100.</span></span> <span data-ttu-id="916f1-250">Порядок сортировки по умолчанию для страниц: `lastModifiedTime desc` (`search` доступен только для пользовательских записных книжек).</span><span class="sxs-lookup"><span data-stu-id="916f1-250">The default sort order for pages is `lastModifiedTime desc` (`search` is available for consumer notebooks only).</span></span>

```
[GET] ../pages?search="cell division"&filter=createdTime ge 2015-01-01&top=5
```

### <a name="search--filter--top--skip"></a><span data-ttu-id="916f1-251">search, filter, top и skip</span><span class="sxs-lookup"><span data-stu-id="916f1-251">search & filter & top & skip</span></span>  

<span data-ttu-id="916f1-252">Получение пяти следующих страниц в результирующем наборе (`search` доступен только для пользовательских записных книжек).</span><span class="sxs-lookup"><span data-stu-id="916f1-252">Get the next five pages in the result set (`search` is available for consumer notebooks only).</span></span>

```
[GET] ../pages?search=biology&filter=createdTime ge 2015-01-01&top=5&skip=5
```

<br/>

<span data-ttu-id="916f1-253">Получение еще пяти (`search` доступен только для пользовательских записных книжек).</span><span class="sxs-lookup"><span data-stu-id="916f1-253">And the next five (`search` is available for consumer notebooks only).</span></span>

```
[GET] ../pages?search=biology&filter=createdTime ge 2015-01-01&top=5&skip=10
```

> <span data-ttu-id="916f1-254">**Примечание.** Если параметры **search** и **filter** применяются к одному запросу, результаты включают только те объекты, которые соответствуют обоим условиям.</span><span class="sxs-lookup"><span data-stu-id="916f1-254">**Note:** If both **search** and **filter** are applied to the same request, the results include only those entities that match both criteria.</span></span>
 
### <a name="select"></a><span data-ttu-id="916f1-255">select</span><span class="sxs-lookup"><span data-stu-id="916f1-255">select</span></span>

<span data-ttu-id="916f1-256">Получение имени, времени создания и ссылки **self** для всех разделов в записных книжках пользователя.</span><span class="sxs-lookup"><span data-stu-id="916f1-256">Get the name, created time, and **self** link for all sections in the user's notebooks.</span></span>

```
[GET] ../sections?select=name,createdTime,self
```

<br/>

<span data-ttu-id="916f1-257">Получение названия, времени создания и клиентских ссылок OneNote для определенной страницы.</span><span class="sxs-lookup"><span data-stu-id="916f1-257">Get the title, created time, and OneNote client links for a specific page.</span></span>

```
[GET] ../pages/{page-id}?select=title,createdTime,links
```

### <a name="select--expand--filter-multiple-levels"></a><span data-ttu-id="916f1-258">select, expand и filter (несколько уровней)</span><span class="sxs-lookup"><span data-stu-id="916f1-258">select & expand & filter (multiple levels)</span></span>  

<span data-ttu-id="916f1-259">Получение имени и ссылки **pagesUrl** для всех разделов в записной книжке по умолчанию пользователя.</span><span class="sxs-lookup"><span data-stu-id="916f1-259">Get the name and **pagesUrl** link for all sections in the user's default notebook.</span></span>

```
[GET] ../notebooks?select=name&expand=sections(select=name,pagesUrl)&filter=isDefault eq true
```

### <a name="top--select--orderby"></a><span data-ttu-id="916f1-260">top, select и orderby</span><span class="sxs-lookup"><span data-stu-id="916f1-260">top & select & orderby</span></span> 

<span data-ttu-id="916f1-261">Получение названия и ссылки **self** для первых 50 страниц, упорядоченных по названию в алфавитном порядке.</span><span class="sxs-lookup"><span data-stu-id="916f1-261">Get the title and **self** link for the first 50 pages, ordered alphabetically by title.</span></span> <span data-ttu-id="916f1-262">По умолчанию API возвращает 20 записей. Максимальное количество записей — 100.</span><span class="sxs-lookup"><span data-stu-id="916f1-262">The API returns 20 entries by default with a maximum of 100.</span></span> <span data-ttu-id="916f1-263">По умолчанию для страниц используется порядок сортировки `lastModifiedTime desc`.</span><span class="sxs-lookup"><span data-stu-id="916f1-263">The default sort order for pages is `lastModifiedTime desc`.</span></span>

```
[GET] ../pages?top=50&select=title,self&orderby=title
```

### <a name="skip--top--select--orderby"></a><span data-ttu-id="916f1-264">skip, top, select и orderby</span><span class="sxs-lookup"><span data-stu-id="916f1-264">skip & top & select & orderby</span></span>  

<span data-ttu-id="916f1-p117">Получение страниц с 51 по 100. По умолчанию API возвращает 20 записей, а максимальное количество составляет 100.</span><span class="sxs-lookup"><span data-stu-id="916f1-p117">Get pages 51 to 100. The API returns 20 entries by default with a maximum of 100.</span></span>

```
[GET] ../pages?skip=50&top=50&select=title,self&orderby=title
```

> <span data-ttu-id="916f1-267">**Примечание.** Запросы GET для страниц, которые получают количество записей по умолчанию (то есть в них не указывается выражение **top**), возвращают в ответе ссылку **@odata.nextLink**, с помощью которой можно получить следующие 20 записей.</span><span class="sxs-lookup"><span data-stu-id="916f1-267">**Note:** GET requests for pages that retrieve the default number of entries (that is, they don't specify a **top** expression) return an **@odata.nextLink** link in the response that you can use to get the next 20 entries.</span></span>
 

<a name="supported-odata-query-string-options"></a>

## <a name="supported-odata-query-string-options"></a><span data-ttu-id="916f1-268">Поддерживаемые параметры строки запроса OData</span><span class="sxs-lookup"><span data-stu-id="916f1-268">Supported OData query string options</span></span>

<span data-ttu-id="916f1-269">Вы можете настраивать запросы GET к Microsoft Graph, используя параметры строки запроса OData, и получать только нужную информацию.</span><span class="sxs-lookup"><span data-stu-id="916f1-269">When sending GET requests to Microsoft Graph, you can use OData query string options to customize your query and get just the information you need.</span></span> <span data-ttu-id="916f1-270">Они также могут повышать производительность, уменьшая количество вызовов службы и размер полезных данных ответа.</span><span class="sxs-lookup"><span data-stu-id="916f1-270">They can also improve performance by reducing the number of calls to the service and the size of the response payload.</span></span>

> <span data-ttu-id="916f1-271">**Примечание.** Для удобства чтения в примерах из этой статьи не используется код %20, которым нужно заменять пробелы в строке запроса URL: `filter=isDefault%20eq%20true`</span><span class="sxs-lookup"><span data-stu-id="916f1-271">**Note:** For readability, the examples in this article don't use the %20 percent-encoding required for spaces in the URL query string: `filter=isDefault%20eq%20true`</span></span>
 
| <span data-ttu-id="916f1-272">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="916f1-272">Query option</span></span> | <span data-ttu-id="916f1-273">Пример и описание</span><span class="sxs-lookup"><span data-stu-id="916f1-273">Example and description</span></span> |  
|------|------|  
| <span data-ttu-id="916f1-274">count</span><span class="sxs-lookup"><span data-stu-id="916f1-274">count</span></span> | <p>`count=true`</p><p><span data-ttu-id="916f1-p119">Количество записей в коллекции. Значение возвращается в свойстве **@odata.count** отклика.</span><span class="sxs-lookup"><span data-stu-id="916f1-p119">The count of entities in the collection. The value is returned in the **@odata.count** property in the response.</span></span></p> |  
| <span data-ttu-id="916f1-277">expand</span><span class="sxs-lookup"><span data-stu-id="916f1-277">expand</span></span> | <p>`expand=sections,sectionGroups`</p><p><span data-ttu-id="916f1-278">Свойства навигации, которые следует вернуть в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="916f1-278">The navigation properties to return inline in the response.</span></span> <span data-ttu-id="916f1-279">Для выражений **expand** поддерживаются следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="916f1-279">The following properties are supported for **expand** expressions:</span></span><br /> <span data-ttu-id="916f1-280">страницы: **parentNotebook**, **parentSection**;</span><span class="sxs-lookup"><span data-stu-id="916f1-280">- Pages: **parentNotebook**, **parentSection**</span></span><br /> <span data-ttu-id="916f1-281">разделы: **parentNotebook**, **parentSectionGroup**;</span><span class="sxs-lookup"><span data-stu-id="916f1-281">- Sections: **parentNotebook**, **parentSectionGroup**</span></span><br /> <span data-ttu-id="916f1-282">группы разделов: **sections**, **sectionGroups**, **parentNotebook**, **parentSectionGroup**;</span><span class="sxs-lookup"><span data-stu-id="916f1-282">- Section groups: **sections**, **sectionGroups**, **parentNotebook**, **parentSectionGroup**</span></span><br /> <span data-ttu-id="916f1-283">записные книжки: **sections**, **sectionGroups**.</span><span class="sxs-lookup"><span data-stu-id="916f1-283">- Notebooks: **sections**, **sectionGroups**</span></span></p><p><span data-ttu-id="916f1-p121">По умолчанию запросы GET для страниц разворачивают **parentSection** и выделяют свойства раздела **id**, **name** и **self**. По умолчанию запросы GET для разделов и групп разделов разворачивают как **parentNotebook**, так и **parentSectionGroup**, а также выделяют родительские свойства **id**, **name** и **self**.</span><span class="sxs-lookup"><span data-stu-id="916f1-p121">By default, GET requests for pages expands **parentSection** and select the section's **id**, **name**, and **self** properties. Default GET requests for sections and section groups expand both **parentNotebook** and **parentSectionGroup**, and select the parents' **id**, **name**, and **self** properties. </span></span></p><p><span data-ttu-id="916f1-286">Может использоваться для одного объекта или коллекции.</span><span class="sxs-lookup"><span data-stu-id="916f1-286">Can be used for a single entity or a collection.</span></span><br /><span data-ttu-id="916f1-287">Свойства следует разделять запятыми.</span><span class="sxs-lookup"><span data-stu-id="916f1-287">Separate multiple properties with commas.</span></span><br /><span data-ttu-id="916f1-288">В именах свойств учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="916f1-288">Property names are case-sensitive.</span></span></p> |   
| <span data-ttu-id="916f1-289">filter</span><span class="sxs-lookup"><span data-stu-id="916f1-289">filter</span></span> | <p>`filter=isDefault eq true`</p><p><span data-ttu-id="916f1-290">Логическое выражение, указывающее, следует ли включать запись в набор результатов.</span><span class="sxs-lookup"><span data-stu-id="916f1-290">A Boolean expression for whether to include an entry in the result set.</span></span> <span data-ttu-id="916f1-291">Поддерживаются следующие функции и операторы OData:</span><span class="sxs-lookup"><span data-stu-id="916f1-291">Supports the following OData operators and functions:</span></span><br /> <span data-ttu-id="916f1-292">— операторы сравнения: **eq**, **ne**, **gt**, **ge**, **lt**, **le**;</span><span class="sxs-lookup"><span data-stu-id="916f1-292">- Comparison operators: **eq**, **ne**, **gt**, **ge**, **lt**, **le**</span></span><br /> <span data-ttu-id="916f1-293">— логические операторы: **and**, **or**, **not**;</span><span class="sxs-lookup"><span data-stu-id="916f1-293">- Logical operators: **and**, **or**, **not**</span></span><br /> <span data-ttu-id="916f1-294">— строковые функции: **contains**, **endswith**, **startswith**, **length**, **indexof**, **substring**, **tolower**, **toupper**, **trim**, **concat**.</span><span class="sxs-lookup"><span data-stu-id="916f1-294">- String functions: **contains**, **endswith**, **startswith**, **length**, **indexof**, **substring**, **tolower**, **toupper**, **trim**, **concat**</span></span></p><p><span data-ttu-id="916f1-295">В случае имен [свойств](#onenote-entity-properties) и сравнения строк OData учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="916f1-295">[Property](#onenote-entity-properties) names and OData string comparisons are case-sensitive.</span></span> <span data-ttu-id="916f1-296">Рекомендуем использовать функцию OData **tolower** для сравнения строк.</span><span class="sxs-lookup"><span data-stu-id="916f1-296">We recommend using the OData **tolower** function for string comparisons.</span></span><br /><br /><span data-ttu-id="916f1-297">**Пример**: `filter=tolower(name) eq 'spring'`.</span><span class="sxs-lookup"><span data-stu-id="916f1-297">**Example**: `filter=tolower(name) eq 'spring'`</span></span></p> |  
| <span data-ttu-id="916f1-298">orderby</span><span class="sxs-lookup"><span data-stu-id="916f1-298">orderby</span></span> | <p>`orderby=title,createdTime desc`</p><p><span data-ttu-id="916f1-p124">
            [Свойства](#onenote-entity-properties) для сортировки с необязательным порядком сортировки \*\*asc\*\* (по умолчанию) или \*\*desc\*\*. Вы можете сортировать по любому свойству сущности в запрошенной коллекции.</span><span class="sxs-lookup"><span data-stu-id="916f1-p124">The [properties](#onenote-entity-properties) to sort by, with an optional **asc** (default) or **desc** sort order. You can sort by any property of the entity in the requested collection.</span></span></p><p><span data-ttu-id="916f1-301">По умолчанию для записных книжек, разделов и групп разделов используется порядок сортировки `name asc`, а для страниц — `lastModifiedTime desc` (сначала отображается последняя измененная страница).</span><span class="sxs-lookup"><span data-stu-id="916f1-301">The default sort order for notebooks, section groups, and sections is `name asc`, and for pages is `lastModifiedTime desc` (last modified page first).</span></span></p><p><span data-ttu-id="916f1-302">Разделяйте свойства запятыми и указывайте их в порядке применения.</span><span class="sxs-lookup"><span data-stu-id="916f1-302">Separate multiple properties with commas, and list them in the order that you want them applied.</span></span> <span data-ttu-id="916f1-303">В именах свойств учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="916f1-303">Property names are case-sensitive.</span></span></p> |  
| <span data-ttu-id="916f1-304">search</span><span class="sxs-lookup"><span data-stu-id="916f1-304">search</span></span> | <p>`search=cell div`</p><p><span data-ttu-id="916f1-305">Доступен только для пользовательских записных книжек.</span><span class="sxs-lookup"><span data-stu-id="916f1-305">Available for consumer notebooks only.</span></span></p><p><span data-ttu-id="916f1-p126">Термин или фраза, которую нужно найти в заголовке и тексте страницы, замещающем тексте изображений и распознанном тексте. По умолчанию поисковые запросы возвращают результаты, отсортированные по релевантности.</span><span class="sxs-lookup"><span data-stu-id="916f1-p126">The term or phrase to search for in the page title, page body, image alt text, and image OCR text. By default, search queries return results sorted by relevance.</span></span></p><p><span data-ttu-id="916f1-308">OneNote использует полнотекстовый поиск Bing для поддержки поиска фраз, выделения корней, игнорирования орфографических ошибок, релевантности и ранжирования, разбиения слов, разных языков и других функций полнотекстового поиска.</span><span class="sxs-lookup"><span data-stu-id="916f1-308">OneNote uses Bing full-text search to support phrase search, stemming, spelling forgiveness, relevance and ranking, word breaking, multiple languages, and other full-text search features.</span></span> <span data-ttu-id="916f1-309">В строках search учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="916f1-309">Search strings are case-insensitive.</span></span></p><p><span data-ttu-id="916f1-310">Применяется только к страницам записных книжек, принадлежащих пользователю.</span><span class="sxs-lookup"><span data-stu-id="916f1-310">Applies only to pages in notebooks owned by the user.</span></span> <span data-ttu-id="916f1-311">Индексированное содержимое является личным и доступно только владельцу.</span><span class="sxs-lookup"><span data-stu-id="916f1-311">Indexed content is private and can only be accessed by the owner.</span></span> <span data-ttu-id="916f1-312">Страницы, защищенные паролем, не индексируются.</span><span class="sxs-lookup"><span data-stu-id="916f1-312">Password-protected pages are not indexed.</span></span> <span data-ttu-id="916f1-313">Применяется только к конечной точке `pages`.</span><span class="sxs-lookup"><span data-stu-id="916f1-313">Applies only to the `pages` endpoint.</span></span></p> |  
| <span data-ttu-id="916f1-314">select</span><span class="sxs-lookup"><span data-stu-id="916f1-314">select</span></span> | <p>`select=id,title`</p><p><span data-ttu-id="916f1-315">Возвращаемые [свойства](#onenote-entity-properties).</span><span class="sxs-lookup"><span data-stu-id="916f1-315">The [properties](#onenote-entity-properties) to return.</span></span> <span data-ttu-id="916f1-316">Может использоваться для одного объекта или коллекции.</span><span class="sxs-lookup"><span data-stu-id="916f1-316">Can be used for a single entity or for a collection.</span></span> <span data-ttu-id="916f1-317">Свойства следует разделять запятыми.</span><span class="sxs-lookup"><span data-stu-id="916f1-317">Separate multiple properties with commas.</span></span> <span data-ttu-id="916f1-318">В именах свойств учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="916f1-318">Property names are case-sensitive.</span></span></p> |  
| <span data-ttu-id="916f1-319">skip</span><span class="sxs-lookup"><span data-stu-id="916f1-319">skip</span></span> | <p>`skip=10`</p><p><span data-ttu-id="916f1-320">Количество записей, которое следует пропустить в наборе результатов.</span><span class="sxs-lookup"><span data-stu-id="916f1-320">The number of entries to skip in the result set.</span></span> <span data-ttu-id="916f1-321">Обычно используется для разбиения результатов на страницы.</span><span class="sxs-lookup"><span data-stu-id="916f1-321">Typically used for paging results.</span></span></p> |  
| <span data-ttu-id="916f1-322">top</span><span class="sxs-lookup"><span data-stu-id="916f1-322">top</span></span> | <p>`top=50`</p><p><span data-ttu-id="916f1-323">Количество записей, которое следует вернуть в наборе результатов, до 100.</span><span class="sxs-lookup"><span data-stu-id="916f1-323">The number of entries to return in the result set, up to a maximum of 100.</span></span> <span data-ttu-id="916f1-324">Значение по умолчанию — 20.</span><span class="sxs-lookup"><span data-stu-id="916f1-324">The default value is 20.</span></span></p> |  

<span data-ttu-id="916f1-325">В Microsoft Graph также доступен параметр строки запроса `pagelevel`, с помощью которого можно получить уровень и порядок страниц в родительском разделе.</span><span class="sxs-lookup"><span data-stu-id="916f1-325">Microsoft Graph also provides the `pagelevel` query string option you can use to get the level and order of pages within the parent section.</span></span> <span data-ttu-id="916f1-326">Применяется только к запросам страниц в определенном разделе и запросам определенной страницы.</span><span class="sxs-lookup"><span data-stu-id="916f1-326">Applies only to queries for pages in a specific section or queries for a specific page.</span></span> 

#### <a name="examples"></a><span data-ttu-id="916f1-327">Примеры</span><span class="sxs-lookup"><span data-stu-id="916f1-327">Examples</span></span> 

- `GET ../sections/{section-id}/pages?pagelevel=true` 
- `GET ../pages/{page-id}?pagelevel=true` 

### <a name="supported-odata-operators-and-functions"></a><span data-ttu-id="916f1-328">Поддерживаемые операторы и функции OData</span><span class="sxs-lookup"><span data-stu-id="916f1-328">Supported OData operators and functions</span></span>

<span data-ttu-id="916f1-329">Microsoft Graph поддерживает указанные ниже функции и операторы OData в выражениях **filter**.</span><span class="sxs-lookup"><span data-stu-id="916f1-329">Microsoft Graph supports the following OData operators and functions in **filter** expressions.</span></span> <span data-ttu-id="916f1-330">Используя выражения OData, помните:</span><span class="sxs-lookup"><span data-stu-id="916f1-330">When using OData expressions, remember:</span></span>

- <span data-ttu-id="916f1-331">Пробелы в строке запроса URL необходимо заменять кодом `%20`.</span><span class="sxs-lookup"><span data-stu-id="916f1-331">Spaces in the URL query string must be replaced with the `%20` encoding.</span></span><br/><br/><span data-ttu-id="916f1-332">**Пример:** `filter=isDefault%20eq%20true`.</span><span class="sxs-lookup"><span data-stu-id="916f1-332">**Example:** `filter=isDefault%20eq%20true`</span></span>

- <span data-ttu-id="916f1-333">В случае имен свойств и сравнения строк OData учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="916f1-333">Property names and OData string comparisons are case-sensitive.</span></span> <span data-ttu-id="916f1-334">Рекомендуем использовать функцию OData **tolower** для сравнения строк.</span><span class="sxs-lookup"><span data-stu-id="916f1-334">We recommend using the OData **tolower** function for string comparisons.</span></span><br/><br/><span data-ttu-id="916f1-335">**Пример:** `filter=tolower(name) eq 'spring'`</span><span class="sxs-lookup"><span data-stu-id="916f1-335">**Example:** `filter=tolower(name) eq 'spring'`</span></span>


| <span data-ttu-id="916f1-336">Оператор сравнения</span><span class="sxs-lookup"><span data-stu-id="916f1-336">Comparison operator</span></span> | <span data-ttu-id="916f1-337">Пример</span><span class="sxs-lookup"><span data-stu-id="916f1-337">Example</span></span> |  
|------|------|  
| <span data-ttu-id="916f1-338">eq</span><span class="sxs-lookup"><span data-stu-id="916f1-338">eq</span></span><br /><span data-ttu-id="916f1-339">(равно)</span><span class="sxs-lookup"><span data-stu-id="916f1-339">(equal to)</span></span> | `createdByAppId eq '{app-id}'` |  
| <span data-ttu-id="916f1-340">ne</span><span class="sxs-lookup"><span data-stu-id="916f1-340">ne</span></span><br /><span data-ttu-id="916f1-341">(не равно)</span><span class="sxs-lookup"><span data-stu-id="916f1-341">(not equal to)</span></span> | `userRole ne 'Owner'` |  
| <span data-ttu-id="916f1-342">gt</span><span class="sxs-lookup"><span data-stu-id="916f1-342">gt</span></span><br /><span data-ttu-id="916f1-343">(больше)</span><span class="sxs-lookup"><span data-stu-id="916f1-343">(greater than)</span></span> | `createdTime gt 2014-02-23` |  
| <span data-ttu-id="916f1-344">ge</span><span class="sxs-lookup"><span data-stu-id="916f1-344">ge</span></span><br /><span data-ttu-id="916f1-345">(больше или равно)</span><span class="sxs-lookup"><span data-stu-id="916f1-345">(greater than or equal to)</span></span> | `lastModifiedTime ge 2014-05-05T07:00:00Z` |  
| <span data-ttu-id="916f1-346">lt</span><span class="sxs-lookup"><span data-stu-id="916f1-346">lt</span></span><br /><span data-ttu-id="916f1-347">(меньше)</span><span class="sxs-lookup"><span data-stu-id="916f1-347">(less than)</span></span> | `createdTime lt 2014-02-23` |  
| <span data-ttu-id="916f1-348">le</span><span class="sxs-lookup"><span data-stu-id="916f1-348">le</span></span><br /><span data-ttu-id="916f1-349">(меньше или равно)</span><span class="sxs-lookup"><span data-stu-id="916f1-349">(less than or equal to)</span></span> | `lastModifiedTime le 2014-02-23` |  

<br/>

| <span data-ttu-id="916f1-350">Логический оператор</span><span class="sxs-lookup"><span data-stu-id="916f1-350">Logical operator</span></span> | <span data-ttu-id="916f1-351">Пример</span><span class="sxs-lookup"><span data-stu-id="916f1-351">Example</span></span> |  
|------|------|  
| <span data-ttu-id="916f1-352">и</span><span class="sxs-lookup"><span data-stu-id="916f1-352">and</span></span> | `createdTime le 2014-01-30 and createdTime gt 2014-01-23` |  
| <span data-ttu-id="916f1-353">Кроме того:</span><span class="sxs-lookup"><span data-stu-id="916f1-353">or</span></span> | `createdByAppId eq '{app-id}' or createdByAppId eq '{app-id}'` |  
| <span data-ttu-id="916f1-354">
not</span><span class="sxs-lookup"><span data-stu-id="916f1-354">not</span></span> | `not contains(tolower(title),'school')` |  

<br/>
  
| <span data-ttu-id="916f1-355">Строкова функция</span><span class="sxs-lookup"><span data-stu-id="916f1-355">String function</span></span> | <span data-ttu-id="916f1-356">Пример</span><span class="sxs-lookup"><span data-stu-id="916f1-356">Example</span></span> |  
|------|------|   
| <span data-ttu-id="916f1-357">contains</span><span class="sxs-lookup"><span data-stu-id="916f1-357">contains</span></span> | `contains(tolower(title),'spring')` |  
| <span data-ttu-id="916f1-358">endswith</span><span class="sxs-lookup"><span data-stu-id="916f1-358">endswith</span></span> | `endswith(tolower(title),'spring')` |  
| <span data-ttu-id="916f1-359">startswith</span><span class="sxs-lookup"><span data-stu-id="916f1-359">startswith</span></span> | `startswith(tolower(title),'spring')` |  
| <span data-ttu-id="916f1-360">length</span><span class="sxs-lookup"><span data-stu-id="916f1-360">length</span></span> | `length(title) eq 19` |  
| <span data-ttu-id="916f1-361">indexof</span><span class="sxs-lookup"><span data-stu-id="916f1-361">indexof</span></span> | `indexof(tolower(title),'spring') eq 1` |  
| <span data-ttu-id="916f1-362">substring</span><span class="sxs-lookup"><span data-stu-id="916f1-362">substring</span></span> | `substring(tolower(title),1) eq 'spring'` |  
| <span data-ttu-id="916f1-363">tolower</span><span class="sxs-lookup"><span data-stu-id="916f1-363">tolower</span></span> | `tolower(title) eq 'spring'` |  
| <span data-ttu-id="916f1-364">toupper</span><span class="sxs-lookup"><span data-stu-id="916f1-364">toupper</span></span> | `toupper(title) eq 'SPRING'` |  
| <span data-ttu-id="916f1-365">trim</span><span class="sxs-lookup"><span data-stu-id="916f1-365">trim</span></span> | `trim(tolower(title)) eq 'spring'` |  
| <span data-ttu-id="916f1-366">concat</span><span class="sxs-lookup"><span data-stu-id="916f1-366">concat</span></span> | `concat(title,'- by MyRecipesApp') eq 'Carrot Cake Recipe - by MyRecipesApp'` |  
 

<a name="properties"></a>

## <a name="onenote-entity-properties"></a><span data-ttu-id="916f1-367">Свойства объектов OneNote</span><span class="sxs-lookup"><span data-stu-id="916f1-367">OneNote entity properties</span></span>

<span data-ttu-id="916f1-368">Выражения запроса **filter**, **select**, **expand** и **orderby** могут включать свойства объектов OneNote.</span><span class="sxs-lookup"><span data-stu-id="916f1-368">The **filter**, **select**, **expand**, and **orderby** query expressions can include properties of OneNote entities.</span></span> 

#### <a name="example"></a><span data-ttu-id="916f1-369">Пример</span><span class="sxs-lookup"><span data-stu-id="916f1-369">Example</span></span>

`../sections?filter=createdTime ge 2015-01-01&select=name,pagesUrl&orderby=lastModifiedTime desc` 

<span data-ttu-id="916f1-370">Для имен свойств в выражениях запроса учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="916f1-370">Property names are case-sensitive in query expressions.</span></span>

<span data-ttu-id="916f1-371">Список свойств и типы свойств см. в следующих статьях документации по API REST Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="916f1-371">For the list of properties and property types, see the following resources in the Microsoft Graph API REST reference:</span></span>

- [<span data-ttu-id="916f1-372">Запрос GET для страниц</span><span class="sxs-lookup"><span data-stu-id="916f1-372">GET Pages</span></span>](/graph/api/page-get?view=graph-rest-1.0)
- [<span data-ttu-id="916f1-373">GET Sections</span><span class="sxs-lookup"><span data-stu-id="916f1-373">GET Sections</span></span>](/graph/api/section-get?view=graph-rest-1.0)
- [<span data-ttu-id="916f1-374">GET SectionGroups</span><span class="sxs-lookup"><span data-stu-id="916f1-374">GET SectionGroups</span></span>](/graph/api/sectiongroup-get?view=graph-rest-1.0)
- [<span data-ttu-id="916f1-375">Запрос GET для записных книжек</span><span class="sxs-lookup"><span data-stu-id="916f1-375">GET Notebooks</span></span>](/graph/api/notebook-get?view=graph-rest-1.0) 



<span data-ttu-id="916f1-376">Параметр строки запроса **expand** можно использовать со следующими свойствами навигации:</span><span class="sxs-lookup"><span data-stu-id="916f1-376">The **expand** query string option can be used with the following navigation properties:</span></span>

- <span data-ttu-id="916f1-377">страницы: **parentNotebook**, **parentSection**;</span><span class="sxs-lookup"><span data-stu-id="916f1-377">Pages: **parentNotebook**, **parentSection**</span></span>
- <span data-ttu-id="916f1-378">разделы: **parentNotebook**, **parentSectionGroup**;</span><span class="sxs-lookup"><span data-stu-id="916f1-378">Sections: **parentNotebook**, **parentSectionGroup**</span></span>
- <span data-ttu-id="916f1-379">группы разделов: **sections**, **sectionGroups**, **parentNotebook**, **parentSectionGroup**;</span><span class="sxs-lookup"><span data-stu-id="916f1-379">Section groups: **sections**, **sectionGroups**, **parentNotebook**, **parentSectionGroup**</span></span>
- <span data-ttu-id="916f1-380">записные книжки: **sections**, **sectionGroups**.</span><span class="sxs-lookup"><span data-stu-id="916f1-380">Notebooks: **sections**, **sectionGroups**</span></span>


<a name="request-response-info"></a>

## <a name="request-and-response-information-for-get-requests"></a><span data-ttu-id="916f1-381">Информация о запросах *GET* и соответствующих ответах</span><span class="sxs-lookup"><span data-stu-id="916f1-381">Request and response information for *GET* requests</span></span>

| <span data-ttu-id="916f1-382">Данные запроса</span><span class="sxs-lookup"><span data-stu-id="916f1-382">Request data</span></span> | <span data-ttu-id="916f1-383">Описание</span><span class="sxs-lookup"><span data-stu-id="916f1-383">Description</span></span> |  
|------|------|  
| <span data-ttu-id="916f1-384">Протокол</span><span class="sxs-lookup"><span data-stu-id="916f1-384">Protocol</span></span> | <span data-ttu-id="916f1-385">Все запросы используют протокол SSL/TLS для HTTPS.</span><span class="sxs-lookup"><span data-stu-id="916f1-385">All requests use the SSL/TLS HTTPS protocol.</span></span> |  
| <span data-ttu-id="916f1-386">Заголовок Authorization</span><span class="sxs-lookup"><span data-stu-id="916f1-386">Authorization header</span></span> | <p><span data-ttu-id="916f1-387">`Bearer {token}`, где `{token}` — действительный маркер доступа OAuth 2.0 для зарегистрированного приложения.</span><span class="sxs-lookup"><span data-stu-id="916f1-387">`Bearer {token}`, where `{token}` is a valid OAuth 2.0 access token for your registered app.</span></span></p><p><span data-ttu-id="916f1-388">Если он отсутствует или является недействительным, запрос завершится ошибкой с кодом состояния 401.</span><span class="sxs-lookup"><span data-stu-id="916f1-388">If missing or invalid, the request fails with a 401 status code.</span></span> <span data-ttu-id="916f1-389">См. статью [Проверка подлинности и разрешения](permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="916f1-389">See [Authentication and permissions](permissions-reference.md).</span></span></p> |  
| <span data-ttu-id="916f1-390">Заголовок Accept</span><span class="sxs-lookup"><span data-stu-id="916f1-390">Accept header</span></span> | <p> <span data-ttu-id="916f1-391">`application/json` — для объектов OneNote и их наборов.</span><span class="sxs-lookup"><span data-stu-id="916f1-391">`application/json` for OneNote entities and entity sets</span></span></p><p> <span data-ttu-id="916f1-392">`text/html` — для содержимого страницы.</span><span class="sxs-lookup"><span data-stu-id="916f1-392">`text/html` for page content</span></span></p> | 

<br/>

| <span data-ttu-id="916f1-393">Данные в отклике</span><span class="sxs-lookup"><span data-stu-id="916f1-393">Response data</span></span> | <span data-ttu-id="916f1-394">Описание</span><span class="sxs-lookup"><span data-stu-id="916f1-394">Description</span></span> |  
|------|------|  
| <span data-ttu-id="916f1-395">Код успешного завершения</span><span class="sxs-lookup"><span data-stu-id="916f1-395">Success code</span></span> | <span data-ttu-id="916f1-396">Код состояния HTTP 200</span><span class="sxs-lookup"><span data-stu-id="916f1-396">A 200 HTTP status code.</span></span> |  
| <span data-ttu-id="916f1-397">Текст ответа</span><span class="sxs-lookup"><span data-stu-id="916f1-397">Response body</span></span> | <span data-ttu-id="916f1-398">Представление объекта или набора объектов в формате JSON, HTML-код страницы или двоичные данные файлового ресурса.</span><span class="sxs-lookup"><span data-stu-id="916f1-398">An OData representation of the entity or entity set in JSON format, the page HTML, or file resource binary data.</span></span>  |  
| <span data-ttu-id="916f1-399">Ошибки</span><span class="sxs-lookup"><span data-stu-id="916f1-399">Errors</span></span> | <span data-ttu-id="916f1-400">Если запрос завершается с ошибкой, API возвращает [ошибки](onenote-error-codes.md) в объекте **@api.diagnostics** в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="916f1-400">If the request fails, the API returns [errors](onenote-error-codes.md) in the **@api.diagnostics** object in the response body.</span></span> |  
| <span data-ttu-id="916f1-401">Заголовок X-CorrelationId</span><span class="sxs-lookup"><span data-stu-id="916f1-401">X-CorrelationId header</span></span> | <span data-ttu-id="916f1-402">GUID, уникальный идентификатор запроса.</span><span class="sxs-lookup"><span data-stu-id="916f1-402">A GUID that uniquely identifies the request.</span></span> <span data-ttu-id="916f1-403">Это значение можно использовать вместе со значением заголовка Date при устранении неполадок совместно со службой поддержки Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="916f1-403">You can use this value along with the value of the Date header when working with Microsoft support to troubleshoot issues.</span></span> |  


<a name="root-url"></a>

### <a name="constructing-the-microsoft-graph-notes-service-root-url"></a><span data-ttu-id="916f1-404">Составление корневого URL-адреса для службы заметок Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="916f1-404">Constructing the Microsoft Graph notes service root URL</span></span>

<span data-ttu-id="916f1-405">Для всех вызовов заметок Microsoft Graph используется следующий формат корневого URL-адреса:</span><span class="sxs-lookup"><span data-stu-id="916f1-405">The Microsoft Graph notes root URL uses the following format for all calls to Microsoft Graph notes:</span></span>

`https://graph.microsoft.com/{version}/me/onenote/`  

<span data-ttu-id="916f1-406">Сегмент `version` URL-адреса представляет нужную версию Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="916f1-406">The `version` segment in the URL represents the version of Microsoft Graph that you want to use.</span></span> <span data-ttu-id="916f1-407">Используйте значение `v1.0` для стабильного кода в рабочей среде.</span><span class="sxs-lookup"><span data-stu-id="916f1-407">Use `v1.0` for stable production code.</span></span> <span data-ttu-id="916f1-408">Используйте значение `beta`, чтобы опробовать функцию, находящуюся на стадии разработки.</span><span class="sxs-lookup"><span data-stu-id="916f1-408">Use `beta` to try out a feature that's in development.</span></span> <span data-ttu-id="916f1-409">Функции бета-версии могут меняться, поэтому не следует использовать их в производственном коде.</span><span class="sxs-lookup"><span data-stu-id="916f1-409">Features and functionality in beta may change, so you shouldn't use it in your production code.</span></span> 

<span data-ttu-id="916f1-410">Используйте значение `me` для содержимого OneNote, доступного текущему пользователю (если он является владельцем или с ним поделились этим содержимым).</span><span class="sxs-lookup"><span data-stu-id="916f1-410">Use `me` for OneNote content that the current user can access (owned and shared).</span></span> <span data-ttu-id="916f1-411">Используйте значение `users/{id}` для содержимого OneNote, которым указанный (в URL-адресе) пользователь поделился с текущим пользователем.</span><span class="sxs-lookup"><span data-stu-id="916f1-411">Use `users/{id}` for OneNote content that the specified user (in the URL) has shared with the current user.</span></span> <span data-ttu-id="916f1-412">Используйте [Microsoft Graph](https://graph.microsoft.com/v1.0/users) для получения ИД пользователей.</span><span class="sxs-lookup"><span data-stu-id="916f1-412">Use [Microsoft Graph](https://graph.microsoft.com/v1.0/users) to get user IDs.</span></span> 


<a name="permissions"></a>

## <a name="permissions-for-get-requests"></a><span data-ttu-id="916f1-413">Разрешения для запросов GET</span><span class="sxs-lookup"><span data-stu-id="916f1-413">Permissions for GET requests</span></span>

<span data-ttu-id="916f1-414">Чтобы получить содержимое или структуру OneNote, необходимо запросить соответствующие разрешения.</span><span class="sxs-lookup"><span data-stu-id="916f1-414">To get OneNote content or structure, you'll need to request appropriate permissions.</span></span> 

<span data-ttu-id="916f1-415">Указанные ниже разрешения позволяют выполнять запросы GET к Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="916f1-415">The following scopes allow GET requests to Microsoft Graph.</span></span> <span data-ttu-id="916f1-416">Выберите минимальный уровень разрешений, необходимый для работы вашего приложения.</span><span class="sxs-lookup"><span data-stu-id="916f1-416">Choose the lowest level of permissions that your app needs to do its work.</span></span>

<span data-ttu-id="916f1-417">Варианты:</span><span class="sxs-lookup"><span data-stu-id="916f1-417">Choose from:</span></span>

- <span data-ttu-id="916f1-418">Notes.read</span><span class="sxs-lookup"><span data-stu-id="916f1-418">Notes.read</span></span>
- <span data-ttu-id="916f1-419">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="916f1-419">Notes.ReadWrite</span></span>
- <span data-ttu-id="916f1-420">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="916f1-420">Notes.ReadWrite.All</span></span>

<span data-ttu-id="916f1-421">Дополнительные сведения об областях разрешений и принципе их использования см. в [справочнике по разрешениям Microsoft Graph](permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="916f1-421">For more information about permission scopes and how they work, see [Microsoft Graph permissions reference](permissions-reference.md).</span></span>

<a name="see-also"></a>

## <a name="see-also"></a><span data-ttu-id="916f1-422">См. также</span><span class="sxs-lookup"><span data-stu-id="916f1-422">See also</span></span>

- [<span data-ttu-id="916f1-423">Входной и выходной HTML-код для страниц OneNote</span><span class="sxs-lookup"><span data-stu-id="916f1-423">Input and output HTML for OneNote pages</span></span>](onenote-input-output-html.md)
- [<span data-ttu-id="916f1-424">Интеграция с OneNote</span><span class="sxs-lookup"><span data-stu-id="916f1-424">Integrate with OneNote</span></span>](integrate-with-onenote.md)
- [<span data-ttu-id="916f1-425">Блог разработчиков OneNote</span><span class="sxs-lookup"><span data-stu-id="916f1-425">OneNote Developer Blog</span></span>](https://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="916f1-426">Вопросы разработки OneNote на сайте Stack Overflow</span><span class="sxs-lookup"><span data-stu-id="916f1-426">OneNote development questions on Stack Overflow</span></span>](https://go.microsoft.com/fwlink/?LinkID=390182)
- [<span data-ttu-id="916f1-427">Репозитории GitHub OneNote</span><span class="sxs-lookup"><span data-stu-id="916f1-427">OneNote GitHub repos</span></span>](https://go.microsoft.com/fwlink/?LinkID=390178)  
