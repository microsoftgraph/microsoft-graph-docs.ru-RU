---
title: Тип ресурса notebook
description: Записная книжка OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 96be6a41424260610794f9a0df4ef8e35dc1597f
ms.sourcegitcommit: bdbc68ed8eaf43386d2cdf7b79e64ebbe1e860c0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/13/2019
ms.locfileid: "29967335"
---
# <a name="notebook-resource-type"></a><span data-ttu-id="cceef-103">Тип ресурса notebook</span><span class="sxs-lookup"><span data-stu-id="cceef-103">notebook resource type</span></span>

<span data-ttu-id="cceef-104">Записная книжка OneNote.</span><span class="sxs-lookup"><span data-stu-id="cceef-104">A OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cceef-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="cceef-105">JSON representation</span></span>

<span data-ttu-id="cceef-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="cceef-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.onenoteEntityHierarchyModel",
  "optionalProperties": [
    "sectionGroups",
    "sections"
  ],
  "@odata.type": "microsoft.graph.notebook"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "isDefault": true,
  "isShared": true,
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "links": {"@odata.type": "microsoft.graph.notebookLinks"},
  "displayName": "string",
  "sectionGroupsUrl": "string",
  "sectionsUrl": "string",
  "self": "string",
  "userRole": "String"
}

```
## <a name="properties"></a><span data-ttu-id="cceef-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="cceef-107">Properties</span></span>
| <span data-ttu-id="cceef-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="cceef-108">Property</span></span>     | <span data-ttu-id="cceef-109">Тип</span><span class="sxs-lookup"><span data-stu-id="cceef-109">Type</span></span>   |<span data-ttu-id="cceef-110">Описание</span><span class="sxs-lookup"><span data-stu-id="cceef-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cceef-111">createdBy</span><span class="sxs-lookup"><span data-stu-id="cceef-111">createdBy</span></span>|[<span data-ttu-id="cceef-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="cceef-112">identitySet</span></span>](identityset.md)|<span data-ttu-id="cceef-p101">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cceef-p101">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="cceef-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cceef-115">createdDateTime</span></span>|<span data-ttu-id="cceef-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cceef-116">DateTimeOffset</span></span>|<span data-ttu-id="cceef-p102">Дата и время создания записной книжки. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cceef-p102">The date and time when the notebook was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="cceef-121">id</span><span class="sxs-lookup"><span data-stu-id="cceef-121">id</span></span>|<span data-ttu-id="cceef-122">Строка</span><span class="sxs-lookup"><span data-stu-id="cceef-122">String</span></span>|<span data-ttu-id="cceef-p103">Уникальный идентификатор записной книжки. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cceef-p103">The unique identifier of the notebook. Read-only.</span></span>|
|<span data-ttu-id="cceef-125">isDefault</span><span class="sxs-lookup"><span data-stu-id="cceef-125">isDefault</span></span>|<span data-ttu-id="cceef-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="cceef-126">Boolean</span></span>|<span data-ttu-id="cceef-p104">Указывает, является ли эта записная книжка записной книжкой пользователя по умолчанию. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cceef-p104">Indicates whether this is the user's default notebook. Read-only.</span></span>|
|<span data-ttu-id="cceef-129">IsShared</span><span class="sxs-lookup"><span data-stu-id="cceef-129">isShared</span></span>|<span data-ttu-id="cceef-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="cceef-130">Boolean</span></span>|<span data-ttu-id="cceef-p105">Указывает, является ли записная книжка общей. Если вы укажете значение true, содержимое записной книжки сможет видеть не только владелец. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cceef-p105">Indicates whether the notebook is shared. If true, the contents of the notebook can be seen by people other than the owner. Read-only.</span></span>|
|<span data-ttu-id="cceef-134">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="cceef-134">lastModifiedBy</span></span>|[<span data-ttu-id="cceef-135">identitySet</span><span class="sxs-lookup"><span data-stu-id="cceef-135">identitySet</span></span>](identityset.md)|<span data-ttu-id="cceef-p106">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cceef-p106">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="cceef-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cceef-138">lastModifiedDateTime</span></span>|<span data-ttu-id="cceef-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cceef-139">DateTimeOffset</span></span>|<span data-ttu-id="cceef-p107">Дата и время последнего изменения записной книжки. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cceef-p107">The date and time when the notebook was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="cceef-144">links</span><span class="sxs-lookup"><span data-stu-id="cceef-144">links</span></span>|[<span data-ttu-id="cceef-145">NotebookLinks</span><span class="sxs-lookup"><span data-stu-id="cceef-145">NotebookLinks</span></span>](notebooklinks.md)|<span data-ttu-id="cceef-p108">Ссылки для открытия записной книжки. Ссылка `oneNoteClientURL` открывает записную книжку в клиенте OneNote, если он установлен. Ссылка `oneNoteWebURL` открывает записную книжку в OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="cceef-p108">Links for opening the notebook. The `oneNoteClientURL` link opens the notebook in the OneNote native client if it's installed. The `oneNoteWebURL` link opens the notebook in OneNote Online.</span></span>|
|<span data-ttu-id="cceef-149">displayName</span><span class="sxs-lookup"><span data-stu-id="cceef-149">displayName</span></span>|<span data-ttu-id="cceef-150">String</span><span class="sxs-lookup"><span data-stu-id="cceef-150">String</span></span>|<span data-ttu-id="cceef-151">Имя записной книжки.</span><span class="sxs-lookup"><span data-stu-id="cceef-151">The name of the notebook.</span></span>|
|<span data-ttu-id="cceef-152">sectionGroupsUrl</span><span class="sxs-lookup"><span data-stu-id="cceef-152">sectionGroupsUrl</span></span>|<span data-ttu-id="cceef-153">Строка</span><span class="sxs-lookup"><span data-stu-id="cceef-153">String</span></span>|<span data-ttu-id="cceef-p109">URL-адрес для свойства навигации `sectionGroups`, который возвращает все группы разделов в записной книжке. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cceef-p109">The URL for the `sectionGroups` navigation property, which returns all the section groups in the notebook. Read-only.</span></span>|
|<span data-ttu-id="cceef-156">sectionsUrl</span><span class="sxs-lookup"><span data-stu-id="cceef-156">sectionsUrl</span></span>|<span data-ttu-id="cceef-157">Строка</span><span class="sxs-lookup"><span data-stu-id="cceef-157">String</span></span>|<span data-ttu-id="cceef-p110">URL-адрес для свойства навигации `sections`, который возвращает все разделы в записной книжке. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cceef-p110">The URL for the `sections` navigation property, which returns all the sections in the notebook. Read-only.</span></span>|
|<span data-ttu-id="cceef-160">self</span><span class="sxs-lookup"><span data-stu-id="cceef-160">self</span></span>|<span data-ttu-id="cceef-161">Строка</span><span class="sxs-lookup"><span data-stu-id="cceef-161">String</span></span>|<span data-ttu-id="cceef-p111">Конечная точка, в которой можно получить сведения о записной книжке. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cceef-p111">The endpoint where you can get details about the notebook. Read-only.</span></span>|
|<span data-ttu-id="cceef-164">userRole</span><span class="sxs-lookup"><span data-stu-id="cceef-164">userRole</span></span>|<span data-ttu-id="cceef-165">onenoteUserRole</span><span class="sxs-lookup"><span data-stu-id="cceef-165">onenoteUserRole</span></span>|<span data-ttu-id="cceef-p112">Возможные значения: `Owner`, `Contributor`, `Reader`, `None`. Owner — доступ к записной книжке на уровне владельца. Contributor — доступ к записной книжке для чтения и записи. Reader — доступ к записной книжке только для чтения. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cceef-p112">Possible values are: `Owner`, `Contributor`, `Reader`, `None`. Owner represents owner-level access to the notebook. Contributor represents read/write access to the notebook. Reader represents read-only access to the notebook. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cceef-171">Связи</span><span class="sxs-lookup"><span data-stu-id="cceef-171">Relationships</span></span>
| <span data-ttu-id="cceef-172">Связь</span><span class="sxs-lookup"><span data-stu-id="cceef-172">Relationship</span></span> | <span data-ttu-id="cceef-173">Тип</span><span class="sxs-lookup"><span data-stu-id="cceef-173">Type</span></span>   |<span data-ttu-id="cceef-174">Описание</span><span class="sxs-lookup"><span data-stu-id="cceef-174">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cceef-175">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="cceef-175">sectionGroups</span></span>|<span data-ttu-id="cceef-176">Коллекция объектов [SectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="cceef-176">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="cceef-p113">Группы разделов в записной книжке. Только для чтения. Допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="cceef-p113">The section groups in the notebook. Read-only. Nullable.</span></span>|
|<span data-ttu-id="cceef-180">sections</span><span class="sxs-lookup"><span data-stu-id="cceef-180">sections</span></span>|<span data-ttu-id="cceef-181">[OnenoteSection](section.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="cceef-181">[OnenoteSection](section.md) collection</span></span>|<span data-ttu-id="cceef-p114">Разделы в записной книжке. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="cceef-p114">The sections in the notebook. Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="cceef-185">Методы</span><span class="sxs-lookup"><span data-stu-id="cceef-185">Methods</span></span>

| <span data-ttu-id="cceef-186">Метод</span><span class="sxs-lookup"><span data-stu-id="cceef-186">Method</span></span>           | <span data-ttu-id="cceef-187">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="cceef-187">Return Type</span></span>    |<span data-ttu-id="cceef-188">Описание</span><span class="sxs-lookup"><span data-stu-id="cceef-188">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cceef-189">Получение записной книжки</span><span class="sxs-lookup"><span data-stu-id="cceef-189">Get notebook</span></span>](../api/notebook-get.md) | [<span data-ttu-id="cceef-190">Notebook</span><span class="sxs-lookup"><span data-stu-id="cceef-190">Notebook</span></span>](notebook.md) |<span data-ttu-id="cceef-191">Считывание свойств и связей записной книжки.</span><span class="sxs-lookup"><span data-stu-id="cceef-191">Read the properties and relationships of the notebook.</span></span>|
|[<span data-ttu-id="cceef-192">getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="cceef-192">getRecentNotebooks</span></span>](../api/notebook-getrecentnotebooks.md) | <span data-ttu-id="cceef-193">Коллекция [recentNotebook](recentnotebook.md)</span><span class="sxs-lookup"><span data-stu-id="cceef-193">[recentNotebook](recentnotebook.md) collection</span></span> | <span data-ttu-id="cceef-194">Получение коллекции недавно открывавшихся записных книжек для пользователя.</span><span class="sxs-lookup"><span data-stu-id="cceef-194">Get a collection of the most recently accessed notebooks for the user.</span></span> |
|[<span data-ttu-id="cceef-195">getNotebookFromWebUrl</span><span class="sxs-lookup"><span data-stu-id="cceef-195">getNotebookFromWebUrl</span></span>](../api/notebook-getnotebookfromweburl.md) | [<span data-ttu-id="cceef-196">Notebook</span><span class="sxs-lookup"><span data-stu-id="cceef-196">Notebook</span></span>](notebook.md) | <span data-ttu-id="cceef-197">Извлечение свойств и связи объекта записной книжки, с помощью его URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="cceef-197">Retrieve the properties and relationships of a notebook object using its URL path.</span></span> |
|[<span data-ttu-id="cceef-198">Создание группы разделов</span><span class="sxs-lookup"><span data-stu-id="cceef-198">Create section group</span></span>](../api/notebook-post-sectiongroups.md) |[<span data-ttu-id="cceef-199">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="cceef-199">SectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="cceef-200">Создайте группу разделов, отправив запрос POST в коллекцию sectionGroups в указанной записной книжке.</span><span class="sxs-lookup"><span data-stu-id="cceef-200">Create a section group by posting to the sectionGroups collection in the specified notebook.</span></span>|
|[<span data-ttu-id="cceef-201">Перечисление групп разделов</span><span class="sxs-lookup"><span data-stu-id="cceef-201">List section groups</span></span>](../api/notebook-list-sectiongroups.md) |<span data-ttu-id="cceef-202">Коллекция объектов [SectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="cceef-202">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="cceef-203">Получение коллекции групп разделов в указанной записной книжке.</span><span class="sxs-lookup"><span data-stu-id="cceef-203">Get a collection of section groups in the specified notebook.</span></span>|
|[<span data-ttu-id="cceef-204">Создание раздела</span><span class="sxs-lookup"><span data-stu-id="cceef-204">Create section</span></span>](../api/notebook-post-sections.md) |[<span data-ttu-id="cceef-205">OnenoteSection</span><span class="sxs-lookup"><span data-stu-id="cceef-205">OnenoteSection</span></span>](section.md)| <span data-ttu-id="cceef-206">Создайте раздел, отправив запрос POST в коллекцию sections в указанной записной книжке.</span><span class="sxs-lookup"><span data-stu-id="cceef-206">Create a section by posting to the sections collection in the specified notebook.</span></span>|
|[<span data-ttu-id="cceef-207">Перечисление разделов</span><span class="sxs-lookup"><span data-stu-id="cceef-207">List sections</span></span>](../api/notebook-list-sections.md) |<span data-ttu-id="cceef-208">[OnenoteSection](section.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="cceef-208">[OnenoteSection](section.md) collection</span></span>| <span data-ttu-id="cceef-209">Получение коллекции разделов в указанной записной книжке.</span><span class="sxs-lookup"><span data-stu-id="cceef-209">Get a collection of sections in the specified notebook.</span></span>|
|[<span data-ttu-id="cceef-210">copyNotebook</span><span class="sxs-lookup"><span data-stu-id="cceef-210">copyNotebook</span></span>](../api/notebook-copynotebook.md)| <span data-ttu-id="cceef-211">Нет</span><span class="sxs-lookup"><span data-stu-id="cceef-211">None</span></span> | <span data-ttu-id="cceef-212">Копирование записной книжки.</span><span class="sxs-lookup"><span data-stu-id="cceef-212">Copies a notebook.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebook resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
