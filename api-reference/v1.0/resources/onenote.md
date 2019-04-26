---
title: Тип ресурса onenote
description: Точка входа для ресурсов OneNote.
author: jewan-microsoft
localization_priority: Priority
ms.prod: onenote
ms.openlocfilehash: 8240336bfcb9e45e33172c2c1551b71a65c315e0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462804"
---
# <a name="onenote-resource-type"></a><span data-ttu-id="c4425-103">Тип ресурса onenote</span><span class="sxs-lookup"><span data-stu-id="c4425-103">onenote resource type</span></span>

<span data-ttu-id="c4425-104">Точка входа для ресурсов OneNote.</span><span class="sxs-lookup"><span data-stu-id="c4425-104">The entry point for OneNote resources.</span></span>

<span data-ttu-id="c4425-105">Все вызовы службы OneNote через API Microsoft Graph выполняются с помощью следующего корневого URL-адреса службы:</span><span class="sxs-lookup"><span data-stu-id="c4425-105">All calls to the OneNote service through the Microsoft Graph API use this service root URL:</span></span>

```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

<span data-ttu-id="c4425-106">В качестве расположений можно задавать записные книжки пользователя в Office 365 или личные хранилища OneDrive, записные книжки группы (в том числе размещенные на сайте SharePoint) в Office 365.</span><span class="sxs-lookup"><span data-stu-id="c4425-106">The location can be user notebooks on Office 365 or consumer OneDrive, group notebooks or SharePoint site-hosted team notebooks on Office 365.</span></span> 

<span data-ttu-id="c4425-107">**Записные книжки пользователей.** Чтобы получить доступ к персональным записным книжкам в OneDrive для бизнеса или личном хранилище OneDrive, воспользуйтесь одним из следующих URL-адресов:</span><span class="sxs-lookup"><span data-stu-id="c4425-107">**User notebooks** To access personal notebooks on consumer OneDrive or OneDrive for Business, use one of the following URLs:</span></span>

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

<span data-ttu-id="c4425-108">**Записные книжки группы.** Чтобы получить доступ к записным книжкам группы, воспользуйтесь следующим корневым URL-адресом службы:</span><span class="sxs-lookup"><span data-stu-id="c4425-108">**Group notebooks** To access notebooks that are owned by a group, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
<span data-ttu-id="c4425-109">**Записные книжки на сайте SharePoint.** Чтобы получить доступ к записным книжкам на сайте группы SharePoint, воспользуйтесь следующим корневым URL-адресом службы:</span><span class="sxs-lookup"><span data-stu-id="c4425-109">**SharePoint site notebooks** To access notebooks that are owned by a SharePoint team site, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
## <a name="authorization"></a><span data-ttu-id="c4425-110">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c4425-110">Authorization</span></span>

<span data-ttu-id="c4425-111">Сведения о разрешениях, необходимых для работы с API OneNote, см. в разделе [Разрешения для заметок](/graph/permissions-reference#notes-permissions).</span><span class="sxs-lookup"><span data-stu-id="c4425-111">For information about the permissions required to work with OneNote APIs, see [Notes permissions](/graph/permissions-reference#notes-permissions).</span></span>


## <a name="relationships"></a><span data-ttu-id="c4425-112">Отношения</span><span class="sxs-lookup"><span data-stu-id="c4425-112">Relationships</span></span>
| <span data-ttu-id="c4425-113">Отношение</span><span class="sxs-lookup"><span data-stu-id="c4425-113">Relationship</span></span> | <span data-ttu-id="c4425-114">Тип</span><span class="sxs-lookup"><span data-stu-id="c4425-114">Type</span></span>   |<span data-ttu-id="c4425-115">Описание</span><span class="sxs-lookup"><span data-stu-id="c4425-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c4425-116">notebooks</span><span class="sxs-lookup"><span data-stu-id="c4425-116">notebooks</span></span>|<span data-ttu-id="c4425-117">Коллекция [Notebook](notebook.md)</span><span class="sxs-lookup"><span data-stu-id="c4425-117">Notebook collection</span></span>|<span data-ttu-id="c4425-118">Коллекция записных книжек OneNote, принадлежащих пользователю или группе.</span><span class="sxs-lookup"><span data-stu-id="c4425-118">The collection of OneNote notebooks that are owned by the user or group.</span></span> <span data-ttu-id="c4425-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c4425-119">Read-only.</span></span> <span data-ttu-id="c4425-120">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c4425-120">Nullable.</span></span>|
|<span data-ttu-id="c4425-121">operations</span><span class="sxs-lookup"><span data-stu-id="c4425-121">operations</span></span>|<span data-ttu-id="c4425-122">Коллекция [OnenoteOperation](onenoteoperation.md)</span><span class="sxs-lookup"><span data-stu-id="c4425-122">[OnenoteOperation](onenoteoperation.md) collection</span></span> |<span data-ttu-id="c4425-123">Состояние операций OneNote.</span><span class="sxs-lookup"><span data-stu-id="c4425-123">The status of OneNote operations.</span></span> <span data-ttu-id="c4425-124">Получение коллекции операций не поддерживается, но можно получить состояние длительных операций, если в отклике возвращается заголовок `Operation-Location`.</span><span class="sxs-lookup"><span data-stu-id="c4425-124">Getting an operations collection is not supported, but you can get the status of long-running operations if the `Operation-Location` header is returned in the response.</span></span> <span data-ttu-id="c4425-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c4425-125">Read-only.</span></span> <span data-ttu-id="c4425-126">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c4425-126">Nullable.</span></span>|
|<span data-ttu-id="c4425-127">pages</span><span class="sxs-lookup"><span data-stu-id="c4425-127">pages</span></span>|<span data-ttu-id="c4425-128">Коллекция [OnenotePage](page.md)</span><span class="sxs-lookup"><span data-stu-id="c4425-128">[OnenotePage](page.md) collection</span></span>|<span data-ttu-id="c4425-129">Страницы всех записных книжек OneNote, принадлежащих пользователю или группе.</span><span class="sxs-lookup"><span data-stu-id="c4425-129">The pages in all OneNote notebooks that are owned by the user or group.</span></span>  <span data-ttu-id="c4425-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c4425-130">Read-only.</span></span> <span data-ttu-id="c4425-131">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c4425-131">Nullable.</span></span>|
|<span data-ttu-id="c4425-132">resources</span><span class="sxs-lookup"><span data-stu-id="c4425-132">resources</span></span>|<span data-ttu-id="c4425-133">Коллекция [OnenoteResource](resource.md)</span><span class="sxs-lookup"><span data-stu-id="c4425-133">[OnenoteResource](resource.md) collection</span></span> |<span data-ttu-id="c4425-134">Изображения и другие файловые ресурсы на страницах OneNote.</span><span class="sxs-lookup"><span data-stu-id="c4425-134">The image and other file resources in OneNote pages.</span></span> <span data-ttu-id="c4425-135">Получение коллекции ресурсов не поддерживается, но можно [получить двоичное содержимое определенного ресурса](resource.md).</span><span class="sxs-lookup"><span data-stu-id="c4425-135">Getting a resources collection is not supported, but you can [get the binary content of a specific resource](resource.md).</span></span> <span data-ttu-id="c4425-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c4425-136">Read-only.</span></span> <span data-ttu-id="c4425-137">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c4425-137">Nullable.</span></span>|
|<span data-ttu-id="c4425-138">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="c4425-138">sectionGroups</span></span>|<span data-ttu-id="c4425-139">Коллекция [SectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="c4425-139">SectionGroup collection</span></span>|<span data-ttu-id="c4425-140">Группы разделов во всех записных книжках OneNote, принадлежащих пользователю или группе.</span><span class="sxs-lookup"><span data-stu-id="c4425-140">The section groups in all OneNote notebooks that are owned by the user or group.</span></span>  <span data-ttu-id="c4425-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c4425-141">Read-only.</span></span> <span data-ttu-id="c4425-142">Допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="c4425-142">Nullable.</span></span>|
|<span data-ttu-id="c4425-143">sections</span><span class="sxs-lookup"><span data-stu-id="c4425-143">sections</span></span>|<span data-ttu-id="c4425-144">Коллекция [OnenoteSection](section.md)</span><span class="sxs-lookup"><span data-stu-id="c4425-144">[OnenoteSection](section.md) collection</span></span>|<span data-ttu-id="c4425-145">Разделы во всех записных книжках OneNote, принадлежащих пользователю или группе.</span><span class="sxs-lookup"><span data-stu-id="c4425-145">The sections in all OneNote notebooks that are owned by the user or group.</span></span>  <span data-ttu-id="c4425-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c4425-146">Read-only.</span></span> <span data-ttu-id="c4425-147">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c4425-147">Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="c4425-148">Методы</span><span class="sxs-lookup"><span data-stu-id="c4425-148">Methods</span></span>

| <span data-ttu-id="c4425-149">Метод</span><span class="sxs-lookup"><span data-stu-id="c4425-149">Method</span></span>           | <span data-ttu-id="c4425-150">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c4425-150">Return Type</span></span>    |<span data-ttu-id="c4425-151">Описание</span><span class="sxs-lookup"><span data-stu-id="c4425-151">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c4425-152">Создание записной книжки</span><span class="sxs-lookup"><span data-stu-id="c4425-152">Create notebook</span></span>](../api/onenote-post-notebooks.md) |[<span data-ttu-id="c4425-153">Notebook</span><span class="sxs-lookup"><span data-stu-id="c4425-153">Notebook</span></span>](notebook.md)| <span data-ttu-id="c4425-154">Создание записной книжки путем публикации в коллекции записных книжек.</span><span class="sxs-lookup"><span data-stu-id="c4425-154">Create a new ContactFolder by posting to the contactFolders collection.</span></span>|
|[<span data-ttu-id="c4425-155">Перечисление записных книжек</span><span class="sxs-lookup"><span data-stu-id="c4425-155">List notebooks</span></span>](../api/onenote-list-notebooks.md) |<span data-ttu-id="c4425-156">Коллекция [Notebook](notebook.md)</span><span class="sxs-lookup"><span data-stu-id="c4425-156">Notebook collection</span></span>| <span data-ttu-id="c4425-157">Получение коллекции записных книжек.</span><span class="sxs-lookup"><span data-stu-id="c4425-157">Represents a collection of notebooks.</span></span>|
|[<span data-ttu-id="c4425-158">Создание страницы</span><span class="sxs-lookup"><span data-stu-id="c4425-158">Create page</span></span>](../api/onenote-post-pages.md) |[<span data-ttu-id="c4425-159">Page</span><span class="sxs-lookup"><span data-stu-id="c4425-159">Page</span></span>](page.md)| <span data-ttu-id="c4425-160">Создание страницы путем публикации в коллекции страниц.</span><span class="sxs-lookup"><span data-stu-id="c4425-160">Create a new ContactFolder by posting to the contactFolders collection.</span></span>|
|[<span data-ttu-id="c4425-161">Перечисление страниц</span><span class="sxs-lookup"><span data-stu-id="c4425-161">List pages</span></span>](../api/onenote-list-pages.md) |<span data-ttu-id="c4425-162">Коллекция [Page](page.md)</span><span class="sxs-lookup"><span data-stu-id="c4425-162">Page collection</span></span>| <span data-ttu-id="c4425-163">Получение коллекции страниц.</span><span class="sxs-lookup"><span data-stu-id="c4425-163">Represents a collection of pages.</span></span>|
|[<span data-ttu-id="c4425-164">Перечисление групп разделов</span><span class="sxs-lookup"><span data-stu-id="c4425-164">List section groups</span></span>](../api/onenote-list-sectiongroups.md) |<span data-ttu-id="c4425-165">Коллекция [SectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="c4425-165">SectionGroup collection</span></span>| <span data-ttu-id="c4425-166">Получение коллекции групп разделов.</span><span class="sxs-lookup"><span data-stu-id="c4425-166">Represents a collection of section groups.</span></span>|
|[<span data-ttu-id="c4425-167">Перечисление разделов</span><span class="sxs-lookup"><span data-stu-id="c4425-167">List sections</span></span>](../api/onenote-list-sections.md) |<span data-ttu-id="c4425-168">Коллекция [OnenoteSection](section.md)</span><span class="sxs-lookup"><span data-stu-id="c4425-168">[OnenoteSection](section.md) collection</span></span>| <span data-ttu-id="c4425-169">Получение коллекции разделов.</span><span class="sxs-lookup"><span data-stu-id="c4425-169">Represents a collection of sections.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="c4425-170">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c4425-170">JSON Representation</span></span>
<span data-ttu-id="c4425-171">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c4425-171">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.onenote"
}-->
``` json
{
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
