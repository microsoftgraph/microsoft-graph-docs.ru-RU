---
title: Использование тегов заметок на страницах OneNote
description: " Корпоративные записные книжки в Microsoft 365"
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 6fe0d1603e2cd5b94e753b4e8d6b1a7e47b5aacf
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921919"
---
# <a name="use-note-tags-in-onenote-pages"></a><span data-ttu-id="5f05f-103">Использование тегов заметок на страницах OneNote</span><span class="sxs-lookup"><span data-stu-id="5f05f-103">Use note tags in OneNote pages</span></span>

<span data-ttu-id="5f05f-104">**Область применения:** Пользовательские записные книжки в OneDrive | Корпоративные записные книжки в Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="5f05f-104">**Applies to** Consumer notebooks on OneDrive | Enterprise notebooks on Microsoft 365</span></span>

<span data-ttu-id="5f05f-105">С помощью атрибута `data-tag` вы можете добавлять и изменять флажки, звездочки и другие встроенные теги заметок на странице OneNote, как показано на рисунке ниже.</span><span class="sxs-lookup"><span data-stu-id="5f05f-105">Use the `data-tag` attribute to add and update check boxes, stars, and other built-in note tags on a OneNote page, as shown in the following image.</span></span>

![Три тега заметок, отображаемые на странице OneNote.](images/note-tags-example.png)


<a name="attributes"></a>

## <a name="note-tag-attributes"></a><span data-ttu-id="5f05f-107">Атрибуты тегов заметок</span><span class="sxs-lookup"><span data-stu-id="5f05f-107">Note tag attributes</span></span>

<span data-ttu-id="5f05f-108">В HTML-коде страницы OneNote тег заметки представлен атрибутом `data-tag`.</span><span class="sxs-lookup"><span data-stu-id="5f05f-108">In the HTML of a OneNote page, a note tag is represented by the `data-tag` attribute.</span></span> <span data-ttu-id="5f05f-109">Пример:</span><span class="sxs-lookup"><span data-stu-id="5f05f-109">For example:</span></span>

- <span data-ttu-id="5f05f-110">Снятый флажок задачи: `<p data-tag="to-do">`</span><span class="sxs-lookup"><span data-stu-id="5f05f-110">An unchecked to-do box:  `<p data-tag="to-do">`</span></span>

- <span data-ttu-id="5f05f-111">Установленный флажок задачи: `<p data-tag="to-do:completed">`</span><span class="sxs-lookup"><span data-stu-id="5f05f-111">A checked to-do box:  `<p data-tag="to-do:completed">`</span></span>

- <span data-ttu-id="5f05f-112">Звездочка: `<h2 data-tag="important">`</span><span class="sxs-lookup"><span data-stu-id="5f05f-112">A star:  `<h2 data-tag="important">`</span></span>

<span data-ttu-id="5f05f-113">Значение `data-tag` состоит из фигуры и (иногда) из состояния (см. все [поддерживаемые значения](#built-in-note-tags-for-onenote)).</span><span class="sxs-lookup"><span data-stu-id="5f05f-113">A `data-tag` value is composed of a shape, and sometimes a status (see all [supported values](#built-in-note-tags-for-onenote)).</span></span>

| <span data-ttu-id="5f05f-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="5f05f-114">Property</span></span> | <span data-ttu-id="5f05f-115">Описание</span><span class="sxs-lookup"><span data-stu-id="5f05f-115">Description</span></span> |
|:------|:------|
| <span data-ttu-id="5f05f-116">shape</span><span class="sxs-lookup"><span data-stu-id="5f05f-116">shape</span></span> | <span data-ttu-id="5f05f-117">Идентификатор тега заметки (пример: `to-do` или `important`).</span><span class="sxs-lookup"><span data-stu-id="5f05f-117">The identifier of the note tag (example: `to-do` or `important`).</span></span> |
| <span data-ttu-id="5f05f-118">status</span><span class="sxs-lookup"><span data-stu-id="5f05f-118">status</span></span> | <span data-ttu-id="5f05f-119">Состояние тегов заметок с флажками.</span><span class="sxs-lookup"><span data-stu-id="5f05f-119">The status of check box note tags.</span></span> <span data-ttu-id="5f05f-120">Это свойство используется только для установки флажков выполненных задач.</span><span class="sxs-lookup"><span data-stu-id="5f05f-120">This is used only to set check boxes as completed.</span></span> |


<a name="note-tags"></a>

## <a name="add-or-update-note-tags"></a><span data-ttu-id="5f05f-121">Добавление или изменение тегов заметок</span><span class="sxs-lookup"><span data-stu-id="5f05f-121">Add or update note tags</span></span>

<span data-ttu-id="5f05f-122">Добавить или изменить тег заметки можно с помощью атрибута `data-tag` в поддерживаемом элементе.</span><span class="sxs-lookup"><span data-stu-id="5f05f-122">To add or update a built-in note tag, just use the `data-tag` attribute on a supported element.</span></span> <span data-ttu-id="5f05f-123">Например, вот абзац, помеченный как важный:</span><span class="sxs-lookup"><span data-stu-id="5f05f-123">For example, here's a paragraph marked as important:</span></span>

```html
<p data-tag="important">...</p>
```

<span data-ttu-id="5f05f-124">Разделение нескольких тегов заметок запятыми:</span><span class="sxs-lookup"><span data-stu-id="5f05f-124">Separate multiple note tags with commas:</span></span>

```html
<p data-tag="important, critical">...</p>
```

<span data-ttu-id="5f05f-125">Вы можете задать атрибут `data-tag` для указанных ниже элементов.</span><span class="sxs-lookup"><span data-stu-id="5f05f-125">You can define a `data-tag` on the following elements:</span></span>

- <span data-ttu-id="5f05f-126">p</span><span class="sxs-lookup"><span data-stu-id="5f05f-126">p</span></span>
- <span data-ttu-id="5f05f-127">ul, ol, li (см. дополнительные сведения о [тегах заметок в списках](#note-tags-on-lists))</span><span class="sxs-lookup"><span data-stu-id="5f05f-127">ul, ol, li (see more about [note tags on lists](#note-tags-on-lists))</span></span>
- <span data-ttu-id="5f05f-128">img</span><span class="sxs-lookup"><span data-stu-id="5f05f-128">img</span></span>
- <span data-ttu-id="5f05f-129">h1–h6</span><span class="sxs-lookup"><span data-stu-id="5f05f-129">h1 - h6</span></span>
- <span data-ttu-id="5f05f-130">title</span><span class="sxs-lookup"><span data-stu-id="5f05f-130">title</span></span>

<span data-ttu-id="5f05f-131">Список тегов заметок, которые можно использовать в Microsoft Graph, см. в разделе [Встроенные теги заметок](#built-in-note-tags-for-onenote).</span><span class="sxs-lookup"><span data-stu-id="5f05f-131">See [Built-in note tags](#built-in-note-tags-for-onenote) for a list of note tags that you can use with Microsoft Graph.</span></span> <span data-ttu-id="5f05f-132">Добавление и изменение пользовательских тегов с помощью Microsoft Graph не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f05f-132">Adding or updating custom tags using Microsoft Graph is not supported.</span></span>

### <a name="examples"></a><span data-ttu-id="5f05f-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="5f05f-133">Examples</span></span>

<span data-ttu-id="5f05f-134">Ниже показан простой список дел, в котором первый элемент завершен.</span><span class="sxs-lookup"><span data-stu-id="5f05f-134">Here's a simple to-do list with the first item completed.</span></span>

```html
<p data-tag="to-do:completed" data-id="prep">Till garden bed</p>
<p data-tag="to-do" data-id="spring">Plant peas and spinach</p>
<p data-tag="to-do" data-id="summer">Plant tomatoes and peppers</p>
```

<span data-ttu-id="5f05f-135">Обратите внимание, что теги `<p>` над каждым пунктом включают атрибут `data-id`.</span><span class="sxs-lookup"><span data-stu-id="5f05f-135">Note that the `<p>` tags above each include a `data-id` attribute.</span></span> <span data-ttu-id="5f05f-136">Это упрощает изменение тегов заметок с флажками.</span><span class="sxs-lookup"><span data-stu-id="5f05f-136">This makes it easier to update the check box note tags.</span></span> <span data-ttu-id="5f05f-137">Например, показанный ниже запрос помечает элемент списка дел (посвященный весенней высадке растений) как выполненный.</span><span class="sxs-lookup"><span data-stu-id="5f05f-137">For example, the following request marks the spring planting to-do item as completed.</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/me/onenote/notebooks/pages/{page-id}/content

Content-Type: application/json
Authorization: Bearer {token}

[
   {
    'target':'#spring',
    'action':'replace',
    'content':'<p data-tag="to-do:completed"  data-id="spring">Plant peas and spinach</p>'
  }
]
```

<span data-ttu-id="5f05f-138">Показанный ниже запрос создает страницу, которая содержит все [встроенные теги заметок](#built-in-note-tags-for-onenote).</span><span class="sxs-lookup"><span data-stu-id="5f05f-138">The following request creates a page that contains all [built-in note tags](#built-in-note-tags-for-onenote).</span></span>

```html
POST https://graph.microsoft.com/v1.0/me/onenote/notebooks/pages

Content-Type: text/html
Authorization: Bearer {token}


<!DOCTYPE html>
<html>
  <head>
    <title data-tag="to-do:completed">All built-in note tags</title>
  </head>
  <body>
    <h1 data-tag="important">Paragraphs with built-in note tags</h1>
    <p data-tag="to-do">to-do</p>
    <p data-tag="important">important</p>
    <p data-tag="question">question</p>
    <p data-tag="definition">definition</p>
    <p data-tag="highlight">highlight</p>
    <p data-tag="contact">contact</p>
    <p data-tag="address">address</p>
    <p data-tag="phone-number">phone-number</p>
    <p data-tag="web-site-to-visit">web-site-to-visit</p>
    <p data-tag="idea">idea</p>
    <p data-tag="password">password</p>
    <p data-tag="critical">critical</p>
    <p data-tag="project-a">project-a</p>
    <p data-tag="project-b">project-b</p>
    <p data-tag="remember-for-later">remember-for-later</p>
    <p data-tag="movie-to-see">movie-to-see</p>
    <p data-tag="book-to-read">book-to-read</p>
    <p data-tag="music-to-listen-to">music-to-listen-to</p>
    <p data-tag="source-for-article">source-for-article</p>
    <p data-tag="remember-for-blog">remember-for-blog</p>
    <p data-tag="discuss-with-person-a">discuss-with-person-a</p>
    <p data-tag="discuss-with-person-b">discuss-with-person-b</p>
    <p data-tag="discuss-with-manager">discuss-with-manager</p>
    <p data-tag="send-in-email">send-in-email</p>
    <p data-tag="schedule-meeting">schedule-meeting</p>
    <p data-tag="call-back">call-back</p>
    <p data-tag="to-do-priority-1">to-do-priority-1</p>
    <p data-tag="to-do-priority-2">to-do-priority-2</p>
    <p data-tag="client-request">client-request</p>
    <h1 data-tag="important">Paragraphs with check boxes marked with "completed" status</h1>
    <p data-tag="to-do:completed">to-do:completed</p>
    <p data-tag="discuss-with-person-a:completed">discuss-with-person-a:completed</p>
    <p data-tag="discuss-with-person-b:completed">discuss-with-person-b:completed</p>
    <p data-tag="discuss-with-manager:completed">discuss-with-manager:completed</p>
    <p data-tag="schedule-meeting:completed">schedule-meeting:completed</p>
    <p data-tag="call-back:completed">call-back:completed</p>
    <p data-tag="to-do-priority-1:completed">to-do-priority-1:completed</p>
    <p data-tag="to-do-priority-2:completed">to-do-priority-2:completed</p>
    <p data-tag="client-request:completed">client-request:completed</p>
    <h1 data-tag="important">Multiple note tags</h1>
    <p data-tag="project-a,  client-request:completed">Two note tags:  project-a, client-request:completed</p>
    <p data-tag="idea, send-in-email, question">Three note tags:  idea, send-in-email, question</p>
    <h1 data-tag="important">Using note tags with other elements</h1>
    <p><b>Note tag on a list item:</b></p>
    <ul>
      <li data-tag="to-do-priority-1:completed">Make a to-do list</li>
    </ul>
    <p><b>Note tag on an image:</b></p>
    <img data-tag="source-for-article" src="https://placecorgi.com/200" />
    <p><b>Note tag with embedded style:</b></p>
    <p data-tag="important">Next time, <b>don't</b> forget to invite <span style="background-color:yellow">Dan</span>.</p>
  </body>
</html>
```

<span data-ttu-id="5f05f-139">Дополнительные сведения о создании страниц см. в статье [Создание страниц в OneNote](onenote-create-page.md).</span><span class="sxs-lookup"><span data-stu-id="5f05f-139">For more information about creating pages, see [Create OneNote pages](onenote-create-page.md).</span></span> <span data-ttu-id="5f05f-140">Дополнительные сведения об изменении страниц см. в статье [Обновление страниц в OneNote](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="5f05f-140">For more about updating pages, see [Update OneNote pages](onenote-update-page.md).</span></span>


<a name="note-tags-lists"></a>

## <a name="note-tags-on-lists"></a><span data-ttu-id="5f05f-141">Теги заметок в списках</span><span class="sxs-lookup"><span data-stu-id="5f05f-141">Note tags on lists</span></span>

<span data-ttu-id="5f05f-142">Ниже приведены рекомендации по работе с тегами заметок в списках.</span><span class="sxs-lookup"><span data-stu-id="5f05f-142">Here are some guidelines for working with note tags on lists:</span></span>

- <span data-ttu-id="5f05f-143">Используйте элементы `p` для списков дел.</span><span class="sxs-lookup"><span data-stu-id="5f05f-143">Use `p` elements for to-do lists.</span></span> <span data-ttu-id="5f05f-144">Они не отображают маркеры или числа, и их проще изменять.</span><span class="sxs-lookup"><span data-stu-id="5f05f-144">They don't display a bullet or number, and they're easier to update.</span></span>

- <span data-ttu-id="5f05f-145">Для создания или обновления списков, в которых отображается **один и тот же** тег заметки для всех элементов списка, определите атрибут `data-tag` в элементе `ul` или `ol`.</span><span class="sxs-lookup"><span data-stu-id="5f05f-145">To create or update lists that display the **same** note tag for all list items, define `data-tag` on the `ul` or `ol`.</span></span> <span data-ttu-id="5f05f-146">Чтобы изменить весь список, вам потребуется повторно определить атрибут `data-tag` в элементе `ul` или `ol`.</span><span class="sxs-lookup"><span data-stu-id="5f05f-146">To update the entire list, you'll need to redefine `data-tag` on the `ul` or `ol`.</span></span>

- <span data-ttu-id="5f05f-147">Для создания или обновления списков, в которых отображается **уникальный** тег заметки для некоторых или всех элементов списка, определите атрибут `data-tag` в элементах `li` и не вкладывайте элементы `li` в элемент `ul` или `ol`.</span><span class="sxs-lookup"><span data-stu-id="5f05f-147">To create or update lists that display a **unique** note tag for some or all list items, define `data-tag` on `li` elements, and don't nest the `li` elements in a `ul` or `ol`.</span></span> <span data-ttu-id="5f05f-148">Чтобы изменить весь список, вам потребуется удалить элемент `ul`, возвращенный в выходном HTML-коде, и предоставить только невложенные элементы `li`.</span><span class="sxs-lookup"><span data-stu-id="5f05f-148">To update the entire list, you'll need to remove the `ul` that's returned in the output HTML and provide only the unnested `li` elements.</span></span>

- <span data-ttu-id="5f05f-149">Чтобы обновить определенные элементы `li`, настройте элементы `li` индивидуально и определите атрибут `data-tag` в элементе `li`.</span><span class="sxs-lookup"><span data-stu-id="5f05f-149">To update specific `li` elements, target the `li` elements individually and define the `data-tag` on the `li` element.</span></span> <span data-ttu-id="5f05f-150">Любой элемент `li` с индивидуальной адресацией можно изменить так, чтобы он отображал уникальный тег заметки независимо от того, как изначально был определен список.</span><span class="sxs-lookup"><span data-stu-id="5f05f-150">Any individually addressed `li` element can be updated to display a unique note tag, no matter how the list was originally defined.</span></span>

  <span data-ttu-id="5f05f-151">Рекомендации основаны на указанных ниже правилах, применяемых Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="5f05f-151">The guidelines are based on the following rules that are applied by Microsoft Graph:</span></span>

  - <span data-ttu-id="5f05f-152">Параметр `data-tag` для элемента `ul` или `ol` переопределяет все параметры в дочерних элементах `li`.</span><span class="sxs-lookup"><span data-stu-id="5f05f-152">The `data-tag` setting for a `ul` or `ol` overrides all settings on child `li` elements.</span></span> <span data-ttu-id="5f05f-153">Это правило применяется, даже если в элементах `ul` или `ol` не указан атрибут `data-tag`, но он указан в дочерних элементах `li`.</span><span class="sxs-lookup"><span data-stu-id="5f05f-153">This applies even when the `ul` or `ol` doesn't specify a `data-tag` but its child `li` elements do.</span></span>

    <span data-ttu-id="5f05f-154">Например, если вы создаете элемент `ul` или `ol`, который определяет атрибут `data-tag="project-a"`, то все его элементы будут отображать тег заметки *Project A*.</span><span class="sxs-lookup"><span data-stu-id="5f05f-154">For example, if you create a `ul` or `ol` that defines `data-tag="project-a"`, all its list items will display the *Project A* note tag.</span></span> <span data-ttu-id="5f05f-155">Если элемент `ul` или `ol` не определяет атрибут `data-tag`, ни один из его элементов не будет отображать тег заметки.</span><span class="sxs-lookup"><span data-stu-id="5f05f-155">Or if the `ul` or `ol` doesn't define a `data-tag`, none of its items will display a note tag.</span></span> <span data-ttu-id="5f05f-156">Это переопределение происходит независимо от любых явных параметров в дочерних элементах `li`.</span><span class="sxs-lookup"><span data-stu-id="5f05f-156">This override happens regardless of any explicit settings on child `li` elements.</span></span>

- <span data-ttu-id="5f05f-157">Уникальные параметры `data-tag` применяются к элементам списка в указанных ниже условиях.</span><span class="sxs-lookup"><span data-stu-id="5f05f-157">Unique `data-tag` settings are honored for list items under the following conditions:</span></span>

  - <span data-ttu-id="5f05f-158">Элементы `li` не вложены в элемент `ul` или `ol` в запросе на создание или изменение.</span><span class="sxs-lookup"><span data-stu-id="5f05f-158">The `li` elements are not nested in a `ul` or `ol` in a create or update request.</span></span>

  - <span data-ttu-id="5f05f-159">Элемент `li` имеет индивидуальную адресацию в запросе на изменение.</span><span class="sxs-lookup"><span data-stu-id="5f05f-159">An `li` element is individually addressed in an update request.</span></span>

- <span data-ttu-id="5f05f-160">Невложенные элементы `li`, отправленные во входном HTML-коде, возвращаются в элементе `ul` в выходном HTML-коде.</span><span class="sxs-lookup"><span data-stu-id="5f05f-160">Unnested `li` elements sent in input HTML are returned in a `ul` in the output HTML.</span></span>

- <span data-ttu-id="5f05f-161">В выходном HTML-коде все параметры списка `data-tag` определены в элементах `span` в элементах списка.</span><span class="sxs-lookup"><span data-stu-id="5f05f-161">In output HTML, all `data-tag` list settings are defined on `span` elements on the list items.</span></span>


<span data-ttu-id="5f05f-162">В приведенном ниже коде показано, как применять некоторые из этих правил.</span><span class="sxs-lookup"><span data-stu-id="5f05f-162">The following code shows how some of these rules are applied.</span></span> <span data-ttu-id="5f05f-163">Входной HTML-код создает два списка с тегами заметок.</span><span class="sxs-lookup"><span data-stu-id="5f05f-163">The input HTML creates two lists with note tags.</span></span> <span data-ttu-id="5f05f-164">Выходной HTML-код — это то, что система возвращает для списков, когда вы получаете контент страницы.</span><span class="sxs-lookup"><span data-stu-id="5f05f-164">The output HTML is what's returned for the lists when you retrieve page content.</span></span>

#### <a name="input-html"></a><span data-ttu-id="5f05f-165">Входной HTML-код</span><span class="sxs-lookup"><span data-stu-id="5f05f-165">Input HTML</span></span>

```html
<!--To display the same note tag on all list items, define note tags on the ul or ol.-->
<ul data-tag="project-a" data-id="agenda">
  <li>An item with a Project A note tag</li>
  <li>An item with a Project A note tag</li>
</ul>

<!--To display unique note tags on list items, don't nest li elements in a ul or ol.-->
<li data-tag="idea" data-id="my-idea">An item with an Idea note tag</li>
<li data-tag="question" data-id="my-question">An item with a Question note tag</li>
```

#### <a name="output-html"></a><span data-ttu-id="5f05f-166">Выходной HTML-код</span><span class="sxs-lookup"><span data-stu-id="5f05f-166">Output HTML</span></span>

```html
<ul>
  <li><span data-tag="project-a">An item with a Project A note tag</span></li>
  <li><span data-tag="project-a">An item with a Project A note tag</span></li>
</ul>
<br />
<ul>
  <li style="..."><span data-tag="idea">An item with an Idea note tag</span></li>
  <li style="..."><span data-tag="question">An item with a Question note tag</span></li>
</ul>
```

<a name="output-html"></a>

## <a name="retrieve-note-tags"></a><span data-ttu-id="5f05f-167">Получение тегов заметок</span><span class="sxs-lookup"><span data-stu-id="5f05f-167">Retrieve note tags</span></span>

<span data-ttu-id="5f05f-168">Встроенные теги заметок включаются в выходной HTML, когда вы получаете контент страницы:</span><span class="sxs-lookup"><span data-stu-id="5f05f-168">Built-in note tags are included in the output HTML when you get page content:</span></span>

`GET ../api/v1.0/pages/{page-id}/content`

<span data-ttu-id="5f05f-169">Атрибут `data-tag` в выходном HTML-коде всегда включает значение фигуры. Он включает состояние, только если он представляет тег заметки с установленным флажком (для выполненного элемента списка).</span><span class="sxs-lookup"><span data-stu-id="5f05f-169">A `data-tag` attribute in the output HTML always includes a shape value, and it only includes a status if it represents a check box note tag that's set to completed.</span></span> <span data-ttu-id="5f05f-170">В примерах ниже показан входной HTML-код, используемый для создания некоторых тегов заметок, и возвращаемый выходной HTML-код.</span><span class="sxs-lookup"><span data-stu-id="5f05f-170">The following examples show the input HTML used to create some note tags and the output HTML that's returned.</span></span>

#### <a name="input-html"></a><span data-ttu-id="5f05f-171">Входной HTML-код</span><span class="sxs-lookup"><span data-stu-id="5f05f-171">Input HTML</span></span>

```html
<h1>Status meeting</h1>
<p data-tag="important">Next week's meeting has been moved to <b>Wednesday</b>.</p>
<p data-tag="question">What are the exact dates for the conference?</p>
<p>Upcoming training opportunities. See Katie for more info.</p>
<p data-tag="project-a">Around the room updates.</p>
<ul data-tag="critical">
  <li>Design handouts</li>
  <li>Plan keynote</li>
</ul>
```

#### <a name="output-html"></a><span data-ttu-id="5f05f-172">Выходной HTML-код</span><span class="sxs-lookup"><span data-stu-id="5f05f-172">Output HTML</span></span>

```html
<h1 style="...">Status meeting</h1>
<p data-tag="important">Next week's meeting has been moved to <span style="font-weight:bold">Wednesday</span>.</p>
<p data-tag="question">What are the exact dates for the conference?</p>
<p>Upcoming training opportunities. See Katie for more info.</p>
<p data-tag="project-a">Around the room updates.</p>
<ul>
  <li><span data-tag="critical">Design handouts</span></li>
  <li><span data-tag="critical">Plan keynote</span></li>
</ul>
```

<span data-ttu-id="5f05f-173">Обратите внимание, что атрибут `data-tag`, определенный на уровне списка, передается в его элементы списка.</span><span class="sxs-lookup"><span data-stu-id="5f05f-173">Note that the `data-tag` attribute defined at the list level is pushed to its list items.</span></span> <span data-ttu-id="5f05f-174">Дополнительные сведения об использовании тегов заметок со списками см. в статье [Теги заметок в списках](#note-tags-on-lists).</span><span class="sxs-lookup"><span data-stu-id="5f05f-174">For more information about using note tags with lists, see [Note tags on lists](#note-tags-on-lists).</span></span>

> <span data-ttu-id="5f05f-175">**Примечание.** В выходном HTML-коде определение и теги заметок "Запомнить" возвращаются в виде атрибута `data-tag="remember-for-later"`.</span><span class="sxs-lookup"><span data-stu-id="5f05f-175">**Note:** In the output HTML, the definition and remember-for-later note tags are both returned as `data-tag="remember-for-later"`.</span></span> <span data-ttu-id="5f05f-176">Элемент `title` не возвращает никаких сведений о тегах заметок.</span><span class="sxs-lookup"><span data-stu-id="5f05f-176">The `title` element doesn't return any note tag information.</span></span>




<a name="built-in-tags"></a>

## <a name="built-in-note-tags-for-onenote"></a><span data-ttu-id="5f05f-177">Встроенные теги заметок для OneNote</span><span class="sxs-lookup"><span data-stu-id="5f05f-177">Built-in note tags for OneNote</span></span>

<span data-ttu-id="5f05f-178">В OneNote имеются указанные ниже встроенные теги заметок.</span><span class="sxs-lookup"><span data-stu-id="5f05f-178">OneNote includes the following built-in note tags:</span></span>

![Все встроенные теги заметок.](images/note-tags-all.png)

<span data-ttu-id="5f05f-180">Значения, которые можно присвоить атрибуту `data-tag`, показаны в следующем списке.</span><span class="sxs-lookup"><span data-stu-id="5f05f-180">The values you can assign to the `data-tag` attribute are shown in the following list.</span></span> <span data-ttu-id="5f05f-181">Пользовательские теги не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="5f05f-181">Custom tags are not supported.</span></span>

- `shape[:status]`
- `to-do`
- `to-do:completed`
- `important`
- `question`
- `definition`
- `highlight`
- `contact`
- `address`
- `phone-number`
- `web-site-to-visit`
- `idea`
- `password`
- `critical`
- `project-a`
- `project-b`
- `remember-for-later`
- `movie-to-see`
- `book-to-read`
- `music-to-listen-to`
- `source-for-article`
- `remember-for-blog`
- `discuss-with-person-a`
- `discuss-with-person-a:completed`
- `discuss-with-person-b`
- `discuss-with-person-b:completed`
- `discuss-with-manager`
- `discuss-with-manager:completed`
- `send-in-email`
- `schedule-meeting`
- `schedule-meeting:completed`
- `call-back`
- `call-back:completed`
- `to-do-priority-1`
- `to-do-priority-1:completed`
- `to-do-priority-2`
- `to-do-priority-2:completed`
- `client-request`
- `client-request:completed`


<a name="request-response-info"></a>

## <a name="response-information"></a><span data-ttu-id="5f05f-182">Сведения в отклике</span><span class="sxs-lookup"><span data-stu-id="5f05f-182">Response information</span></span>

<span data-ttu-id="5f05f-183">Microsoft Graph возвращает указанные ниже сведения в отклике.</span><span class="sxs-lookup"><span data-stu-id="5f05f-183">Microsoft Graph returns the following information in the response.</span></span>

| <span data-ttu-id="5f05f-184">Данные в отклике</span><span class="sxs-lookup"><span data-stu-id="5f05f-184">Response data</span></span> | <span data-ttu-id="5f05f-185">Описание</span><span class="sxs-lookup"><span data-stu-id="5f05f-185">Description</span></span> |
|------|------|
| <span data-ttu-id="5f05f-186">Код успешного завершения действия</span><span class="sxs-lookup"><span data-stu-id="5f05f-186">Success code</span></span> | <span data-ttu-id="5f05f-187">Код состояния HTTP 201 при успешном выполнении запроса POST и код состояния HTTP 204 при успешном выполнении запроса PATCH.</span><span class="sxs-lookup"><span data-stu-id="5f05f-187">A 201 HTTP status code for a successful POST request, and a 204 HTTP status code for a successful PATCH request.</span></span> |
| <span data-ttu-id="5f05f-188">Ошибки</span><span class="sxs-lookup"><span data-stu-id="5f05f-188">Errors</span></span> | <span data-ttu-id="5f05f-189">Дополнительные сведения об ошибках OneNote, которые может возвращать Microsoft Graph, см. в статье [Коды ошибок для API OneNote в Microsoft Graph](onenote-error-codes.md).</span><span class="sxs-lookup"><span data-stu-id="5f05f-189">Read [Error codes for OneNote APIs in Microsoft Graph](onenote-error-codes.md) to learn about OneNote errors that Microsoft Graph can return.</span></span> |


<a name="permissions"></a>

## <a name="permissions"></a><span data-ttu-id="5f05f-190">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5f05f-190">Permissions</span></span>

<span data-ttu-id="5f05f-191">Чтобы можно было создавать или изменять страницы OneNote, вам придется запросить соответствующие разрешения.</span><span class="sxs-lookup"><span data-stu-id="5f05f-191">To create or update OneNote pages, you'll need to request appropriate permissions.</span></span> <span data-ttu-id="5f05f-192">Выберите минимальный уровень разрешений, необходимый для работы вашего приложения.</span><span class="sxs-lookup"><span data-stu-id="5f05f-192">Choose the lowest level of permissions that your app needs to do its work.</span></span>

#### <a name="permissions-for-post-pages"></a><span data-ttu-id="5f05f-193">Разрешения для запросов POST со страницами</span><span class="sxs-lookup"><span data-stu-id="5f05f-193">Permissions for POST pages</span></span>

- <span data-ttu-id="5f05f-194">Notes.Create</span><span class="sxs-lookup"><span data-stu-id="5f05f-194">Notes.Create</span></span>
- <span data-ttu-id="5f05f-195">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5f05f-195">Notes.ReadWrite</span></span>
- <span data-ttu-id="5f05f-196">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f05f-196">Notes.ReadWrite.All</span></span>

#### <a name="permissions-for-patch-pages"></a><span data-ttu-id="5f05f-197">Разрешения в случае запросов PATCH для страниц</span><span class="sxs-lookup"><span data-stu-id="5f05f-197">Permissions for PATCH pages</span></span>

- <span data-ttu-id="5f05f-198">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5f05f-198">Notes.ReadWrite</span></span>
- <span data-ttu-id="5f05f-199">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f05f-199">Notes.ReadWrite.All</span></span>

<span data-ttu-id="5f05f-200">Дополнительные сведения об областях разрешений и принципе их работы см. в разделе [Области разрешений OneNote](permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="5f05f-200">For more information about permission scopes and how they work, see [OneNote permission scopes](permissions-reference.md).</span></span>


<a name="see-also"></a>

## <a name="see-also"></a><span data-ttu-id="5f05f-201">См. также</span><span class="sxs-lookup"><span data-stu-id="5f05f-201">See also</span></span>

- [<span data-ttu-id="5f05f-202">Создание страниц OneNote</span><span class="sxs-lookup"><span data-stu-id="5f05f-202">Create OneNote pages</span></span>](onenote-create-page.md)
- [<span data-ttu-id="5f05f-203">Обновление содержимого страницы OneNote</span><span class="sxs-lookup"><span data-stu-id="5f05f-203">Update OneNote page content</span></span>](onenote-update-page.md)
- [<span data-ttu-id="5f05f-204">Интеграция с OneNote</span><span class="sxs-lookup"><span data-stu-id="5f05f-204">Integrate with OneNote</span></span>](integrate-with-onenote.md)
- [<span data-ttu-id="5f05f-205">Блог разработчиков OneNote</span><span class="sxs-lookup"><span data-stu-id="5f05f-205">OneNote Developer Blog</span></span>](https://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="5f05f-206">Вопросы разработки OneNote на сайте «Вопросы и ответы Майкрософт»</span><span class="sxs-lookup"><span data-stu-id="5f05f-206">OneNote development questions on Microsoft Q&A</span></span>](/answers/topics/microsoft-graph-notes.html)
- [<span data-ttu-id="5f05f-207">Репозитории GitHub OneNote</span><span class="sxs-lookup"><span data-stu-id="5f05f-207">OneNote GitHub repos</span></span>](https://go.microsoft.com/fwlink/?LinkID=390178)