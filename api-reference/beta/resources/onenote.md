---
title: Тип ресурса onenote
description: Точка входа для ресурсов OneNote.
ms.openlocfilehash: c1b875b686015df8134103b0793a1e342e7f4b89
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076993"
---
# <a name="onenote-resource-type"></a><span data-ttu-id="bd0e3-103">Тип ресурса onenote</span><span class="sxs-lookup"><span data-stu-id="bd0e3-103">onenote resource type</span></span>

> <span data-ttu-id="bd0e3-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bd0e3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bd0e3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd0e3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bd0e3-106">Точка входа для ресурсов OneNote.</span><span class="sxs-lookup"><span data-stu-id="bd0e3-106">The entry point for OneNote resources.</span></span>

<span data-ttu-id="bd0e3-107">Все вызовы службы OneNote через API Microsoft Graph выполняются с помощью следующего корневого URL-адреса службы:</span><span class="sxs-lookup"><span data-stu-id="bd0e3-107">All calls to the OneNote service through the Microsoft Graph API use this service root URL:</span></span>

```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

<span data-ttu-id="bd0e3-108">Расположение может быть записных книжек пользователя на Office 365 или потребитель OneDrive, группа записных книжек или записных книжек размещенного сайта группы SharePoint на Office 365.</span><span class="sxs-lookup"><span data-stu-id="bd0e3-108">The location can be user notebooks on Office 365 or consumer OneDrive, group notebooks, or SharePoint site-hosted team notebooks on Office 365.</span></span> 

<span data-ttu-id="bd0e3-109">**Записные книжки пользователей.** Чтобы получить доступ к персональным записным книжкам в OneDrive для бизнеса или личном хранилище OneDrive, воспользуйтесь одним из следующих URL-адресов:</span><span class="sxs-lookup"><span data-stu-id="bd0e3-109">**User notebooks** To access personal notebooks on consumer OneDrive or OneDrive for Business, use one of the following URLs:</span></span>

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

<span data-ttu-id="bd0e3-110">**Записные книжки группы.** Чтобы получить доступ к записным книжкам группы, воспользуйтесь следующим корневым URL-адресом службы:</span><span class="sxs-lookup"><span data-stu-id="bd0e3-110">**Group notebooks** To access notebooks that are owned by a group, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
<span data-ttu-id="bd0e3-111">**Записные книжки на сайте SharePoint.** Чтобы получить доступ к записным книжкам на сайте группы SharePoint, воспользуйтесь следующим корневым URL-адресом службы:</span><span class="sxs-lookup"><span data-stu-id="bd0e3-111">**SharePoint site notebooks** To access notebooks that are owned by a SharePoint team site, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

## <a name="authorization"></a><span data-ttu-id="bd0e3-112">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bd0e3-112">Authorization</span></span>

<span data-ttu-id="bd0e3-113">Сведения о разрешениях, необходимых для работы с API OneNote, см. в разделе [Разрешения для заметок](/graph/permissions-reference#notes-permissions).</span><span class="sxs-lookup"><span data-stu-id="bd0e3-113">For information about the permissions required to work with OneNote APIs, see [Notes permissions](/graph/permissions-reference#notes-permissions).</span></span>

## <a name="relationships"></a><span data-ttu-id="bd0e3-114">Отношения</span><span class="sxs-lookup"><span data-stu-id="bd0e3-114">Relationships</span></span>
| <span data-ttu-id="bd0e3-115">Связь</span><span class="sxs-lookup"><span data-stu-id="bd0e3-115">Relationship</span></span> | <span data-ttu-id="bd0e3-116">Тип</span><span class="sxs-lookup"><span data-stu-id="bd0e3-116">Type</span></span>   |<span data-ttu-id="bd0e3-117">Описание</span><span class="sxs-lookup"><span data-stu-id="bd0e3-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bd0e3-118">notebooks</span><span class="sxs-lookup"><span data-stu-id="bd0e3-118">notebooks</span></span>|<span data-ttu-id="bd0e3-119">Коллекция [Notebook](notebook.md)</span><span class="sxs-lookup"><span data-stu-id="bd0e3-119">[Notebook](notebook.md) collection</span></span>|<span data-ttu-id="bd0e3-p102">Коллекция записных книжек OneNote, принадлежащих пользователю или группе. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="bd0e3-p102">The collection of OneNote notebooks that are owned by the user or group. Read-only. Nullable.</span></span>|
|<span data-ttu-id="bd0e3-123">operations</span><span class="sxs-lookup"><span data-stu-id="bd0e3-123">operations</span></span>|<span data-ttu-id="bd0e3-124">Коллекция объектов [Operation](onenoteoperation.md)</span><span class="sxs-lookup"><span data-stu-id="bd0e3-124">[Operation](onenoteoperation.md) collection</span></span> |<span data-ttu-id="bd0e3-p103">Состояние операций OneNote. Получение коллекции операций не поддерживается, но можно получить состояние длительных операций, если в отклике возвращается заголовок `Operation-Location`. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="bd0e3-p103">The status of OneNote operations. Getting an operations collection is not supported, but you can get the status of long-running operations if the `Operation-Location` header is returned in the response. Read-only. Nullable.</span></span>|
|<span data-ttu-id="bd0e3-129">pages</span><span class="sxs-lookup"><span data-stu-id="bd0e3-129">pages</span></span>|<span data-ttu-id="bd0e3-130">Коллекция [Page](page.md)</span><span class="sxs-lookup"><span data-stu-id="bd0e3-130">[Page](page.md) collection</span></span>|<span data-ttu-id="bd0e3-p104">Страницы всех записных книжек OneNote, принадлежащих пользователю или группе.  Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="bd0e3-p104">The pages in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|
|<span data-ttu-id="bd0e3-134">resources</span><span class="sxs-lookup"><span data-stu-id="bd0e3-134">resources</span></span>|<span data-ttu-id="bd0e3-135">Коллекция объектов [Resource](resource.md)</span><span class="sxs-lookup"><span data-stu-id="bd0e3-135">[Resource](resource.md) collection</span></span> |<span data-ttu-id="bd0e3-p105">Изображения и другие ресурсы file на страницах OneNote. Получение коллекции ресурсов не поддерживается, но можно [получить двоичное содержимое определенного ресурса](resource.md). Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="bd0e3-p105">The image and other file resources in OneNote pages. Getting a resources collection is not supported, but you can [get the binary content of a specific resource](resource.md). Read-only. Nullable.</span></span>|
|<span data-ttu-id="bd0e3-140">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="bd0e3-140">sectionGroups</span></span>|<span data-ttu-id="bd0e3-141">Коллекция [SectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="bd0e3-141">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="bd0e3-p106">Группы разделов во всех записных книжках OneNote, принадлежащих пользователю или группе.  Только для чтения. Допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="bd0e3-p106">The section groups in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|
|<span data-ttu-id="bd0e3-145">sections</span><span class="sxs-lookup"><span data-stu-id="bd0e3-145">sections</span></span>|<span data-ttu-id="bd0e3-146">Коллекция [Section](section.md)</span><span class="sxs-lookup"><span data-stu-id="bd0e3-146">[Section](section.md) collection</span></span>|<span data-ttu-id="bd0e3-p107">Разделы во всех записных книжках OneNote, принадлежащих пользователю или группе.  Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="bd0e3-p107">The sections in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="bd0e3-150">Методы</span><span class="sxs-lookup"><span data-stu-id="bd0e3-150">Methods</span></span>

| <span data-ttu-id="bd0e3-151">Метод</span><span class="sxs-lookup"><span data-stu-id="bd0e3-151">Method</span></span>           | <span data-ttu-id="bd0e3-152">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bd0e3-152">Return Type</span></span>    |<span data-ttu-id="bd0e3-153">Описание</span><span class="sxs-lookup"><span data-stu-id="bd0e3-153">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bd0e3-154">Создание записной книжки</span><span class="sxs-lookup"><span data-stu-id="bd0e3-154">Create notebook</span></span>](../api/onenote-post-notebooks.md) |[<span data-ttu-id="bd0e3-155">Notebook</span><span class="sxs-lookup"><span data-stu-id="bd0e3-155">Notebook</span></span>](notebook.md)| <span data-ttu-id="bd0e3-156">Создание записной книжки путем публикации в коллекции записных книжек.</span><span class="sxs-lookup"><span data-stu-id="bd0e3-156">Create a notebook by posting to the notebooks collection.</span></span>|
|[<span data-ttu-id="bd0e3-157">Перечисление записных книжек</span><span class="sxs-lookup"><span data-stu-id="bd0e3-157">List notebooks</span></span>](../api/onenote-list-notebooks.md) |<span data-ttu-id="bd0e3-158">Коллекция [Notebook](notebook.md)</span><span class="sxs-lookup"><span data-stu-id="bd0e3-158">[Notebook](notebook.md) collection</span></span>| <span data-ttu-id="bd0e3-159">Получение коллекции записных книжек.</span><span class="sxs-lookup"><span data-stu-id="bd0e3-159">Get a collection of notebooks.</span></span>|
|[<span data-ttu-id="bd0e3-160">Создание страницы</span><span class="sxs-lookup"><span data-stu-id="bd0e3-160">Create page</span></span>](../api/onenote-post-pages.md) |[<span data-ttu-id="bd0e3-161">Page</span><span class="sxs-lookup"><span data-stu-id="bd0e3-161">Page</span></span>](page.md)| <span data-ttu-id="bd0e3-162">Создание страницы путем публикации в коллекции страниц.</span><span class="sxs-lookup"><span data-stu-id="bd0e3-162">Create a page by posting to the pages collection.</span></span>|
|[<span data-ttu-id="bd0e3-163">Перечисление страниц</span><span class="sxs-lookup"><span data-stu-id="bd0e3-163">List pages</span></span>](../api/onenote-list-pages.md) |<span data-ttu-id="bd0e3-164">Коллекция [Page](page.md)</span><span class="sxs-lookup"><span data-stu-id="bd0e3-164">[Page](page.md) collection</span></span>| <span data-ttu-id="bd0e3-165">Получение коллекции страниц.</span><span class="sxs-lookup"><span data-stu-id="bd0e3-165">Get a collection of pages.</span></span>|
|[<span data-ttu-id="bd0e3-166">Перечисление групп разделов</span><span class="sxs-lookup"><span data-stu-id="bd0e3-166">List section groups</span></span>](../api/onenote-list-sectiongroups.md) |<span data-ttu-id="bd0e3-167">Коллекция [SectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="bd0e3-167">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="bd0e3-168">Получение коллекции групп разделов.</span><span class="sxs-lookup"><span data-stu-id="bd0e3-168">Get a collection of section groups.</span></span>|
|[<span data-ttu-id="bd0e3-169">Перечисление разделов</span><span class="sxs-lookup"><span data-stu-id="bd0e3-169">List sections</span></span>](../api/onenote-list-sections.md) |<span data-ttu-id="bd0e3-170">Коллекция [Section](section.md)</span><span class="sxs-lookup"><span data-stu-id="bd0e3-170">[Section](section.md) collection</span></span>| <span data-ttu-id="bd0e3-171">Получение коллекции разделов.</span><span class="sxs-lookup"><span data-stu-id="bd0e3-171">Get a collection of sections.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenote resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
