---
title: Тип ресурса OneNote
description: Точка входа для ресурсов OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 5ed063fb485acdbd029a977ffb6cd721bf7085c8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561665"
---
# <a name="onenote-resource-type"></a><span data-ttu-id="b5fe0-103">Тип ресурса OneNote</span><span class="sxs-lookup"><span data-stu-id="b5fe0-103">onenote resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5fe0-104">Точка входа для ресурсов OneNote.</span><span class="sxs-lookup"><span data-stu-id="b5fe0-104">The entry point for OneNote resources.</span></span>

<span data-ttu-id="b5fe0-105">Все вызовы службы OneNote через API Microsoft Graph используют следующий корневой URL-адрес службы:</span><span class="sxs-lookup"><span data-stu-id="b5fe0-105">All calls to the OneNote service through the Microsoft Graph API use this service root URL:</span></span>

```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

<span data-ttu-id="b5fe0-106">Местоположение может представлять собой записные книжки для пользователей в Office 365 или OneDrive для пользователей, групповых записных книжек или размещенных на сайте SharePoint записных книжек группы в Office 365.</span><span class="sxs-lookup"><span data-stu-id="b5fe0-106">The location can be user notebooks on Office 365 or consumer OneDrive, group notebooks, or SharePoint site-hosted team notebooks on Office 365.</span></span> 

<span data-ttu-id="b5fe0-107">**Записные книжКи пользователя** Чтобы получить доступ к личным записным книжкам в OneDrive для бизнеса или OneDrive для бизнеса, используйте один из следующих URL-адресов:</span><span class="sxs-lookup"><span data-stu-id="b5fe0-107">**User notebooks** To access personal notebooks on consumer OneDrive or OneDrive for Business, use one of the following URLs:</span></span>

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

<span data-ttu-id="b5fe0-108">**Записные книжки для групп** Чтобы получить доступ к записным книжкам, принадлежащим группе, используйте следующий корневой URL-адрес службы:</span><span class="sxs-lookup"><span data-stu-id="b5fe0-108">**Group notebooks** To access notebooks that are owned by a group, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
<span data-ttu-id="b5fe0-109">**Записные книжки сайта SharePoint** Чтобы получить доступ к записным книжкам, принадлежащим сайту группы SharePoint, используйте следующий корневой URL-адрес службы:</span><span class="sxs-lookup"><span data-stu-id="b5fe0-109">**SharePoint site notebooks** To access notebooks that are owned by a SharePoint team site, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

## <a name="authorization"></a><span data-ttu-id="b5fe0-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5fe0-110">Authorization</span></span>

<span data-ttu-id="b5fe0-111">Для получения сведений о разрешениях, необходимых для работы с API [](/graph/permissions-reference#notes-permissions)OneNote, ознакомьтесь с разрешениями для заметок.</span><span class="sxs-lookup"><span data-stu-id="b5fe0-111">For information about the permissions required to work with OneNote APIs, see [Notes permissions](/graph/permissions-reference#notes-permissions).</span></span>

## <a name="relationships"></a><span data-ttu-id="b5fe0-112">Отношения</span><span class="sxs-lookup"><span data-stu-id="b5fe0-112">Relationships</span></span>
| <span data-ttu-id="b5fe0-113">Отношение</span><span class="sxs-lookup"><span data-stu-id="b5fe0-113">Relationship</span></span> | <span data-ttu-id="b5fe0-114">Тип</span><span class="sxs-lookup"><span data-stu-id="b5fe0-114">Type</span></span>   |<span data-ttu-id="b5fe0-115">Описание</span><span class="sxs-lookup"><span data-stu-id="b5fe0-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b5fe0-116">notebooks</span><span class="sxs-lookup"><span data-stu-id="b5fe0-116">notebooks</span></span>|<span data-ttu-id="b5fe0-117">[](notebook.md) Коллекция записных книжек</span><span class="sxs-lookup"><span data-stu-id="b5fe0-117">[Notebook](notebook.md) collection</span></span>|<span data-ttu-id="b5fe0-118">Коллекция записных книжек OneNote, принадлежащих пользователю или группе.</span><span class="sxs-lookup"><span data-stu-id="b5fe0-118">The collection of OneNote notebooks that are owned by the user or group.</span></span> <span data-ttu-id="b5fe0-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b5fe0-119">Read-only.</span></span> <span data-ttu-id="b5fe0-120">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="b5fe0-120">Nullable.</span></span>|
|<span data-ttu-id="b5fe0-121">operations</span><span class="sxs-lookup"><span data-stu-id="b5fe0-121">operations</span></span>|<span data-ttu-id="b5fe0-122">Коллекция [Operation](onenoteoperation.md)</span><span class="sxs-lookup"><span data-stu-id="b5fe0-122">[Operation](onenoteoperation.md) collection</span></span> |<span data-ttu-id="b5fe0-123">Состояние операций OneNote.</span><span class="sxs-lookup"><span data-stu-id="b5fe0-123">The status of OneNote operations.</span></span> <span data-ttu-id="b5fe0-124">Получение коллекции Operations не поддерживается, но вы можете получить состояние длительно выполняемых операций, если `Operation-Location` заголовок возвращается в ответе.</span><span class="sxs-lookup"><span data-stu-id="b5fe0-124">Getting an operations collection is not supported, but you can get the status of long-running operations if the `Operation-Location` header is returned in the response.</span></span> <span data-ttu-id="b5fe0-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b5fe0-125">Read-only.</span></span> <span data-ttu-id="b5fe0-126">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="b5fe0-126">Nullable.</span></span>|
|<span data-ttu-id="b5fe0-127">pages</span><span class="sxs-lookup"><span data-stu-id="b5fe0-127">pages</span></span>|<span data-ttu-id="b5fe0-128">Коллекция [страниц](page.md)</span><span class="sxs-lookup"><span data-stu-id="b5fe0-128">[Page](page.md) collection</span></span>|<span data-ttu-id="b5fe0-129">Страницы во всех записных книжках OneNote, принадлежащие пользователю или группе.</span><span class="sxs-lookup"><span data-stu-id="b5fe0-129">The pages in all OneNote notebooks that are owned by the user or group.</span></span>  <span data-ttu-id="b5fe0-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b5fe0-130">Read-only.</span></span> <span data-ttu-id="b5fe0-131">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="b5fe0-131">Nullable.</span></span>|
|<span data-ttu-id="b5fe0-132">resources</span><span class="sxs-lookup"><span data-stu-id="b5fe0-132">resources</span></span>|<span data-ttu-id="b5fe0-133">Коллекция [ресурсов](resource.md)</span><span class="sxs-lookup"><span data-stu-id="b5fe0-133">[Resource](resource.md) collection</span></span> |<span data-ttu-id="b5fe0-134">Изображение и другие файловые ресурсы на страницах OneNote.</span><span class="sxs-lookup"><span data-stu-id="b5fe0-134">The image and other file resources in OneNote pages.</span></span> <span data-ttu-id="b5fe0-135">Получение коллекции ресурсов не поддерживается, но вы можете [получить двоичное содержимое определенного ресурса](resource.md).</span><span class="sxs-lookup"><span data-stu-id="b5fe0-135">Getting a resources collection is not supported, but you can [get the binary content of a specific resource](resource.md).</span></span> <span data-ttu-id="b5fe0-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b5fe0-136">Read-only.</span></span> <span data-ttu-id="b5fe0-137">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="b5fe0-137">Nullable.</span></span>|
|<span data-ttu-id="b5fe0-138">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="b5fe0-138">sectionGroups</span></span>|<span data-ttu-id="b5fe0-139">Коллекция [sectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="b5fe0-139">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="b5fe0-140">Группы разделов во всех записных книжках OneNote, принадлежащие пользователю или группе.</span><span class="sxs-lookup"><span data-stu-id="b5fe0-140">The section groups in all OneNote notebooks that are owned by the user or group.</span></span>  <span data-ttu-id="b5fe0-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b5fe0-141">Read-only.</span></span> <span data-ttu-id="b5fe0-142">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="b5fe0-142">Nullable.</span></span>|
|<span data-ttu-id="b5fe0-143">sections</span><span class="sxs-lookup"><span data-stu-id="b5fe0-143">sections</span></span>|<span data-ttu-id="b5fe0-144">Коллекция [section](section.md)</span><span class="sxs-lookup"><span data-stu-id="b5fe0-144">[Section](section.md) collection</span></span>|<span data-ttu-id="b5fe0-145">Разделы во всех записных книжках OneNote, принадлежащие пользователю или группе.</span><span class="sxs-lookup"><span data-stu-id="b5fe0-145">The sections in all OneNote notebooks that are owned by the user or group.</span></span>  <span data-ttu-id="b5fe0-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b5fe0-146">Read-only.</span></span> <span data-ttu-id="b5fe0-147">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="b5fe0-147">Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="b5fe0-148">Методы</span><span class="sxs-lookup"><span data-stu-id="b5fe0-148">Methods</span></span>

| <span data-ttu-id="b5fe0-149">Метод</span><span class="sxs-lookup"><span data-stu-id="b5fe0-149">Method</span></span>           | <span data-ttu-id="b5fe0-150">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b5fe0-150">Return Type</span></span>    |<span data-ttu-id="b5fe0-151">Описание</span><span class="sxs-lookup"><span data-stu-id="b5fe0-151">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b5fe0-152">Создание записной книжки</span><span class="sxs-lookup"><span data-stu-id="b5fe0-152">Create notebook</span></span>](../api/onenote-post-notebooks.md) |[<span data-ttu-id="b5fe0-153">Notebook</span><span class="sxs-lookup"><span data-stu-id="b5fe0-153">Notebook</span></span>](notebook.md)| <span data-ttu-id="b5fe0-154">Создание записной книжки путем публикации в коллекции записных книжек.</span><span class="sxs-lookup"><span data-stu-id="b5fe0-154">Create a notebook by posting to the notebooks collection.</span></span>|
|[<span data-ttu-id="b5fe0-155">Список записных книжек</span><span class="sxs-lookup"><span data-stu-id="b5fe0-155">List notebooks</span></span>](../api/onenote-list-notebooks.md) |<span data-ttu-id="b5fe0-156">[](notebook.md) Коллекция записных книжек</span><span class="sxs-lookup"><span data-stu-id="b5fe0-156">[Notebook](notebook.md) collection</span></span>| <span data-ttu-id="b5fe0-157">Получение коллекции записных книжек.</span><span class="sxs-lookup"><span data-stu-id="b5fe0-157">Get a collection of notebooks.</span></span>|
|[<span data-ttu-id="b5fe0-158">Создание страницы</span><span class="sxs-lookup"><span data-stu-id="b5fe0-158">Create page</span></span>](../api/onenote-post-pages.md) |[<span data-ttu-id="b5fe0-159">Page</span><span class="sxs-lookup"><span data-stu-id="b5fe0-159">Page</span></span>](page.md)| <span data-ttu-id="b5fe0-160">Создание страницы путем публикации в коллекции Pages.</span><span class="sxs-lookup"><span data-stu-id="b5fe0-160">Create a page by posting to the pages collection.</span></span>|
|[<span data-ttu-id="b5fe0-161">Перечисление страниц</span><span class="sxs-lookup"><span data-stu-id="b5fe0-161">List pages</span></span>](../api/onenote-list-pages.md) |<span data-ttu-id="b5fe0-162">Коллекция [страниц](page.md)</span><span class="sxs-lookup"><span data-stu-id="b5fe0-162">[Page](page.md) collection</span></span>| <span data-ttu-id="b5fe0-163">Получение коллекции страниц.</span><span class="sxs-lookup"><span data-stu-id="b5fe0-163">Get a collection of pages.</span></span>|
|[<span data-ttu-id="b5fe0-164">Список групп разделов</span><span class="sxs-lookup"><span data-stu-id="b5fe0-164">List section groups</span></span>](../api/onenote-list-sectiongroups.md) |<span data-ttu-id="b5fe0-165">Коллекция [sectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="b5fe0-165">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="b5fe0-166">Получение коллекции групп разделов.</span><span class="sxs-lookup"><span data-stu-id="b5fe0-166">Get a collection of section groups.</span></span>|
|[<span data-ttu-id="b5fe0-167">Вывод списка разделов</span><span class="sxs-lookup"><span data-stu-id="b5fe0-167">List sections</span></span>](../api/onenote-list-sections.md) |<span data-ttu-id="b5fe0-168">Коллекция [section](section.md)</span><span class="sxs-lookup"><span data-stu-id="b5fe0-168">[Section](section.md) collection</span></span>| <span data-ttu-id="b5fe0-169">Получение коллекции разделов.</span><span class="sxs-lookup"><span data-stu-id="b5fe0-169">Get a collection of sections.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onenote resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/onenote.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
