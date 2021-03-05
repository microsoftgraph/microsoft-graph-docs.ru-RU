---
title: Обновление содержимого страниц OneNote
description: " Корпоративная записная книжка в Microsoft 365"
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 9a30197744cb3d03255ea3d215ff0774546ae023
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472337"
---
# <a name="update-onenote-page-content"></a><span data-ttu-id="a5e7c-103">Обновление содержимого страниц OneNote</span><span class="sxs-lookup"><span data-stu-id="a5e7c-103">Update OneNote page content</span></span>

<span data-ttu-id="a5e7c-104">**Область применения:** Пользовательские записные книжки в OneDrive | Корпоративные записные книжки в Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-104">**Applies to** Consumer notebooks on OneDrive | Enterprise notebooks on Microsoft 365</span></span>


<span data-ttu-id="a5e7c-105">Чтобы обновить содержимое страницы OneNote, необходимо отправить запрос PATCH в конечную точку *content* страницы:</span><span class="sxs-lookup"><span data-stu-id="a5e7c-105">To update the content of a OneNote page, you send a PATCH request to the page's *content* endpoint:</span></span>

`PATCH ../notes/pages/{id}/content`</p>

<span data-ttu-id="a5e7c-p101">Отправьте объект изменений JSON в тексте сообщения. Если запрос будет выполнен успешно, Microsoft Graph вернет код состояния HTTP 204.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-p101">Send a JSON change object in the message body. If the request is successful, Microsoft Graph returns a 204 HTTP status code.</span></span>


<a name="request-uri"></a>

## <a name="construct-the-request-uri"></a><span data-ttu-id="a5e7c-108">Создание URI запроса</span><span class="sxs-lookup"><span data-stu-id="a5e7c-108">Construct the request URI</span></span>

<span data-ttu-id="a5e7c-109">Чтобы создать URI запроса, начните с корневого URL-адреса службы:</span><span class="sxs-lookup"><span data-stu-id="a5e7c-109">To construct the request URI, start with the service root URL:</span></span>

`https://graph.microsoft.com/v1.0/me/onenote`

<br/>

<span data-ttu-id="a5e7c-110">Затем добавьте конечную точку *content* страницы:</span><span class="sxs-lookup"><span data-stu-id="a5e7c-110">Then append the page's *content* endpoint:</span></span>

- <span data-ttu-id="a5e7c-111">**Получение HTML-кода страницы и всех определенных значений *data-id***</span><span class="sxs-lookup"><span data-stu-id="a5e7c-111">**Get the page HTML and all defined *data-id* values**</span></span><br/><br/>`../pages/{id}/content`   

- <span data-ttu-id="a5e7c-112">**Получение HTML-кода страницы, всех определенных значений *data-id* и всех созданных значений *id***</span><span class="sxs-lookup"><span data-stu-id="a5e7c-112">**Get the page HTML, all defined *data-id* values, and all generated *id* values**</span></span><br/><br/>`../pages/{page-id}/content?includeIDs=true` 

<span data-ttu-id="a5e7c-113">Значения **data-id** и **id** используются в качестве идентификаторов **target** для элементов, которые требуется изменить.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-113">The **data-id** and **id** values are used as **target** identifiers for the elements you want to update.</span></span>

 
<span data-ttu-id="a5e7c-114">Полный URI запроса будет выглядеть так:</span><span class="sxs-lookup"><span data-stu-id="a5e7c-114">Your full request URI will look like this:</span></span><br/><br/>`https://graph.microsoft.com/v1.0/me/onenote/pages/{id}/content`


<span data-ttu-id="a5e7c-115">Узнайте больше о [корневом URL-адресе службы](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0#root-url).</span><span class="sxs-lookup"><span data-stu-id="a5e7c-115">Learn more about the [service root URL](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0#root-url).</span></span>


<a name="message-body"></a>

## <a name="construct-the-message-body"></a><span data-ttu-id="a5e7c-116">Составление текста сообщения</span><span class="sxs-lookup"><span data-stu-id="a5e7c-116">Construct the message body</span></span>

<span data-ttu-id="a5e7c-117">HTML-код страницы OneNote содержит текст, изображения и другое содержимое, структурированные с помощью таких элементов, как **div**, **img** и **ol**.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-117">The HTML of a OneNote page contains text, images, and other content organized into structures such as **div**, **img**, and **ol** elements.</span></span> <span data-ttu-id="a5e7c-118">Для обновления содержимого страницы OneNote необходимо добавлять и заменять элементы HTML на странице.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-118">To update OneNote page content, you add and replace HTML elements on the page.</span></span>

<span data-ttu-id="a5e7c-119">Изменения отправляются в тексте сообщения в виде массива объектов JSON.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-119">Your changes are sent in the message body as an array of JSON change objects.</span></span> <span data-ttu-id="a5e7c-120">В каждом объекте указываются целевой элемент, новое содержимое HTML и действия, которые нужно выполнить с содержимым.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-120">Each object specifies the target element, new HTML content, and what to do with the content.</span></span>

<span data-ttu-id="a5e7c-p104">Следующий массив определяет два изменения. Первое вставляет изображение над абзацем в качестве элемента того же уровня, а второе добавляет элемент в список в качестве последнего дочернего элемента.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-p104">The following array defines two changes. The first inserts an image above a paragraph as a sibling, and the second appends an item to a list as a last child.</span></span>

> [!NOTE]
> <span data-ttu-id="a5e7c-123">При обновлении изображения на странице OneNote нельзя использовать ссылки www.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-123">When updating an image on a OneNote page, you can't use www links.</span></span> <span data-ttu-id="a5e7c-124">Служба не будет пытаться скачивать случайные ресурсы.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-124">The service won't try to download random resources.</span></span> <span data-ttu-id="a5e7c-125">Вместо этого изображение должно быть частью запроса либо url-адресом изображений, либо имям части многопартийного запроса.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-125">Instead, the image must be part of the request, either by an image-data-url or a part-name of a multipart request.</span></span>

```json
[
   {
    'target':'#para-id',
    'action':'insert',
    'position':'before',
    'content':'<img src="image-data-url-or-part-name" alt="Image above the target paragraph" />'
  }, 
  {
    'target':'#list-id',
    'action':'append',
    'content':'<li>Item at the end of the list</li>'
  }
]
```

<span data-ttu-id="a5e7c-126">См. [другие примеры](#example-requests).</span><span class="sxs-lookup"><span data-stu-id="a5e7c-126">See [more examples](#example-requests).</span></span>


### <a name="attributes-for-json-change-objects"></a><span data-ttu-id="a5e7c-127">Атрибуты объектов JSON</span><span class="sxs-lookup"><span data-stu-id="a5e7c-127">Attributes for JSON change objects</span></span>

<span data-ttu-id="a5e7c-128">Для определения объектов JSON в запросах PATCH используются атрибуты **target**, **action**, **position** и **content**.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-128">Use the **target**, **action**, **position**, and **content** attributes to define JSON objects for PATCH requests.</span></span>

#### <a name="target"></a><span data-ttu-id="a5e7c-129">target</span><span class="sxs-lookup"><span data-stu-id="a5e7c-129">target</span></span>

<span data-ttu-id="a5e7c-p106">Обновляемый элемент. Значением должен быть один из следующих идентификаторов:</span><span class="sxs-lookup"><span data-stu-id="a5e7c-p106">The element to update. The value must be one of the following identifiers:</span></span>

| <span data-ttu-id="a5e7c-132">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="a5e7c-132">Identifier</span></span> | <span data-ttu-id="a5e7c-133">Описание</span><span class="sxs-lookup"><span data-stu-id="a5e7c-133">Description</span></span> |  
|------|------|  
| <span data-ttu-id="a5e7c-134">#{data-id}</span><span class="sxs-lookup"><span data-stu-id="a5e7c-134">#{data-id}</span></span> | <p><span data-ttu-id="a5e7c-135">Этот идентификатор при желании определяется для элементов входного HTML-кода при [создании](onenote-create-page.md) или [обновлении страницы](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="a5e7c-135">This ID is optionally defined on elements in the input HTML when [creating a page](onenote-create-page.md) or [updating a page](onenote-update-page.md).</span></span> <span data-ttu-id="a5e7c-136">Добавьте перед этим значением префикс #.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-136">Prefix the value with a #.</span></span></p><p> <span data-ttu-id="a5e7c-137">Пример:</span><span class="sxs-lookup"><span data-stu-id="a5e7c-137">Example:</span></span><br/><span data-ttu-id="a5e7c-138">`'target':'#intro'` задает в качестве целевого элемент `<div data-id="intro" ...>`</span><span class="sxs-lookup"><span data-stu-id="a5e7c-138">`'target':'#intro'` targets the element `<div data-id="intro" ...>`</span></span></p> |  
| <span data-ttu-id="a5e7c-139">id</span><span class="sxs-lookup"><span data-stu-id="a5e7c-139">id</span></span> | <p><span data-ttu-id="a5e7c-140">Это [сгенерированный идентификатор](#generated-ids) из Microsoft Graph, необходимый для большинства операций замены.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-140">This is the [generated ID](#generated-ids) from Microsoft Graph, and is required for most replace operations.</span></span> <span data-ttu-id="a5e7c-141">Не добавляйте перед ним префикс #.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-141">Do not prefix with a #.</span></span></p><p> <span data-ttu-id="a5e7c-142">Пример:</span><span class="sxs-lookup"><span data-stu-id="a5e7c-142">Example:</span></span><br/><span data-ttu-id="a5e7c-143">`'target':'div:{33f8a2...}{37}'` задает в качестве целевого элемент `<div id="div:{33f8a2...}{37}" ...>`</span><span class="sxs-lookup"><span data-stu-id="a5e7c-143">`'target':'div:{33f8a2...}{37}'` targets the element `<div id="div:{33f8a2...}{37}" ...>`</span></span></p><p><span data-ttu-id="a5e7c-144">Не путайте эти идентификаторы со значениями **id**, определенными во [входном HTML-коде](onenote-input-output-html.md).</span><span class="sxs-lookup"><span data-stu-id="a5e7c-144">Don't confuse these with any **id** values defined in the [input HTML](onenote-input-output-html.md).</span></span> <span data-ttu-id="a5e7c-145">Все значения **id**, отправляемые во входном HTML-коде, отклоняются.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-145">All **id** values sent in the input HTML are discarded.</span></span></p> |  
| <span data-ttu-id="a5e7c-146">body</span><span class="sxs-lookup"><span data-stu-id="a5e7c-146">body</span></span> | <span data-ttu-id="a5e7c-147">Ключевое слово, указывающее на первый разделитель на странице.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-147">The keyword that targets the first div on the page.</span></span> <span data-ttu-id="a5e7c-148">Не добавляйте перед ним префикс #.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-148">Do not prefix with a #.</span></span> |  
| <span data-ttu-id="a5e7c-149">title</span><span class="sxs-lookup"><span data-stu-id="a5e7c-149">title</span></span> | <span data-ttu-id="a5e7c-150">Ключевое слово, указывающее на заголовок страницы.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-150">The keyword that targets the page title.</span></span> <span data-ttu-id="a5e7c-151">Не добавляйте перед ним префикс #.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-151">Do not prefix with a #.</span></span> |  
 
#### <a name="action"></a><span data-ttu-id="a5e7c-152">action</span><span class="sxs-lookup"><span data-stu-id="a5e7c-152">action</span></span>

<span data-ttu-id="a5e7c-p112">Действие, которое нужно выполнить с целевым элементом. См. [поддерживаемые действия для элементов](#supported-elements-and-actions).</span><span class="sxs-lookup"><span data-stu-id="a5e7c-p112">The action to perform on the target element. See [supported actions for elements](#supported-elements-and-actions).</span></span>

| <span data-ttu-id="a5e7c-155">Действие</span><span class="sxs-lookup"><span data-stu-id="a5e7c-155">Action</span></span> | <span data-ttu-id="a5e7c-156">Описание</span><span class="sxs-lookup"><span data-stu-id="a5e7c-156">Description</span></span> |  
|------|------|  
| <span data-ttu-id="a5e7c-157">append</span><span class="sxs-lookup"><span data-stu-id="a5e7c-157">append</span></span> | <p><span data-ttu-id="a5e7c-158">Добавляет указанное содержимое к целевому элементу в качестве первого или последнего дочернего элемента, в зависимости от значения атрибута **position**.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-158">Adds the supplied content to the target as a first or last child, as determined by the **position** attribute.</span></span></p><p><span data-ttu-id="a5e7c-159">Применяется только к элементам **body**, **div**, **ol** и **ul**.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-159">Applies only to **body**, **div**, **ol**, and **ul** elements.</span></span></p> |  
| <span data-ttu-id="a5e7c-160">insert</span><span class="sxs-lookup"><span data-stu-id="a5e7c-160">insert</span></span> | <span data-ttu-id="a5e7c-161">Добавляет указанное содержимое в качестве элемента того же уровня перед целевым элементом или после него, в зависимости от значения атрибута **position**.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-161">Adds the supplied content as a sibling before or after the target, as determined by the **position** attribute.</span></span> |  
| <span data-ttu-id="a5e7c-162">prepend</span><span class="sxs-lookup"><span data-stu-id="a5e7c-162">prepend</span></span> | <p><span data-ttu-id="a5e7c-163">Добавляет указанное содержимое к целевому элементу в качестве первого дочернего элемента.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-163">Adds the supplied content to the target as a first child.</span></span> <span data-ttu-id="a5e7c-164">Сокращение от действия **append** + **before**.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-164">Shortcut for **append** + **before**.</span></span></p><p><span data-ttu-id="a5e7c-165">Применяется только к элементам **body**, **div**, **ol** и **ul**.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-165">Applies only to **body**, **div**, **ol**, and **ul** elements.</span></span></p> |  
| <span data-ttu-id="a5e7c-166">replace</span><span class="sxs-lookup"><span data-stu-id="a5e7c-166">replace</span></span> | <p><span data-ttu-id="a5e7c-167">Заменяет целевой элемент указанным содержимым.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-167">Replaces the target with the supplied content.</span></span></p><p><span data-ttu-id="a5e7c-168">Для большинства действий **replace** необходимо использовать [сгенерированный идентификатор](#generated-ids) целевого элемента (кроме элементов **img** и **object** внутри разделителя, которые также поддерживают использование **data-id**).</span><span class="sxs-lookup"><span data-stu-id="a5e7c-168">Most **replace** actions require using the [generated ID](#generated-ids) for the target (except **img** and **object** elements within a div, which also support using **data-id**).</span></span></p> |  
 
#### <a name="position"></a><span data-ttu-id="a5e7c-169">position</span><span class="sxs-lookup"><span data-stu-id="a5e7c-169">position</span></span>

<span data-ttu-id="a5e7c-p114">Место для добавления предоставленного контента относительно целевого элемента. Если атрибут опущен, по умолчанию он принимает значение **after**.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-p114">The location to add the supplied content, relative to the target element. Defaults to **after** if omitted.</span></span>

| <span data-ttu-id="a5e7c-172">Position</span><span class="sxs-lookup"><span data-stu-id="a5e7c-172">Position</span></span> | <span data-ttu-id="a5e7c-173">Описание</span><span class="sxs-lookup"><span data-stu-id="a5e7c-173">Description</span></span> |  
|------|------|  
| <span data-ttu-id="a5e7c-174">after (по умолчанию)</span><span class="sxs-lookup"><span data-stu-id="a5e7c-174">after (default)</span></span> |<p><span data-ttu-id="a5e7c-175">С действием **append**: последний дочерний элемент целевого элемента.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-175">With **append**: The last child of the target element.</span></span></p><p><span data-ttu-id="a5e7c-176">С действием **insert**: следующий элемент того же уровня, что и целевой элемент.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-176">With **insert**: The subsequent sibling of the target element.</span></span></p> |
| <span data-ttu-id="a5e7c-177">before</span><span class="sxs-lookup"><span data-stu-id="a5e7c-177">before</span></span> | <p><span data-ttu-id="a5e7c-178">С действием **append**: первый дочерний элемент целевого элемента.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-178">With **append**: The first child of the target element.</span></span></p><p><span data-ttu-id="a5e7c-179">С действием **insert**: предыдущий элемент того же уровня, что и целевой элемент.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-179">With **insert**: The preceding sibling of the target element.</span></span></p> |

#### <a name="content"></a><span data-ttu-id="a5e7c-180">content</span><span class="sxs-lookup"><span data-stu-id="a5e7c-180">content</span></span>

<span data-ttu-id="a5e7c-181">Строка правильно оформленного HTML-кода, который нужно добавить на страницу, а также двоичные данные изображения или файла.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-181">A string of well-formed HTML to add to the page, and any image or file binary data.</span></span> <span data-ttu-id="a5e7c-182">Если в содержимом есть двоичные данные, необходимо отправить запрос с использованием типа контента `multipart/form-data` с частью Commands (см. [пример](#multipart-request-with-binary-content)).</span><span class="sxs-lookup"><span data-stu-id="a5e7c-182">If the content contains binary data, the request must be sent using the `multipart/form-data` content type with a "Commands" part (see an [example](#multipart-request-with-binary-content)).</span></span> 
 

<a name="generated-ids"></a>

### <a name="generated-ids"></a><span data-ttu-id="a5e7c-183">Сгенерированные идентификаторы</span><span class="sxs-lookup"><span data-stu-id="a5e7c-183">Generated IDs</span></span>
<span data-ttu-id="a5e7c-184">Microsoft Graph создает значения **id** для тех элементов на странице, которые можно обновить.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-184">Microsoft Graph generates **id** values for the elements on the page that can be updated.</span></span> <span data-ttu-id="a5e7c-185">Чтобы получить сгенерированные идентификаторы, используйте выражение строки `includeIDs=true` в запросе GET:</span><span class="sxs-lookup"><span data-stu-id="a5e7c-185">To get generated IDs, use the `includeIDs=true` query string expression in your GET request:</span></span>

`GET ../notes/pages/{page-id}/content?includeIDs=true` 

> <span data-ttu-id="a5e7c-186">**Примечание.** API отклоняет все значения **id**, определенные во [входном HTML-коде](onenote-input-output-html.md) запросов create-page и update-page.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-186">**Note:** The API discards all **id** values that are defined in the [input HTML](onenote-input-output-html.md) of create-page and update-page requests.</span></span>

<span data-ttu-id="a5e7c-187">Ниже показаны сгенерированные идентификаторы для абзаца и изображения в [выходном HTML-коде](onenote-input-output-html.md) страницы.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-187">The following example shows generated IDs for a paragraph and an image in the [output HTML](onenote-input-output-html.md) of a page.</span></span>

```html
<p id="p:{33f8a242-7c33-4bb2-90c5-8425a68cc5bf}{40}">Some text on the page</p>
<img id="img:{33f8a242-7c33-4bb2-90c5-8425a68cc5bf}{45}" ... />
```

<span data-ttu-id="a5e7c-188">Сгенерированные значения **id** могут изменяться после обновления страницы, поэтому вам следует получить текущие значения до создания использующего их PATCH-запроса.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-188">Generated **id** values might change after a page update, so you should get the current values before building a PATCH request that uses them.</span></span>
 
<span data-ttu-id="a5e7c-189">Вы можете указать целевые элементы, используя значение **data-id** или **id**, как указано ниже.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-189">You can specify target elements by using the **data-id** or **id** value, as follows:</span></span>

- <span data-ttu-id="a5e7c-190">Для действий **append** и **insert** в качестве целевого значения можно использовать любой идентификатор.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-190">For **append** and **insert** actions, you can use either ID as the target value.</span></span>
- <span data-ttu-id="a5e7c-191">Для действий **replace** необходимо использовать сгенерированный идентификатор для всех элементов, кроме заголовка, а также изображений и объектов, находящихся внутри разделителя.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-191">For **replace** actions, you must use the generated ID for all elements except for the page title and images and objects that are within a div.</span></span> 
  - <span data-ttu-id="a5e7c-192">Чтобы заменить заголовок, используйте ключевое слово **title**.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-192">To replace a title, use the **title** keyword.</span></span> 
  - <span data-ttu-id="a5e7c-193">Чтобы заменить изображения и объекты, находящиеся внутри разделителя, используйте атрибут **data-id** или **id**.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-193">To replace images and objects that are within a div, use either **data-id** or **id**.</span></span>

<span data-ttu-id="a5e7c-194">В приведенном ниже примере используется значение **id** целевого элемента.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-194">The following example uses the **id** value for the target.</span></span> <span data-ttu-id="a5e7c-195">Не используйте префикс # со сгенерированным идентификатором.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-195">Don't use the # prefix with a generated ID.</span></span>

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

## <a name="supported-elements-and-actions"></a><span data-ttu-id="a5e7c-196">Поддерживаемые элементы и действия</span><span class="sxs-lookup"><span data-stu-id="a5e7c-196">Supported elements and actions</span></span>

<span data-ttu-id="a5e7c-197">Многие элементы на странице можно обновлять, но каждый тип элемента поддерживает определенные действия.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-197">Many elements on the page can be updated, but each element type supports specific actions.</span></span> <span data-ttu-id="a5e7c-198">Ниже показаны поддерживаемые целевые элементы и поддерживаемые ими действия по обновлению.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-198">The following table shows supported target elements and the update actions that they support.</span></span>

| <span data-ttu-id="a5e7c-199">Элемент</span><span class="sxs-lookup"><span data-stu-id="a5e7c-199">Element</span></span> | <span data-ttu-id="a5e7c-200">Заменить</span><span class="sxs-lookup"><span data-stu-id="a5e7c-200">Replace</span></span> | <span data-ttu-id="a5e7c-201">Добавление дочернего элемента</span><span class="sxs-lookup"><span data-stu-id="a5e7c-201">Append child</span></span> | <span data-ttu-id="a5e7c-202">Вставка элемента того же уровня</span><span class="sxs-lookup"><span data-stu-id="a5e7c-202">Insert sibling</span></span> |  
|------|:------:|:------:|:------:|  
| <span data-ttu-id="a5e7c-203">body</span><span class="sxs-lookup"><span data-stu-id="a5e7c-203">body</span></span><br /> <span data-ttu-id="a5e7c-204">(делает целевым первый разделитель на странице)</span><span class="sxs-lookup"><span data-stu-id="a5e7c-204">(targets first div on the page)</span></span> | <span data-ttu-id="a5e7c-205">нет</span><span class="sxs-lookup"><span data-stu-id="a5e7c-205">no</span></span> | <span data-ttu-id="a5e7c-206">**да**</span><span class="sxs-lookup"><span data-stu-id="a5e7c-206">**yes**</span></span> | <span data-ttu-id="a5e7c-207">нет</span><span class="sxs-lookup"><span data-stu-id="a5e7c-207">no</span></span> |  
| <span data-ttu-id="a5e7c-208">div</span><span class="sxs-lookup"><span data-stu-id="a5e7c-208">div</span></span><br /> <span data-ttu-id="a5e7c-209">([абсолютное расположение](onenote-abs-pos.md))</span><span class="sxs-lookup"><span data-stu-id="a5e7c-209">([absolute positioned](onenote-abs-pos.md))</span></span> | <span data-ttu-id="a5e7c-210">нет</span><span class="sxs-lookup"><span data-stu-id="a5e7c-210">no</span></span> | <span data-ttu-id="a5e7c-211">**да**</span><span class="sxs-lookup"><span data-stu-id="a5e7c-211">**yes**</span></span> | <span data-ttu-id="a5e7c-212">нет</span><span class="sxs-lookup"><span data-stu-id="a5e7c-212">no</span></span> |  
| <span data-ttu-id="a5e7c-213">div</span><span class="sxs-lookup"><span data-stu-id="a5e7c-213">div</span></span><br /> <span data-ttu-id="a5e7c-214">(внутри разделителя)</span><span class="sxs-lookup"><span data-stu-id="a5e7c-214">(within a div)</span></span> | <span data-ttu-id="a5e7c-215">**да**</span><span class="sxs-lookup"><span data-stu-id="a5e7c-215">**yes**</span></span><br/><span data-ttu-id="a5e7c-216">(только идентификатор)</span><span class="sxs-lookup"><span data-stu-id="a5e7c-216">(id only)</span></span> | <span data-ttu-id="a5e7c-217">**да**</span><span class="sxs-lookup"><span data-stu-id="a5e7c-217">**yes**</span></span> | <span data-ttu-id="a5e7c-218">**да**</span><span class="sxs-lookup"><span data-stu-id="a5e7c-218">**yes**</span></span> |   
| <span data-ttu-id="a5e7c-219">img, object</span><span class="sxs-lookup"><span data-stu-id="a5e7c-219">img, object</span></span><br /> <span data-ttu-id="a5e7c-220">(внутри разделителя)</span><span class="sxs-lookup"><span data-stu-id="a5e7c-220">(within a div)</span></span> | <span data-ttu-id="a5e7c-221">**да**</span><span class="sxs-lookup"><span data-stu-id="a5e7c-221">**yes**</span></span> | <span data-ttu-id="a5e7c-222">нет</span><span class="sxs-lookup"><span data-stu-id="a5e7c-222">no</span></span> | <span data-ttu-id="a5e7c-223">**да**</span><span class="sxs-lookup"><span data-stu-id="a5e7c-223">**yes**</span></span> |   
| <span data-ttu-id="a5e7c-224">ol, ul</span><span class="sxs-lookup"><span data-stu-id="a5e7c-224">ol, ul</span></span> | <span data-ttu-id="a5e7c-225">**да**</span><span class="sxs-lookup"><span data-stu-id="a5e7c-225">**yes**</span></span><br/><span data-ttu-id="a5e7c-226">(только идентификатор)</span><span class="sxs-lookup"><span data-stu-id="a5e7c-226">(id only)</span></span> | <span data-ttu-id="a5e7c-227">**да**</span><span class="sxs-lookup"><span data-stu-id="a5e7c-227">**yes**</span></span> | <span data-ttu-id="a5e7c-228">**да**</span><span class="sxs-lookup"><span data-stu-id="a5e7c-228">**yes**</span></span> |   
| <span data-ttu-id="a5e7c-229">table</span><span class="sxs-lookup"><span data-stu-id="a5e7c-229">table</span></span> | <span data-ttu-id="a5e7c-230">**да**</span><span class="sxs-lookup"><span data-stu-id="a5e7c-230">**yes**</span></span><br/><span data-ttu-id="a5e7c-231">(только идентификатор)</span><span class="sxs-lookup"><span data-stu-id="a5e7c-231">(id only)</span></span> | <span data-ttu-id="a5e7c-232">нет</span><span class="sxs-lookup"><span data-stu-id="a5e7c-232">no</span></span> | <span data-ttu-id="a5e7c-233">**да**</span><span class="sxs-lookup"><span data-stu-id="a5e7c-233">**yes**</span></span> |   
| <span data-ttu-id="a5e7c-234">p, li, h1-h6</span><span class="sxs-lookup"><span data-stu-id="a5e7c-234">p, li, h1-h6</span></span> | <span data-ttu-id="a5e7c-235">**да**</span><span class="sxs-lookup"><span data-stu-id="a5e7c-235">**yes**</span></span><br/><span data-ttu-id="a5e7c-236">(только идентификатор)</span><span class="sxs-lookup"><span data-stu-id="a5e7c-236">(id only)</span></span> | <span data-ttu-id="a5e7c-237">нет</span><span class="sxs-lookup"><span data-stu-id="a5e7c-237">no</span></span> | <span data-ttu-id="a5e7c-238">**да**</span><span class="sxs-lookup"><span data-stu-id="a5e7c-238">**yes**</span></span> |   
| <span data-ttu-id="a5e7c-239">title</span><span class="sxs-lookup"><span data-stu-id="a5e7c-239">title</span></span> | <span data-ttu-id="a5e7c-240">**да**</span><span class="sxs-lookup"><span data-stu-id="a5e7c-240">**yes**</span></span> | <span data-ttu-id="a5e7c-241">нет</span><span class="sxs-lookup"><span data-stu-id="a5e7c-241">no</span></span> | <span data-ttu-id="a5e7c-242">нет</span><span class="sxs-lookup"><span data-stu-id="a5e7c-242">no</span></span> |  
 
<br/>

<span data-ttu-id="a5e7c-243">Указанные ниже элементы не поддерживают никаких действий обновления.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-243">The following elements do not support any update actions.</span></span>

- <span data-ttu-id="a5e7c-244">img ([абсолютное расположение](onenote-abs-pos.md))</span><span class="sxs-lookup"><span data-stu-id="a5e7c-244">img ([absolute positioned](onenote-abs-pos.md))</span></span>
- <span data-ttu-id="a5e7c-245">object ([абсолютное расположение](onenote-abs-pos.md))</span><span class="sxs-lookup"><span data-stu-id="a5e7c-245">object ([absolute positioned](onenote-abs-pos.md))</span></span>
- <span data-ttu-id="a5e7c-246">tr, td</span><span class="sxs-lookup"><span data-stu-id="a5e7c-246">tr, td</span></span>
- <span data-ttu-id="a5e7c-247">meta</span><span class="sxs-lookup"><span data-stu-id="a5e7c-247">meta</span></span>
- <span data-ttu-id="a5e7c-248">head</span><span class="sxs-lookup"><span data-stu-id="a5e7c-248">head</span></span>
- <span data-ttu-id="a5e7c-249">span</span><span class="sxs-lookup"><span data-stu-id="a5e7c-249">span</span></span>
- <span data-ttu-id="a5e7c-250">a</span><span class="sxs-lookup"><span data-stu-id="a5e7c-250">a</span></span>
- <span data-ttu-id="a5e7c-251">Теги style</span><span class="sxs-lookup"><span data-stu-id="a5e7c-251">style tags</span></span>


<a name="examples"></a>

## <a name="example-requests"></a><span data-ttu-id="a5e7c-252">Примеры запросов</span><span class="sxs-lookup"><span data-stu-id="a5e7c-252">Example requests</span></span>

<span data-ttu-id="a5e7c-253">Запрос на обновление содержит одно или несколько изменений, представленных в виде объектов JSON.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-253">An update request contains one or more changes represented as JSON change objects.</span></span> <span data-ttu-id="a5e7c-254">Эти объекты могут определять различные целевые элементы на странице, а также различные действия и содержимое для целевых элементов.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-254">These objects can define different targets on the page and different actions and content for the targets.</span></span>

<span data-ttu-id="a5e7c-255">Следующие примеры включают объекты JSON, используемые в запросах PATCH, а также готовые запросы PATCH:</span><span class="sxs-lookup"><span data-stu-id="a5e7c-255">The following examples include JSON objects used in PATCH requests and complete PATCH requests:</span></span>

- [<span data-ttu-id="a5e7c-256">Добавление дочерних элементов</span><span class="sxs-lookup"><span data-stu-id="a5e7c-256">Append child elements</span></span>](#append-child-elements)
- [<span data-ttu-id="a5e7c-257">Вставка элементов того же уровня</span><span class="sxs-lookup"><span data-stu-id="a5e7c-257">Insert sibling elements</span></span>](#insert-sibling-elements)
- [<span data-ttu-id="a5e7c-258">Замена элементов</span><span class="sxs-lookup"><span data-stu-id="a5e7c-258">Replace elements</span></span>](#replace-elements)
- [<span data-ttu-id="a5e7c-259">Выполнение запросов PATCH</span><span class="sxs-lookup"><span data-stu-id="a5e7c-259">Complete PATCH requests</span></span>](#complete-patch-request-examples)


<a name="append-examples"></a>

### <a name="append-child-elements"></a><span data-ttu-id="a5e7c-260">Добавление дочерних элементов</span><span class="sxs-lookup"><span data-stu-id="a5e7c-260">Append child elements</span></span>

<span data-ttu-id="a5e7c-p120">Действие **append** добавляет дочерний элемент в элемент **body**, **div** (в составе разделителя), **ol** или **ul**. Атрибут **position** определяет, следует ли добавить дочерний элемент перед целевым элементом или после него. Расположение по умолчанию — **after**.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-p120">The **append** action adds a child to a **body**, **div** (within a div), **ol**, or **ul** element. The **position** attribute determines whether to append the child before or after the target. The default position is **after**.</span></span>

#### <a name="append-to-a-div"></a><span data-ttu-id="a5e7c-264">Добавление в разделитель</span><span class="sxs-lookup"><span data-stu-id="a5e7c-264">Append to a div</span></span>

<span data-ttu-id="a5e7c-265">В приведенном ниже примере в элемент **div1** добавляется два дочерних узла.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-265">The following example adds two child nodes to the **div1** element.</span></span> <span data-ttu-id="a5e7c-266">Изображение добавляется в качестве первого дочернего элемента, а абзац — в качестве последнего.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-266">It adds an image as the first child and a paragraph as the last child.</span></span> 

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
 

#### <a name="append-to-the-body-element"></a><span data-ttu-id="a5e7c-267">Добавление к элементу *body*</span><span class="sxs-lookup"><span data-stu-id="a5e7c-267">Append to the *body* element</span></span>

<span data-ttu-id="a5e7c-268">Вы можете использовать сокращение **body** для добавления дочернего элемента внутри первого разделителя на любой странице.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-268">You can use the **body** shortcut to append a child element inside the first div on any page.</span></span>

<span data-ttu-id="a5e7c-269">В приведенном ниже примере в первый разделитель на странице добавляется два абзаца: один в качестве первого дочернего элемента, а другой — в качестве последнего.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-269">The following example adds two paragraphs as the first child and the last child to the first div on the page.</span></span> <span data-ttu-id="a5e7c-270">Не используйте префикс # с целевым элементом **body**.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-270">Don't use a # with the **body** target.</span></span> <span data-ttu-id="a5e7c-271">В этом примере действие **prepend** используется в качестве сокращения от действия **append** + **before**.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-271">This example uses the **prepend** action as a shortcut for **append** + **before**.</span></span>

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
 

#### <a name="append-to-a-list"></a><span data-ttu-id="a5e7c-272">Добавление в список</span><span class="sxs-lookup"><span data-stu-id="a5e7c-272">Append to a list</span></span>

<span data-ttu-id="a5e7c-p123">В следующем примере элемент списка добавляется в качестве последнего дочернего элемента к целевому списку. Свойство **list-style-type** определено, так как элемент использует стиль списка не по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-p123">The following example adds a list item as a last child to the target list. The **list-style-type** property is defined because the item uses a non-default list style.</span></span>

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

### <a name="insert-sibling-elements"></a><span data-ttu-id="a5e7c-275">Вставка элементов того же уровня</span><span class="sxs-lookup"><span data-stu-id="a5e7c-275">Insert sibling elements</span></span>

<span data-ttu-id="a5e7c-276">Действие **insert** добавляет элемент того же уровня в целевой элемент.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-276">The **insert** action adds a sibling to the target element.</span></span> <span data-ttu-id="a5e7c-277">Атрибут **position** определяет, где следует вставлять элемент: до или после целевого элемента.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-277">The **position** attribute determines whether to insert the sibling before or after the target.</span></span> <span data-ttu-id="a5e7c-278">По умолчанию задано положение **after**.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-278">The default position is **after**.</span></span> <span data-ttu-id="a5e7c-279">См. [элементы, поддерживающие действие **insert**](#supported-elements-and-actions).</span><span class="sxs-lookup"><span data-stu-id="a5e7c-279">See [elements that support **insert**](#supported-elements-and-actions).</span></span>

#### <a name="insert-siblings"></a><span data-ttu-id="a5e7c-280">Вставка элементов того же уровня</span><span class="sxs-lookup"><span data-stu-id="a5e7c-280">Insert siblings</span></span>

<span data-ttu-id="a5e7c-p125">В следующем примере два узла того же уровня добавляются на страницу. Над элементом **para1** добавляется изображение, а под элементом **para2** — абзац.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-p125">The following example adds two sibling nodes to the page. It adds an image above the **para1** element and a paragraph below the **para2** element.</span></span>

```json
[
  {
     'target':'#para1',
     'action':'insert',
     'position':'before',
     'content':'<img src="image-data-url-or-part-name" alt="Image inserted above the target" />'
  },
  {
    'target':'#para2',
     'action':'insert',
     'content':'<p data-id="next-sibling">Paragraph inserted below the target</p>'
  }
]
```
 

<a name="replace-examples"></a>

### <a name="replace-elements"></a><span data-ttu-id="a5e7c-283">Замена элементов</span><span class="sxs-lookup"><span data-stu-id="a5e7c-283">Replace elements</span></span>

<span data-ttu-id="a5e7c-284">Вы можете использовать **data-id** или сгенерированный **id** в качестве целевого значения для замены элементов **img** и **object** внутри разделителя.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-284">You can use either the **data-id** or generated **id** as the target value to replace **img** and **object** elements that are within a div.</span></span> <span data-ttu-id="a5e7c-285">Чтобы заменить заголовок, используйте ключевое слово **title**.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-285">To replace the page title, use the **title** keyword.</span></span> <span data-ttu-id="a5e7c-286">Для всех остальных [элементов, поддерживающих действие **replace**](#supported-elements-and-actions), необходимо использовать сгенерированный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-286">For all other [elements that support **replace**](#supported-elements-and-actions), you must use the generated ID.</span></span>

#### <a name="replace-an-image"></a><span data-ttu-id="a5e7c-287">Замена изображения</span><span class="sxs-lookup"><span data-stu-id="a5e7c-287">Replace an image</span></span>

<span data-ttu-id="a5e7c-288">В приведенном ниже примере изображение заменяется разделителем; в качестве целевого элемента используется **data-id** изображения.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-288">The following example replaces an image with a div by using the image's **data-id** as the target.</span></span> 

```json
[
  {
    'target':'#img1',
    'action':'replace',
    'content':'<div data-id="new-div"><p>This div replaces the image</p></div>'
  }
]
```
 

#### <a name="update-a-table"></a><span data-ttu-id="a5e7c-289">Обновление таблицы</span><span class="sxs-lookup"><span data-stu-id="a5e7c-289">Update a table</span></span> 

<span data-ttu-id="a5e7c-p127">Этот пример демонстрирует, как обновить таблицу при помощи ее сгенерированного ИД. Замена элементов **tr** и **td** не поддерживается, но вы можете заменить таблицу целиком.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-p127">This example shows how to update a table by using its generated ID. Replacing **tr** and **td** elements is not supported, but you can replace the entire table.</span></span>

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
 

#### <a name="change-the-title"></a><span data-ttu-id="a5e7c-292">Изменение заголовка</span><span class="sxs-lookup"><span data-stu-id="a5e7c-292">Change the title</span></span> 

<span data-ttu-id="a5e7c-293">В этом примере показано, как изменить заголовок страницы.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-293">This example shows how to change the title of a page.</span></span> <span data-ttu-id="a5e7c-294">Чтобы изменить заголовок, используйте ключевое слово **title** в качестве целевого значения.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-294">To change the title, use the **title** keyword as the target value.</span></span> <span data-ttu-id="a5e7c-295">Не используйте префикс # в целевом заголовке.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-295">Don't use a # with the title target.</span></span>

```json
[
  {
    'target':'title',
    'action':'replace',
    'content':'New title'
  }
]
```
 

#### <a name="update-a-to-do-item"></a><span data-ttu-id="a5e7c-296">Обновление элемента списка дел</span><span class="sxs-lookup"><span data-stu-id="a5e7c-296">Update a to-do item</span></span>

<span data-ttu-id="a5e7c-297">В приведенном ниже примере используется действие replace, чтобы перевести флажок в списке дел в состояние "Выполнено".</span><span class="sxs-lookup"><span data-stu-id="a5e7c-297">The following example uses the replace action to change a to-do check box item to a completed state.</span></span>

```json
[
  {
    'target':'#task1',
    'action':'replace',
    'content':'<p data-tag="to-do:completed" data-id="task1">First task</p>'
  }
]
```

<span data-ttu-id="a5e7c-298">Дополнительные сведения об использовании атрибута [data-tag](onenote-note-tags.md) см. в **этой статье**.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-298">See [Use note tags](onenote-note-tags.md) for more about using the **data-tag** attribute.</span></span>


<a name="complete-requests"></a>

### <a name="complete-patch-request-examples"></a><span data-ttu-id="a5e7c-299">Примеры выполнения запросов PATCH</span><span class="sxs-lookup"><span data-stu-id="a5e7c-299">Complete PATCH request examples</span></span>

<span data-ttu-id="a5e7c-300">В следующих примерах показаны готовые запросы PATCH.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-300">The following examples show complete PATCH requests.</span></span>

#### <a name="request-with-text-content-only"></a><span data-ttu-id="a5e7c-301">Запрос с текстовым содержимым</span><span class="sxs-lookup"><span data-stu-id="a5e7c-301">Request with text content only</span></span>

<span data-ttu-id="a5e7c-302">В приведенном ниже примере показан запрос PATCH, в котором используется тип контента **application/json**.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-302">The following example shows a PATCH request that uses the **application/json** content type.</span></span> <span data-ttu-id="a5e7c-303">Этот формат можно использовать, если контент не содержит двоичных данных.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-303">You can use this format when your content doesn't contain binary data.</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/me/onenote/notebooks/pages/{page-id}/content

Content-Type: application/json
Authorization: Bearer {token}

[
   {
    'target':'#para-id',
    'action':'insert',
    'position':'before',
    'content':'<img src="image-data-url" alt="New image from a URL" />'
  }, 
  {
    'target':'#list-id',
    'action':'append',
    'content':'<li>Item at the bottom of the list</li>'
  }
]
```
 
<a name="multipart"></a>

#### <a name="multipart-request-with-binary-content"></a><span data-ttu-id="a5e7c-304">Составной запрос с двоичным содержимым</span><span class="sxs-lookup"><span data-stu-id="a5e7c-304">Multipart request with binary content</span></span> 

<span data-ttu-id="a5e7c-305">В приведенном ниже примере показан составной запрос PATCH, включающий двоичные данные.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-305">The following example shows a multipart PATCH request that includes binary data.</span></span> <span data-ttu-id="a5e7c-306">Составные запросы включают часть Commands, в которой указывается тип контента **application/json** и предоставляется массив объектов изменений JSON.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-306">Multipart requests require a "Commands" part that specifies the **application/json** content type and contains the array of JSON change objects.</span></span> <span data-ttu-id="a5e7c-307">Другие части данных могут содержать двоичные данные.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-307">Other data parts can contain binary data.</span></span> <span data-ttu-id="a5e7c-308">Как правило, имена частей представляют собой строки, к которым добавлено текущее время в миллисекундах или случайный GUID.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-308">Part names typically are strings appended with the current time in milliseconds or a random GUID.</span></span>

```http
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

## <a name="request-and-response-information-for-patch-requests"></a><span data-ttu-id="a5e7c-309">Информация о запросах PATCH и соответствующих ответах</span><span class="sxs-lookup"><span data-stu-id="a5e7c-309">Request and response information for PATCH requests</span></span>

| <span data-ttu-id="a5e7c-310">Данные запроса</span><span class="sxs-lookup"><span data-stu-id="a5e7c-310">Request data</span></span> | <span data-ttu-id="a5e7c-311">Описание</span><span class="sxs-lookup"><span data-stu-id="a5e7c-311">Description</span></span> |  
|------|------|  
| <span data-ttu-id="a5e7c-312">Протокол</span><span class="sxs-lookup"><span data-stu-id="a5e7c-312">Protocol</span></span> | <span data-ttu-id="a5e7c-313">Все запросы используют протокол SSL/TLS для HTTPS.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-313">All requests use the SSL/TLS HTTPS protocol.</span></span> |  
| <span data-ttu-id="a5e7c-314">Заголовок Authorization</span><span class="sxs-lookup"><span data-stu-id="a5e7c-314">Authorization header</span></span> | <p><span data-ttu-id="a5e7c-315">`Bearer {token}`, где `{token}` — действительный маркер доступа OAuth 2.0 для зарегистрированного приложения.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-315">`Bearer {token}`, where `{token}` is a valid OAuth 2.0 access token for your registered app.</span></span></p><p><span data-ttu-id="a5e7c-316">Если он отсутствует или является недействительным, запрос завершится ошибкой с кодом состояния 401.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-316">If missing or invalid, the request fails with a 401 status code.</span></span> <span data-ttu-id="a5e7c-317">См. статью [Проверка подлинности и разрешения](permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a5e7c-317">See [Authentication and permissions](permissions-reference.md).</span></span></p> |  
| <span data-ttu-id="a5e7c-318">Заголовок Content-Type</span><span class="sxs-lookup"><span data-stu-id="a5e7c-318">Content-Type header</span></span> | <p><span data-ttu-id="a5e7c-319">`application/json` для массива объектов изменений JSON, отправленного либо непосредственно в тексте сообщения, либо в обязательной части Commands [составных запросов](#multipart-request-with-binary-content).</span><span class="sxs-lookup"><span data-stu-id="a5e7c-319">`application/json` for the array of JSON change objects, whether sent directly in the message body or in the required "Commands" part of [multipart requests](#multipart-request-with-binary-content).</span></span></p><p><span data-ttu-id="a5e7c-320">Составные запросы необходимы при отправке двоичных данных и используют тип контента `multipart/form-data; boundary=part-boundary`, где `{part-boundary}` — это строка, обозначающая начало и конец каждой части данных.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-320">Multipart requests are required when sending binary data, and use the `multipart/form-data; boundary=part-boundary` content type, where `{part-boundary}` is a string that signals the start and end of each data part.</span></span></p> |  

<br/> 

| <span data-ttu-id="a5e7c-321">Данные в отклике</span><span class="sxs-lookup"><span data-stu-id="a5e7c-321">Response data</span></span> | <span data-ttu-id="a5e7c-322">Описание</span><span class="sxs-lookup"><span data-stu-id="a5e7c-322">Description</span></span> |  
|------|------|  
| <span data-ttu-id="a5e7c-323">Код успешного завершения</span><span class="sxs-lookup"><span data-stu-id="a5e7c-323">Success code</span></span> | <span data-ttu-id="a5e7c-p132">Код состояния HTTP 204. Данные JSON не возвращаются по PATCH-запросу.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-p132">A 204 HTTP status code. No JSON data is returned for a PATCH request.</span></span> |  
| <span data-ttu-id="a5e7c-326">Ошибки</span><span class="sxs-lookup"><span data-stu-id="a5e7c-326">Errors</span></span> | <span data-ttu-id="a5e7c-327">Дополнительные сведения об ошибках OneNote, которые может возвращать Microsoft Graph, см. в статье [Коды ошибок для API OneNote в Microsoft Graph](onenote-error-codes.md).</span><span class="sxs-lookup"><span data-stu-id="a5e7c-327">Read [Error codes for OneNote APIs in Microsoft Graph](onenote-error-codes.md) to learn about OneNote errors that Microsoft Graph can return.</span></span> |  
 
 

<a name="root-url"></a>

### <a name="constructing-the-microsoft-graph-service-root-url"></a><span data-ttu-id="a5e7c-328">Составление корневого URL-адреса службы Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="a5e7c-328">Constructing the Microsoft Graph service root URL</span></span>

<span data-ttu-id="a5e7c-329">Для всех вызовов API OneNote используется следующий формат корневого URL-адреса службы OneNote:</span><span class="sxs-lookup"><span data-stu-id="a5e7c-329">The OneNote service root URL uses the following format for all calls to the OneNote API:</span></span>

`https://graph.microsoft.com/{version}/me/onenote/`

<span data-ttu-id="a5e7c-330">Сегмент `version` URL-адреса представляет нужную версию Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-330">The `version` segment in the URL represents the version of Microsoft Graph that you want to use.</span></span> <span data-ttu-id="a5e7c-331">Значение `v1.0` предназначено для стабильного производственного кода.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-331">`v1.0` is for stable production code.</span></span> <span data-ttu-id="a5e7c-332">Используйте значение `beta`, чтобы опробовать функцию, находящуюся на стадии разработки.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-332">`beta` is to try out a feature that's in development.</span></span> <span data-ttu-id="a5e7c-333">Функции бета-версии могут меняться, поэтому не следует использовать их в производственном коде.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-333">Features and functionality in beta may change, so you shouldn't use it in your production code.</span></span>

<span data-ttu-id="a5e7c-334">Значение `me` предназначено для содержимого OneNote, доступного текущему пользователю (если он является владельцем или с ним поделились этим содержимым).</span><span class="sxs-lookup"><span data-stu-id="a5e7c-334">`me` is for OneNote content that the current user can access (owned and shared).</span></span> <span data-ttu-id="a5e7c-335">Значение `users/{id}` предназначено для содержимого OneNote, которым указанный (в URL-адресе) пользователь поделился с текущим пользователем.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-335">`users/{id}` is for OneNote content that the specified user (in the URL) has shared with the current user.</span></span> <span data-ttu-id="a5e7c-336">Использование [API Graph для Azure AD](/previous-versions/azure/ad/graph/api/api-catalog)</span><span class="sxs-lookup"><span data-stu-id="a5e7c-336">Use the [Azure AD Graph API](/previous-versions/azure/ad/graph/api/api-catalog).</span></span>


> <span data-ttu-id="a5e7c-337">**Примечание.** Вы можете получить идентификаторы пользователей, отправив запрос GET к конечной точке `https://graph.microsoft.com/v1.0/users`.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-337">**Note:** You can get user ids by making a GET request on `https://graph.microsoft.com/v1.0/users`.</span></span>



<a name="permissions"></a>

## <a name="permissions"></a><span data-ttu-id="a5e7c-338">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a5e7c-338">Permissions</span></span>

<span data-ttu-id="a5e7c-339">Для обновления страниц OneNote необходимо запрашивать соответствующие разрешения.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-339">To update OneNote pages, you'll need to request appropriate permissions.</span></span> <span data-ttu-id="a5e7c-340">Выберите минимальный уровень разрешений, необходимый для работы вашего приложения.</span><span class="sxs-lookup"><span data-stu-id="a5e7c-340">Choose the lowest level of permissions that your app needs to do its work.</span></span>

- <span data-ttu-id="a5e7c-341">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a5e7c-341">Notes.ReadWrite</span></span>
- <span data-ttu-id="a5e7c-342">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5e7c-342">Notes.ReadWrite.All</span></span>

<span data-ttu-id="a5e7c-343">Дополнительные сведения об областях разрешений и принципе их работы см. в разделе [Области разрешений OneNote](permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a5e7c-343">For more information about permission scopes and how they work, see [OneNote permission scopes](permissions-reference.md).</span></span>
   

<a name="see-also"></a>

## <a name="see-also"></a><span data-ttu-id="a5e7c-344">См. также</span><span class="sxs-lookup"><span data-stu-id="a5e7c-344">See also</span></span>

- [<span data-ttu-id="a5e7c-345">Добавление изображений и файлов</span><span class="sxs-lookup"><span data-stu-id="a5e7c-345">Add images and files</span></span>](onenote-images-files.md)
- [<span data-ttu-id="a5e7c-346">Интеграция с OneNote</span><span class="sxs-lookup"><span data-stu-id="a5e7c-346">Integrate with OneNote</span></span>](integrate-with-onenote.md)
- [<span data-ttu-id="a5e7c-347">Блог разработчиков OneNote</span><span class="sxs-lookup"><span data-stu-id="a5e7c-347">OneNote Developer Blog</span></span>](https://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="a5e7c-348">Вопросы разработки OneNote для Microsoft Q&A</span><span class="sxs-lookup"><span data-stu-id="a5e7c-348">OneNote development questions on Microsoft Q&A</span></span>](https://docs.microsoft.com/answers/topics/microsoft-graph-notes.html)
- [<span data-ttu-id="a5e7c-349">Репозитории GitHub OneNote</span><span class="sxs-lookup"><span data-stu-id="a5e7c-349">OneNote GitHub repos</span></span>](https://go.microsoft.com/fwlink/?LinkID=390178)