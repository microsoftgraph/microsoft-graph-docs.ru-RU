# <a name="onenote-resource-type"></a><span data-ttu-id="beacc-101">Тип ресурса onenote</span><span class="sxs-lookup"><span data-stu-id="beacc-101">onenote resource type</span></span>

<span data-ttu-id="beacc-102">Точка входа для ресурсов OneNote.</span><span class="sxs-lookup"><span data-stu-id="beacc-102">The entry point for OneNote resources.</span></span>

<span data-ttu-id="beacc-103">Все вызовы службы OneNote через API Microsoft Graph выполняются с помощью следующего корневого URL-адреса службы:</span><span class="sxs-lookup"><span data-stu-id="beacc-103">All calls to the OneNote service through the Microsoft Graph API use this service root URL:</span></span>

```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

<span data-ttu-id="beacc-104">В качестве расположений можно задавать записные книжки пользователя в Office 365 или личные хранилища OneDrive, записные книжки группы (в том числе размещенные на сайте SharePoint) в Office 365.</span><span class="sxs-lookup"><span data-stu-id="beacc-104">The location can be user notebooks on Office 365 or consumer OneDrive, group notebooks or SharePoint site-hosted team notebooks on Office 365.</span></span> 

<span data-ttu-id="beacc-105">**Записные книжки пользователей.** Чтобы получить доступ к персональным записным книжкам в OneDrive для бизнеса или личном хранилище OneDrive, воспользуйтесь одним из следующих URL-адресов:</span><span class="sxs-lookup"><span data-stu-id="beacc-105">**User notebooks** To access personal notebooks on consumer OneDrive or OneDrive for Business, use one of the following URLs:</span></span>

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

<span data-ttu-id="beacc-106">**Записные книжки группы.** Чтобы получить доступ к записным книжкам группы, воспользуйтесь следующим корневым URL-адресом службы:</span><span class="sxs-lookup"><span data-stu-id="beacc-106">**Group notebooks** To access notebooks that are owned by a group, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
<span data-ttu-id="beacc-107">**Записные книжки на сайте SharePoint.** Чтобы получить доступ к записным книжкам на сайте группы SharePoint, воспользуйтесь следующим корневым URL-адресом службы:</span><span class="sxs-lookup"><span data-stu-id="beacc-107">**SharePoint site notebooks** To access notebooks that are owned by a SharePoint team site, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
## <a name="authorization"></a><span data-ttu-id="beacc-108">Авторизация</span><span class="sxs-lookup"><span data-stu-id="beacc-108">Authorization</span></span>

<span data-ttu-id="beacc-109">Сведения о разрешениях, необходимых для работы с API OneNote, см. в разделе [Разрешения для заметок](../../../concepts/permissions_reference.md#notes-permissions).</span><span class="sxs-lookup"><span data-stu-id="beacc-109">For information about the permissions required to work with OneNote APIs, see [Notes permissions](../../../concepts/permissions_reference.md#notes-permissions).</span></span>


## <a name="relationships"></a><span data-ttu-id="beacc-110">Отношения</span><span class="sxs-lookup"><span data-stu-id="beacc-110">Relationships</span></span>
| <span data-ttu-id="beacc-111">Связь</span><span class="sxs-lookup"><span data-stu-id="beacc-111">Relationship</span></span> | <span data-ttu-id="beacc-112">Тип</span><span class="sxs-lookup"><span data-stu-id="beacc-112">Type</span></span>   |<span data-ttu-id="beacc-113">Описание</span><span class="sxs-lookup"><span data-stu-id="beacc-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="beacc-114">notebooks</span><span class="sxs-lookup"><span data-stu-id="beacc-114">notebooks</span></span>|<span data-ttu-id="beacc-115">Коллекция [Notebook](notebook.md)</span><span class="sxs-lookup"><span data-stu-id="beacc-115">[Notebook](notebook.md) collection</span></span>|<span data-ttu-id="beacc-p101">Коллекция записных книжек OneNote, принадлежащих пользователю или группе. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="beacc-p101">The collection of OneNote notebooks that are owned by the user or group. Read-only. Nullable.</span></span>|
|<span data-ttu-id="beacc-119">operations</span><span class="sxs-lookup"><span data-stu-id="beacc-119">operations</span></span>|<span data-ttu-id="beacc-120">Коллекция [OnenoteOperation](onenoteoperation.md)</span><span class="sxs-lookup"><span data-stu-id="beacc-120">[OnenoteOperation](onenoteoperation.md) collection</span></span> |<span data-ttu-id="beacc-p102">Состояние операций OneNote. Получение коллекции операций не поддерживается, но можно получить состояние длительных операций, если в отклике возвращается заголовок `Operation-Location`. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="beacc-p102">The status of OneNote operations. Getting an operations collection is not supported, but you can get the status of long-running operations if the `Operation-Location` header is returned in the response. Read-only. Nullable.</span></span>|
|<span data-ttu-id="beacc-125">pages</span><span class="sxs-lookup"><span data-stu-id="beacc-125">pages</span></span>|<span data-ttu-id="beacc-126">Коллекция [OnenotePage](page.md)</span><span class="sxs-lookup"><span data-stu-id="beacc-126">[OnenotePage](page.md) collection</span></span>|<span data-ttu-id="beacc-p103">Страницы всех записных книжек OneNote, принадлежащих пользователю или группе. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="beacc-p103">The pages in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|
|<span data-ttu-id="beacc-130">resources</span><span class="sxs-lookup"><span data-stu-id="beacc-130">resources</span></span>|<span data-ttu-id="beacc-131">Коллекция [OnenoteResource](resource.md)</span><span class="sxs-lookup"><span data-stu-id="beacc-131">[OnenoteResource](resource.md) collection</span></span> |<span data-ttu-id="beacc-p104">Изображения и другие ресурсы file на страницах OneNote. Получение коллекции ресурсов не поддерживается, но можно [получить двоичное содержимое определенного ресурса](resource.md). Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="beacc-p104">The image and other file resources in OneNote pages. Getting a resources collection is not supported, but you can [get the binary content of a specific resource](resource.md). Read-only. Nullable.</span></span>|
|<span data-ttu-id="beacc-136">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="beacc-136">sectionGroups</span></span>|<span data-ttu-id="beacc-137">Коллекция [SectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="beacc-137">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="beacc-p105">Группы разделов во всех записных книжках OneNote, принадлежащих пользователю или группе.  Только для чтения. Допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="beacc-p105">The section groups in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|
|<span data-ttu-id="beacc-141">sections</span><span class="sxs-lookup"><span data-stu-id="beacc-141">sections</span></span>|<span data-ttu-id="beacc-142">Коллекция [OnenoteSection](section.md)</span><span class="sxs-lookup"><span data-stu-id="beacc-142">[OnenoteSection](section.md) collection</span></span>|<span data-ttu-id="beacc-p106">Разделы во всех записных книжках OneNote, принадлежащих пользователю или группе. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="beacc-p106">The sections in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="beacc-146">Методы</span><span class="sxs-lookup"><span data-stu-id="beacc-146">Methods</span></span>

| <span data-ttu-id="beacc-147">Метод</span><span class="sxs-lookup"><span data-stu-id="beacc-147">Method</span></span>           | <span data-ttu-id="beacc-148">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="beacc-148">Return Type</span></span>    |<span data-ttu-id="beacc-149">Описание</span><span class="sxs-lookup"><span data-stu-id="beacc-149">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="beacc-150">Создание записной книжки</span><span class="sxs-lookup"><span data-stu-id="beacc-150">Create notebook</span></span>](../api/onenote_post_notebooks.md) |[<span data-ttu-id="beacc-151">Notebook</span><span class="sxs-lookup"><span data-stu-id="beacc-151">Notebook</span></span>](notebook.md)| <span data-ttu-id="beacc-152">Создание записной книжки путем публикации в коллекции записных книжек.</span><span class="sxs-lookup"><span data-stu-id="beacc-152">Create a notebook by posting to the notebooks collection.</span></span>|
|[<span data-ttu-id="beacc-153">Перечисление записных книжек</span><span class="sxs-lookup"><span data-stu-id="beacc-153">List notebooks</span></span>](../api/onenote_list_notebooks.md) |<span data-ttu-id="beacc-154">Коллекция [Notebook](notebook.md)</span><span class="sxs-lookup"><span data-stu-id="beacc-154">[Notebook](notebook.md) collection</span></span>| <span data-ttu-id="beacc-155">Получение коллекции записных книжек.</span><span class="sxs-lookup"><span data-stu-id="beacc-155">Get a collection of notebooks.</span></span>|
|[<span data-ttu-id="beacc-156">Создание страницы</span><span class="sxs-lookup"><span data-stu-id="beacc-156">Create page</span></span>](../api/onenote_post_pages.md) |[<span data-ttu-id="beacc-157">Page</span><span class="sxs-lookup"><span data-stu-id="beacc-157">Page</span></span>](page.md)| <span data-ttu-id="beacc-158">Создание страницы путем публикации в коллекции страниц.</span><span class="sxs-lookup"><span data-stu-id="beacc-158">Create a page by posting to the pages collection.</span></span>|
|[<span data-ttu-id="beacc-159">Перечисление страниц</span><span class="sxs-lookup"><span data-stu-id="beacc-159">List pages</span></span>](../api/onenote_list_pages.md) |<span data-ttu-id="beacc-160">Коллекция [Page](page.md)</span><span class="sxs-lookup"><span data-stu-id="beacc-160">[Page](page.md) collection</span></span>| <span data-ttu-id="beacc-161">Получение коллекции страниц.</span><span class="sxs-lookup"><span data-stu-id="beacc-161">Get a collection of pages.</span></span>|
|[<span data-ttu-id="beacc-162">Перечисление групп разделов</span><span class="sxs-lookup"><span data-stu-id="beacc-162">List section groups</span></span>](../api/onenote_list_sectiongroups.md) |<span data-ttu-id="beacc-163">Коллекция [SectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="beacc-163">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="beacc-164">Получение коллекции групп разделов.</span><span class="sxs-lookup"><span data-stu-id="beacc-164">Get a collection of section groups.</span></span>|
|[<span data-ttu-id="beacc-165">Перечисление разделов</span><span class="sxs-lookup"><span data-stu-id="beacc-165">List sections</span></span>](../api/onenote_list_sections.md) |<span data-ttu-id="beacc-166">Коллекция [OnenoteSection](section.md)</span><span class="sxs-lookup"><span data-stu-id="beacc-166">[OnenoteSection](section.md) collection</span></span>| <span data-ttu-id="beacc-167">Получение коллекции разделов.</span><span class="sxs-lookup"><span data-stu-id="beacc-167">Get a collection of sections.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="beacc-168">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="beacc-168">JSON Representation</span></span>
<span data-ttu-id="beacc-169">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="beacc-169">Here is a JSON representation of the resource.</span></span>
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
