---
title: Тип ресурса section
description: Раздел в записной книжке OneNote. Разделы могут содержать страницы.
ms.openlocfilehash: c07f8f2e5c9f9f9d367cbc1186983c0870b2e979
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075496"
---
# <a name="section-resource-type"></a><span data-ttu-id="069f4-104">Тип ресурса section</span><span class="sxs-lookup"><span data-stu-id="069f4-104">section resource type</span></span>

> <span data-ttu-id="069f4-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="069f4-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="069f4-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="069f4-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="069f4-p103">Раздел в записной книжке OneNote. Разделы могут содержать страницы.</span><span class="sxs-lookup"><span data-stu-id="069f4-p103">A section in a OneNote notebook. Sections can contain pages.</span></span>

## <a name="json-representation"></a><span data-ttu-id="069f4-109">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="069f4-109">JSON representation</span></span>

<span data-ttu-id="069f4-110">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="069f4-110">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "pages",
    "parentNotebook",
    "parentSectionGroup"
  ],
  "@odata.type": "microsoft.graph.onenoteSection"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "isDefault": true,
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "links": {"@odata.type": "microsoft.graph.sectionLinks"},
  "displayName": "string",
  "pagesUrl": "string",
  "self": "string"
}

```
## <a name="properties"></a><span data-ttu-id="069f4-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="069f4-111">Properties</span></span>
| <span data-ttu-id="069f4-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="069f4-112">Property</span></span>     | <span data-ttu-id="069f4-113">Тип</span><span class="sxs-lookup"><span data-stu-id="069f4-113">Type</span></span>   |<span data-ttu-id="069f4-114">Описание</span><span class="sxs-lookup"><span data-stu-id="069f4-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="069f4-115">createdBy</span><span class="sxs-lookup"><span data-stu-id="069f4-115">createdBy</span></span>|[<span data-ttu-id="069f4-116">identitySet</span><span class="sxs-lookup"><span data-stu-id="069f4-116">identitySet</span></span>](identityset.md)|<span data-ttu-id="069f4-p104">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="069f4-p104">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="069f4-119">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="069f4-119">createdDateTime</span></span>|<span data-ttu-id="069f4-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="069f4-120">DateTimeOffset</span></span>|<span data-ttu-id="069f4-p105">Дата и время создания раздела. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="069f4-p105">The date and time when the section was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="069f4-125">id</span><span class="sxs-lookup"><span data-stu-id="069f4-125">id</span></span>|<span data-ttu-id="069f4-126">String</span><span class="sxs-lookup"><span data-stu-id="069f4-126">String</span></span>|<span data-ttu-id="069f4-p106">Уникальный идентификатор раздела.  Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="069f4-p106">The unique identifier of the section.  Read-only.</span></span>|
|<span data-ttu-id="069f4-129">isDefault</span><span class="sxs-lookup"><span data-stu-id="069f4-129">isDefault</span></span>|<span data-ttu-id="069f4-130">Логический</span><span class="sxs-lookup"><span data-stu-id="069f4-130">Boolean</span></span>|<span data-ttu-id="069f4-p107">Указывает, является ли этот раздел разделом пользователя по умолчанию. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="069f4-p107">Indicates whether this is the user's default section. Read-only.</span></span>|
|<span data-ttu-id="069f4-133">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="069f4-133">lastModifiedBy</span></span>|[<span data-ttu-id="069f4-134">identitySet</span><span class="sxs-lookup"><span data-stu-id="069f4-134">identitySet</span></span>](identityset.md)|<span data-ttu-id="069f4-p108">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="069f4-p108">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="069f4-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="069f4-137">lastModifiedDateTime</span></span>|<span data-ttu-id="069f4-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="069f4-138">DateTimeOffset</span></span>|<span data-ttu-id="069f4-p109">Дата и время последнего изменения раздела. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="069f4-p109">The date and time when the section was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="069f4-143">links</span><span class="sxs-lookup"><span data-stu-id="069f4-143">links</span></span>|[<span data-ttu-id="069f4-144">SectionLinks</span><span class="sxs-lookup"><span data-stu-id="069f4-144">SectionLinks</span></span>](sectionlinks.md)|<span data-ttu-id="069f4-p110">Ссылки для открытия раздела. Ссылка `oneNoteClientURL` открывает раздел в клиенте OneNote, если он установлен. Ссылка `oneNoteWebURL` открывает раздел в OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="069f4-p110">Links for opening the section. The `oneNoteClientURL` link opens the section in the OneNote native client if it's installed. The `oneNoteWebURL` link opens the section in OneNote Online.</span></span>|
|<span data-ttu-id="069f4-148">displayName</span><span class="sxs-lookup"><span data-stu-id="069f4-148">displayName</span></span>|<span data-ttu-id="069f4-149">Строка</span><span class="sxs-lookup"><span data-stu-id="069f4-149">String</span></span>|<span data-ttu-id="069f4-150">Имя раздела.</span><span class="sxs-lookup"><span data-stu-id="069f4-150">The name of the section.</span></span> |
|<span data-ttu-id="069f4-151">pagesUrl</span><span class="sxs-lookup"><span data-stu-id="069f4-151">pagesUrl</span></span>|<span data-ttu-id="069f4-152">Строка</span><span class="sxs-lookup"><span data-stu-id="069f4-152">String</span></span>|<span data-ttu-id="069f4-p111">`pages` — конечная точка, в которой можно получить сведения обо всех страницах в разделе. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="069f4-p111">The `pages` endpoint where you can get details for all the pages in the section. Read-only.</span></span>|
|<span data-ttu-id="069f4-155">self</span><span class="sxs-lookup"><span data-stu-id="069f4-155">self</span></span>|<span data-ttu-id="069f4-156">String</span><span class="sxs-lookup"><span data-stu-id="069f4-156">String</span></span>|<span data-ttu-id="069f4-p112">Конечная точка, в которой можно получить сведения о разделе. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="069f4-p112">The endpoint where you can get details about the section. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="069f4-159">Связи</span><span class="sxs-lookup"><span data-stu-id="069f4-159">Relationships</span></span>
| <span data-ttu-id="069f4-160">Связь</span><span class="sxs-lookup"><span data-stu-id="069f4-160">Relationship</span></span> | <span data-ttu-id="069f4-161">Тип</span><span class="sxs-lookup"><span data-stu-id="069f4-161">Type</span></span>   |<span data-ttu-id="069f4-162">Описание</span><span class="sxs-lookup"><span data-stu-id="069f4-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="069f4-163">pages</span><span class="sxs-lookup"><span data-stu-id="069f4-163">pages</span></span>|<span data-ttu-id="069f4-164">Коллекция объектов [Page](page.md)</span><span class="sxs-lookup"><span data-stu-id="069f4-164">[Page](page.md) collection</span></span>|<span data-ttu-id="069f4-p113">Коллекция страниц в разделе.  Только для чтения. Допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="069f4-p113">The collection of pages in the section.  Read-only. Nullable.</span></span>|
|<span data-ttu-id="069f4-168">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="069f4-168">parentNotebook</span></span>|[<span data-ttu-id="069f4-169">Notebook</span><span class="sxs-lookup"><span data-stu-id="069f4-169">Notebook</span></span>](notebook.md)|<span data-ttu-id="069f4-p114">Записная книжка, содержащая раздел.  Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="069f4-p114">The notebook that contains the section.  Read-only.</span></span>|
|<span data-ttu-id="069f4-172">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="069f4-172">parentSectionGroup</span></span>|[<span data-ttu-id="069f4-173">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="069f4-173">SectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="069f4-p115">Группа объектов, содержащая раздел.  Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="069f4-p115">The section group that contains the section.  Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="069f4-176">Методы</span><span class="sxs-lookup"><span data-stu-id="069f4-176">Methods</span></span>

| <span data-ttu-id="069f4-177">Метод</span><span class="sxs-lookup"><span data-stu-id="069f4-177">Method</span></span>           | <span data-ttu-id="069f4-178">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="069f4-178">Return Type</span></span>    |<span data-ttu-id="069f4-179">Описание</span><span class="sxs-lookup"><span data-stu-id="069f4-179">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="069f4-180">Получение раздела</span><span class="sxs-lookup"><span data-stu-id="069f4-180">Get section</span></span>](../api/section-get.md) | [<span data-ttu-id="069f4-181">Section</span><span class="sxs-lookup"><span data-stu-id="069f4-181">Section</span></span>](section.md) |<span data-ttu-id="069f4-182">Чтение свойств и отношений раздела.</span><span class="sxs-lookup"><span data-stu-id="069f4-182">Read the properties and relationships of the section.</span></span>|
|[<span data-ttu-id="069f4-183">Создание страницы</span><span class="sxs-lookup"><span data-stu-id="069f4-183">Create page</span></span>](../api/section-post-pages.md) |[<span data-ttu-id="069f4-184">Page</span><span class="sxs-lookup"><span data-stu-id="069f4-184">Page</span></span>](page.md)| <span data-ttu-id="069f4-185">Создайте страницу, отправив запрос POST в коллекцию pages в указанном разделе.</span><span class="sxs-lookup"><span data-stu-id="069f4-185">Create a page by posting to the pages collection in the specified section.</span></span>|
|[<span data-ttu-id="069f4-186">Перечисление страниц</span><span class="sxs-lookup"><span data-stu-id="069f4-186">List pages</span></span>](../api/section-list-pages.md) |<span data-ttu-id="069f4-187">Коллекция объектов [Page](page.md)</span><span class="sxs-lookup"><span data-stu-id="069f4-187">[Page](page.md) collection</span></span>| <span data-ttu-id="069f4-188">Получение коллекции страниц в указанном разделе.</span><span class="sxs-lookup"><span data-stu-id="069f4-188">Get a collection of pages in the specified section.</span></span>|
|[<span data-ttu-id="069f4-189">copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="069f4-189">copyToNotebook</span></span>](../api/section-copytonotebook.md)|<span data-ttu-id="069f4-190">Нет</span><span class="sxs-lookup"><span data-stu-id="069f4-190">None</span></span>|<span data-ttu-id="069f4-191">Копирование раздела в указанную записную книжку.</span><span class="sxs-lookup"><span data-stu-id="069f4-191">Copy the section to a specific notebook.</span></span>|
|[<span data-ttu-id="069f4-192">copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="069f4-192">copyToSectionGroup</span></span>](../api/section-copytosectiongroup.md)|<span data-ttu-id="069f4-193">Нет</span><span class="sxs-lookup"><span data-stu-id="069f4-193">None</span></span>|<span data-ttu-id="069f4-194">Копирование раздела в указанную группу разделов.</span><span class="sxs-lookup"><span data-stu-id="069f4-194">Copy the section to a specific section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteSection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
