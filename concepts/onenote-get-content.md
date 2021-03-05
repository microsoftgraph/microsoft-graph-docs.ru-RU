---
title: Получение содержимого и структуры OneNote с помощью Microsoft Graph
description: " Корпоративная записная книжка в Microsoft 365"
author: jewan-microsoft
localization_priority: Priority
ms.prod: onenote
ms.openlocfilehash: 9efc445fa1d239cc180b7bfeeb71bb5d0848f227
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50474948"
---
# <a name="get-onenote-content-and-structure-with-microsoft-graph"></a><span data-ttu-id="c4f00-103">Получение содержимого и структуры OneNote с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="c4f00-103">Get OneNote content and structure with Microsoft Graph</span></span>

<span data-ttu-id="c4f00-104">**Область применения:** Пользовательские записные книжки в OneDrive | Корпоративные записные книжки в Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="c4f00-104">**Applies to**: Consumer notebooks on OneDrive | Enterprise notebooks on Microsoft 365</span></span>

<span data-ttu-id="c4f00-105">Чтобы получить содержимое и структуру OneNote, необходимо отправить запрос GET к целевой конечной точке.</span><span class="sxs-lookup"><span data-stu-id="c4f00-105">To get OneNote content and structure, you send a GET request to the target endpoint.</span></span> <span data-ttu-id="c4f00-106">Пример:</span><span class="sxs-lookup"><span data-stu-id="c4f00-106">For example:</span></span>

`GET ../onenote/pages/{id}`

<span data-ttu-id="c4f00-107">Если запрос выполнен успешно, Microsoft Graph возвращает код состояния HTTP 200 и запрашиваемые объекты или содержимое.</span><span class="sxs-lookup"><span data-stu-id="c4f00-107">If the request is successful, Microsoft Graph returns a 200 HTTP status code and the entities or content that you requested.</span></span> <span data-ttu-id="c4f00-108">Объекты OneNote возвращаются в виде объектов JSON, соответствующих спецификации OData версии 4.0.</span><span class="sxs-lookup"><span data-stu-id="c4f00-108">OneNote entities are returned as JSON objects that conform to the OData version 4.0 specification.</span></span>

<span data-ttu-id="c4f00-109">С помощью параметров строки запроса вы можете фильтровать запросы и повышать производительность.</span><span class="sxs-lookup"><span data-stu-id="c4f00-109">By using query string options, you can filter your queries and improve performance.</span></span>


<a name="request-uri"></a>

## <a name="construct-the-request-uri"></a><span data-ttu-id="c4f00-110">Создание URI запроса</span><span class="sxs-lookup"><span data-stu-id="c4f00-110">Construct the request URI</span></span>

<span data-ttu-id="c4f00-111">Чтобы создать URI запроса, начните с корневого URL-адреса службы:</span><span class="sxs-lookup"><span data-stu-id="c4f00-111">To construct the request URI, start with the service root URL:</span></span>

`https://graph.microsoft.com/v1.0/me/onenote`

<br/>

<span data-ttu-id="c4f00-112">Затем добавьте конечную точку нужного ресурса.</span><span class="sxs-lookup"><span data-stu-id="c4f00-112">Then append the endpoint of the resource you want to retrieve.</span></span> <span data-ttu-id="c4f00-113">([Пути к ресурсам](#resource-paths-for-get-requests) показаны в следующем разделе.)</span><span class="sxs-lookup"><span data-stu-id="c4f00-113">([Resource paths](#resource-paths-for-get-requests) are shown in the next section.)</span></span>

<span data-ttu-id="c4f00-114">Полный URI запроса будет выглядеть так, как в одном из следующих примеров:</span><span class="sxs-lookup"><span data-stu-id="c4f00-114">Your full request URI will look like one of these examples:</span></span>

- `https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}/sections`
- `https://graph.microsoft.com/v1.0/me/onenote/notes/pages`
- `https://graph.microsoft.com/v1.0/me/onenote/pages?select=title,self`

> <span data-ttu-id="c4f00-115">**Примечание.** Узнайте больше о [корневом URL-адресе службы](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0#root-url).</span><span class="sxs-lookup"><span data-stu-id="c4f00-115">**Note:** Learn more about the [service root URL](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0#root-url).</span></span>

<a name="resource-paths"></a>

## <a name="resource-paths-for-get-requests"></a><span data-ttu-id="c4f00-116">Пути к ресурсам для запросов GET</span><span class="sxs-lookup"><span data-stu-id="c4f00-116">Resource paths for GET requests</span></span>

<span data-ttu-id="c4f00-117">Используйте приведенные ниже пути к ресурсам, чтобы получать страницы, разделы, группы разделов, записные книжки, а также изображения или файлы.</span><span class="sxs-lookup"><span data-stu-id="c4f00-117">Use the following resource paths to get pages, sections, section groups, notebooks, and image or file resources.</span></span>

- [<span data-ttu-id="c4f00-118">Коллекция Page</span><span class="sxs-lookup"><span data-stu-id="c4f00-118">Page collection</span></span>](#page-collection)
- [<span data-ttu-id="c4f00-119">Объект Page</span><span class="sxs-lookup"><span data-stu-id="c4f00-119">Page entity</span></span>](#page-entity)
- [<span data-ttu-id="c4f00-120">Предварительный просмотр страницы</span><span class="sxs-lookup"><span data-stu-id="c4f00-120">Page preview</span></span>](#page-preview)
- [<span data-ttu-id="c4f00-121">HTML-контент страницы</span><span class="sxs-lookup"><span data-stu-id="c4f00-121">Page HTML content</span></span>](#page-html-content)
- [<span data-ttu-id="c4f00-122">Коллекция Section</span><span class="sxs-lookup"><span data-stu-id="c4f00-122">Section collection</span></span>](#section-collection)
- [<span data-ttu-id="c4f00-123">Объект Section</span><span class="sxs-lookup"><span data-stu-id="c4f00-123">Section entity</span></span>](#section-entity)
- [<span data-ttu-id="c4f00-124">Коллекция SectionGroup</span><span class="sxs-lookup"><span data-stu-id="c4f00-124">SectionGroup collection</span></span>](#sectiongroup-collection)
- [<span data-ttu-id="c4f00-125">Объект SectionGroup</span><span class="sxs-lookup"><span data-stu-id="c4f00-125">SectionGroup entity</span></span>](#sectiongroup-entity)
- [<span data-ttu-id="c4f00-126">Коллекция Notebook</span><span class="sxs-lookup"><span data-stu-id="c4f00-126">Notebook collection</span></span>](#notebook-collection)
- [<span data-ttu-id="c4f00-127">Объект Notebook</span><span class="sxs-lookup"><span data-stu-id="c4f00-127">Notebook entity</span></span>](#notebook-entity)
- [<span data-ttu-id="c4f00-128">Ресурс изображений или других файлов</span><span class="sxs-lookup"><span data-stu-id="c4f00-128">Image or other file resource</span></span>](#image-or-other-file-resource)

<a name="get-pages"></a>

### <a name="page-collection"></a><span data-ttu-id="c4f00-129">Коллекция Page</span><span class="sxs-lookup"><span data-stu-id="c4f00-129">Page collection</span></span>

<span data-ttu-id="c4f00-130">Получение страниц (метаданных) из всех записных книжек.</span><span class="sxs-lookup"><span data-stu-id="c4f00-130">Get pages (metadata) across all notebooks.</span></span>

`../pages[?filter,orderby,select,expand,top,skip,search,count]`

<br/>

<span data-ttu-id="c4f00-131">Получение страниц (метаданных) из определенного раздела.</span><span class="sxs-lookup"><span data-stu-id="c4f00-131">Get pages (metadata) from a specific section.</span></span>

`../sections/{section-id}/pages[?filter,orderby,select,expand,top,skip,search,count,pagelevel]`

<br/>
 
<span data-ttu-id="c4f00-132">Параметр строки запроса `search` доступен только для пользовательских записных книжек.</span><span class="sxs-lookup"><span data-stu-id="c4f00-132">The `search` query string option is available for consumer notebooks only.</span></span>

<span data-ttu-id="c4f00-133">По умолчанию для страниц используется порядок сортировки `lastModifiedTime desc`.</span><span class="sxs-lookup"><span data-stu-id="c4f00-133">The default sort order for pages is `lastModifiedTime desc`.</span></span>

<span data-ttu-id="c4f00-134">Запрос по умолчанию разворачивает родительский раздел и выбирает свойства `id`, `name` и `self` этого раздела.</span><span class="sxs-lookup"><span data-stu-id="c4f00-134">The default query expands the parent section and selects the section's `id`, `name`, and `self` properties.</span></span>

<span data-ttu-id="c4f00-135">По умолчанию в ответ на запросы *GET для страниц* возвращаются только первые 20 записей.</span><span class="sxs-lookup"><span data-stu-id="c4f00-135">By default, only the top 20 entries are returned for *GET pages* requests.</span></span> <span data-ttu-id="c4f00-136">В ответах на запросы, в которых не указан параметр **top**, возвращается ссылка `@odata.nextLink`, с помощью которой можно получить следующие 20 записей.</span><span class="sxs-lookup"><span data-stu-id="c4f00-136">Requests that don't specify a **top** query string option return an `@odata.nextLink` link in the response that you can use to get the next 20 entries.</span></span>

<span data-ttu-id="c4f00-137">Для коллекции страниц в разделе используйте параметр **pagelevel**, чтобы возвращать уровень отступа страниц и их порядок в разделе.</span><span class="sxs-lookup"><span data-stu-id="c4f00-137">For the pages collection in a section, use **pagelevel** to return the indentation level of pages and their order within the section.</span></span> 

#### <a name="example"></a><span data-ttu-id="c4f00-138">Пример</span><span class="sxs-lookup"><span data-stu-id="c4f00-138">Example</span></span>

`GET ../sections/{section-id}/pages?pagelevel=true`



<a name="get-page"></a> 

### <a name="page-entity"></a><span data-ttu-id="c4f00-139">Объект Page</span><span class="sxs-lookup"><span data-stu-id="c4f00-139">Page entity</span></span>

<span data-ttu-id="c4f00-140">Получение метаданных определенной страницы.</span><span class="sxs-lookup"><span data-stu-id="c4f00-140">Get the metadata for a specific page.</span></span> 

`../pages/{page-id}[?select,expand,pagelevel]` 

<br/>

<span data-ttu-id="c4f00-141">Запросы страниц могут разворачивать свойства **parentNotebook** и **parentSection**.</span><span class="sxs-lookup"><span data-stu-id="c4f00-141">Pages can expand the **parentNotebook** and **parentSection** properties.</span></span>

<span data-ttu-id="c4f00-142">Запрос по умолчанию разворачивает родительский раздел и выбирает свойства `id`, `name` и `self` этого раздела.</span><span class="sxs-lookup"><span data-stu-id="c4f00-142">The default query expands the parent section and selects the section's `id`, `name`, and `self` properties.</span></span>

<span data-ttu-id="c4f00-143">С помощью параметра **pagelevel** можно вернуть уровень отступа страницы и ее порядковый номер в родительском разделе.</span><span class="sxs-lookup"><span data-stu-id="c4f00-143">Use **pagelevel** to return the indentation level of the page and its order within its parent section.</span></span> 

#### <a name="example"></a><span data-ttu-id="c4f00-144">Пример</span><span class="sxs-lookup"><span data-stu-id="c4f00-144">Example</span></span>

`GET ../pages/{page-id}?pagelevel=true`



<a name="get-page-preview"></a> 

### <a name="page-preview"></a><span data-ttu-id="c4f00-145">Предварительный просмотр страницы</span><span class="sxs-lookup"><span data-stu-id="c4f00-145">Page preview</span></span>

<span data-ttu-id="c4f00-146">Получение текста и изображений на странице для предварительного просмотра.</span><span class="sxs-lookup"><span data-stu-id="c4f00-146">Get text and image preview content for a page.</span></span>

`../pages/{page-id}/preview`

<br/>


<span data-ttu-id="c4f00-147">Отклик JSON содержит часть контента для предварительного просмотра, благодаря которому пользователи могут узнать, что находится на странице.</span><span class="sxs-lookup"><span data-stu-id="c4f00-147">The JSON response contains the preview content, which you can use to help users identify what's in the page.</span></span>

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

<span data-ttu-id="c4f00-148">Свойство **previewText** содержит фрагмент текста со страницы.</span><span class="sxs-lookup"><span data-stu-id="c4f00-148">The **previewText** property contains a text snippet from the page.</span></span> <span data-ttu-id="c4f00-149">Microsoft Graph возвращает полные фразы длиной до 300 символов.</span><span class="sxs-lookup"><span data-stu-id="c4f00-149">Microsoft Graph returns complete phrases, up to a maximum of 300 characters.</span></span> 

<span data-ttu-id="c4f00-150">Если на странице есть изображение, подходящее для предварительного просмотра, то свойство **href** объекта **previewImageUrl** будет содержать ссылку на общедоступный [ресурс изображения](#image-or-other-file-resource).</span><span class="sxs-lookup"><span data-stu-id="c4f00-150">If the page has an image that can be used to build a preview UI, the **href** property in the **previewImageUrl** object contains a link to a public [image resource](#image-or-other-file-resource).</span></span> <span data-ttu-id="c4f00-151">Эту ссылку можно использовать в коде HTML.</span><span class="sxs-lookup"><span data-stu-id="c4f00-151">You can use this link in HTML.</span></span> <span data-ttu-id="c4f00-152">Если не сделать этого, свойство **href** возвратит значение NULL.</span><span class="sxs-lookup"><span data-stu-id="c4f00-152">Otherwise, **href** returns null.</span></span>

#### <a name="example"></a><span data-ttu-id="c4f00-153">Пример</span><span class="sxs-lookup"><span data-stu-id="c4f00-153">Example</span></span> 

`<img src="https://www.onenote.com/api/v1.0/resources/{id}/content?publicAuth=true&mimeType=image/png" />`


<a name="get-page-content"></a> 

### <a name="page-html-content"></a><span data-ttu-id="c4f00-154">HTML-контент страницы</span><span class="sxs-lookup"><span data-stu-id="c4f00-154">Page HTML content</span></span>

<span data-ttu-id="c4f00-155">Получение HTML-контента страницы.</span><span class="sxs-lookup"><span data-stu-id="c4f00-155">Get the HTML content of a page.</span></span>

`../pages/{page-id}/content[?includeIDs]`

<span data-ttu-id="c4f00-156">(*Дополнительные сведения о [возвращаемом HTML-контенте](onenote-input-output-html.md)*.)</span><span class="sxs-lookup"><span data-stu-id="c4f00-156">(*learn more about [returned HTML content](onenote-input-output-html.md)*)</span></span> 

<br/>

<span data-ttu-id="c4f00-157">Указав в строке запроса параметр **includeIDs=true**, можно получить созданные идентификаторы, используемые для [обновления страницы](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="c4f00-157">Use the **includeIDs=true** query string option to get generated IDs used to [update the page](onenote-update-page.md).</span></span>



<a name="get-sections"></a>

### <a name="section-collection"></a><span data-ttu-id="c4f00-158">Коллекция Section</span><span class="sxs-lookup"><span data-stu-id="c4f00-158">Section collection</span></span>

<span data-ttu-id="c4f00-159">Получение всех разделов всех записных книжек, принадлежащих пользователю, включая разделы из вложенных групп разделов.</span><span class="sxs-lookup"><span data-stu-id="c4f00-159">Get all sections from all notebooks that are owned by the user, including sections in nested section groups.</span></span>

`../sections[?filter,orderby,select,top,skip,expand,count]` 

<br/>

<span data-ttu-id="c4f00-160">Получение всех разделов, вложенных непосредственно в определенную группу разделов.</span><span class="sxs-lookup"><span data-stu-id="c4f00-160">Get all sections that are directly under a specific section group.</span></span>

`../sectionGroups/{sectiongroup-id}/sections[?filter,orderby,select,top,skip,expand,count]` 

<br/>

<span data-ttu-id="c4f00-161">Получение всех разделов, вложенных непосредственно в определенную записную книжку.</span><span class="sxs-lookup"><span data-stu-id="c4f00-161">Get all sections that are directly under a specific notebook.</span></span>

`../notebooks/{notebook-id}/sections[?filter,orderby,select,top,skip,expand,count]` 

<br/>

<span data-ttu-id="c4f00-162">Запросы разделов могут разворачивать свойства **parentNotebook** и **parentSectionGroup**.</span><span class="sxs-lookup"><span data-stu-id="c4f00-162">Sections can expand the **parentNotebook** and **parentSectionGroup** properties.</span></span>

<span data-ttu-id="c4f00-163">По умолчанию для разделов используется порядок сортировки `name asc`.</span><span class="sxs-lookup"><span data-stu-id="c4f00-163">The default sort order for sections is `name asc`.</span></span>

<span data-ttu-id="c4f00-164">Запрос по умолчанию разворачивает родительскую записную книжку и родительскую группу разделов и выбирает их свойства `id`, `name` и `self`.</span><span class="sxs-lookup"><span data-stu-id="c4f00-164">The default query expands the parent notebook and parent section group and selects their `id`, `name`, and `self` properties.</span></span>



<a name="get-section"></a>

### <a name="section-entity"></a><span data-ttu-id="c4f00-165">Объект Section</span><span class="sxs-lookup"><span data-stu-id="c4f00-165">Section entity</span></span>

<span data-ttu-id="c4f00-166">Получение определенного раздела.</span><span class="sxs-lookup"><span data-stu-id="c4f00-166">Get a specific section.</span></span>

`../sections/{section-id}[?select,expand]` 

<br/>

<span data-ttu-id="c4f00-167">Запросы разделов могут разворачивать свойства **parentNotebook** и **parentSectionGroup**.</span><span class="sxs-lookup"><span data-stu-id="c4f00-167">Sections can expand the **parentNotebook** and **parentSectionGroup** properties.</span></span>

<span data-ttu-id="c4f00-168">Запрос по умолчанию разворачивает родительскую записную книжку и родительскую группу разделов и выбирает их свойства `id`, `name` и `self`.</span><span class="sxs-lookup"><span data-stu-id="c4f00-168">The default query expands the parent notebook and parent section group and selects their `id`, `name`, and `self` properties.</span></span>



<a name="get-section-groups"></a>

### <a name="sectiongroup-collection"></a><span data-ttu-id="c4f00-169">Коллекция SectionGroup</span><span class="sxs-lookup"><span data-stu-id="c4f00-169">SectionGroup collection</span></span>

<span data-ttu-id="c4f00-170">Получение всех групп разделов из всех записных книжек, принадлежащих пользователю, включая вложенные.</span><span class="sxs-lookup"><span data-stu-id="c4f00-170">Get all section groups from all notebooks that are owned by the user, including nested section groups.</span></span>

`../sectionGroups[?filter,orderby,select,top,skip,expand,count]` 

<br/>

<span data-ttu-id="c4f00-171">Получение всех групп разделов, вложенных непосредственно в определенную записную книжку.</span><span class="sxs-lookup"><span data-stu-id="c4f00-171">Get all section groups that are directly under a specific notebook.</span></span> 

`../notebooks/{notebook-id}/sectionGroups[?filter,orderby,select,top,skip,expand,count]` 

<br/>

<span data-ttu-id="c4f00-172">Запросы групп разделов могут разворачивать свойства **sections**, **sectionGroups**, **parentNotebook** и **parentSectionGroup**.</span><span class="sxs-lookup"><span data-stu-id="c4f00-172">Section groups can expand the **sections**, **sectionGroups**, **parentNotebook**, and **parentSectionGroup** properties.</span></span>

<span data-ttu-id="c4f00-173">По умолчанию для групп разделов используется порядок сортировки `name asc`.</span><span class="sxs-lookup"><span data-stu-id="c4f00-173">The default sort order for section groups is `name asc`.</span></span>

<span data-ttu-id="c4f00-174">Запрос по умолчанию разворачивает родительскую записную книжку и родительскую группу разделов и выбирает их свойства `id`, `name` и `self`.</span><span class="sxs-lookup"><span data-stu-id="c4f00-174">The default query expands the parent notebook and parent section group and selects their `id`, `name`, and `self` properties.</span></span>



<a name="get-section-group"></a>

### <a name="sectiongroup-entity"></a><span data-ttu-id="c4f00-175">Объект SectionGroup</span><span class="sxs-lookup"><span data-stu-id="c4f00-175">SectionGroup entity</span></span>

<span data-ttu-id="c4f00-176">Получение определенной группы разделов.</span><span class="sxs-lookup"><span data-stu-id="c4f00-176">Get a specific section group.</span></span>

`../sectionGroups/{sectiongroup-id}[?select,expand]` 

<br/>

<span data-ttu-id="c4f00-177">Запросы групп разделов могут разворачивать свойства **sections**, **sectionGroups**, **parentNotebook** и **parentSectionGroup**.</span><span class="sxs-lookup"><span data-stu-id="c4f00-177">Section groups can expand the **sections**, **sectionGroups**, **parentNotebook**, and **parentSectionGroup** properties.</span></span>

<span data-ttu-id="c4f00-178">Запрос по умолчанию разворачивает родительскую записную книжку и родительскую группу разделов и выбирает их свойства `id`, `name` и `self`.</span><span class="sxs-lookup"><span data-stu-id="c4f00-178">The default query expands the parent notebook and parent section group and selects their `id`, `name`, and `self` properties.</span></span>



<a name="get-notebooks"></a>

### <a name="notebook-collection"></a><span data-ttu-id="c4f00-179">Коллекция Notebook</span><span class="sxs-lookup"><span data-stu-id="c4f00-179">Notebook collection</span></span>

<span data-ttu-id="c4f00-180">Получение всех записных книжек, принадлежащих пользователю.</span><span class="sxs-lookup"><span data-stu-id="c4f00-180">Get all the notebooks that are owned by the user.</span></span> 

`../notebooks[?filter,orderby,select,top,skip,expand,count]` 

<br/>

<span data-ttu-id="c4f00-181">Запросы записных книжек могут разворачивать свойства **sections** и **sectionGroups**.</span><span class="sxs-lookup"><span data-stu-id="c4f00-181">Notebooks can expand the **sections** and **sectionGroups** properties.</span></span>

<span data-ttu-id="c4f00-182">По умолчанию для записных книжек используется порядок сортировки `name asc`.</span><span class="sxs-lookup"><span data-stu-id="c4f00-182">The default sort order for notebooks is `name asc`.</span></span> 



<a name="get-notebook"></a>

### <a name="notebook-entity"></a><span data-ttu-id="c4f00-183">Объект Notebook</span><span class="sxs-lookup"><span data-stu-id="c4f00-183">Notebook entity</span></span>

<span data-ttu-id="c4f00-184">Получение определенной записной книжки.</span><span class="sxs-lookup"><span data-stu-id="c4f00-184">Get a specific notebook.</span></span>

`../notebooks/{notebook-id}[?select,expand]` 

<br/>

<span data-ttu-id="c4f00-185">Запросы записных книжек могут разворачивать свойства **sections** и **sectionGroups**.</span><span class="sxs-lookup"><span data-stu-id="c4f00-185">Notebooks can expand the **sections** and **sectionGroups** properties.</span></span>



<a name="get-resource"></a>

### <a name="image-or-other-file-resource"></a><span data-ttu-id="c4f00-186">Ресурс изображений или других файлов</span><span class="sxs-lookup"><span data-stu-id="c4f00-186">Image or other file resource</span></span>

<span data-ttu-id="c4f00-187">Получение двоичных данных определенного ресурса.</span><span class="sxs-lookup"><span data-stu-id="c4f00-187">Get the binary data of a specific resource.</span></span> 

`../resources/{resource-id}/$value` 

<br/>

<span data-ttu-id="c4f00-188">URI ресурса файла можно найти в [выходном HTML-коде](onenote-input-output-html.md) страницы.</span><span class="sxs-lookup"><span data-stu-id="c4f00-188">You can find the file's resource URI in the page's [output HTML](onenote-input-output-html.md).</span></span>

<span data-ttu-id="c4f00-189">Например, тег **img** содержит конечные точки для исходного изображения в атрибуте **data-fullres-src** и оптимизированное изображение в атрибуте **src**.</span><span class="sxs-lookup"><span data-stu-id="c4f00-189">For example, an **img** tag includes endpoints for the original image in the **data-fullres-src** attribute and the optimized image in the **src** attribute.</span></span> 

#### <a name="example"></a><span data-ttu-id="c4f00-190">Пример</span><span class="sxs-lookup"><span data-stu-id="c4f00-190">Example</span></span>

```html
<img 
    src="https://www.onenote.com/api/v1.0/me/notes/resources/{image-id}/$value"  
    data-src-type="image/png"
    data-fullres-src="https://www.onenote.com/api/v1.0/resources/{image-id}/$value"  
    data-fullres-src-type="image/png" ... />
```

<span data-ttu-id="c4f00-191">Тег **object** содержит конечную точку файлового ресурса в атрибуте **data**.</span><span class="sxs-lookup"><span data-stu-id="c4f00-191">And an **object** tag includes the endpoint for the file resource in the **data** attribute.</span></span> 

#### <a name="example"></a><span data-ttu-id="c4f00-192">Пример</span><span class="sxs-lookup"><span data-stu-id="c4f00-192">Example</span></span>

```html
<object
    data="https://www.onenote.com/api/v1.0/me/notes/resources/{file-id}/$value"
    data-attachment="fileName.pdf" 
    type="application/pdf" ... />
```

> <span data-ttu-id="c4f00-193">**Примечание.** Получение коллекции ресурсов не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4f00-193">**Note:** Getting a collection of resources is not supported.</span></span> 

<span data-ttu-id="c4f00-194">При получении файлового ресурса не требуется включать в запрос тип контента **Accept**.</span><span class="sxs-lookup"><span data-stu-id="c4f00-194">When you get a file resource, you don't need to include an **Accept** content type in the request.</span></span>

<span data-ttu-id="c4f00-195">Дополнительные сведения о запросах GET см. в следующих статьях документации по API REST Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="c4f00-195">For more information about GET requests, see the following resources in the Microsoft Graph API REST reference:</span></span>

- [<span data-ttu-id="c4f00-196">Запрос GET для страниц</span><span class="sxs-lookup"><span data-stu-id="c4f00-196">GET Pages</span></span>](/graph/api/page-get?view=graph-rest-1.0)
- [<span data-ttu-id="c4f00-197">GET Sections</span><span class="sxs-lookup"><span data-stu-id="c4f00-197">GET Sections</span></span>](/graph/api/section-get?view=graph-rest-1.0)
- [<span data-ttu-id="c4f00-198">GET SectionGroups</span><span class="sxs-lookup"><span data-stu-id="c4f00-198">GET SectionGroups</span></span>](/graph/api/sectiongroup-get?view=graph-rest-1.0)
- [<span data-ttu-id="c4f00-199">Запрос GET для записных книжек</span><span class="sxs-lookup"><span data-stu-id="c4f00-199">GET Notebooks</span></span>](/graph/api/notebook-get?view=graph-rest-1.0) 




<a name="example"></a>

## <a name="example-get-requests"></a><span data-ttu-id="c4f00-200">Примеры запросов GET</span><span class="sxs-lookup"><span data-stu-id="c4f00-200">Example GET requests</span></span>

<span data-ttu-id="c4f00-201">Вы можете запрашивать объекты OneNote и содержимое страницы поиска, чтобы получать только нужные вам сведения.</span><span class="sxs-lookup"><span data-stu-id="c4f00-201">You can query for OneNote entities and search page content to get just the information you need.</span></span> <span data-ttu-id="c4f00-202">Ниже показаны некоторые способы использования [поддерживаемых параметров строки](#supported-odata-query-string-options) в запросах GET к Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c4f00-202">The following examples show some ways you can use [supported query string options](#supported-odata-query-string-options) in GET requests to Microsoft Graph.</span></span> 

<span data-ttu-id="c4f00-203">**Помните:**</span><span class="sxs-lookup"><span data-stu-id="c4f00-203">**Remember:**</span></span>

- <span data-ttu-id="c4f00-204">Все запросы GET начинаются с [корневого URL-адреса службы](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0#root-url).</span><span class="sxs-lookup"><span data-stu-id="c4f00-204">All GET requests start with the [service root URL](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0#root-url).</span></span> <br/><br/><span data-ttu-id="c4f00-205">**Примеры**: `https://www.onenote.com/api/v1.0/me/notes` и `https://www.onenote.com/api/v1.0/myOrganization/siteCollections/{id}/sites/{id}/notes/`.</span><span class="sxs-lookup"><span data-stu-id="c4f00-205">**Examples**: `https://www.onenote.com/api/v1.0/me/notes` and `https://www.onenote.com/api/v1.0/myOrganization/siteCollections/{id}/sites/{id}/notes/`</span></span>

- <span data-ttu-id="c4f00-206">Пробелы в строке запроса URL следует кодировать как %20.</span><span class="sxs-lookup"><span data-stu-id="c4f00-206">Spaces in the URL query string must use %20 encoding.</span></span><br/><br/><span data-ttu-id="c4f00-207">**Пример**: `filter=title%20eq%20'biology'`.</span><span class="sxs-lookup"><span data-stu-id="c4f00-207">**Example**: `filter=title%20eq%20'biology'`</span></span>

- <span data-ttu-id="c4f00-208">В случае имен свойств и сравнения строк OData учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="c4f00-208">Property names and OData string comparisons are case-sensitive.</span></span> <span data-ttu-id="c4f00-209">Рекомендуем использовать функцию OData **tolower** для сравнения строк.</span><span class="sxs-lookup"><span data-stu-id="c4f00-209">We recommend using the OData **tolower** function for string comparisons.</span></span><br/><br/><span data-ttu-id="c4f00-210">**Пример**: `filter=tolower(name) eq 'spring'`.</span><span class="sxs-lookup"><span data-stu-id="c4f00-210">**Example**: `filter=tolower(name) eq 'spring'`</span></span>
 

### <a name="search--filter"></a><span data-ttu-id="c4f00-211">search и filter</span><span class="sxs-lookup"><span data-stu-id="c4f00-211">search & filter</span></span>  

<span data-ttu-id="c4f00-212">Получение всех страниц с термином *recipe*, созданных определенным приложением (`search` доступен только для пользовательских записных книжек).</span><span class="sxs-lookup"><span data-stu-id="c4f00-212">Get all pages that contain the term *recipe* that were created by a specific app (`search` is available for consumer notebooks only).</span></span>

```
[GET] ../pages?search=recipe&filter=createdByAppId eq 'WLID-000000004C12821A'
```
 
### <a name="search--select"></a><span data-ttu-id="c4f00-213">search и select</span><span class="sxs-lookup"><span data-stu-id="c4f00-213">search & select</span></span>  

<span data-ttu-id="c4f00-214">Получение заголовка, клиентских ссылок OneNote и ссылки **contentUrl** для всех страниц, содержащих термин *golgi app* (`search` доступен только для пользовательских записных книжек).</span><span class="sxs-lookup"><span data-stu-id="c4f00-214">Get the title, OneNote client links, and **contentUrl** link for all pages that contain the term *golgi app* (`search` is available for consumer notebooks only).</span></span>

```
[GET] ../pages?search=golgi app&select=title,links,contentUrl
```
 
### <a name="expand"></a><span data-ttu-id="c4f00-215">expand</span><span class="sxs-lookup"><span data-stu-id="c4f00-215">expand</span></span> 

<span data-ttu-id="c4f00-216">Получение всех записных книжек, а также разворачивание их разделов и групп разделов.</span><span class="sxs-lookup"><span data-stu-id="c4f00-216">Get all notebooks and expand their sections and section groups.</span></span>  

```
[GET] ../notebooks?expand=sections,sectionGroups
```

<br/>

<span data-ttu-id="c4f00-217">Получение определенной группы разделов и разворачивание ее разделов и групп разделов.</span><span class="sxs-lookup"><span data-stu-id="c4f00-217">Get a specific section group and expand its sections and section groups.</span></span>  

```
[GET] ../sectionGroups/{sectiongroup-id}?expand=sections,sectionGroups
```

<br/>

<span data-ttu-id="c4f00-218">Получение страницы и разворачивание ее родительского раздела и родительской записной книжки.</span><span class="sxs-lookup"><span data-stu-id="c4f00-218">Get a page and expand its parent section and parent notebook.</span></span>

```
[GET] ../pages/{page-id}?expand=parentSection,parentNotebook
```

### <a name="expand-multiple-levels"></a><span data-ttu-id="c4f00-219">expand (несколько уровней)</span><span class="sxs-lookup"><span data-stu-id="c4f00-219">expand (multiple levels)</span></span>  

<span data-ttu-id="c4f00-220">Получение всех записных книжек и разворачивание их разделов и групп разделов, а также разворачивание всех разделов в каждой группе разделов.</span><span class="sxs-lookup"><span data-stu-id="c4f00-220">Get all notebooks and expand their sections and section groups, and expand all sections in each section group.</span></span>  

```
[GET] ../notebooks?expand=sections,sectionGroups(expand=sections)
```
 
> <span data-ttu-id="c4f00-221">**Примечание.** Разворачивание родительских элементов объектов или разворачивание дочерних элементов объектов создает циклическую ссылку и не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4f00-221">**Note:** Expanding parents of child entities or expanding children of parent entities creates a circular reference and is not supported.</span></span>

 
### <a name="expand--select-multiple-levels"></a><span data-ttu-id="c4f00-222">expand и select (несколько уровней)</span><span class="sxs-lookup"><span data-stu-id="c4f00-222">expand & select (multiple levels)</span></span>  

<span data-ttu-id="c4f00-223">Получение имени и ссылки **self** для определенной группы разделов, а также получение имени и ссылок **self** для всех ее разделов.</span><span class="sxs-lookup"><span data-stu-id="c4f00-223">Get the name and **self** link for a specific section group, and get the name and **self** links for all its sections.</span></span>  

```
[GET] ../sectionGroups/{sectiongroup-id}?expand=sections(select=name,self)&select=name,self
```

<br/>

<span data-ttu-id="c4f00-224">Получение имени и ссылки **self** для всех разделов, а также получение имени и времени создания родительской записной книжки каждого раздела.</span><span class="sxs-lookup"><span data-stu-id="c4f00-224">Get the name and **self** link for all sections, and get the name and created time of each section's parent notebook.</span></span>  

```
[GET] ../sections?expand=parentNotebook(select=name,createdTime)&select=name,self
```

<br/>
 
<span data-ttu-id="c4f00-225">Получение названий и идентификаторов всех страниц, а также получение названия родительского раздела и родительской записной книжки.</span><span class="sxs-lookup"><span data-stu-id="c4f00-225">Get the title and ID for all pages, and get the name of the parent section and parent notebook.</span></span>

```
[GET] ../pages?select=id,title&expand=parentSection(select=name),parentNotebook(select=name)
```

### <a name="expand--levels-multiple-levels"></a><span data-ttu-id="c4f00-226">expand и levels (несколько уровней)</span><span class="sxs-lookup"><span data-stu-id="c4f00-226">expand & levels (multiple levels)</span></span>  

<span data-ttu-id="c4f00-227">Получение всех записных книжек, разделов и групп разделов.</span><span class="sxs-lookup"><span data-stu-id="c4f00-227">Get all notebooks, sections, and section groups.</span></span>  

```
[GET] ../notebooks?expand=sections,sectionGroups(expand=sections,sectionGroups(levels=max;expand=sections))
```
 
### <a name="filter"></a><span data-ttu-id="c4f00-228">filter</span><span class="sxs-lookup"><span data-stu-id="c4f00-228">filter</span></span>

<span data-ttu-id="c4f00-229">Получение всех разделов, созданных в октябре 2014 г.</span><span class="sxs-lookup"><span data-stu-id="c4f00-229">Get all sections that were created in October 2014.</span></span>

```
[GET] ../sections?filter=createdTime ge 2014-10-01 and createdTime le 2014-10-31
```

<br/>

<span data-ttu-id="c4f00-230">Получение страниц, созданных определенным приложением с 1 января 2015 г.</span><span class="sxs-lookup"><span data-stu-id="c4f00-230">Get the pages that were created by a specific app since January 1, 2015.</span></span>

```
[GET] ../pages?filter=createdByAppId eq 'WLID-0000000048118631' and createdTime ge 2015-01-01
```

### <a name="filter--expand"></a><span data-ttu-id="c4f00-231">filter и expand</span><span class="sxs-lookup"><span data-stu-id="c4f00-231">filter & expand</span></span>  

<span data-ttu-id="c4f00-232">Получение всех страниц определенной записной книжки.</span><span class="sxs-lookup"><span data-stu-id="c4f00-232">Get all pages in a specific notebook.</span></span> <span data-ttu-id="c4f00-233">По умолчанию API возвращает 20 записей.</span><span class="sxs-lookup"><span data-stu-id="c4f00-233">The API returns 20 entries by default.</span></span>

```
[GET] ../pages?filter=parentNotebook/id eq '{notebook-id}'&expand=parentNotebook
```

<br/>

<span data-ttu-id="c4f00-234">Получение имени и ссылки **pagesUrl** для всех разделов в записной книжке *School*.</span><span class="sxs-lookup"><span data-stu-id="c4f00-234">Get the name and **pagesUrl** link for all sections from the *School* notebook.</span></span> <span data-ttu-id="c4f00-235">При сравнении строк OData учитывается регистр, поэтому рекомендуем использовать функцию **tolower**.</span><span class="sxs-lookup"><span data-stu-id="c4f00-235">OData string comparisons are case-sensitive, so use the **tolower** function as a best practice.</span></span>

```
[GET] ../notebooks?filter=tolower(name) eq 'school'&expand=sections(select=name,pagesUrl)
```

### <a name="filter--select--orderby"></a><span data-ttu-id="c4f00-236">filter, select и orderby</span><span class="sxs-lookup"><span data-stu-id="c4f00-236">filter & select & orderby</span></span>   

<span data-ttu-id="c4f00-237">Получение имени и ссылки **pagesUrl** для всех разделов, имена которых содержат термин *spring*.</span><span class="sxs-lookup"><span data-stu-id="c4f00-237">Get the name and **pagesUrl** link for all sections that contain the term *spring* in the section name.</span></span> <span data-ttu-id="c4f00-238">Упорядочивание разделов по дате последнего изменения.</span><span class="sxs-lookup"><span data-stu-id="c4f00-238">Order sections by last modified date.</span></span>

```
[GET] ../sections?filter=contains(tolower(name),'spring')&select=name,pagesUrl&orderby=lastModifiedTime desc
```
 
### <a name="orderby"></a><span data-ttu-id="c4f00-239">orderby</span><span class="sxs-lookup"><span data-stu-id="c4f00-239">orderby</span></span>

<span data-ttu-id="c4f00-240">Получение первых 20 страниц, отсортированных по свойству **createdByAppId** и времени создания (по убыванию).</span><span class="sxs-lookup"><span data-stu-id="c4f00-240">Get the first 20 pages ordered by **createdByAppId** property and then by most recent created time.</span></span> <span data-ttu-id="c4f00-241">По умолчанию API возвращает 20 записей.</span><span class="sxs-lookup"><span data-stu-id="c4f00-241">The API returns 20 entries by default.</span></span>

```
[GET] ../pages?orderby=createdByAppId,createdTime desc
```

### <a name="search--filter--top"></a><span data-ttu-id="c4f00-242">search, filter и top</span><span class="sxs-lookup"><span data-stu-id="c4f00-242">search & filter & top</span></span> 

<span data-ttu-id="c4f00-243">Получение пяти последних страниц, созданных с 1 января 2015 г. и содержащих фразу *cell division*.</span><span class="sxs-lookup"><span data-stu-id="c4f00-243">Get the five newest pages created since January 1, 2015 that contain the phrase *cell division*.</span></span> <span data-ttu-id="c4f00-244">По умолчанию API возвращает 20 записей. Максимальное количество записей — 100.</span><span class="sxs-lookup"><span data-stu-id="c4f00-244">The API returns 20 entries by default with a maximum of 100.</span></span> <span data-ttu-id="c4f00-245">Порядок сортировки по умолчанию для страниц: `lastModifiedTime desc` (`search` доступен только для пользовательских записных книжек).</span><span class="sxs-lookup"><span data-stu-id="c4f00-245">The default sort order for pages is `lastModifiedTime desc` (`search` is available for consumer notebooks only).</span></span>

```
[GET] ../pages?search="cell division"&filter=createdTime ge 2015-01-01&top=5
```

### <a name="search--filter--top--skip"></a><span data-ttu-id="c4f00-246">search, filter, top и skip</span><span class="sxs-lookup"><span data-stu-id="c4f00-246">search & filter & top & skip</span></span>  

<span data-ttu-id="c4f00-247">Получение пяти следующих страниц в результирующем наборе (`search` доступен только для пользовательских записных книжек).</span><span class="sxs-lookup"><span data-stu-id="c4f00-247">Get the next five pages in the result set (`search` is available for consumer notebooks only).</span></span>

```
[GET] ../pages?search=biology&filter=createdTime ge 2015-01-01&top=5&skip=5
```

<br/>

<span data-ttu-id="c4f00-248">Получение еще пяти (`search` доступен только для пользовательских записных книжек).</span><span class="sxs-lookup"><span data-stu-id="c4f00-248">And the next five (`search` is available for consumer notebooks only).</span></span>

```
[GET] ../pages?search=biology&filter=createdTime ge 2015-01-01&top=5&skip=10
```

> <span data-ttu-id="c4f00-249">**Примечание.** Если параметры **search** и **filter** применяются к одному запросу, результаты включают только те объекты, которые соответствуют обоим условиям.</span><span class="sxs-lookup"><span data-stu-id="c4f00-249">**Note:** If both **search** and **filter** are applied to the same request, the results include only those entities that match both criteria.</span></span>
 
### <a name="select"></a><span data-ttu-id="c4f00-250">select</span><span class="sxs-lookup"><span data-stu-id="c4f00-250">select</span></span>

<span data-ttu-id="c4f00-251">Получение имени, времени создания и ссылки **self** для всех разделов в записных книжках пользователя.</span><span class="sxs-lookup"><span data-stu-id="c4f00-251">Get the name, created time, and **self** link for all sections in the user's notebooks.</span></span>

```
[GET] ../sections?select=name,createdTime,self
```

<br/>

<span data-ttu-id="c4f00-252">Получение названия, времени создания и клиентских ссылок OneNote для определенной страницы.</span><span class="sxs-lookup"><span data-stu-id="c4f00-252">Get the title, created time, and OneNote client links for a specific page.</span></span>

```
[GET] ../pages/{page-id}?select=title,createdTime,links
```

### <a name="select--expand--filter-multiple-levels"></a><span data-ttu-id="c4f00-253">select, expand и filter (несколько уровней)</span><span class="sxs-lookup"><span data-stu-id="c4f00-253">select & expand & filter (multiple levels)</span></span>  

<span data-ttu-id="c4f00-254">Получение имени и ссылки **pagesUrl** для всех разделов в записной книжке по умолчанию пользователя.</span><span class="sxs-lookup"><span data-stu-id="c4f00-254">Get the name and **pagesUrl** link for all sections in the user's default notebook.</span></span>

```
[GET] ../notebooks?select=name&expand=sections(select=name,pagesUrl)&filter=isDefault eq true
```

### <a name="top--select--orderby"></a><span data-ttu-id="c4f00-255">top, select и orderby</span><span class="sxs-lookup"><span data-stu-id="c4f00-255">top & select & orderby</span></span> 

<span data-ttu-id="c4f00-256">Получение названия и ссылки **self** для первых 50 страниц, упорядоченных по названию в алфавитном порядке.</span><span class="sxs-lookup"><span data-stu-id="c4f00-256">Get the title and **self** link for the first 50 pages, ordered alphabetically by title.</span></span> <span data-ttu-id="c4f00-257">По умолчанию API возвращает 20 записей. Максимальное количество записей — 100.</span><span class="sxs-lookup"><span data-stu-id="c4f00-257">The API returns 20 entries by default with a maximum of 100.</span></span> <span data-ttu-id="c4f00-258">По умолчанию для страниц используется порядок сортировки `lastModifiedTime desc`.</span><span class="sxs-lookup"><span data-stu-id="c4f00-258">The default sort order for pages is `lastModifiedTime desc`.</span></span>

```
[GET] ../pages?top=50&select=title,self&orderby=title
```

### <a name="skip--top--select--orderby"></a><span data-ttu-id="c4f00-259">skip, top, select и orderby</span><span class="sxs-lookup"><span data-stu-id="c4f00-259">skip & top & select & orderby</span></span>  

<span data-ttu-id="c4f00-p115">Получение страниц с 51 по 100. По умолчанию API возвращает 20 записей, а максимальное количество составляет 100.</span><span class="sxs-lookup"><span data-stu-id="c4f00-p115">Get pages 51 to 100. The API returns 20 entries by default with a maximum of 100.</span></span>

```
[GET] ../pages?skip=50&top=50&select=title,self&orderby=title
```

> <span data-ttu-id="c4f00-262">**Примечание.** Запросы GET для страниц, которые восстанавливают количество записей по умолчанию (то есть в них не указывается выражение **top**), возвращают в ответе ссылку **\@odata.nextLink**, с помощью которой можно получить следующие 20 записей.</span><span class="sxs-lookup"><span data-stu-id="c4f00-262">**Note:** GET requests for pages that retrieve the default number of entries (that is, they don't specify a **top** expression) return an **\@odata.nextLink** link in the response that you can use to get the next 20 entries.</span></span>
 

<a name="supported-odata-query-string-options"></a>

## <a name="supported-odata-query-string-options"></a><span data-ttu-id="c4f00-263">Поддерживаемые параметры строки запроса OData</span><span class="sxs-lookup"><span data-stu-id="c4f00-263">Supported OData query string options</span></span>

<span data-ttu-id="c4f00-264">Вы можете настраивать запросы GET к Microsoft Graph, используя параметры строки запроса OData, и получать только нужную информацию.</span><span class="sxs-lookup"><span data-stu-id="c4f00-264">When sending GET requests to Microsoft Graph, you can use OData query string options to customize your query and get just the information you need.</span></span> <span data-ttu-id="c4f00-265">Они также могут повышать производительность, уменьшая количество вызовов службы и размер полезных данных ответа.</span><span class="sxs-lookup"><span data-stu-id="c4f00-265">They can also improve performance by reducing the number of calls to the service and the size of the response payload.</span></span>

> <span data-ttu-id="c4f00-266">**Примечание.** Для удобства чтения в примерах из этой статьи не используется код %20, которым нужно заменять пробелы в строке запроса URL: `filter=isDefault%20eq%20true`</span><span class="sxs-lookup"><span data-stu-id="c4f00-266">**Note:** For readability, the examples in this article don't use the %20 percent-encoding required for spaces in the URL query string: `filter=isDefault%20eq%20true`</span></span>
 
| <span data-ttu-id="c4f00-267">Параметр запроса</span><span class="sxs-lookup"><span data-stu-id="c4f00-267">Query option</span></span> | <span data-ttu-id="c4f00-268">Пример и описание</span><span class="sxs-lookup"><span data-stu-id="c4f00-268">Example and description</span></span> |  
|------|------|  
| <span data-ttu-id="c4f00-269">count</span><span class="sxs-lookup"><span data-stu-id="c4f00-269">count</span></span> | <p>`count=true`</p><p><span data-ttu-id="c4f00-p117">Количество объектов в коллекции. Значение возвращается в свойстве **\@odata.count** ответа.</span><span class="sxs-lookup"><span data-stu-id="c4f00-p117">The count of entities in the collection. The value is returned in the **\@odata.count** property in the response.</span></span></p> |  
| <span data-ttu-id="c4f00-272">expand</span><span class="sxs-lookup"><span data-stu-id="c4f00-272">expand</span></span> | <p>`expand=sections,sectionGroups`</p><p><span data-ttu-id="c4f00-273">Свойства навигации, которые следует вернуть в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c4f00-273">The navigation properties to return inline in the response.</span></span> <span data-ttu-id="c4f00-274">Для выражений **expand** поддерживаются следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="c4f00-274">The following properties are supported for **expand** expressions:</span></span><br /> <span data-ttu-id="c4f00-275">страницы: **parentNotebook**, **parentSection**;</span><span class="sxs-lookup"><span data-stu-id="c4f00-275">- Pages: **parentNotebook**, **parentSection**</span></span><br /> <span data-ttu-id="c4f00-276">разделы: **parentNotebook**, **parentSectionGroup**;</span><span class="sxs-lookup"><span data-stu-id="c4f00-276">- Sections: **parentNotebook**, **parentSectionGroup**</span></span><br /> <span data-ttu-id="c4f00-277">группы разделов: **sections**, **sectionGroups**, **parentNotebook**, **parentSectionGroup**;</span><span class="sxs-lookup"><span data-stu-id="c4f00-277">- Section groups: **sections**, **sectionGroups**, **parentNotebook**, **parentSectionGroup**</span></span><br /> <span data-ttu-id="c4f00-278">записные книжки: **sections**, **sectionGroups**.</span><span class="sxs-lookup"><span data-stu-id="c4f00-278">- Notebooks: **sections**, **sectionGroups**</span></span></p><p><span data-ttu-id="c4f00-p119">По умолчанию запросы GET для страниц разворачивают **parentSection** и выделяют свойства раздела **id**, **name** и **self**. По умолчанию запросы GET для разделов и групп разделов разворачивают как **parentNotebook**, так и **parentSectionGroup**, а также выделяют родительские свойства **id**, **name** и **self**.</span><span class="sxs-lookup"><span data-stu-id="c4f00-p119">By default, GET requests for pages expands **parentSection** and select the section's **id**, **name**, and **self** properties. Default GET requests for sections and section groups expand both **parentNotebook** and **parentSectionGroup**, and select the parents' **id**, **name**, and **self** properties. </span></span></p><p><span data-ttu-id="c4f00-281">Может использоваться для одного объекта или коллекции.</span><span class="sxs-lookup"><span data-stu-id="c4f00-281">Can be used for a single entity or a collection.</span></span><br /><span data-ttu-id="c4f00-282">Свойства следует разделять запятыми.</span><span class="sxs-lookup"><span data-stu-id="c4f00-282">Separate multiple properties with commas.</span></span><br /><span data-ttu-id="c4f00-283">В именах свойств учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="c4f00-283">Property names are case-sensitive.</span></span></p> |   
| <span data-ttu-id="c4f00-284">filter</span><span class="sxs-lookup"><span data-stu-id="c4f00-284">filter</span></span> | <p>`filter=isDefault eq true`</p><p><span data-ttu-id="c4f00-285">Логическое выражение, указывающее, следует ли включать запись в набор результатов.</span><span class="sxs-lookup"><span data-stu-id="c4f00-285">A Boolean expression for whether to include an entry in the result set.</span></span> <span data-ttu-id="c4f00-286">Поддерживаются следующие функции и операторы OData:</span><span class="sxs-lookup"><span data-stu-id="c4f00-286">Supports the following OData operators and functions:</span></span><br /> <span data-ttu-id="c4f00-287">— операторы сравнения: **eq**, **ne**, **gt**, **ge**, **lt**, **le**;</span><span class="sxs-lookup"><span data-stu-id="c4f00-287">- Comparison operators: **eq**, **ne**, **gt**, **ge**, **lt**, **le**</span></span><br /> <span data-ttu-id="c4f00-288">— логические операторы: **and**, **or**, **not**;</span><span class="sxs-lookup"><span data-stu-id="c4f00-288">- Logical operators: **and**, **or**, **not**</span></span><br /> <span data-ttu-id="c4f00-289">— строковые функции: **contains**, **endswith**, **startswith**, **length**, **indexof**, **substring**, **tolower**, **toupper**, **trim**, **concat**.</span><span class="sxs-lookup"><span data-stu-id="c4f00-289">- String functions: **contains**, **endswith**, **startswith**, **length**, **indexof**, **substring**, **tolower**, **toupper**, **trim**, **concat**</span></span></p><p><span data-ttu-id="c4f00-290">В случае имен [свойств](#onenote-entity-properties) и сравнения строк OData учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="c4f00-290">[Property](#onenote-entity-properties) names and OData string comparisons are case-sensitive.</span></span> <span data-ttu-id="c4f00-291">Рекомендуем использовать функцию OData **tolower** для сравнения строк.</span><span class="sxs-lookup"><span data-stu-id="c4f00-291">We recommend using the OData **tolower** function for string comparisons.</span></span><br /><br /><span data-ttu-id="c4f00-292">**Пример**: `filter=tolower(name) eq 'spring'`.</span><span class="sxs-lookup"><span data-stu-id="c4f00-292">**Example**: `filter=tolower(name) eq 'spring'`</span></span></p> |  
| <span data-ttu-id="c4f00-293">orderby</span><span class="sxs-lookup"><span data-stu-id="c4f00-293">orderby</span></span> | <p>`orderby=title,createdTime desc`</p><p><span data-ttu-id="c4f00-p122">
            [Свойства](#onenote-entity-properties) для сортировки с необязательным порядком сортировки \*\*asc\*\* (по умолчанию) или \*\*desc\*\*. Вы можете сортировать по любому свойству сущности в запрошенной коллекции.</span><span class="sxs-lookup"><span data-stu-id="c4f00-p122">The [properties](#onenote-entity-properties) to sort by, with an optional **asc** (default) or **desc** sort order. You can sort by any property of the entity in the requested collection.</span></span></p><p><span data-ttu-id="c4f00-296">По умолчанию для записных книжек, разделов и групп разделов используется порядок сортировки `name asc`, а для страниц — `lastModifiedTime desc` (сначала отображается последняя измененная страница).</span><span class="sxs-lookup"><span data-stu-id="c4f00-296">The default sort order for notebooks, section groups, and sections is `name asc`, and for pages is `lastModifiedTime desc` (last modified page first).</span></span></p><p><span data-ttu-id="c4f00-297">Разделяйте свойства запятыми и указывайте их в порядке применения.</span><span class="sxs-lookup"><span data-stu-id="c4f00-297">Separate multiple properties with commas, and list them in the order that you want them applied.</span></span> <span data-ttu-id="c4f00-298">В именах свойств учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="c4f00-298">Property names are case-sensitive.</span></span></p> |  
| <span data-ttu-id="c4f00-299">search</span><span class="sxs-lookup"><span data-stu-id="c4f00-299">search</span></span> | <p>`search=cell div`</p><p><span data-ttu-id="c4f00-300">Доступен только для пользовательских записных книжек.</span><span class="sxs-lookup"><span data-stu-id="c4f00-300">Available for consumer notebooks only.</span></span></p><p><span data-ttu-id="c4f00-p124">Термин или фраза, которую нужно найти в заголовке и тексте страницы, замещающем тексте изображений и распознанном тексте. По умолчанию поисковые запросы возвращают результаты, отсортированные по релевантности.</span><span class="sxs-lookup"><span data-stu-id="c4f00-p124">The term or phrase to search for in the page title, page body, image alt text, and image OCR text. By default, search queries return results sorted by relevance.</span></span></p><p><span data-ttu-id="c4f00-303">OneNote использует полнотекстовый поиск Bing для поддержки поиска фраз, выделения корней, игнорирования орфографических ошибок, релевантности и ранжирования, разбиения слов, разных языков и других функций полнотекстового поиска.</span><span class="sxs-lookup"><span data-stu-id="c4f00-303">OneNote uses Bing full-text search to support phrase search, stemming, spelling forgiveness, relevance and ranking, word breaking, multiple languages, and other full-text search features.</span></span> <span data-ttu-id="c4f00-304">В строках search учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="c4f00-304">Search strings are case-insensitive.</span></span></p><p><span data-ttu-id="c4f00-305">Применяется только к страницам записных книжек, принадлежащих пользователю.</span><span class="sxs-lookup"><span data-stu-id="c4f00-305">Applies only to pages in notebooks owned by the user.</span></span> <span data-ttu-id="c4f00-306">Индексированное содержимое является личным и доступно только владельцу.</span><span class="sxs-lookup"><span data-stu-id="c4f00-306">Indexed content is private and can only be accessed by the owner.</span></span> <span data-ttu-id="c4f00-307">Страницы, защищенные паролем, не индексируются.</span><span class="sxs-lookup"><span data-stu-id="c4f00-307">Password-protected pages are not indexed.</span></span> <span data-ttu-id="c4f00-308">Применяется только к конечной точке `pages`.</span><span class="sxs-lookup"><span data-stu-id="c4f00-308">Applies only to the `pages` endpoint.</span></span></p> |  
| <span data-ttu-id="c4f00-309">select</span><span class="sxs-lookup"><span data-stu-id="c4f00-309">select</span></span> | <p>`select=id,title`</p><p><span data-ttu-id="c4f00-310">Возвращаемые [свойства](#onenote-entity-properties).</span><span class="sxs-lookup"><span data-stu-id="c4f00-310">The [properties](#onenote-entity-properties) to return.</span></span> <span data-ttu-id="c4f00-311">Может использоваться для одного объекта или коллекции.</span><span class="sxs-lookup"><span data-stu-id="c4f00-311">Can be used for a single entity or for a collection.</span></span> <span data-ttu-id="c4f00-312">Свойства следует разделять запятыми.</span><span class="sxs-lookup"><span data-stu-id="c4f00-312">Separate multiple properties with commas.</span></span> <span data-ttu-id="c4f00-313">В именах свойств учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="c4f00-313">Property names are case-sensitive.</span></span></p> |  
| <span data-ttu-id="c4f00-314">skip</span><span class="sxs-lookup"><span data-stu-id="c4f00-314">skip</span></span> | <p>`skip=10`</p><p><span data-ttu-id="c4f00-315">Количество записей, которое следует пропустить в наборе результатов.</span><span class="sxs-lookup"><span data-stu-id="c4f00-315">The number of entries to skip in the result set.</span></span> <span data-ttu-id="c4f00-316">Обычно используется для разбиения результатов на страницы.</span><span class="sxs-lookup"><span data-stu-id="c4f00-316">Typically used for paging results.</span></span></p> |  
| <span data-ttu-id="c4f00-317">top</span><span class="sxs-lookup"><span data-stu-id="c4f00-317">top</span></span> | <p>`top=50`</p><p><span data-ttu-id="c4f00-318">Количество записей, которое следует вернуть в наборе результатов, до 100.</span><span class="sxs-lookup"><span data-stu-id="c4f00-318">The number of entries to return in the result set, up to a maximum of 100.</span></span> <span data-ttu-id="c4f00-319">Значение по умолчанию — 20.</span><span class="sxs-lookup"><span data-stu-id="c4f00-319">The default value is 20.</span></span></p> |  

<span data-ttu-id="c4f00-320">В Microsoft Graph также доступен параметр строки запроса `pagelevel`, с помощью которого можно получить уровень и порядок страниц в родительском разделе.</span><span class="sxs-lookup"><span data-stu-id="c4f00-320">Microsoft Graph also provides the `pagelevel` query string option you can use to get the level and order of pages within the parent section.</span></span> <span data-ttu-id="c4f00-321">Применяется только к запросам страниц в определенном разделе и запросам определенной страницы.</span><span class="sxs-lookup"><span data-stu-id="c4f00-321">Applies only to queries for pages in a specific section or queries for a specific page.</span></span> 

#### <a name="examples"></a><span data-ttu-id="c4f00-322">Примеры</span><span class="sxs-lookup"><span data-stu-id="c4f00-322">Examples</span></span> 

- `GET ../sections/{section-id}/pages?pagelevel=true` 
- `GET ../pages/{page-id}?pagelevel=true` 

### <a name="supported-odata-operators-and-functions"></a><span data-ttu-id="c4f00-323">Поддерживаемые операторы и функции OData</span><span class="sxs-lookup"><span data-stu-id="c4f00-323">Supported OData operators and functions</span></span>

<span data-ttu-id="c4f00-324">Microsoft Graph поддерживает указанные ниже функции и операторы OData в выражениях **filter**.</span><span class="sxs-lookup"><span data-stu-id="c4f00-324">Microsoft Graph supports the following OData operators and functions in **filter** expressions.</span></span> <span data-ttu-id="c4f00-325">Используя выражения OData, помните:</span><span class="sxs-lookup"><span data-stu-id="c4f00-325">When using OData expressions, remember:</span></span>

- <span data-ttu-id="c4f00-326">Пробелы в строке запроса URL необходимо заменять кодом `%20`.</span><span class="sxs-lookup"><span data-stu-id="c4f00-326">Spaces in the URL query string must be replaced with the `%20` encoding.</span></span><br/><br/><span data-ttu-id="c4f00-327">**Пример:** `filter=isDefault%20eq%20true`.</span><span class="sxs-lookup"><span data-stu-id="c4f00-327">**Example:** `filter=isDefault%20eq%20true`</span></span>

- <span data-ttu-id="c4f00-328">В случае имен свойств и сравнения строк OData учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="c4f00-328">Property names and OData string comparisons are case-sensitive.</span></span> <span data-ttu-id="c4f00-329">Рекомендуем использовать функцию OData **tolower** для сравнения строк.</span><span class="sxs-lookup"><span data-stu-id="c4f00-329">We recommend using the OData **tolower** function for string comparisons.</span></span><br/><br/><span data-ttu-id="c4f00-330">**Пример:** `filter=tolower(name) eq 'spring'`</span><span class="sxs-lookup"><span data-stu-id="c4f00-330">**Example:** `filter=tolower(name) eq 'spring'`</span></span>


| <span data-ttu-id="c4f00-331">Оператор сравнения</span><span class="sxs-lookup"><span data-stu-id="c4f00-331">Comparison operator</span></span> | <span data-ttu-id="c4f00-332">Пример</span><span class="sxs-lookup"><span data-stu-id="c4f00-332">Example</span></span> |  
|------|------|  
| <span data-ttu-id="c4f00-333">eq</span><span class="sxs-lookup"><span data-stu-id="c4f00-333">eq</span></span><br /><span data-ttu-id="c4f00-334">(равно)</span><span class="sxs-lookup"><span data-stu-id="c4f00-334">(equal to)</span></span> | `createdByAppId eq '{app-id}'` |  
| <span data-ttu-id="c4f00-335">ne</span><span class="sxs-lookup"><span data-stu-id="c4f00-335">ne</span></span><br /><span data-ttu-id="c4f00-336">(не равно)</span><span class="sxs-lookup"><span data-stu-id="c4f00-336">(not equal to)</span></span> | `userRole ne 'Owner'` |  
| <span data-ttu-id="c4f00-337">gt</span><span class="sxs-lookup"><span data-stu-id="c4f00-337">gt</span></span><br /><span data-ttu-id="c4f00-338">(больше)</span><span class="sxs-lookup"><span data-stu-id="c4f00-338">(greater than)</span></span> | `createdTime gt 2014-02-23` |  
| <span data-ttu-id="c4f00-339">ge</span><span class="sxs-lookup"><span data-stu-id="c4f00-339">ge</span></span><br /><span data-ttu-id="c4f00-340">(больше или равно)</span><span class="sxs-lookup"><span data-stu-id="c4f00-340">(greater than or equal to)</span></span> | `lastModifiedTime ge 2014-05-05T07:00:00Z` |  
| <span data-ttu-id="c4f00-341">lt</span><span class="sxs-lookup"><span data-stu-id="c4f00-341">lt</span></span><br /><span data-ttu-id="c4f00-342">(меньше)</span><span class="sxs-lookup"><span data-stu-id="c4f00-342">(less than)</span></span> | `createdTime lt 2014-02-23` |  
| <span data-ttu-id="c4f00-343">le</span><span class="sxs-lookup"><span data-stu-id="c4f00-343">le</span></span><br /><span data-ttu-id="c4f00-344">(меньше или равно)</span><span class="sxs-lookup"><span data-stu-id="c4f00-344">(less than or equal to)</span></span> | `lastModifiedTime le 2014-02-23` |  

<br/>

| <span data-ttu-id="c4f00-345">Логический оператор</span><span class="sxs-lookup"><span data-stu-id="c4f00-345">Logical operator</span></span> | <span data-ttu-id="c4f00-346">Пример</span><span class="sxs-lookup"><span data-stu-id="c4f00-346">Example</span></span> |  
|------|------|  
| <span data-ttu-id="c4f00-347">и</span><span class="sxs-lookup"><span data-stu-id="c4f00-347">and</span></span> | `createdTime le 2014-01-30 and createdTime gt 2014-01-23` |  
| <span data-ttu-id="c4f00-348">Кроме того:</span><span class="sxs-lookup"><span data-stu-id="c4f00-348">or</span></span> | `createdByAppId eq '{app-id}' or createdByAppId eq '{app-id}'` |  
| <span data-ttu-id="c4f00-349">
not</span><span class="sxs-lookup"><span data-stu-id="c4f00-349">not</span></span> | `not contains(tolower(title),'school')` |  

<br/>
  
| <span data-ttu-id="c4f00-350">Строкова функция</span><span class="sxs-lookup"><span data-stu-id="c4f00-350">String function</span></span> | <span data-ttu-id="c4f00-351">Пример</span><span class="sxs-lookup"><span data-stu-id="c4f00-351">Example</span></span> |  
|------|------|   
| <span data-ttu-id="c4f00-352">contains</span><span class="sxs-lookup"><span data-stu-id="c4f00-352">contains</span></span> | `contains(tolower(title),'spring')` |  
| <span data-ttu-id="c4f00-353">endswith</span><span class="sxs-lookup"><span data-stu-id="c4f00-353">endswith</span></span> | `endswith(tolower(title),'spring')` |  
| <span data-ttu-id="c4f00-354">startswith</span><span class="sxs-lookup"><span data-stu-id="c4f00-354">startswith</span></span> | `startswith(tolower(title),'spring')` |  
| <span data-ttu-id="c4f00-355">length</span><span class="sxs-lookup"><span data-stu-id="c4f00-355">length</span></span> | `length(title) eq 19` |  
| <span data-ttu-id="c4f00-356">indexof</span><span class="sxs-lookup"><span data-stu-id="c4f00-356">indexof</span></span> | `indexof(tolower(title),'spring') eq 1` |  
| <span data-ttu-id="c4f00-357">substring</span><span class="sxs-lookup"><span data-stu-id="c4f00-357">substring</span></span> | `substring(tolower(title),1) eq 'spring'` |  
| <span data-ttu-id="c4f00-358">tolower</span><span class="sxs-lookup"><span data-stu-id="c4f00-358">tolower</span></span> | `tolower(title) eq 'spring'` |  
| <span data-ttu-id="c4f00-359">toupper</span><span class="sxs-lookup"><span data-stu-id="c4f00-359">toupper</span></span> | `toupper(title) eq 'SPRING'` |  
| <span data-ttu-id="c4f00-360">trim</span><span class="sxs-lookup"><span data-stu-id="c4f00-360">trim</span></span> | `trim(tolower(title)) eq 'spring'` |  
| <span data-ttu-id="c4f00-361">concat</span><span class="sxs-lookup"><span data-stu-id="c4f00-361">concat</span></span> | `concat(title,'- by MyRecipesApp') eq 'Carrot Cake Recipe - by MyRecipesApp'` |  
 

<a name="properties"></a>

## <a name="onenote-entity-properties"></a><span data-ttu-id="c4f00-362">Свойства объектов OneNote</span><span class="sxs-lookup"><span data-stu-id="c4f00-362">OneNote entity properties</span></span>

<span data-ttu-id="c4f00-363">Выражения запроса **filter**, **select**, **expand** и **orderby** могут включать свойства объектов OneNote.</span><span class="sxs-lookup"><span data-stu-id="c4f00-363">The **filter**, **select**, **expand**, and **orderby** query expressions can include properties of OneNote entities.</span></span> 

#### <a name="example"></a><span data-ttu-id="c4f00-364">Пример</span><span class="sxs-lookup"><span data-stu-id="c4f00-364">Example</span></span>

`../sections?filter=createdTime ge 2015-01-01&select=name,pagesUrl&orderby=lastModifiedTime desc` 

<span data-ttu-id="c4f00-365">Для имен свойств в выражениях запроса учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="c4f00-365">Property names are case-sensitive in query expressions.</span></span>

<span data-ttu-id="c4f00-366">Список свойств и типы свойств см. в следующих статьях документации по API REST Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="c4f00-366">For the list of properties and property types, see the following resources in the Microsoft Graph API REST reference:</span></span>

- [<span data-ttu-id="c4f00-367">Запрос GET для страниц</span><span class="sxs-lookup"><span data-stu-id="c4f00-367">GET Pages</span></span>](/graph/api/page-get?view=graph-rest-1.0)
- [<span data-ttu-id="c4f00-368">GET Sections</span><span class="sxs-lookup"><span data-stu-id="c4f00-368">GET Sections</span></span>](/graph/api/section-get?view=graph-rest-1.0)
- [<span data-ttu-id="c4f00-369">GET SectionGroups</span><span class="sxs-lookup"><span data-stu-id="c4f00-369">GET SectionGroups</span></span>](/graph/api/sectiongroup-get?view=graph-rest-1.0)
- [<span data-ttu-id="c4f00-370">Запрос GET для записных книжек</span><span class="sxs-lookup"><span data-stu-id="c4f00-370">GET Notebooks</span></span>](/graph/api/notebook-get?view=graph-rest-1.0) 



<span data-ttu-id="c4f00-371">Параметр строки запроса **expand** можно использовать со следующими свойствами навигации:</span><span class="sxs-lookup"><span data-stu-id="c4f00-371">The **expand** query string option can be used with the following navigation properties:</span></span>

- <span data-ttu-id="c4f00-372">страницы: **parentNotebook**, **parentSection**;</span><span class="sxs-lookup"><span data-stu-id="c4f00-372">Pages: **parentNotebook**, **parentSection**</span></span>
- <span data-ttu-id="c4f00-373">разделы: **parentNotebook**, **parentSectionGroup**;</span><span class="sxs-lookup"><span data-stu-id="c4f00-373">Sections: **parentNotebook**, **parentSectionGroup**</span></span>
- <span data-ttu-id="c4f00-374">группы разделов: **sections**, **sectionGroups**, **parentNotebook**, **parentSectionGroup**;</span><span class="sxs-lookup"><span data-stu-id="c4f00-374">Section groups: **sections**, **sectionGroups**, **parentNotebook**, **parentSectionGroup**</span></span>
- <span data-ttu-id="c4f00-375">записные книжки: **sections**, **sectionGroups**.</span><span class="sxs-lookup"><span data-stu-id="c4f00-375">Notebooks: **sections**, **sectionGroups**</span></span>


<a name="request-response-info"></a>

## <a name="request-and-response-information-for-get-requests"></a><span data-ttu-id="c4f00-376">Информация о запросах *GET* и соответствующих ответах</span><span class="sxs-lookup"><span data-stu-id="c4f00-376">Request and response information for *GET* requests</span></span>

| <span data-ttu-id="c4f00-377">Данные запроса</span><span class="sxs-lookup"><span data-stu-id="c4f00-377">Request data</span></span> | <span data-ttu-id="c4f00-378">Описание</span><span class="sxs-lookup"><span data-stu-id="c4f00-378">Description</span></span> |  
|------|------|  
| <span data-ttu-id="c4f00-379">Протокол</span><span class="sxs-lookup"><span data-stu-id="c4f00-379">Protocol</span></span> | <span data-ttu-id="c4f00-380">Все запросы используют протокол SSL/TLS для HTTPS.</span><span class="sxs-lookup"><span data-stu-id="c4f00-380">All requests use the SSL/TLS HTTPS protocol.</span></span> |  
| <span data-ttu-id="c4f00-381">Заголовок Authorization</span><span class="sxs-lookup"><span data-stu-id="c4f00-381">Authorization header</span></span> | <p><span data-ttu-id="c4f00-382">`Bearer {token}`, где `{token}` — действительный маркер доступа OAuth 2.0 для зарегистрированного приложения.</span><span class="sxs-lookup"><span data-stu-id="c4f00-382">`Bearer {token}`, where `{token}` is a valid OAuth 2.0 access token for your registered app.</span></span></p><p><span data-ttu-id="c4f00-383">Если он отсутствует или является недействительным, запрос завершится ошибкой с кодом состояния 401.</span><span class="sxs-lookup"><span data-stu-id="c4f00-383">If missing or invalid, the request fails with a 401 status code.</span></span> <span data-ttu-id="c4f00-384">См. статью [Проверка подлинности и разрешения](permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c4f00-384">See [Authentication and permissions](permissions-reference.md).</span></span></p> |  
| <span data-ttu-id="c4f00-385">Заголовок Accept</span><span class="sxs-lookup"><span data-stu-id="c4f00-385">Accept header</span></span> | <p> <span data-ttu-id="c4f00-386">`application/json` — для объектов OneNote и их наборов.</span><span class="sxs-lookup"><span data-stu-id="c4f00-386">`application/json` for OneNote entities and entity sets</span></span></p><p> <span data-ttu-id="c4f00-387">`text/html` — для содержимого страницы.</span><span class="sxs-lookup"><span data-stu-id="c4f00-387">`text/html` for page content</span></span></p> | 

<br/>

| <span data-ttu-id="c4f00-388">Данные в отклике</span><span class="sxs-lookup"><span data-stu-id="c4f00-388">Response data</span></span> | <span data-ttu-id="c4f00-389">Описание</span><span class="sxs-lookup"><span data-stu-id="c4f00-389">Description</span></span> |  
|------|------|  
| <span data-ttu-id="c4f00-390">Код успешного завершения</span><span class="sxs-lookup"><span data-stu-id="c4f00-390">Success code</span></span> | <span data-ttu-id="c4f00-391">Код состояния HTTP 200</span><span class="sxs-lookup"><span data-stu-id="c4f00-391">A 200 HTTP status code.</span></span> |  
| <span data-ttu-id="c4f00-392">Текст ответа</span><span class="sxs-lookup"><span data-stu-id="c4f00-392">Response body</span></span> | <span data-ttu-id="c4f00-393">Представление объекта или набора объектов в формате JSON, HTML-код страницы или двоичные данные файлового ресурса.</span><span class="sxs-lookup"><span data-stu-id="c4f00-393">An OData representation of the entity or entity set in JSON format, the page HTML, or file resource binary data.</span></span>  |  
| <span data-ttu-id="c4f00-394">Ошибки</span><span class="sxs-lookup"><span data-stu-id="c4f00-394">Errors</span></span> | <span data-ttu-id="c4f00-395">Если запрос завершается сбоем, API возвращает [ошибки](onenote-error-codes.md) в объекте **\@api.diagnostics** в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c4f00-395">If the request fails, the API returns [errors](onenote-error-codes.md) in the **\@api.diagnostics** object in the response body.</span></span> |  
| <span data-ttu-id="c4f00-396">Заголовок X-CorrelationId</span><span class="sxs-lookup"><span data-stu-id="c4f00-396">X-CorrelationId header</span></span> | <span data-ttu-id="c4f00-397">GUID, уникальный идентификатор запроса.</span><span class="sxs-lookup"><span data-stu-id="c4f00-397">A GUID that uniquely identifies the request.</span></span> <span data-ttu-id="c4f00-398">Это значение можно использовать вместе со значением заголовка Date при устранении неполадок совместно со службой поддержки Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="c4f00-398">You can use this value along with the value of the Date header when working with Microsoft support to troubleshoot issues.</span></span> |  


<a name="root-url"></a>

### <a name="constructing-the-microsoft-graph-notes-service-root-url"></a><span data-ttu-id="c4f00-399">Составление корневого URL-адреса для службы заметок Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="c4f00-399">Constructing the Microsoft Graph notes service root URL</span></span>

<span data-ttu-id="c4f00-400">Для всех вызовов заметок Microsoft Graph используется следующий формат корневого URL-адреса:</span><span class="sxs-lookup"><span data-stu-id="c4f00-400">The Microsoft Graph notes root URL uses the following format for all calls to Microsoft Graph notes:</span></span>

`https://graph.microsoft.com/{version}/me/onenote/`  

<span data-ttu-id="c4f00-401">Сегмент `version` URL-адреса представляет нужную версию Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c4f00-401">The `version` segment in the URL represents the version of Microsoft Graph that you want to use.</span></span> <span data-ttu-id="c4f00-402">Используйте значение `v1.0` для стабильного кода в рабочей среде.</span><span class="sxs-lookup"><span data-stu-id="c4f00-402">Use `v1.0` for stable production code.</span></span> <span data-ttu-id="c4f00-403">Используйте значение `beta`, чтобы опробовать функцию, находящуюся на стадии разработки.</span><span class="sxs-lookup"><span data-stu-id="c4f00-403">Use `beta` to try out a feature that's in development.</span></span> <span data-ttu-id="c4f00-404">Функции бета-версии могут меняться, поэтому не следует использовать их в производственном коде.</span><span class="sxs-lookup"><span data-stu-id="c4f00-404">Features and functionality in beta may change, so you shouldn't use it in your production code.</span></span> 

<span data-ttu-id="c4f00-405">Используйте значение `me` для содержимого OneNote, доступного текущему пользователю (если он является владельцем или с ним поделились этим содержимым).</span><span class="sxs-lookup"><span data-stu-id="c4f00-405">Use `me` for OneNote content that the current user can access (owned and shared).</span></span> <span data-ttu-id="c4f00-406">Используйте значение `users/{id}` для содержимого OneNote, которым указанный (в URL-адресе) пользователь поделился с текущим пользователем.</span><span class="sxs-lookup"><span data-stu-id="c4f00-406">Use `users/{id}` for OneNote content that the specified user (in the URL) has shared with the current user.</span></span> <span data-ttu-id="c4f00-407">Используйте [Microsoft Graph](https://graph.microsoft.com/v1.0/users) для получения ИД пользователей.</span><span class="sxs-lookup"><span data-stu-id="c4f00-407">Use [Microsoft Graph](https://graph.microsoft.com/v1.0/users) to get user IDs.</span></span> 


<a name="permissions"></a>

## <a name="permissions-for-get-requests"></a><span data-ttu-id="c4f00-408">Разрешения для запросов GET</span><span class="sxs-lookup"><span data-stu-id="c4f00-408">Permissions for GET requests</span></span>

<span data-ttu-id="c4f00-409">Чтобы получить содержимое или структуру OneNote, необходимо запросить соответствующие разрешения.</span><span class="sxs-lookup"><span data-stu-id="c4f00-409">To get OneNote content or structure, you'll need to request appropriate permissions.</span></span> 

<span data-ttu-id="c4f00-410">Указанные ниже разрешения позволяют выполнять запросы GET к Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c4f00-410">The following scopes allow GET requests to Microsoft Graph.</span></span> <span data-ttu-id="c4f00-411">Выберите минимальный уровень разрешений, необходимый для работы вашего приложения.</span><span class="sxs-lookup"><span data-stu-id="c4f00-411">Choose the lowest level of permissions that your app needs to do its work.</span></span>

<span data-ttu-id="c4f00-412">Варианты:</span><span class="sxs-lookup"><span data-stu-id="c4f00-412">Choose from:</span></span>

- <span data-ttu-id="c4f00-413">Notes.read</span><span class="sxs-lookup"><span data-stu-id="c4f00-413">Notes.read</span></span>
- <span data-ttu-id="c4f00-414">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c4f00-414">Notes.ReadWrite</span></span>
- <span data-ttu-id="c4f00-415">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4f00-415">Notes.ReadWrite.All</span></span>

<span data-ttu-id="c4f00-416">Дополнительные сведения об областях разрешений и принципе их использования см. в [справочнике по разрешениям Microsoft Graph](permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c4f00-416">For more information about permission scopes and how they work, see [Microsoft Graph permissions reference](permissions-reference.md).</span></span>

<a name="see-also"></a>

## <a name="see-also"></a><span data-ttu-id="c4f00-417">См. также</span><span class="sxs-lookup"><span data-stu-id="c4f00-417">See also</span></span>

- [<span data-ttu-id="c4f00-418">Входной и выходной HTML-код для страниц OneNote</span><span class="sxs-lookup"><span data-stu-id="c4f00-418">Input and output HTML for OneNote pages</span></span>](onenote-input-output-html.md)
- [<span data-ttu-id="c4f00-419">Интеграция с OneNote</span><span class="sxs-lookup"><span data-stu-id="c4f00-419">Integrate with OneNote</span></span>](integrate-with-onenote.md)
- [<span data-ttu-id="c4f00-420">Блог разработчиков OneNote</span><span class="sxs-lookup"><span data-stu-id="c4f00-420">OneNote Developer Blog</span></span>](https://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="c4f00-421">Вопросы разработки OneNote на сайте «Вопросы и ответы Майкрософт»</span><span class="sxs-lookup"><span data-stu-id="c4f00-421">OneNote development questions on Microsoft Q&A</span></span>](https://docs.microsoft.com/ru-RU/answers/topics/microsoft-graph-notes.html)
- [<span data-ttu-id="c4f00-422">Репозитории GitHub OneNote</span><span class="sxs-lookup"><span data-stu-id="c4f00-422">OneNote GitHub repos</span></span>](https://go.microsoft.com/fwlink/?LinkID=390178)  
