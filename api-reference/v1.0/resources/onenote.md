---
title: Тип ресурса onenote
description: Точка входа для ресурсов OneNote.
author: jewan-microsoft
localization_priority: Priority
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 8c81804c9ea93e6da9f0f9b7134f5b38aa4afd64
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961981"
---
# <a name="onenote-resource-type"></a><span data-ttu-id="0f7e8-103">Тип ресурса onenote</span><span class="sxs-lookup"><span data-stu-id="0f7e8-103">onenote resource type</span></span>

<span data-ttu-id="0f7e8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f7e8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0f7e8-105">Точка входа для ресурсов OneNote.</span><span class="sxs-lookup"><span data-stu-id="0f7e8-105">The entry point for OneNote resources.</span></span>

<span data-ttu-id="0f7e8-106">Все вызовы службы OneNote через API Microsoft Graph выполняются с помощью следующего корневого URL-адреса службы:</span><span class="sxs-lookup"><span data-stu-id="0f7e8-106">All calls to the OneNote service through the Microsoft Graph API use this service root URL:</span></span>

```http
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

<span data-ttu-id="0f7e8-107">В качестве расположений можно задавать записные книжки пользователя в Microsoft 365 или личные хранилища OneDrive, записные книжки группы (в том числе размещенные на сайте SharePoint) в Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="0f7e8-107">The location can be user notebooks on Microsoft 365 or consumer OneDrive, group notebooks or SharePoint site-hosted team notebooks on Microsoft 365.</span></span> 

<span data-ttu-id="0f7e8-108">**Записные книжки пользователей.** Чтобы получить доступ к персональным записным книжкам в OneDrive для бизнеса или личном хранилище OneDrive, воспользуйтесь одним из следующих URL-адресов:</span><span class="sxs-lookup"><span data-stu-id="0f7e8-108">**User notebooks** To access personal notebooks on consumer OneDrive or OneDrive for Business, use one of the following URLs:</span></span>

```http
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

<span data-ttu-id="0f7e8-109">**Записные книжки группы.** Чтобы получить доступ к записным книжкам группы, воспользуйтесь следующим корневым URL-адресом службы:</span><span class="sxs-lookup"><span data-stu-id="0f7e8-109">**Group notebooks** To access notebooks that are owned by a group, use the following service root URL:</span></span>

```http
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
<span data-ttu-id="0f7e8-110">**Записные книжки на сайте SharePoint.** Чтобы получить доступ к записным книжкам на сайте группы SharePoint, воспользуйтесь следующим корневым URL-адресом службы:</span><span class="sxs-lookup"><span data-stu-id="0f7e8-110">**SharePoint site notebooks** To access notebooks that are owned by a SharePoint team site, use the following service root URL:</span></span>

```http
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
## <a name="authorization"></a><span data-ttu-id="0f7e8-111">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0f7e8-111">Authorization</span></span>

<span data-ttu-id="0f7e8-112">Сведения о разрешениях, необходимых для работы с API OneNote, см. в разделе [Разрешения для заметок](/graph/permissions-reference#notes-permissions).</span><span class="sxs-lookup"><span data-stu-id="0f7e8-112">For information about the permissions required to work with OneNote APIs, see [Notes permissions](/graph/permissions-reference#notes-permissions).</span></span>


## <a name="relationships"></a><span data-ttu-id="0f7e8-113">Отношения</span><span class="sxs-lookup"><span data-stu-id="0f7e8-113">Relationships</span></span>
| <span data-ttu-id="0f7e8-114">Связь</span><span class="sxs-lookup"><span data-stu-id="0f7e8-114">Relationship</span></span> | <span data-ttu-id="0f7e8-115">Тип</span><span class="sxs-lookup"><span data-stu-id="0f7e8-115">Type</span></span>   |<span data-ttu-id="0f7e8-116">Описание</span><span class="sxs-lookup"><span data-stu-id="0f7e8-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0f7e8-117">notebooks</span><span class="sxs-lookup"><span data-stu-id="0f7e8-117">notebooks</span></span>|<span data-ttu-id="0f7e8-118">Коллекция [notebook](notebook.md)</span><span class="sxs-lookup"><span data-stu-id="0f7e8-118">[notebook](notebook.md) collection</span></span>|<span data-ttu-id="0f7e8-119">Коллекция записных книжек OneNote, принадлежащих пользователю или группе.</span><span class="sxs-lookup"><span data-stu-id="0f7e8-119">The collection of OneNote notebooks that are owned by the user or group.</span></span> <span data-ttu-id="0f7e8-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0f7e8-120">Read-only.</span></span> <span data-ttu-id="0f7e8-121">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="0f7e8-121">Nullable.</span></span>|
|<span data-ttu-id="0f7e8-122">operations</span><span class="sxs-lookup"><span data-stu-id="0f7e8-122">operations</span></span>|<span data-ttu-id="0f7e8-123">Коллекция [onenoteOperation](onenoteoperation.md)</span><span class="sxs-lookup"><span data-stu-id="0f7e8-123">[onenoteOperation](onenoteoperation.md) collection</span></span> |<span data-ttu-id="0f7e8-124">Состояние операций OneNote.</span><span class="sxs-lookup"><span data-stu-id="0f7e8-124">The status of OneNote operations.</span></span> <span data-ttu-id="0f7e8-125">Получение коллекции операций не поддерживается, но можно получить состояние длительных операций, если в отклике возвращается заголовок `Operation-Location`.</span><span class="sxs-lookup"><span data-stu-id="0f7e8-125">Getting an operations collection is not supported, but you can get the status of long-running operations if the `Operation-Location` header is returned in the response.</span></span> <span data-ttu-id="0f7e8-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0f7e8-126">Read-only.</span></span> <span data-ttu-id="0f7e8-127">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="0f7e8-127">Nullable.</span></span>|
|<span data-ttu-id="0f7e8-128">pages</span><span class="sxs-lookup"><span data-stu-id="0f7e8-128">pages</span></span>|<span data-ttu-id="0f7e8-129">Коллекция [OnenotePage](page.md)</span><span class="sxs-lookup"><span data-stu-id="0f7e8-129">[OnenotePage](page.md) collection</span></span>|<span data-ttu-id="0f7e8-130">Страницы всех записных книжек OneNote, принадлежащих пользователю или группе.</span><span class="sxs-lookup"><span data-stu-id="0f7e8-130">The pages in all OneNote notebooks that are owned by the user or group.</span></span>  <span data-ttu-id="0f7e8-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0f7e8-131">Read-only.</span></span> <span data-ttu-id="0f7e8-132">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="0f7e8-132">Nullable.</span></span>|
|<span data-ttu-id="0f7e8-133">resources</span><span class="sxs-lookup"><span data-stu-id="0f7e8-133">resources</span></span>|<span data-ttu-id="0f7e8-134">Коллекция [OnenoteResource](resource.md)</span><span class="sxs-lookup"><span data-stu-id="0f7e8-134">[OnenoteResource](resource.md) collection</span></span> |<span data-ttu-id="0f7e8-135">Изображения и другие файловые ресурсы на страницах OneNote.</span><span class="sxs-lookup"><span data-stu-id="0f7e8-135">The image and other file resources in OneNote pages.</span></span> <span data-ttu-id="0f7e8-136">Получение коллекции ресурсов не поддерживается, но можно [получить двоичное содержимое определенного ресурса](resource.md).</span><span class="sxs-lookup"><span data-stu-id="0f7e8-136">Getting a resources collection is not supported, but you can [get the binary content of a specific resource](resource.md).</span></span> <span data-ttu-id="0f7e8-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0f7e8-137">Read-only.</span></span> <span data-ttu-id="0f7e8-138">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="0f7e8-138">Nullable.</span></span>|
|<span data-ttu-id="0f7e8-139">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="0f7e8-139">sectionGroups</span></span>|<span data-ttu-id="0f7e8-140">Коллекция [sectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="0f7e8-140">[sectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="0f7e8-141">Группы разделов во всех записных книжках OneNote, принадлежащих пользователю или группе.</span><span class="sxs-lookup"><span data-stu-id="0f7e8-141">The section groups in all OneNote notebooks that are owned by the user or group.</span></span>  <span data-ttu-id="0f7e8-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0f7e8-142">Read-only.</span></span> <span data-ttu-id="0f7e8-143">Допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="0f7e8-143">Nullable.</span></span>|
|<span data-ttu-id="0f7e8-144">sections</span><span class="sxs-lookup"><span data-stu-id="0f7e8-144">sections</span></span>|<span data-ttu-id="0f7e8-145">Коллекция [OnenoteSection](section.md)</span><span class="sxs-lookup"><span data-stu-id="0f7e8-145">[OnenoteSection](section.md) collection</span></span>|<span data-ttu-id="0f7e8-146">Разделы во всех записных книжках OneNote, принадлежащих пользователю или группе.</span><span class="sxs-lookup"><span data-stu-id="0f7e8-146">The sections in all OneNote notebooks that are owned by the user or group.</span></span>  <span data-ttu-id="0f7e8-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0f7e8-147">Read-only.</span></span> <span data-ttu-id="0f7e8-148">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="0f7e8-148">Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="0f7e8-149">Методы</span><span class="sxs-lookup"><span data-stu-id="0f7e8-149">Methods</span></span>

| <span data-ttu-id="0f7e8-150">Метод</span><span class="sxs-lookup"><span data-stu-id="0f7e8-150">Method</span></span>           | <span data-ttu-id="0f7e8-151">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0f7e8-151">Return Type</span></span>    |<span data-ttu-id="0f7e8-152">Описание</span><span class="sxs-lookup"><span data-stu-id="0f7e8-152">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0f7e8-153">Создание записной книжки</span><span class="sxs-lookup"><span data-stu-id="0f7e8-153">Create notebook</span></span>](../api/onenote-post-notebooks.md) |[<span data-ttu-id="0f7e8-154">Notebook</span><span class="sxs-lookup"><span data-stu-id="0f7e8-154">Notebook</span></span>](notebook.md)| <span data-ttu-id="0f7e8-155">Создание записной книжки путем публикации в коллекции записных книжек.</span><span class="sxs-lookup"><span data-stu-id="0f7e8-155">Create a notebook by posting to the notebooks collection.</span></span>|
|[<span data-ttu-id="0f7e8-156">Перечисление записных книжек</span><span class="sxs-lookup"><span data-stu-id="0f7e8-156">List notebooks</span></span>](../api/onenote-list-notebooks.md) |<span data-ttu-id="0f7e8-157">Коллекция [Notebook](notebook.md)</span><span class="sxs-lookup"><span data-stu-id="0f7e8-157">[Notebook](notebook.md) collection</span></span>| <span data-ttu-id="0f7e8-158">Получение коллекции записных книжек.</span><span class="sxs-lookup"><span data-stu-id="0f7e8-158">Get a collection of notebooks.</span></span>|
|[<span data-ttu-id="0f7e8-159">Создание страницы</span><span class="sxs-lookup"><span data-stu-id="0f7e8-159">Create page</span></span>](../api/onenote-post-pages.md) |[<span data-ttu-id="0f7e8-160">Page</span><span class="sxs-lookup"><span data-stu-id="0f7e8-160">Page</span></span>](page.md)| <span data-ttu-id="0f7e8-161">Создание страницы путем публикации в коллекции страниц.</span><span class="sxs-lookup"><span data-stu-id="0f7e8-161">Create a page by posting to the pages collection.</span></span>|
|[<span data-ttu-id="0f7e8-162">Перечисление страниц</span><span class="sxs-lookup"><span data-stu-id="0f7e8-162">List pages</span></span>](../api/onenote-list-pages.md) |<span data-ttu-id="0f7e8-163">Коллекция [Page](page.md)</span><span class="sxs-lookup"><span data-stu-id="0f7e8-163">[Page](page.md) collection</span></span>| <span data-ttu-id="0f7e8-164">Получение коллекции страниц.</span><span class="sxs-lookup"><span data-stu-id="0f7e8-164">Get a collection of pages.</span></span>|
|[<span data-ttu-id="0f7e8-165">Перечисление групп разделов</span><span class="sxs-lookup"><span data-stu-id="0f7e8-165">List section groups</span></span>](../api/onenote-list-sectiongroups.md) |<span data-ttu-id="0f7e8-166">Коллекция [SectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="0f7e8-166">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="0f7e8-167">Получение коллекции групп разделов.</span><span class="sxs-lookup"><span data-stu-id="0f7e8-167">Get a collection of section groups.</span></span>|
|[<span data-ttu-id="0f7e8-168">Перечисление разделов</span><span class="sxs-lookup"><span data-stu-id="0f7e8-168">List sections</span></span>](../api/onenote-list-sections.md) |<span data-ttu-id="0f7e8-169">Коллекция [OnenoteSection](section.md)</span><span class="sxs-lookup"><span data-stu-id="0f7e8-169">[OnenoteSection](section.md) collection</span></span>| <span data-ttu-id="0f7e8-170">Получение коллекции разделов.</span><span class="sxs-lookup"><span data-stu-id="0f7e8-170">Get a collection of sections.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="0f7e8-171">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0f7e8-171">JSON Representation</span></span>
<span data-ttu-id="0f7e8-172">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0f7e8-172">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.onenote"
}-->
```json
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
<!-- {
  "type": "#page.annotation",
  "description": "onenote resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

