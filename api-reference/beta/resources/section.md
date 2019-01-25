---
title: Тип ресурса section
description: Раздел в записной книжке OneNote. Разделы могут содержать страницы.
localization_priority: Normal
ms.openlocfilehash: faecf31ad09f3ea3b5614480fc051ad1054d442b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526097"
---
# <a name="section-resource-type"></a><span data-ttu-id="2ce53-104">Тип ресурса section</span><span class="sxs-lookup"><span data-stu-id="2ce53-104">section resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ce53-p102">Раздел в записной книжке OneNote. Разделы могут содержать страницы.</span><span class="sxs-lookup"><span data-stu-id="2ce53-p102">A section in a OneNote notebook. Sections can contain pages.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2ce53-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2ce53-107">JSON representation</span></span>

<span data-ttu-id="2ce53-108">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2ce53-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="2ce53-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="2ce53-109">Properties</span></span>
| <span data-ttu-id="2ce53-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="2ce53-110">Property</span></span>     | <span data-ttu-id="2ce53-111">Тип</span><span class="sxs-lookup"><span data-stu-id="2ce53-111">Type</span></span>   |<span data-ttu-id="2ce53-112">Описание</span><span class="sxs-lookup"><span data-stu-id="2ce53-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2ce53-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="2ce53-113">createdBy</span></span>|[<span data-ttu-id="2ce53-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="2ce53-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="2ce53-p103">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2ce53-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="2ce53-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2ce53-117">createdDateTime</span></span>|<span data-ttu-id="2ce53-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ce53-118">DateTimeOffset</span></span>|<span data-ttu-id="2ce53-p104">Дата и время создания раздела. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2ce53-p104">The date and time when the section was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="2ce53-123">id</span><span class="sxs-lookup"><span data-stu-id="2ce53-123">id</span></span>|<span data-ttu-id="2ce53-124">String</span><span class="sxs-lookup"><span data-stu-id="2ce53-124">String</span></span>|<span data-ttu-id="2ce53-p105">Уникальный идентификатор раздела.  Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2ce53-p105">The unique identifier of the section.  Read-only.</span></span>|
|<span data-ttu-id="2ce53-127">isDefault</span><span class="sxs-lookup"><span data-stu-id="2ce53-127">isDefault</span></span>|<span data-ttu-id="2ce53-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ce53-128">Boolean</span></span>|<span data-ttu-id="2ce53-p106">Указывает, является ли этот раздел разделом пользователя по умолчанию. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2ce53-p106">Indicates whether this is the user's default section. Read-only.</span></span>|
|<span data-ttu-id="2ce53-131">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="2ce53-131">lastModifiedBy</span></span>|[<span data-ttu-id="2ce53-132">identitySet</span><span class="sxs-lookup"><span data-stu-id="2ce53-132">identitySet</span></span>](identityset.md)|<span data-ttu-id="2ce53-p107">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2ce53-p107">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="2ce53-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2ce53-135">lastModifiedDateTime</span></span>|<span data-ttu-id="2ce53-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ce53-136">DateTimeOffset</span></span>|<span data-ttu-id="2ce53-p108">Дата и время последнего изменения раздела. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2ce53-p108">The date and time when the section was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="2ce53-141">links</span><span class="sxs-lookup"><span data-stu-id="2ce53-141">links</span></span>|[<span data-ttu-id="2ce53-142">SectionLinks</span><span class="sxs-lookup"><span data-stu-id="2ce53-142">SectionLinks</span></span>](sectionlinks.md)|<span data-ttu-id="2ce53-p109">Ссылки для открытия раздела. Ссылка `oneNoteClientURL` открывает раздел в клиенте OneNote, если он установлен. Ссылка `oneNoteWebURL` открывает раздел в OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="2ce53-p109">Links for opening the section. The `oneNoteClientURL` link opens the section in the OneNote native client if it's installed. The `oneNoteWebURL` link opens the section in OneNote Online.</span></span>|
|<span data-ttu-id="2ce53-146">displayName</span><span class="sxs-lookup"><span data-stu-id="2ce53-146">displayName</span></span>|<span data-ttu-id="2ce53-147">String</span><span class="sxs-lookup"><span data-stu-id="2ce53-147">String</span></span>|<span data-ttu-id="2ce53-148">Имя раздела.</span><span class="sxs-lookup"><span data-stu-id="2ce53-148">The name of the section.</span></span> |
|<span data-ttu-id="2ce53-149">pagesUrl</span><span class="sxs-lookup"><span data-stu-id="2ce53-149">pagesUrl</span></span>|<span data-ttu-id="2ce53-150">Строка</span><span class="sxs-lookup"><span data-stu-id="2ce53-150">String</span></span>|<span data-ttu-id="2ce53-p110">`pages` — конечная точка, в которой можно получить сведения обо всех страницах в разделе. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2ce53-p110">The `pages` endpoint where you can get details for all the pages in the section. Read-only.</span></span>|
|<span data-ttu-id="2ce53-153">self</span><span class="sxs-lookup"><span data-stu-id="2ce53-153">self</span></span>|<span data-ttu-id="2ce53-154">String</span><span class="sxs-lookup"><span data-stu-id="2ce53-154">String</span></span>|<span data-ttu-id="2ce53-p111">Конечная точка, в которой можно получить сведения о разделе. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2ce53-p111">The endpoint where you can get details about the section. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ce53-157">Отношения</span><span class="sxs-lookup"><span data-stu-id="2ce53-157">Relationships</span></span>
| <span data-ttu-id="2ce53-158">Связь</span><span class="sxs-lookup"><span data-stu-id="2ce53-158">Relationship</span></span> | <span data-ttu-id="2ce53-159">Тип</span><span class="sxs-lookup"><span data-stu-id="2ce53-159">Type</span></span>   |<span data-ttu-id="2ce53-160">Описание</span><span class="sxs-lookup"><span data-stu-id="2ce53-160">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2ce53-161">pages</span><span class="sxs-lookup"><span data-stu-id="2ce53-161">pages</span></span>|<span data-ttu-id="2ce53-162">Коллекция объектов [Page](page.md)</span><span class="sxs-lookup"><span data-stu-id="2ce53-162">[Page](page.md) collection</span></span>|<span data-ttu-id="2ce53-p112">Коллекция страниц в разделе.  Только для чтения. Допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="2ce53-p112">The collection of pages in the section.  Read-only. Nullable.</span></span>|
|<span data-ttu-id="2ce53-166">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="2ce53-166">parentNotebook</span></span>|[<span data-ttu-id="2ce53-167">Notebook</span><span class="sxs-lookup"><span data-stu-id="2ce53-167">Notebook</span></span>](notebook.md)|<span data-ttu-id="2ce53-p113">Записная книжка, содержащая раздел.  Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2ce53-p113">The notebook that contains the section.  Read-only.</span></span>|
|<span data-ttu-id="2ce53-170">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="2ce53-170">parentSectionGroup</span></span>|[<span data-ttu-id="2ce53-171">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="2ce53-171">SectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="2ce53-p114">Группа объектов, содержащая раздел.  Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2ce53-p114">The section group that contains the section.  Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="2ce53-174">Методы</span><span class="sxs-lookup"><span data-stu-id="2ce53-174">Methods</span></span>

| <span data-ttu-id="2ce53-175">Метод</span><span class="sxs-lookup"><span data-stu-id="2ce53-175">Method</span></span>           | <span data-ttu-id="2ce53-176">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2ce53-176">Return Type</span></span>    |<span data-ttu-id="2ce53-177">Описание</span><span class="sxs-lookup"><span data-stu-id="2ce53-177">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2ce53-178">Получение раздела</span><span class="sxs-lookup"><span data-stu-id="2ce53-178">Get section</span></span>](../api/section-get.md) | [<span data-ttu-id="2ce53-179">Section</span><span class="sxs-lookup"><span data-stu-id="2ce53-179">Section</span></span>](section.md) |<span data-ttu-id="2ce53-180">Чтение свойств и отношений раздела.</span><span class="sxs-lookup"><span data-stu-id="2ce53-180">Read the properties and relationships of the section.</span></span>|
|[<span data-ttu-id="2ce53-181">Создание страницы</span><span class="sxs-lookup"><span data-stu-id="2ce53-181">Create page</span></span>](../api/section-post-pages.md) |[<span data-ttu-id="2ce53-182">Page</span><span class="sxs-lookup"><span data-stu-id="2ce53-182">Page</span></span>](page.md)| <span data-ttu-id="2ce53-183">Создайте страницу, отправив запрос POST в коллекцию pages в указанном разделе.</span><span class="sxs-lookup"><span data-stu-id="2ce53-183">Create a page by posting to the pages collection in the specified section.</span></span>|
|[<span data-ttu-id="2ce53-184">Перечисление страниц</span><span class="sxs-lookup"><span data-stu-id="2ce53-184">List pages</span></span>](../api/section-list-pages.md) |<span data-ttu-id="2ce53-185">Коллекция объектов [Page](page.md)</span><span class="sxs-lookup"><span data-stu-id="2ce53-185">[Page](page.md) collection</span></span>| <span data-ttu-id="2ce53-186">Получение коллекции страниц в указанном разделе.</span><span class="sxs-lookup"><span data-stu-id="2ce53-186">Get a collection of pages in the specified section.</span></span>|
|[<span data-ttu-id="2ce53-187">copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="2ce53-187">copyToNotebook</span></span>](../api/section-copytonotebook.md)|<span data-ttu-id="2ce53-188">Нет</span><span class="sxs-lookup"><span data-stu-id="2ce53-188">None</span></span>|<span data-ttu-id="2ce53-189">Копирование раздела в указанную записную книжку.</span><span class="sxs-lookup"><span data-stu-id="2ce53-189">Copy the section to a specific notebook.</span></span>|
|[<span data-ttu-id="2ce53-190">copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="2ce53-190">copyToSectionGroup</span></span>](../api/section-copytosectiongroup.md)|<span data-ttu-id="2ce53-191">Нет</span><span class="sxs-lookup"><span data-stu-id="2ce53-191">None</span></span>|<span data-ttu-id="2ce53-192">Копирование раздела в указанную группу разделов.</span><span class="sxs-lookup"><span data-stu-id="2ce53-192">Copy the section to a specific section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onenoteSection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/section.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
