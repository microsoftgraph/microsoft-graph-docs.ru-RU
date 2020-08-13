---
title: Тип ресурса onenote
description: Точка входа для ресурсов OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: f542c58d6b824b678afbe493d03ae760b3be428f
ms.sourcegitcommit: 7dcd32f9e959bea2dfd81d9e0d4092f93da43cb7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2020
ms.locfileid: "46657926"
---
# <a name="onenote-resource-type"></a><span data-ttu-id="6e02f-103">Тип ресурса onenote</span><span class="sxs-lookup"><span data-stu-id="6e02f-103">onenote resource type</span></span>

<span data-ttu-id="6e02f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e02f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e02f-105">Точка входа для ресурсов OneNote.</span><span class="sxs-lookup"><span data-stu-id="6e02f-105">The entry point for OneNote resources.</span></span>

<span data-ttu-id="6e02f-106">Все вызовы службы OneNote через API Microsoft Graph выполняются с помощью следующего корневого URL-адреса службы:</span><span class="sxs-lookup"><span data-stu-id="6e02f-106">All calls to the OneNote service through the Microsoft Graph API use this service root URL:</span></span>

```http
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

<span data-ttu-id="6e02f-107">В качестве расположений можно задавать записные книжки пользователя в Microsoft 365 или личные хранилища OneDrive, записные книжки группы (в том числе размещенные на сайте SharePoint) в Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="6e02f-107">The location can be user notebooks on Microsoft 365 or consumer OneDrive, group notebooks, or SharePoint site-hosted team notebooks on Microsoft 365.</span></span> 

<span data-ttu-id="6e02f-108">**Записные книжки пользователей.** Чтобы получить доступ к персональным записным книжкам в OneDrive для бизнеса или личном хранилище OneDrive, воспользуйтесь одним из следующих URL-адресов:</span><span class="sxs-lookup"><span data-stu-id="6e02f-108">**User notebooks** To access personal notebooks on consumer OneDrive or OneDrive for Business, use one of the following URLs:</span></span>

```http
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

<span data-ttu-id="6e02f-109">**Записные книжки группы.** Чтобы получить доступ к записным книжкам группы, воспользуйтесь следующим корневым URL-адресом службы:</span><span class="sxs-lookup"><span data-stu-id="6e02f-109">**Group notebooks** To access notebooks that are owned by a group, use the following service root URL:</span></span>

```http
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
<span data-ttu-id="6e02f-110">**Записные книжки на сайте SharePoint.** Чтобы получить доступ к записным книжкам на сайте группы SharePoint, воспользуйтесь следующим корневым URL-адресом службы:</span><span class="sxs-lookup"><span data-stu-id="6e02f-110">**SharePoint site notebooks** To access notebooks that are owned by a SharePoint team site, use the following service root URL:</span></span>

```http
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

## <a name="authorization"></a><span data-ttu-id="6e02f-111">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6e02f-111">Authorization</span></span>

<span data-ttu-id="6e02f-112">Сведения о разрешениях, необходимых для работы с API OneNote, см. в разделе [Разрешения для заметок](/graph/permissions-reference#notes-permissions).</span><span class="sxs-lookup"><span data-stu-id="6e02f-112">For information about the permissions required to work with OneNote APIs, see [Notes permissions](/graph/permissions-reference#notes-permissions).</span></span>

## <a name="relationships"></a><span data-ttu-id="6e02f-113">Отношения</span><span class="sxs-lookup"><span data-stu-id="6e02f-113">Relationships</span></span>
| <span data-ttu-id="6e02f-114">Связь</span><span class="sxs-lookup"><span data-stu-id="6e02f-114">Relationship</span></span> | <span data-ttu-id="6e02f-115">Тип</span><span class="sxs-lookup"><span data-stu-id="6e02f-115">Type</span></span>   |<span data-ttu-id="6e02f-116">Описание</span><span class="sxs-lookup"><span data-stu-id="6e02f-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6e02f-117">notebooks</span><span class="sxs-lookup"><span data-stu-id="6e02f-117">notebooks</span></span>|<span data-ttu-id="6e02f-118">Коллекция объектов [notebook](notebook.md)</span><span class="sxs-lookup"><span data-stu-id="6e02f-118">[notebook](notebook.md) collection</span></span>|<span data-ttu-id="6e02f-119">Коллекция записных книжек OneNote, принадлежащих пользователю или группе.</span><span class="sxs-lookup"><span data-stu-id="6e02f-119">The collection of OneNote notebooks that are owned by the user or group.</span></span> <span data-ttu-id="6e02f-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6e02f-120">Read-only.</span></span> <span data-ttu-id="6e02f-121">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="6e02f-121">Nullable.</span></span>|
|<span data-ttu-id="6e02f-122">operations</span><span class="sxs-lookup"><span data-stu-id="6e02f-122">operations</span></span>|<span data-ttu-id="6e02f-123">Коллекция [onenoteOperation](onenoteoperation.md)</span><span class="sxs-lookup"><span data-stu-id="6e02f-123">[onenoteOperation](onenoteoperation.md) collection</span></span> |<span data-ttu-id="6e02f-124">Состояние операций OneNote.</span><span class="sxs-lookup"><span data-stu-id="6e02f-124">The status of OneNote operations.</span></span> <span data-ttu-id="6e02f-125">Получение коллекции операций не поддерживается, но можно получить состояние длительных операций, если в отклике возвращается заголовок `Operation-Location`.</span><span class="sxs-lookup"><span data-stu-id="6e02f-125">Getting an operations collection is not supported, but you can get the status of long-running operations if the `Operation-Location` header is returned in the response.</span></span> <span data-ttu-id="6e02f-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6e02f-126">Read-only.</span></span> <span data-ttu-id="6e02f-127">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="6e02f-127">Nullable.</span></span>|
|<span data-ttu-id="6e02f-128">pages</span><span class="sxs-lookup"><span data-stu-id="6e02f-128">pages</span></span>|<span data-ttu-id="6e02f-129">Коллекция [оненотепаже](onenotepage.md)</span><span class="sxs-lookup"><span data-stu-id="6e02f-129">[onenotePage](onenotepage.md) collection</span></span>|<span data-ttu-id="6e02f-130">Страницы всех записных книжек OneNote, принадлежащих пользователю или группе.</span><span class="sxs-lookup"><span data-stu-id="6e02f-130">The pages in all OneNote notebooks that are owned by the user or group.</span></span>  <span data-ttu-id="6e02f-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6e02f-131">Read-only.</span></span> <span data-ttu-id="6e02f-132">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="6e02f-132">Nullable.</span></span>|
|<span data-ttu-id="6e02f-133">resources</span><span class="sxs-lookup"><span data-stu-id="6e02f-133">resources</span></span>|<span data-ttu-id="6e02f-134">Коллекция [оненотересаурце](onenoteresource.md)</span><span class="sxs-lookup"><span data-stu-id="6e02f-134">[onenoteResource](onenoteresource.md) collection</span></span> |<span data-ttu-id="6e02f-135">Изображения и другие файловые ресурсы на страницах OneNote.</span><span class="sxs-lookup"><span data-stu-id="6e02f-135">The image and other file resources in OneNote pages.</span></span> <span data-ttu-id="6e02f-136">Получение коллекции ресурсов не поддерживается, но можно [получить двоичное содержимое определенного ресурса](onenoteresource.md).</span><span class="sxs-lookup"><span data-stu-id="6e02f-136">Getting a resources collection is not supported, but you can [get the binary content of a specific resource](onenoteresource.md).</span></span> <span data-ttu-id="6e02f-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6e02f-137">Read-only.</span></span> <span data-ttu-id="6e02f-138">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="6e02f-138">Nullable.</span></span>|
|<span data-ttu-id="6e02f-139">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="6e02f-139">sectionGroups</span></span>|<span data-ttu-id="6e02f-140">Коллекция [sectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="6e02f-140">[sectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="6e02f-141">Группы разделов во всех записных книжках OneNote, принадлежащих пользователю или группе.</span><span class="sxs-lookup"><span data-stu-id="6e02f-141">The section groups in all OneNote notebooks that are owned by the user or group.</span></span>  <span data-ttu-id="6e02f-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6e02f-142">Read-only.</span></span> <span data-ttu-id="6e02f-143">Допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="6e02f-143">Nullable.</span></span>|
|<span data-ttu-id="6e02f-144">sections</span><span class="sxs-lookup"><span data-stu-id="6e02f-144">sections</span></span>|<span data-ttu-id="6e02f-145">Коллекция [оненотесектион](onenotesection.md)</span><span class="sxs-lookup"><span data-stu-id="6e02f-145">[onenoteSection](onenotesection.md) collection</span></span>|<span data-ttu-id="6e02f-146">Разделы во всех записных книжках OneNote, принадлежащих пользователю или группе.</span><span class="sxs-lookup"><span data-stu-id="6e02f-146">The sections in all OneNote notebooks that are owned by the user or group.</span></span>  <span data-ttu-id="6e02f-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6e02f-147">Read-only.</span></span> <span data-ttu-id="6e02f-148">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="6e02f-148">Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="6e02f-149">Методы</span><span class="sxs-lookup"><span data-stu-id="6e02f-149">Methods</span></span>

| <span data-ttu-id="6e02f-150">Метод</span><span class="sxs-lookup"><span data-stu-id="6e02f-150">Method</span></span>           | <span data-ttu-id="6e02f-151">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6e02f-151">Return Type</span></span>    |<span data-ttu-id="6e02f-152">Описание</span><span class="sxs-lookup"><span data-stu-id="6e02f-152">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6e02f-153">Создание записной книжки</span><span class="sxs-lookup"><span data-stu-id="6e02f-153">Create notebook</span></span>](../api/onenote-post-notebooks.md) |[<span data-ttu-id="6e02f-154">notebook</span><span class="sxs-lookup"><span data-stu-id="6e02f-154">notebook</span></span>](notebook.md)| <span data-ttu-id="6e02f-155">Создание записной книжки путем публикации в коллекции записных книжек.</span><span class="sxs-lookup"><span data-stu-id="6e02f-155">Create a notebook by posting to the notebooks collection.</span></span>|
|[<span data-ttu-id="6e02f-156">Перечисление записных книжек</span><span class="sxs-lookup"><span data-stu-id="6e02f-156">List notebooks</span></span>](../api/onenote-list-notebooks.md) |<span data-ttu-id="6e02f-157">Коллекция объектов [notebook](notebook.md)</span><span class="sxs-lookup"><span data-stu-id="6e02f-157">[notebook](notebook.md) collection</span></span>| <span data-ttu-id="6e02f-158">Получение коллекции записных книжек.</span><span class="sxs-lookup"><span data-stu-id="6e02f-158">Get a collection of notebooks.</span></span>|
|[<span data-ttu-id="6e02f-159">Создание страницы</span><span class="sxs-lookup"><span data-stu-id="6e02f-159">Create page</span></span>](../api/onenote-post-pages.md) |[<span data-ttu-id="6e02f-160">оненотепаже</span><span class="sxs-lookup"><span data-stu-id="6e02f-160">onenotePage</span></span>](onenotepage.md) | <span data-ttu-id="6e02f-161">Создание страницы путем публикации в коллекции страниц.</span><span class="sxs-lookup"><span data-stu-id="6e02f-161">Create a page by posting to the pages collection.</span></span>|
|[<span data-ttu-id="6e02f-162">Перечисление страниц</span><span class="sxs-lookup"><span data-stu-id="6e02f-162">List pages</span></span>](../api/onenote-list-pages.md) |<span data-ttu-id="6e02f-163">Коллекция [оненотепаже](onenotepage.md)</span><span class="sxs-lookup"><span data-stu-id="6e02f-163">[onenotePage](onenotepage.md)  collection</span></span>| <span data-ttu-id="6e02f-164">Получение коллекции страниц.</span><span class="sxs-lookup"><span data-stu-id="6e02f-164">Get a collection of pages.</span></span>|
|[<span data-ttu-id="6e02f-165">Перечисление групп разделов</span><span class="sxs-lookup"><span data-stu-id="6e02f-165">List section groups</span></span>](../api/onenote-list-sectiongroups.md) |<span data-ttu-id="6e02f-166">Коллекция [sectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="6e02f-166">[sectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="6e02f-167">Получение коллекции групп разделов.</span><span class="sxs-lookup"><span data-stu-id="6e02f-167">Get a collection of section groups.</span></span>|
|[<span data-ttu-id="6e02f-168">Перечисление разделов</span><span class="sxs-lookup"><span data-stu-id="6e02f-168">List sections</span></span>](../api/onenote-list-sections.md) |<span data-ttu-id="6e02f-169">Коллекция [оненотесектион](onenotesection.md)</span><span class="sxs-lookup"><span data-stu-id="6e02f-169">[onenoteSection](onenotesection.md) collection</span></span>| <span data-ttu-id="6e02f-170">Получение коллекции разделов.</span><span class="sxs-lookup"><span data-stu-id="6e02f-170">Get a collection of sections.</span></span>|
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
