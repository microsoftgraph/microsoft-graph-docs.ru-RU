---
title: Тип ресурса onenote
description: Точка входа для ресурсов OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 44dfe7b33632bb6691802e46b66f54015b6aa6ae
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341493"
---
# <a name="onenote-resource-type"></a><span data-ttu-id="ab4cb-103">Тип ресурса onenote</span><span class="sxs-lookup"><span data-stu-id="ab4cb-103">onenote resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab4cb-104">Точка входа для ресурсов OneNote.</span><span class="sxs-lookup"><span data-stu-id="ab4cb-104">The entry point for OneNote resources.</span></span>

<span data-ttu-id="ab4cb-105">Все вызовы службы OneNote через API Microsoft Graph выполняются с помощью следующего корневого URL-адреса службы:</span><span class="sxs-lookup"><span data-stu-id="ab4cb-105">All calls to the OneNote service through the Microsoft Graph API use this service root URL:</span></span>

```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

<span data-ttu-id="ab4cb-106">Местоположение может представлять собой записные книжки для пользователей в Office 365 или OneDrive для пользователей, групповых записных книжек или размещенных на сайте SharePoint записных книжек группы в Office 365.</span><span class="sxs-lookup"><span data-stu-id="ab4cb-106">The location can be user notebooks on Office 365 or consumer OneDrive, group notebooks, or SharePoint site-hosted team notebooks on Office 365.</span></span> 

<span data-ttu-id="ab4cb-107">**Записные книжки пользователей.** Чтобы получить доступ к персональным записным книжкам в OneDrive для бизнеса или личном хранилище OneDrive, воспользуйтесь одним из следующих URL-адресов:</span><span class="sxs-lookup"><span data-stu-id="ab4cb-107">**User notebooks** To access personal notebooks on consumer OneDrive or OneDrive for Business, use one of the following URLs:</span></span>

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

<span data-ttu-id="ab4cb-108">**Записные книжки группы.** Чтобы получить доступ к записным книжкам группы, воспользуйтесь следующим корневым URL-адресом службы:</span><span class="sxs-lookup"><span data-stu-id="ab4cb-108">**Group notebooks** To access notebooks that are owned by a group, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
<span data-ttu-id="ab4cb-109">**Записные книжки на сайте SharePoint.** Чтобы получить доступ к записным книжкам на сайте группы SharePoint, воспользуйтесь следующим корневым URL-адресом службы:</span><span class="sxs-lookup"><span data-stu-id="ab4cb-109">**SharePoint site notebooks** To access notebooks that are owned by a SharePoint team site, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

## <a name="authorization"></a><span data-ttu-id="ab4cb-110">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ab4cb-110">Authorization</span></span>

<span data-ttu-id="ab4cb-111">Сведения о разрешениях, необходимых для работы с API OneNote, см. в разделе [Разрешения для заметок](/graph/permissions-reference#notes-permissions).</span><span class="sxs-lookup"><span data-stu-id="ab4cb-111">For information about the permissions required to work with OneNote APIs, see [Notes permissions](/graph/permissions-reference#notes-permissions).</span></span>

## <a name="relationships"></a><span data-ttu-id="ab4cb-112">Отношения</span><span class="sxs-lookup"><span data-stu-id="ab4cb-112">Relationships</span></span>
| <span data-ttu-id="ab4cb-113">Отношение</span><span class="sxs-lookup"><span data-stu-id="ab4cb-113">Relationship</span></span> | <span data-ttu-id="ab4cb-114">Тип</span><span class="sxs-lookup"><span data-stu-id="ab4cb-114">Type</span></span>   |<span data-ttu-id="ab4cb-115">Описание</span><span class="sxs-lookup"><span data-stu-id="ab4cb-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ab4cb-116">notebooks</span><span class="sxs-lookup"><span data-stu-id="ab4cb-116">notebooks</span></span>|<span data-ttu-id="ab4cb-117">Коллекция [notebook](notebook.md)</span><span class="sxs-lookup"><span data-stu-id="ab4cb-117">[notebook](notebook.md) collection</span></span>|<span data-ttu-id="ab4cb-118">Коллекция записных книжек OneNote, принадлежащих пользователю или группе.</span><span class="sxs-lookup"><span data-stu-id="ab4cb-118">The collection of OneNote notebooks that are owned by the user or group.</span></span> <span data-ttu-id="ab4cb-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab4cb-119">Read-only.</span></span> <span data-ttu-id="ab4cb-120">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="ab4cb-120">Nullable.</span></span>|
|<span data-ttu-id="ab4cb-121">operations</span><span class="sxs-lookup"><span data-stu-id="ab4cb-121">operations</span></span>|<span data-ttu-id="ab4cb-122">Коллекция [onenoteOperation](onenoteoperation.md)</span><span class="sxs-lookup"><span data-stu-id="ab4cb-122">[onenoteOperation](onenoteoperation.md) collection</span></span> |<span data-ttu-id="ab4cb-123">Состояние операций OneNote.</span><span class="sxs-lookup"><span data-stu-id="ab4cb-123">The status of OneNote operations.</span></span> <span data-ttu-id="ab4cb-124">Получение коллекции операций не поддерживается, но можно получить состояние длительных операций, если в отклике возвращается заголовок `Operation-Location`.</span><span class="sxs-lookup"><span data-stu-id="ab4cb-124">Getting an operations collection is not supported, but you can get the status of long-running operations if the `Operation-Location` header is returned in the response.</span></span> <span data-ttu-id="ab4cb-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab4cb-125">Read-only.</span></span> <span data-ttu-id="ab4cb-126">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="ab4cb-126">Nullable.</span></span>|
|<span data-ttu-id="ab4cb-127">pages</span><span class="sxs-lookup"><span data-stu-id="ab4cb-127">pages</span></span>|<span data-ttu-id="ab4cb-128">Коллекция [оненотепаже](onenotepage.md)</span><span class="sxs-lookup"><span data-stu-id="ab4cb-128">[onenotePage](onenotepage.md) collection</span></span>|<span data-ttu-id="ab4cb-129">Страницы всех записных книжек OneNote, принадлежащих пользователю или группе.</span><span class="sxs-lookup"><span data-stu-id="ab4cb-129">The pages in all OneNote notebooks that are owned by the user or group.</span></span>  <span data-ttu-id="ab4cb-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab4cb-130">Read-only.</span></span> <span data-ttu-id="ab4cb-131">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="ab4cb-131">Nullable.</span></span>|
|<span data-ttu-id="ab4cb-132">resources</span><span class="sxs-lookup"><span data-stu-id="ab4cb-132">resources</span></span>|<span data-ttu-id="ab4cb-133">Коллекция [оненотересаурце](onenoteresource.md)</span><span class="sxs-lookup"><span data-stu-id="ab4cb-133">[onenoteResource](onenoteresource.md) collection</span></span> |<span data-ttu-id="ab4cb-134">Изображения и другие файловые ресурсы на страницах OneNote.</span><span class="sxs-lookup"><span data-stu-id="ab4cb-134">The image and other file resources in OneNote pages.</span></span> <span data-ttu-id="ab4cb-135">Получение коллекции ресурсов не поддерживается, но можно [получить двоичное содержимое определенного ресурса](onenoteresource.md).</span><span class="sxs-lookup"><span data-stu-id="ab4cb-135">Getting a resources collection is not supported, but you can [get the binary content of a specific resource](onenoteresource.md).</span></span> <span data-ttu-id="ab4cb-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab4cb-136">Read-only.</span></span> <span data-ttu-id="ab4cb-137">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="ab4cb-137">Nullable.</span></span>|
|<span data-ttu-id="ab4cb-138">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="ab4cb-138">sectionGroups</span></span>|<span data-ttu-id="ab4cb-139">Коллекция [sectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="ab4cb-139">[sectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="ab4cb-140">Группы разделов во всех записных книжках OneNote, принадлежащих пользователю или группе.</span><span class="sxs-lookup"><span data-stu-id="ab4cb-140">The section groups in all OneNote notebooks that are owned by the user or group.</span></span>  <span data-ttu-id="ab4cb-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab4cb-141">Read-only.</span></span> <span data-ttu-id="ab4cb-142">Допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="ab4cb-142">Nullable.</span></span>|
|<span data-ttu-id="ab4cb-143">sections</span><span class="sxs-lookup"><span data-stu-id="ab4cb-143">sections</span></span>|<span data-ttu-id="ab4cb-144">Коллекция [оненотесектион](onenotesection.md)</span><span class="sxs-lookup"><span data-stu-id="ab4cb-144">[onenoteSection](onenotesection.md) collection</span></span>|<span data-ttu-id="ab4cb-145">Разделы во всех записных книжках OneNote, принадлежащих пользователю или группе.</span><span class="sxs-lookup"><span data-stu-id="ab4cb-145">The sections in all OneNote notebooks that are owned by the user or group.</span></span>  <span data-ttu-id="ab4cb-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab4cb-146">Read-only.</span></span> <span data-ttu-id="ab4cb-147">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="ab4cb-147">Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="ab4cb-148">Методы</span><span class="sxs-lookup"><span data-stu-id="ab4cb-148">Methods</span></span>

| <span data-ttu-id="ab4cb-149">Метод</span><span class="sxs-lookup"><span data-stu-id="ab4cb-149">Method</span></span>           | <span data-ttu-id="ab4cb-150">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ab4cb-150">Return Type</span></span>    |<span data-ttu-id="ab4cb-151">Описание</span><span class="sxs-lookup"><span data-stu-id="ab4cb-151">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ab4cb-152">Создание записной книжки</span><span class="sxs-lookup"><span data-stu-id="ab4cb-152">Create notebook</span></span>](../api/onenote-post-notebooks.md) |[<span data-ttu-id="ab4cb-153">записной книжки</span><span class="sxs-lookup"><span data-stu-id="ab4cb-153">notebook</span></span>](notebook.md)| <span data-ttu-id="ab4cb-154">Создание записной книжки путем публикации в коллекции записных книжек.</span><span class="sxs-lookup"><span data-stu-id="ab4cb-154">Create a notebook by posting to the notebooks collection.</span></span>|
|[<span data-ttu-id="ab4cb-155">Перечисление записных книжек</span><span class="sxs-lookup"><span data-stu-id="ab4cb-155">List notebooks</span></span>](../api/onenote-list-notebooks.md) |<span data-ttu-id="ab4cb-156">Коллекция [notebook](notebook.md)</span><span class="sxs-lookup"><span data-stu-id="ab4cb-156">[notebook](notebook.md) collection</span></span>| <span data-ttu-id="ab4cb-157">Получение коллекции записных книжек.</span><span class="sxs-lookup"><span data-stu-id="ab4cb-157">Get a collection of notebooks.</span></span>|
|[<span data-ttu-id="ab4cb-158">Создание страницы</span><span class="sxs-lookup"><span data-stu-id="ab4cb-158">Create page</span></span>](../api/onenote-post-pages.md) |[<span data-ttu-id="ab4cb-159">Оненотепаже</span><span class="sxs-lookup"><span data-stu-id="ab4cb-159">onenotePage</span></span>](onenotepage.md) | <span data-ttu-id="ab4cb-160">Создание страницы путем публикации в коллекции страниц.</span><span class="sxs-lookup"><span data-stu-id="ab4cb-160">Create a page by posting to the pages collection.</span></span>|
|[<span data-ttu-id="ab4cb-161">Перечисление страниц</span><span class="sxs-lookup"><span data-stu-id="ab4cb-161">List pages</span></span>](../api/onenote-list-pages.md) |<span data-ttu-id="ab4cb-162">Коллекция [оненотепаже](onenotepage.md)</span><span class="sxs-lookup"><span data-stu-id="ab4cb-162">[onenotePage](onenotepage.md)  collection</span></span>| <span data-ttu-id="ab4cb-163">Получение коллекции страниц.</span><span class="sxs-lookup"><span data-stu-id="ab4cb-163">Get a collection of pages.</span></span>|
|[<span data-ttu-id="ab4cb-164">Перечисление групп разделов</span><span class="sxs-lookup"><span data-stu-id="ab4cb-164">List section groups</span></span>](../api/onenote-list-sectiongroups.md) |<span data-ttu-id="ab4cb-165">Коллекция [sectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="ab4cb-165">[sectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="ab4cb-166">Получение коллекции групп разделов.</span><span class="sxs-lookup"><span data-stu-id="ab4cb-166">Get a collection of section groups.</span></span>|
|[<span data-ttu-id="ab4cb-167">Перечисление разделов</span><span class="sxs-lookup"><span data-stu-id="ab4cb-167">List sections</span></span>](../api/onenote-list-sections.md) |<span data-ttu-id="ab4cb-168">Коллекция [оненотесектион](onenotesection.md)</span><span class="sxs-lookup"><span data-stu-id="ab4cb-168">[onenoteSection](onenotesection.md) collection</span></span>| <span data-ttu-id="ab4cb-169">Получение коллекции разделов.</span><span class="sxs-lookup"><span data-stu-id="ab4cb-169">Get a collection of sections.</span></span>|
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.onenote"
}-->
``` json
{
  "notebooks": [{ "@odata.type": "microsoft.graph.notebook" }],
  "operations": [{ "@odata.type": "microsoft.graph.onenoteOperation" }],
  "pages": [{ "@odata.type": "microsoft.graph.onenotePage" }],
  "resources": [ { "@odata.type": "microsoft.graph.onenoteResource" } ],
  "sectionGroups": [ { "@odata.type": "microsoft.graph.sectionGroup" } ],
  "sections": [ { "@odata.type": "microsoft.graph.onenoteSection" } ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onenote resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
