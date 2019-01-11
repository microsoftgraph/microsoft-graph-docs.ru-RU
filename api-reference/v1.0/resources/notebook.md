---
title: Тип ресурса notebook
description: Записная книжка OneNote.
author: Jewan-microsoft
localization_priority: Normal
ms.openlocfilehash: 0a657ea6d5837674a7881bc9ef6095af5529355a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894448"
---
# <a name="notebook-resource-type"></a><span data-ttu-id="a217a-103">Тип ресурса notebook</span><span class="sxs-lookup"><span data-stu-id="a217a-103">notebook resource type</span></span>

<span data-ttu-id="a217a-104">Записная книжка OneNote.</span><span class="sxs-lookup"><span data-stu-id="a217a-104">A OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a217a-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a217a-105">JSON representation</span></span>

<span data-ttu-id="a217a-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="a217a-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="a217a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a217a-107">Properties</span></span>
| <span data-ttu-id="a217a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a217a-108">Property</span></span>     | <span data-ttu-id="a217a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a217a-109">Type</span></span>   |<span data-ttu-id="a217a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a217a-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a217a-111">createdBy</span><span class="sxs-lookup"><span data-stu-id="a217a-111">createdBy</span></span>|[<span data-ttu-id="a217a-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="a217a-112">identitySet</span></span>](identityset.md)|<span data-ttu-id="a217a-p101">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a217a-p101">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="a217a-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a217a-115">createdDateTime</span></span>|<span data-ttu-id="a217a-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a217a-116">DateTimeOffset</span></span>|<span data-ttu-id="a217a-p102">Дата и время создания записной книжки. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a217a-p102">The date and time when the notebook was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="a217a-121">id</span><span class="sxs-lookup"><span data-stu-id="a217a-121">id</span></span>|<span data-ttu-id="a217a-122">Строка</span><span class="sxs-lookup"><span data-stu-id="a217a-122">String</span></span>|<span data-ttu-id="a217a-p103">Уникальный идентификатор записной книжки. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a217a-p103">The unique identifier of the notebook. Read-only.</span></span>|
|<span data-ttu-id="a217a-125">isDefault</span><span class="sxs-lookup"><span data-stu-id="a217a-125">isDefault</span></span>|<span data-ttu-id="a217a-126">Логический</span><span class="sxs-lookup"><span data-stu-id="a217a-126">Boolean</span></span>|<span data-ttu-id="a217a-p104">Указывает, является ли эта записная книжка записной книжкой пользователя по умолчанию. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a217a-p104">Indicates whether this is the user's default notebook. Read-only.</span></span>|
|<span data-ttu-id="a217a-129">IsShared</span><span class="sxs-lookup"><span data-stu-id="a217a-129">isShared</span></span>|<span data-ttu-id="a217a-130">Логический</span><span class="sxs-lookup"><span data-stu-id="a217a-130">Boolean</span></span>|<span data-ttu-id="a217a-p105">Указывает, является ли записная книжка общей. Если вы укажете значение true, содержимое записной книжки сможет видеть не только владелец. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a217a-p105">Indicates whether the notebook is shared. If true, the contents of the notebook can be seen by people other than the owner. Read-only.</span></span>|
|<span data-ttu-id="a217a-134">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="a217a-134">lastModifiedBy</span></span>|[<span data-ttu-id="a217a-135">identitySet</span><span class="sxs-lookup"><span data-stu-id="a217a-135">identitySet</span></span>](identityset.md)|<span data-ttu-id="a217a-p106">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a217a-p106">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="a217a-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a217a-138">lastModifiedDateTime</span></span>|<span data-ttu-id="a217a-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a217a-139">DateTimeOffset</span></span>|<span data-ttu-id="a217a-p107">Дата и время последнего изменения записной книжки. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a217a-p107">The date and time when the notebook was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="a217a-144">links</span><span class="sxs-lookup"><span data-stu-id="a217a-144">links</span></span>|[<span data-ttu-id="a217a-145">NotebookLinks</span><span class="sxs-lookup"><span data-stu-id="a217a-145">NotebookLinks</span></span>](notebooklinks.md)|<span data-ttu-id="a217a-p108">Ссылки для открытия записной книжки. Ссылка `oneNoteClientURL` открывает записную книжку в клиенте OneNote, если он установлен. Ссылка `oneNoteWebURL` открывает записную книжку в OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="a217a-p108">Links for opening the notebook. The `oneNoteClientURL` link opens the notebook in the OneNote native client if it's installed. The `oneNoteWebURL` link opens the notebook in OneNote Online.</span></span>|
|<span data-ttu-id="a217a-149">displayName</span><span class="sxs-lookup"><span data-stu-id="a217a-149">displayName</span></span>|<span data-ttu-id="a217a-150">Строка</span><span class="sxs-lookup"><span data-stu-id="a217a-150">String</span></span>|<span data-ttu-id="a217a-151">Имя записной книжки.</span><span class="sxs-lookup"><span data-stu-id="a217a-151">The name of the notebook.</span></span>|
|<span data-ttu-id="a217a-152">sectionGroupsUrl</span><span class="sxs-lookup"><span data-stu-id="a217a-152">sectionGroupsUrl</span></span>|<span data-ttu-id="a217a-153">Строка</span><span class="sxs-lookup"><span data-stu-id="a217a-153">String</span></span>|<span data-ttu-id="a217a-p109">URL-адрес для свойства навигации `sectionGroups`, который возвращает все группы разделов в записной книжке. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a217a-p109">The URL for the `sectionGroups` navigation property, which returns all the section groups in the notebook. Read-only.</span></span>|
|<span data-ttu-id="a217a-156">sectionsUrl</span><span class="sxs-lookup"><span data-stu-id="a217a-156">sectionsUrl</span></span>|<span data-ttu-id="a217a-157">Строка</span><span class="sxs-lookup"><span data-stu-id="a217a-157">String</span></span>|<span data-ttu-id="a217a-p110">URL-адрес для свойства навигации `sections`, который возвращает все разделы в записной книжке. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a217a-p110">The URL for the `sections` navigation property, which returns all the sections in the notebook. Read-only.</span></span>|
|<span data-ttu-id="a217a-160">self</span><span class="sxs-lookup"><span data-stu-id="a217a-160">self</span></span>|<span data-ttu-id="a217a-161">Строка</span><span class="sxs-lookup"><span data-stu-id="a217a-161">String</span></span>|<span data-ttu-id="a217a-p111">Конечная точка, в которой можно получить сведения о записной книжке. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a217a-p111">The endpoint where you can get details about the notebook. Read-only.</span></span>|
|<span data-ttu-id="a217a-164">userRole</span><span class="sxs-lookup"><span data-stu-id="a217a-164">userRole</span></span>|<span data-ttu-id="a217a-165">onenoteUserRole</span><span class="sxs-lookup"><span data-stu-id="a217a-165">onenoteUserRole</span></span>|<span data-ttu-id="a217a-p112">Возможные значения: `Owner`, `Contributor`, `Reader`, `None`. Owner — доступ к записной книжке на уровне владельца. Contributor — доступ к записной книжке для чтения и записи. Reader — доступ к записной книжке только для чтения. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a217a-p112">Possible values are: `Owner`, `Contributor`, `Reader`, `None`. Owner represents owner-level access to the notebook. Contributor represents read/write access to the notebook. Reader represents read-only access to the notebook. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a217a-171">Связи</span><span class="sxs-lookup"><span data-stu-id="a217a-171">Relationships</span></span>
| <span data-ttu-id="a217a-172">Связь</span><span class="sxs-lookup"><span data-stu-id="a217a-172">Relationship</span></span> | <span data-ttu-id="a217a-173">Тип</span><span class="sxs-lookup"><span data-stu-id="a217a-173">Type</span></span>   |<span data-ttu-id="a217a-174">Описание</span><span class="sxs-lookup"><span data-stu-id="a217a-174">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a217a-175">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="a217a-175">sectionGroups</span></span>|<span data-ttu-id="a217a-176">Коллекция объектов [SectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="a217a-176">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="a217a-p113">Группы разделов в записной книжке. Только для чтения. Допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="a217a-p113">The section groups in the notebook. Read-only. Nullable.</span></span>|
|<span data-ttu-id="a217a-180">sections</span><span class="sxs-lookup"><span data-stu-id="a217a-180">sections</span></span>|<span data-ttu-id="a217a-181">[OnenoteSection](section.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="a217a-181">[OnenoteSection](section.md) collection</span></span>|<span data-ttu-id="a217a-p114">Разделы в записной книжке. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="a217a-p114">The sections in the notebook. Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="a217a-185">Методы</span><span class="sxs-lookup"><span data-stu-id="a217a-185">Methods</span></span>

| <span data-ttu-id="a217a-186">Метод</span><span class="sxs-lookup"><span data-stu-id="a217a-186">Method</span></span>           | <span data-ttu-id="a217a-187">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a217a-187">Return Type</span></span>    |<span data-ttu-id="a217a-188">Описание</span><span class="sxs-lookup"><span data-stu-id="a217a-188">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a217a-189">Получение записной книжки</span><span class="sxs-lookup"><span data-stu-id="a217a-189">Get notebook</span></span>](../api/notebook-get.md) | [<span data-ttu-id="a217a-190">Notebook</span><span class="sxs-lookup"><span data-stu-id="a217a-190">Notebook</span></span>](notebook.md) |<span data-ttu-id="a217a-191">Считывание свойств и связей записной книжки.</span><span class="sxs-lookup"><span data-stu-id="a217a-191">Read the properties and relationships of the notebook.</span></span>|
|[<span data-ttu-id="a217a-192">getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="a217a-192">getRecentNotebooks</span></span>](../api/notebook-getrecentnotebooks.md) | <span data-ttu-id="a217a-193">Коллекция [recentNotebook](recentnotebook.md)</span><span class="sxs-lookup"><span data-stu-id="a217a-193">[recentNotebook](recentnotebook.md) collection</span></span> | <span data-ttu-id="a217a-194">Получение коллекции недавно открывавшихся записных книжек для пользователя.</span><span class="sxs-lookup"><span data-stu-id="a217a-194">Get a collection of the most recently accessed notebooks for the user.</span></span> |
|[<span data-ttu-id="a217a-195">Создание группы разделов</span><span class="sxs-lookup"><span data-stu-id="a217a-195">Create section group</span></span>](../api/notebook-post-sectiongroups.md) |[<span data-ttu-id="a217a-196">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="a217a-196">SectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="a217a-197">Создайте группу разделов, отправив запрос POST в коллекцию sectionGroups в указанной записной книжке.</span><span class="sxs-lookup"><span data-stu-id="a217a-197">Create a section group by posting to the sectionGroups collection in the specified notebook.</span></span>|
|[<span data-ttu-id="a217a-198">Перечисление групп разделов</span><span class="sxs-lookup"><span data-stu-id="a217a-198">List section groups</span></span>](../api/notebook-list-sectiongroups.md) |<span data-ttu-id="a217a-199">Коллекция объектов [SectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="a217a-199">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="a217a-200">Получение коллекции групп разделов в указанной записной книжке.</span><span class="sxs-lookup"><span data-stu-id="a217a-200">Get a collection of section groups in the specified notebook.</span></span>|
|[<span data-ttu-id="a217a-201">Создание раздела</span><span class="sxs-lookup"><span data-stu-id="a217a-201">Create section</span></span>](../api/notebook-post-sections.md) |[<span data-ttu-id="a217a-202">OnenoteSection</span><span class="sxs-lookup"><span data-stu-id="a217a-202">OnenoteSection</span></span>](section.md)| <span data-ttu-id="a217a-203">Создайте раздел, отправив запрос POST в коллекцию sections в указанной записной книжке.</span><span class="sxs-lookup"><span data-stu-id="a217a-203">Create a section by posting to the sections collection in the specified notebook.</span></span>|
|[<span data-ttu-id="a217a-204">Перечисление разделов</span><span class="sxs-lookup"><span data-stu-id="a217a-204">List sections</span></span>](../api/notebook-list-sections.md) |<span data-ttu-id="a217a-205">[OnenoteSection](section.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="a217a-205">[OnenoteSection](section.md) collection</span></span>| <span data-ttu-id="a217a-206">Получение коллекции разделов в указанной записной книжке.</span><span class="sxs-lookup"><span data-stu-id="a217a-206">Get a collection of sections in the specified notebook.</span></span>|
|[<span data-ttu-id="a217a-207">copyNotebook</span><span class="sxs-lookup"><span data-stu-id="a217a-207">copyNotebook</span></span>](../api/notebook-copynotebook.md)| <span data-ttu-id="a217a-208">Нет</span><span class="sxs-lookup"><span data-stu-id="a217a-208">None</span></span> | <span data-ttu-id="a217a-209">Копирование записной книжки.</span><span class="sxs-lookup"><span data-stu-id="a217a-209">Copies a notebook.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebook resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
