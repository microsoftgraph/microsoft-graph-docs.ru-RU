---
title: Тип ресурса section
description: Раздел в записной книжке OneNote. Разделы могут содержать страницы.
localization_priority: Normal
ms.openlocfilehash: f9cb5a8e3ddf9cf4a045103e4ecc7909653d797c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853237"
---
# <a name="section-resource-type"></a><span data-ttu-id="7a1b6-104">Тип ресурса section</span><span class="sxs-lookup"><span data-stu-id="7a1b6-104">section resource type</span></span>

<span data-ttu-id="7a1b6-p102">Раздел в записной книжке OneNote. Разделы могут содержать страницы.</span><span class="sxs-lookup"><span data-stu-id="7a1b6-p102">A section in a OneNote notebook. Sections can contain pages.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7a1b6-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7a1b6-107">JSON representation</span></span>

<span data-ttu-id="7a1b6-108">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7a1b6-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.onenoteEntityHierarchyModel",
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
## <a name="properties"></a><span data-ttu-id="7a1b6-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="7a1b6-109">Properties</span></span>
| <span data-ttu-id="7a1b6-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="7a1b6-110">Property</span></span>     | <span data-ttu-id="7a1b6-111">Тип</span><span class="sxs-lookup"><span data-stu-id="7a1b6-111">Type</span></span>   |<span data-ttu-id="7a1b6-112">Описание</span><span class="sxs-lookup"><span data-stu-id="7a1b6-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7a1b6-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="7a1b6-113">createdBy</span></span>|[<span data-ttu-id="7a1b6-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="7a1b6-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="7a1b6-p103">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7a1b6-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="7a1b6-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7a1b6-117">createdDateTime</span></span>|<span data-ttu-id="7a1b6-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7a1b6-118">DateTimeOffset</span></span>|<span data-ttu-id="7a1b6-p104">Дата и время создания раздела. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7a1b6-p104">The date and time when the section was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="7a1b6-123">id</span><span class="sxs-lookup"><span data-stu-id="7a1b6-123">id</span></span>|<span data-ttu-id="7a1b6-124">Строка</span><span class="sxs-lookup"><span data-stu-id="7a1b6-124">String</span></span>|<span data-ttu-id="7a1b6-p105">Уникальный идентификатор раздела.  Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7a1b6-p105">The unique identifier of the section.  Read-only.</span></span>|
|<span data-ttu-id="7a1b6-127">isDefault</span><span class="sxs-lookup"><span data-stu-id="7a1b6-127">isDefault</span></span>|<span data-ttu-id="7a1b6-128">Логический</span><span class="sxs-lookup"><span data-stu-id="7a1b6-128">Boolean</span></span>|<span data-ttu-id="7a1b6-p106">Указывает, является ли этот раздел разделом пользователя по умолчанию. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7a1b6-p106">Indicates whether this is the user's default section. Read-only.</span></span>|
|<span data-ttu-id="7a1b6-131">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="7a1b6-131">lastModifiedBy</span></span>|[<span data-ttu-id="7a1b6-132">identitySet</span><span class="sxs-lookup"><span data-stu-id="7a1b6-132">identitySet</span></span>](identityset.md)|<span data-ttu-id="7a1b6-p107">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7a1b6-p107">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="7a1b6-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7a1b6-135">lastModifiedDateTime</span></span>|<span data-ttu-id="7a1b6-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7a1b6-136">DateTimeOffset</span></span>|<span data-ttu-id="7a1b6-p108">Дата и время последнего изменения раздела. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7a1b6-p108">The date and time when the section was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="7a1b6-141">links</span><span class="sxs-lookup"><span data-stu-id="7a1b6-141">links</span></span>|[<span data-ttu-id="7a1b6-142">SectionLinks</span><span class="sxs-lookup"><span data-stu-id="7a1b6-142">SectionLinks</span></span>](sectionlinks.md)|<span data-ttu-id="7a1b6-p109">Ссылки для открытия раздела. Ссылка `oneNoteClientURL` открывает раздел в клиенте OneNote, если он установлен. Ссылка `oneNoteWebURL` открывает раздел в OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="7a1b6-p109">Links for opening the section. The `oneNoteClientURL` link opens the section in the OneNote native client if it's installed. The `oneNoteWebURL` link opens the section in OneNote Online.</span></span>|
|<span data-ttu-id="7a1b6-146">displayName</span><span class="sxs-lookup"><span data-stu-id="7a1b6-146">displayName</span></span>|<span data-ttu-id="7a1b6-147">Строка</span><span class="sxs-lookup"><span data-stu-id="7a1b6-147">String</span></span>|<span data-ttu-id="7a1b6-148">Имя раздела.</span><span class="sxs-lookup"><span data-stu-id="7a1b6-148">The name of the section.</span></span> |
|<span data-ttu-id="7a1b6-149">pagesUrl</span><span class="sxs-lookup"><span data-stu-id="7a1b6-149">pagesUrl</span></span>|<span data-ttu-id="7a1b6-150">Строка</span><span class="sxs-lookup"><span data-stu-id="7a1b6-150">String</span></span>|<span data-ttu-id="7a1b6-p110">`pages` — конечная точка, в которой можно получить сведения обо всех страницах в разделе. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7a1b6-p110">The `pages` endpoint where you can get details for all the pages in the section. Read-only.</span></span>|
|<span data-ttu-id="7a1b6-153">self</span><span class="sxs-lookup"><span data-stu-id="7a1b6-153">self</span></span>|<span data-ttu-id="7a1b6-154">Строка</span><span class="sxs-lookup"><span data-stu-id="7a1b6-154">String</span></span>|<span data-ttu-id="7a1b6-p111">Конечная точка, в которой можно получить сведения о разделе. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7a1b6-p111">The endpoint where you can get details about the section. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7a1b6-157">Связи</span><span class="sxs-lookup"><span data-stu-id="7a1b6-157">Relationships</span></span>
| <span data-ttu-id="7a1b6-158">Связь</span><span class="sxs-lookup"><span data-stu-id="7a1b6-158">Relationship</span></span> | <span data-ttu-id="7a1b6-159">Тип</span><span class="sxs-lookup"><span data-stu-id="7a1b6-159">Type</span></span>   |<span data-ttu-id="7a1b6-160">Описание</span><span class="sxs-lookup"><span data-stu-id="7a1b6-160">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7a1b6-161">pages</span><span class="sxs-lookup"><span data-stu-id="7a1b6-161">pages</span></span>|<span data-ttu-id="7a1b6-162">[OnenotePage](page.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="7a1b6-162">[OnenotePage](page.md) collection</span></span>|<span data-ttu-id="7a1b6-p112">Коллекция страниц в разделе.  Только для чтения. Допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="7a1b6-p112">The collection of pages in the section.  Read-only. Nullable.</span></span>|
|<span data-ttu-id="7a1b6-166">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="7a1b6-166">parentNotebook</span></span>|[<span data-ttu-id="7a1b6-167">Notebook</span><span class="sxs-lookup"><span data-stu-id="7a1b6-167">Notebook</span></span>](notebook.md)|<span data-ttu-id="7a1b6-p113">Записная книжка, содержащая раздел.  Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7a1b6-p113">The notebook that contains the section.  Read-only.</span></span>|
|<span data-ttu-id="7a1b6-170">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="7a1b6-170">parentSectionGroup</span></span>|[<span data-ttu-id="7a1b6-171">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="7a1b6-171">SectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="7a1b6-p114">Группа объектов, содержащая раздел.  Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7a1b6-p114">The section group that contains the section.  Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="7a1b6-174">Методы</span><span class="sxs-lookup"><span data-stu-id="7a1b6-174">Methods</span></span>

| <span data-ttu-id="7a1b6-175">Метод</span><span class="sxs-lookup"><span data-stu-id="7a1b6-175">Method</span></span>           | <span data-ttu-id="7a1b6-176">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7a1b6-176">Return Type</span></span>    |<span data-ttu-id="7a1b6-177">Описание</span><span class="sxs-lookup"><span data-stu-id="7a1b6-177">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7a1b6-178">Получение раздела</span><span class="sxs-lookup"><span data-stu-id="7a1b6-178">Get section</span></span>](../api/section-get.md) | [<span data-ttu-id="7a1b6-179">OnenoteSection</span><span class="sxs-lookup"><span data-stu-id="7a1b6-179">OnenoteSection</span></span>](section.md) |<span data-ttu-id="7a1b6-180">Чтение свойств и отношений раздела.</span><span class="sxs-lookup"><span data-stu-id="7a1b6-180">Read the properties and relationships of the section.</span></span>|
|[<span data-ttu-id="7a1b6-181">Создание страницы</span><span class="sxs-lookup"><span data-stu-id="7a1b6-181">Create page</span></span>](../api/section-post-pages.md) |[<span data-ttu-id="7a1b6-182">Page</span><span class="sxs-lookup"><span data-stu-id="7a1b6-182">Page</span></span>](page.md)| <span data-ttu-id="7a1b6-183">Создайте страницу, отправив запрос POST в коллекцию pages в указанном разделе.</span><span class="sxs-lookup"><span data-stu-id="7a1b6-183">Create a page by posting to the pages collection in the specified section.</span></span>|
|[<span data-ttu-id="7a1b6-184">Перечисление страниц</span><span class="sxs-lookup"><span data-stu-id="7a1b6-184">List pages</span></span>](../api/section-list-pages.md) |<span data-ttu-id="7a1b6-185">Коллекция объектов [Page](page.md)</span><span class="sxs-lookup"><span data-stu-id="7a1b6-185">[Page](page.md) collection</span></span>| <span data-ttu-id="7a1b6-186">Получение коллекции страниц в указанном разделе.</span><span class="sxs-lookup"><span data-stu-id="7a1b6-186">Get a collection of pages in the specified section.</span></span>|
|[<span data-ttu-id="7a1b6-187">copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="7a1b6-187">copyToNotebook</span></span>](../api/section-copytonotebook.md)|<span data-ttu-id="7a1b6-188">Нет</span><span class="sxs-lookup"><span data-stu-id="7a1b6-188">None</span></span>|<span data-ttu-id="7a1b6-189">Копирование раздела в указанную записную книжку.</span><span class="sxs-lookup"><span data-stu-id="7a1b6-189">Copy the section to a specific notebook.</span></span>|
|[<span data-ttu-id="7a1b6-190">copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="7a1b6-190">copyToSectionGroup</span></span>](../api/section-copytosectiongroup.md)|<span data-ttu-id="7a1b6-191">Нет</span><span class="sxs-lookup"><span data-stu-id="7a1b6-191">None</span></span>|<span data-ttu-id="7a1b6-192">Копирование раздела в указанную группу разделов.</span><span class="sxs-lookup"><span data-stu-id="7a1b6-192">Copy the section to a specific section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteSection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
