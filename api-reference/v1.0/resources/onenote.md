---
title: Тип ресурса onenote
description: Точка входа для ресурсов OneNote.
ms.openlocfilehash: f244fdf1770cbe34110097d8885b05e6407ee45f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027686"
---
# <a name="onenote-resource-type"></a><span data-ttu-id="a9656-103">Тип ресурса onenote</span><span class="sxs-lookup"><span data-stu-id="a9656-103">onenote resource type</span></span>

<span data-ttu-id="a9656-104">Точка входа для ресурсов OneNote.</span><span class="sxs-lookup"><span data-stu-id="a9656-104">The entry point for OneNote resources.</span></span>

<span data-ttu-id="a9656-105">Все вызовы службы OneNote через API Microsoft Graph выполняются с помощью следующего корневого URL-адреса службы:</span><span class="sxs-lookup"><span data-stu-id="a9656-105">All calls to the OneNote service through the Microsoft Graph API use this service root URL:</span></span>

```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

<span data-ttu-id="a9656-106">В качестве расположений можно задавать записные книжки пользователя в Office 365 или личные хранилища OneDrive, записные книжки группы (в том числе размещенные на сайте SharePoint) в Office 365.</span><span class="sxs-lookup"><span data-stu-id="a9656-106">The location can be user notebooks on Office 365 or consumer OneDrive, group notebooks or SharePoint site-hosted team notebooks on Office 365.</span></span> 

<span data-ttu-id="a9656-107">**Записные книжки пользователей.** Чтобы получить доступ к персональным записным книжкам в OneDrive для бизнеса или личном хранилище OneDrive, воспользуйтесь одним из следующих URL-адресов:</span><span class="sxs-lookup"><span data-stu-id="a9656-107">**User notebooks** To access personal notebooks on consumer OneDrive or OneDrive for Business, use one of the following URLs:</span></span>

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

<span data-ttu-id="a9656-108">**Записные книжки группы.** Чтобы получить доступ к записным книжкам группы, воспользуйтесь следующим корневым URL-адресом службы:</span><span class="sxs-lookup"><span data-stu-id="a9656-108">**Group notebooks** To access notebooks that are owned by a group, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
<span data-ttu-id="a9656-109">**Записные книжки на сайте SharePoint.** Чтобы получить доступ к записным книжкам на сайте группы SharePoint, воспользуйтесь следующим корневым URL-адресом службы:</span><span class="sxs-lookup"><span data-stu-id="a9656-109">**SharePoint site notebooks** To access notebooks that are owned by a SharePoint team site, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
## <a name="authorization"></a><span data-ttu-id="a9656-110">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a9656-110">Authorization</span></span>

<span data-ttu-id="a9656-111">Сведения о разрешениях, необходимых для работы с API OneNote, см. в разделе [Разрешения для заметок](/graph/permissions-reference#notes-permissions).</span><span class="sxs-lookup"><span data-stu-id="a9656-111">For information about the permissions required to work with OneNote APIs, see [Notes permissions](/graph/permissions-reference#notes-permissions).</span></span>


## <a name="relationships"></a><span data-ttu-id="a9656-112">Отношения</span><span class="sxs-lookup"><span data-stu-id="a9656-112">Relationships</span></span>
| <span data-ttu-id="a9656-113">Связь</span><span class="sxs-lookup"><span data-stu-id="a9656-113">Relationship</span></span> | <span data-ttu-id="a9656-114">Тип</span><span class="sxs-lookup"><span data-stu-id="a9656-114">Type</span></span>   |<span data-ttu-id="a9656-115">Описание</span><span class="sxs-lookup"><span data-stu-id="a9656-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a9656-116">notebooks</span><span class="sxs-lookup"><span data-stu-id="a9656-116">notebooks</span></span>|<span data-ttu-id="a9656-117">Коллекция [Notebook](notebook.md)</span><span class="sxs-lookup"><span data-stu-id="a9656-117">[Notebook](notebook.md) collection</span></span>|<span data-ttu-id="a9656-p101">Коллекция записных книжек OneNote, принадлежащих пользователю или группе. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="a9656-p101">The collection of OneNote notebooks that are owned by the user or group. Read-only. Nullable.</span></span>|
|<span data-ttu-id="a9656-121">operations</span><span class="sxs-lookup"><span data-stu-id="a9656-121">operations</span></span>|<span data-ttu-id="a9656-122">[OnenoteOperation](onenoteoperation.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="a9656-122">[OnenoteOperation](onenoteoperation.md) collection</span></span> |<span data-ttu-id="a9656-p102">Состояние операций OneNote. Получение коллекции операций не поддерживается, но можно получить состояние длительных операций, если в отклике возвращается заголовок `Operation-Location`. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="a9656-p102">The status of OneNote operations. Getting an operations collection is not supported, but you can get the status of long-running operations if the `Operation-Location` header is returned in the response. Read-only. Nullable.</span></span>|
|<span data-ttu-id="a9656-127">pages</span><span class="sxs-lookup"><span data-stu-id="a9656-127">pages</span></span>|<span data-ttu-id="a9656-128">[OnenotePage](page.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="a9656-128">[OnenotePage](page.md) collection</span></span>|<span data-ttu-id="a9656-p103">Страницы всех записных книжек OneNote, принадлежащих пользователю или группе.  Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="a9656-p103">The pages in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|
|<span data-ttu-id="a9656-132">resources</span><span class="sxs-lookup"><span data-stu-id="a9656-132">resources</span></span>|<span data-ttu-id="a9656-133">[OnenoteResource](resource.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="a9656-133">[OnenoteResource](resource.md) collection</span></span> |<span data-ttu-id="a9656-p104">Изображения и другие ресурсы file на страницах OneNote. Получение коллекции ресурсов не поддерживается, но можно [получить двоичное содержимое определенного ресурса](resource.md). Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="a9656-p104">The image and other file resources in OneNote pages. Getting a resources collection is not supported, but you can [get the binary content of a specific resource](resource.md). Read-only. Nullable.</span></span>|
|<span data-ttu-id="a9656-138">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="a9656-138">sectionGroups</span></span>|<span data-ttu-id="a9656-139">Коллекция [SectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="a9656-139">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="a9656-p105">Группы разделов во всех записных книжках OneNote, принадлежащих пользователю или группе.  Только для чтения. Допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="a9656-p105">The section groups in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|
|<span data-ttu-id="a9656-143">sections</span><span class="sxs-lookup"><span data-stu-id="a9656-143">sections</span></span>|<span data-ttu-id="a9656-144">[OnenoteSection](section.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="a9656-144">[OnenoteSection](section.md) collection</span></span>|<span data-ttu-id="a9656-p106">Разделы во всех записных книжках OneNote, принадлежащих пользователю или группе.  Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="a9656-p106">The sections in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="a9656-148">Методы</span><span class="sxs-lookup"><span data-stu-id="a9656-148">Methods</span></span>

| <span data-ttu-id="a9656-149">Метод</span><span class="sxs-lookup"><span data-stu-id="a9656-149">Method</span></span>           | <span data-ttu-id="a9656-150">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a9656-150">Return Type</span></span>    |<span data-ttu-id="a9656-151">Описание</span><span class="sxs-lookup"><span data-stu-id="a9656-151">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a9656-152">Создание записной книжки</span><span class="sxs-lookup"><span data-stu-id="a9656-152">Create notebook</span></span>](../api/onenote-post-notebooks.md) |[<span data-ttu-id="a9656-153">Notebook</span><span class="sxs-lookup"><span data-stu-id="a9656-153">Notebook</span></span>](notebook.md)| <span data-ttu-id="a9656-154">Создание записной книжки путем публикации в коллекции записных книжек.</span><span class="sxs-lookup"><span data-stu-id="a9656-154">Create a notebook by posting to the notebooks collection.</span></span>|
|[<span data-ttu-id="a9656-155">Перечисление записных книжек</span><span class="sxs-lookup"><span data-stu-id="a9656-155">List notebooks</span></span>](../api/onenote-list-notebooks.md) |<span data-ttu-id="a9656-156">Коллекция [Notebook](notebook.md)</span><span class="sxs-lookup"><span data-stu-id="a9656-156">[Notebook](notebook.md) collection</span></span>| <span data-ttu-id="a9656-157">Получение коллекции записных книжек.</span><span class="sxs-lookup"><span data-stu-id="a9656-157">Get a collection of notebooks.</span></span>|
|[<span data-ttu-id="a9656-158">Создание страницы</span><span class="sxs-lookup"><span data-stu-id="a9656-158">Create page</span></span>](../api/onenote-post-pages.md) |[<span data-ttu-id="a9656-159">Page</span><span class="sxs-lookup"><span data-stu-id="a9656-159">Page</span></span>](page.md)| <span data-ttu-id="a9656-160">Создание страницы путем публикации в коллекции страниц.</span><span class="sxs-lookup"><span data-stu-id="a9656-160">Create a page by posting to the pages collection.</span></span>|
|[<span data-ttu-id="a9656-161">Перечисление страниц</span><span class="sxs-lookup"><span data-stu-id="a9656-161">List pages</span></span>](../api/onenote-list-pages.md) |<span data-ttu-id="a9656-162">Коллекция [Page](page.md)</span><span class="sxs-lookup"><span data-stu-id="a9656-162">[Page](page.md) collection</span></span>| <span data-ttu-id="a9656-163">Получение коллекции страниц.</span><span class="sxs-lookup"><span data-stu-id="a9656-163">Get a collection of pages.</span></span>|
|[<span data-ttu-id="a9656-164">Перечисление групп разделов</span><span class="sxs-lookup"><span data-stu-id="a9656-164">List section groups</span></span>](../api/onenote-list-sectiongroups.md) |<span data-ttu-id="a9656-165">Коллекция [SectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="a9656-165">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="a9656-166">Получение коллекции групп разделов.</span><span class="sxs-lookup"><span data-stu-id="a9656-166">Get a collection of section groups.</span></span>|
|[<span data-ttu-id="a9656-167">Перечисление разделов</span><span class="sxs-lookup"><span data-stu-id="a9656-167">List sections</span></span>](../api/onenote-list-sections.md) |<span data-ttu-id="a9656-168">[OnenoteSection](section.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="a9656-168">[OnenoteSection](section.md) collection</span></span>| <span data-ttu-id="a9656-169">Получение коллекции разделов.</span><span class="sxs-lookup"><span data-stu-id="a9656-169">Get a collection of sections.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="a9656-170">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a9656-170">JSON Representation</span></span>
<span data-ttu-id="a9656-171">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a9656-171">Here is a JSON representation of the resource.</span></span>
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
