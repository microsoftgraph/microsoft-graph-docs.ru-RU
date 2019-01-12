---
title: Тип ресурса notebook
description: Записная книжка OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 5038e1c79e85275afbb65e41a57768e83b0d2e16
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933346"
---
# <a name="notebook-resource-type"></a><span data-ttu-id="e0e36-103">Тип ресурса notebook</span><span class="sxs-lookup"><span data-stu-id="e0e36-103">notebook resource type</span></span>

> <span data-ttu-id="e0e36-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e0e36-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e0e36-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0e36-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e0e36-106">Записная книжка OneNote.</span><span class="sxs-lookup"><span data-stu-id="e0e36-106">A OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e0e36-107">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e0e36-107">JSON representation</span></span>

<span data-ttu-id="e0e36-108">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="e0e36-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
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
## <a name="properties"></a><span data-ttu-id="e0e36-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="e0e36-109">Properties</span></span>
| <span data-ttu-id="e0e36-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="e0e36-110">Property</span></span>     | <span data-ttu-id="e0e36-111">Тип</span><span class="sxs-lookup"><span data-stu-id="e0e36-111">Type</span></span>   |<span data-ttu-id="e0e36-112">Описание</span><span class="sxs-lookup"><span data-stu-id="e0e36-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e0e36-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="e0e36-113">createdBy</span></span>|[<span data-ttu-id="e0e36-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="e0e36-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="e0e36-p102">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e0e36-p102">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="e0e36-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e0e36-117">createdDateTime</span></span>|<span data-ttu-id="e0e36-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0e36-118">DateTimeOffset</span></span>|<span data-ttu-id="e0e36-p103">Дата и время создания записной книжки. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e0e36-p103">The date and time when the notebook was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="e0e36-123">id</span><span class="sxs-lookup"><span data-stu-id="e0e36-123">id</span></span>|<span data-ttu-id="e0e36-124">Строка</span><span class="sxs-lookup"><span data-stu-id="e0e36-124">String</span></span>|<span data-ttu-id="e0e36-p104">Уникальный идентификатор записной книжки. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e0e36-p104">The unique identifier of the notebook. Read-only.</span></span>|
|<span data-ttu-id="e0e36-127">isDefault</span><span class="sxs-lookup"><span data-stu-id="e0e36-127">isDefault</span></span>|<span data-ttu-id="e0e36-128">Логический</span><span class="sxs-lookup"><span data-stu-id="e0e36-128">Boolean</span></span>|<span data-ttu-id="e0e36-p105">Указывает, является ли эта записная книжка записной книжкой пользователя по умолчанию. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e0e36-p105">Indicates whether this is the user's default notebook. Read-only.</span></span>|
|<span data-ttu-id="e0e36-131">IsShared</span><span class="sxs-lookup"><span data-stu-id="e0e36-131">isShared</span></span>|<span data-ttu-id="e0e36-132">Логический</span><span class="sxs-lookup"><span data-stu-id="e0e36-132">Boolean</span></span>|<span data-ttu-id="e0e36-p106">Указывает, является ли записная книжка общей. Если вы укажете значение true, содержимое записной книжки сможет видеть не только владелец. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e0e36-p106">Indicates whether the notebook is shared. If true, the contents of the notebook can be seen by people other than the owner. Read-only.</span></span>|
|<span data-ttu-id="e0e36-136">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="e0e36-136">lastModifiedBy</span></span>|[<span data-ttu-id="e0e36-137">identitySet</span><span class="sxs-lookup"><span data-stu-id="e0e36-137">identitySet</span></span>](identityset.md)|<span data-ttu-id="e0e36-p107">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e0e36-p107">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="e0e36-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e0e36-140">lastModifiedDateTime</span></span>|<span data-ttu-id="e0e36-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0e36-141">DateTimeOffset</span></span>|<span data-ttu-id="e0e36-p108">Дата и время последнего изменения записной книжки. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e0e36-p108">The date and time when the notebook was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="e0e36-146">links</span><span class="sxs-lookup"><span data-stu-id="e0e36-146">links</span></span>|[<span data-ttu-id="e0e36-147">NotebookLinks</span><span class="sxs-lookup"><span data-stu-id="e0e36-147">NotebookLinks</span></span>](notebooklinks.md)|<span data-ttu-id="e0e36-p109">Ссылки для открытия записной книжки. Ссылка `oneNoteClientURL` открывает записную книжку в клиенте OneNote, если он установлен. Ссылка `oneNoteWebURL` открывает записную книжку в OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="e0e36-p109">Links for opening the notebook. The `oneNoteClientURL` link opens the notebook in the OneNote native client if it's installed. The `oneNoteWebURL` link opens the notebook in OneNote Online.</span></span>|
|<span data-ttu-id="e0e36-151">displayName</span><span class="sxs-lookup"><span data-stu-id="e0e36-151">displayName</span></span>|<span data-ttu-id="e0e36-152">Строка</span><span class="sxs-lookup"><span data-stu-id="e0e36-152">String</span></span>|<span data-ttu-id="e0e36-153">Имя записной книжки.</span><span class="sxs-lookup"><span data-stu-id="e0e36-153">The name of the notebook.</span></span>|
|<span data-ttu-id="e0e36-154">sectionGroupsUrl</span><span class="sxs-lookup"><span data-stu-id="e0e36-154">sectionGroupsUrl</span></span>|<span data-ttu-id="e0e36-155">Строка</span><span class="sxs-lookup"><span data-stu-id="e0e36-155">String</span></span>|<span data-ttu-id="e0e36-p110">URL-адрес для свойства навигации `sectionGroups`, который возвращает все группы разделов в записной книжке. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e0e36-p110">The URL for the `sectionGroups` navigation property, which returns all the section groups in the notebook. Read-only.</span></span>|
|<span data-ttu-id="e0e36-158">sectionsUrl</span><span class="sxs-lookup"><span data-stu-id="e0e36-158">sectionsUrl</span></span>|<span data-ttu-id="e0e36-159">Строка</span><span class="sxs-lookup"><span data-stu-id="e0e36-159">String</span></span>|<span data-ttu-id="e0e36-p111">URL-адрес для свойства навигации `sections`, который возвращает все разделы в записной книжке. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e0e36-p111">The URL for the `sections` navigation property, which returns all the sections in the notebook. Read-only.</span></span>|
|<span data-ttu-id="e0e36-162">self</span><span class="sxs-lookup"><span data-stu-id="e0e36-162">self</span></span>|<span data-ttu-id="e0e36-163">Строка</span><span class="sxs-lookup"><span data-stu-id="e0e36-163">String</span></span>|<span data-ttu-id="e0e36-p112">Конечная точка, в которой можно получить сведения о записной книжке. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e0e36-p112">The endpoint where you can get details about the notebook. Read-only.</span></span>|
|<span data-ttu-id="e0e36-166">userRole</span><span class="sxs-lookup"><span data-stu-id="e0e36-166">userRole</span></span>|<span data-ttu-id="e0e36-167">Строка</span><span class="sxs-lookup"><span data-stu-id="e0e36-167">String</span></span>|<span data-ttu-id="e0e36-p113">Возможные значения: `Owner`, `Contributor`, `Reader`, `None`. Owner — доступ к записной книжке на уровне владельца. Contributor — доступ к записной книжке для чтения и записи. Reader — доступ к записной книжке только для чтения. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e0e36-p113">Possible values are: `Owner`, `Contributor`, `Reader`, `None`. Owner represents owner-level access to the notebook. Contributor represents read/write access to the notebook. Reader represents read-only access to the notebook. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e0e36-173">Связи</span><span class="sxs-lookup"><span data-stu-id="e0e36-173">Relationships</span></span>
| <span data-ttu-id="e0e36-174">Связь</span><span class="sxs-lookup"><span data-stu-id="e0e36-174">Relationship</span></span> | <span data-ttu-id="e0e36-175">Тип</span><span class="sxs-lookup"><span data-stu-id="e0e36-175">Type</span></span>   |<span data-ttu-id="e0e36-176">Описание</span><span class="sxs-lookup"><span data-stu-id="e0e36-176">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e0e36-177">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="e0e36-177">sectionGroups</span></span>|<span data-ttu-id="e0e36-178">Коллекция объектов [SectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="e0e36-178">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="e0e36-p114">Группы разделов в записной книжке. Только для чтения. Допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="e0e36-p114">The section groups in the notebook. Read-only. Nullable.</span></span>|
|<span data-ttu-id="e0e36-182">sections</span><span class="sxs-lookup"><span data-stu-id="e0e36-182">sections</span></span>|<span data-ttu-id="e0e36-183">Коллекция объектов [Section](section.md)</span><span class="sxs-lookup"><span data-stu-id="e0e36-183">[Section](section.md) collection</span></span>|<span data-ttu-id="e0e36-p115">Разделы в записной книжке. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="e0e36-p115">The sections in the notebook. Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="e0e36-187">Методы</span><span class="sxs-lookup"><span data-stu-id="e0e36-187">Methods</span></span>

| <span data-ttu-id="e0e36-188">Метод</span><span class="sxs-lookup"><span data-stu-id="e0e36-188">Method</span></span>           | <span data-ttu-id="e0e36-189">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e0e36-189">Return Type</span></span>    |<span data-ttu-id="e0e36-190">Описание</span><span class="sxs-lookup"><span data-stu-id="e0e36-190">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e0e36-191">Получение записной книжки</span><span class="sxs-lookup"><span data-stu-id="e0e36-191">Get notebook</span></span>](../api/notebook-get.md) | [<span data-ttu-id="e0e36-192">Notebook</span><span class="sxs-lookup"><span data-stu-id="e0e36-192">Notebook</span></span>](notebook.md) |<span data-ttu-id="e0e36-193">Считывание свойств и связей записной книжки.</span><span class="sxs-lookup"><span data-stu-id="e0e36-193">Read the properties and relationships of the notebook.</span></span>|
|[<span data-ttu-id="e0e36-194">getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="e0e36-194">getRecentNotebooks</span></span>](../api/notebook-getrecentnotebooks.md) | <span data-ttu-id="e0e36-195">Коллекция [recentNotebook](recentnotebook.md)</span><span class="sxs-lookup"><span data-stu-id="e0e36-195">[recentNotebook](recentnotebook.md) collection</span></span> | <span data-ttu-id="e0e36-196">Получение коллекции недавно открывавшихся записных книжек для пользователя.</span><span class="sxs-lookup"><span data-stu-id="e0e36-196">Get a collection of the most recently accessed notebooks for the user.</span></span> |
|[<span data-ttu-id="e0e36-197">Создание группы разделов</span><span class="sxs-lookup"><span data-stu-id="e0e36-197">Create section group</span></span>](../api/notebook-post-sectiongroups.md) |[<span data-ttu-id="e0e36-198">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="e0e36-198">SectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="e0e36-199">Создайте группу разделов, отправив запрос POST в коллекцию sectionGroups в указанной записной книжке.</span><span class="sxs-lookup"><span data-stu-id="e0e36-199">Create a section group by posting to the sectionGroups collection in the specified notebook.</span></span>|
|[<span data-ttu-id="e0e36-200">Перечисление групп разделов</span><span class="sxs-lookup"><span data-stu-id="e0e36-200">List section groups</span></span>](../api/notebook-list-sectiongroups.md) |<span data-ttu-id="e0e36-201">Коллекция объектов [SectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="e0e36-201">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="e0e36-202">Получение коллекции групп разделов в указанной записной книжке.</span><span class="sxs-lookup"><span data-stu-id="e0e36-202">Get a collection of section groups in the specified notebook.</span></span>|
|[<span data-ttu-id="e0e36-203">Создание раздела</span><span class="sxs-lookup"><span data-stu-id="e0e36-203">Create section</span></span>](../api/notebook-post-sections.md) |[<span data-ttu-id="e0e36-204">Section</span><span class="sxs-lookup"><span data-stu-id="e0e36-204">Section</span></span>](section.md)| <span data-ttu-id="e0e36-205">Создайте раздел, отправив запрос POST в коллекцию sections в указанной записной книжке.</span><span class="sxs-lookup"><span data-stu-id="e0e36-205">Create a section by posting to the sections collection in the specified notebook.</span></span>|
|[<span data-ttu-id="e0e36-206">Перечисление разделов</span><span class="sxs-lookup"><span data-stu-id="e0e36-206">List sections</span></span>](../api/notebook-list-sections.md) |<span data-ttu-id="e0e36-207">Коллекция объектов [Section](section.md)</span><span class="sxs-lookup"><span data-stu-id="e0e36-207">[Section](section.md) collection</span></span>| <span data-ttu-id="e0e36-208">Получение коллекции разделов в указанной записной книжке.</span><span class="sxs-lookup"><span data-stu-id="e0e36-208">Get a collection of sections in the specified notebook.</span></span>|
|[<span data-ttu-id="e0e36-209">copyNotebook</span><span class="sxs-lookup"><span data-stu-id="e0e36-209">copyNotebook</span></span>](../api/notebook-copynotebook.md)| <span data-ttu-id="e0e36-210">Нет</span><span class="sxs-lookup"><span data-stu-id="e0e36-210">None</span></span> | <span data-ttu-id="e0e36-211">Копирование записной книжки.</span><span class="sxs-lookup"><span data-stu-id="e0e36-211">Copies a notebook.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebook resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
