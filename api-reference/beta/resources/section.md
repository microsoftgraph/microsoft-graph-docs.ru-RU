---
title: Тип ресурса "раздел"
description: Раздел в записной книжке OneNote. Разделы могут содержать страницы.
localization_priority: Normal
ms.openlocfilehash: faecf31ad09f3ea3b5614480fc051ad1054d442b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562951"
---
# <a name="section-resource-type"></a><span data-ttu-id="c77fb-104">Тип ресурса "раздел"</span><span class="sxs-lookup"><span data-stu-id="c77fb-104">section resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c77fb-105">Раздел в записной книжке OneNote.</span><span class="sxs-lookup"><span data-stu-id="c77fb-105">A section in a OneNote notebook.</span></span> <span data-ttu-id="c77fb-106">Разделы могут содержать страницы.</span><span class="sxs-lookup"><span data-stu-id="c77fb-106">Sections can contain pages.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c77fb-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c77fb-107">JSON representation</span></span>

<span data-ttu-id="c77fb-108">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c77fb-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="c77fb-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="c77fb-109">Properties</span></span>
| <span data-ttu-id="c77fb-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="c77fb-110">Property</span></span>     | <span data-ttu-id="c77fb-111">Тип</span><span class="sxs-lookup"><span data-stu-id="c77fb-111">Type</span></span>   |<span data-ttu-id="c77fb-112">Описание</span><span class="sxs-lookup"><span data-stu-id="c77fb-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c77fb-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="c77fb-113">createdBy</span></span>|[<span data-ttu-id="c77fb-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="c77fb-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="c77fb-p103">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c77fb-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="c77fb-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c77fb-117">createdDateTime</span></span>|<span data-ttu-id="c77fb-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c77fb-118">DateTimeOffset</span></span>|<span data-ttu-id="c77fb-119">Дата и время создания раздела.</span><span class="sxs-lookup"><span data-stu-id="c77fb-119">The date and time when the section was created.</span></span> <span data-ttu-id="c77fb-120">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="c77fb-120">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c77fb-121">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="c77fb-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="c77fb-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c77fb-122">Read-only.</span></span>|
|<span data-ttu-id="c77fb-123">id</span><span class="sxs-lookup"><span data-stu-id="c77fb-123">id</span></span>|<span data-ttu-id="c77fb-124">String</span><span class="sxs-lookup"><span data-stu-id="c77fb-124">String</span></span>|<span data-ttu-id="c77fb-125">Уникальный идентификатор раздела.</span><span class="sxs-lookup"><span data-stu-id="c77fb-125">The unique identifier of the section.</span></span>  <span data-ttu-id="c77fb-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c77fb-126">Read-only.</span></span>|
|<span data-ttu-id="c77fb-127">isDefault</span><span class="sxs-lookup"><span data-stu-id="c77fb-127">isDefault</span></span>|<span data-ttu-id="c77fb-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="c77fb-128">Boolean</span></span>|<span data-ttu-id="c77fb-129">Указывает, является ли этот раздел разделом пользователя по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="c77fb-129">Indicates whether this is the user's default section.</span></span> <span data-ttu-id="c77fb-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c77fb-130">Read-only.</span></span>|
|<span data-ttu-id="c77fb-131">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="c77fb-131">lastModifiedBy</span></span>|[<span data-ttu-id="c77fb-132">identitySet</span><span class="sxs-lookup"><span data-stu-id="c77fb-132">identitySet</span></span>](identityset.md)|<span data-ttu-id="c77fb-p107">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c77fb-p107">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="c77fb-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c77fb-135">lastModifiedDateTime</span></span>|<span data-ttu-id="c77fb-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c77fb-136">DateTimeOffset</span></span>|<span data-ttu-id="c77fb-137">Дата и время последнего изменения раздела.</span><span class="sxs-lookup"><span data-stu-id="c77fb-137">The date and time when the section was last modified.</span></span> <span data-ttu-id="c77fb-138">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="c77fb-138">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c77fb-139">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="c77fb-139">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="c77fb-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c77fb-140">Read-only.</span></span>|
|<span data-ttu-id="c77fb-141">links</span><span class="sxs-lookup"><span data-stu-id="c77fb-141">links</span></span>|[<span data-ttu-id="c77fb-142">Сектионлинкс</span><span class="sxs-lookup"><span data-stu-id="c77fb-142">SectionLinks</span></span>](sectionlinks.md)|<span data-ttu-id="c77fb-143">Ссылки для открытия раздела.</span><span class="sxs-lookup"><span data-stu-id="c77fb-143">Links for opening the section.</span></span> <span data-ttu-id="c77fb-144">`oneNoteClientURL` Ссылка открывает раздел в собственном клиенте OneNote, если он установлен.</span><span class="sxs-lookup"><span data-stu-id="c77fb-144">The `oneNoteClientURL` link opens the section in the OneNote native client if it's installed.</span></span> <span data-ttu-id="c77fb-145">`oneNoteWebURL` Ссылка открывает раздел в OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="c77fb-145">The `oneNoteWebURL` link opens the section in OneNote Online.</span></span>|
|<span data-ttu-id="c77fb-146">displayName</span><span class="sxs-lookup"><span data-stu-id="c77fb-146">displayName</span></span>|<span data-ttu-id="c77fb-147">String</span><span class="sxs-lookup"><span data-stu-id="c77fb-147">String</span></span>|<span data-ttu-id="c77fb-148">Имя раздела.</span><span class="sxs-lookup"><span data-stu-id="c77fb-148">The name of the section.</span></span> |
|<span data-ttu-id="c77fb-149">Ссылки pagesurl</span><span class="sxs-lookup"><span data-stu-id="c77fb-149">pagesUrl</span></span>|<span data-ttu-id="c77fb-150">String</span><span class="sxs-lookup"><span data-stu-id="c77fb-150">String</span></span>|<span data-ttu-id="c77fb-151">Конечная точка, `pages` в которой можно получить сведения обо всех страницах в разделе.</span><span class="sxs-lookup"><span data-stu-id="c77fb-151">The `pages` endpoint where you can get details for all the pages in the section.</span></span> <span data-ttu-id="c77fb-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c77fb-152">Read-only.</span></span>|
|<span data-ttu-id="c77fb-153">Self</span><span class="sxs-lookup"><span data-stu-id="c77fb-153">self</span></span>|<span data-ttu-id="c77fb-154">String</span><span class="sxs-lookup"><span data-stu-id="c77fb-154">String</span></span>|<span data-ttu-id="c77fb-155">Конечная точка, где можно получить сведения о разделе.</span><span class="sxs-lookup"><span data-stu-id="c77fb-155">The endpoint where you can get details about the section.</span></span> <span data-ttu-id="c77fb-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c77fb-156">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c77fb-157">Отношения</span><span class="sxs-lookup"><span data-stu-id="c77fb-157">Relationships</span></span>
| <span data-ttu-id="c77fb-158">Отношение</span><span class="sxs-lookup"><span data-stu-id="c77fb-158">Relationship</span></span> | <span data-ttu-id="c77fb-159">Тип</span><span class="sxs-lookup"><span data-stu-id="c77fb-159">Type</span></span>   |<span data-ttu-id="c77fb-160">Описание</span><span class="sxs-lookup"><span data-stu-id="c77fb-160">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c77fb-161">pages</span><span class="sxs-lookup"><span data-stu-id="c77fb-161">pages</span></span>|<span data-ttu-id="c77fb-162">Коллекция [страниц](page.md)</span><span class="sxs-lookup"><span data-stu-id="c77fb-162">[Page](page.md) collection</span></span>|<span data-ttu-id="c77fb-163">Коллекция страниц в разделе.</span><span class="sxs-lookup"><span data-stu-id="c77fb-163">The collection of pages in the section.</span></span>  <span data-ttu-id="c77fb-164">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c77fb-164">Read-only.</span></span> <span data-ttu-id="c77fb-165">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c77fb-165">Nullable.</span></span>|
|<span data-ttu-id="c77fb-166">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="c77fb-166">parentNotebook</span></span>|[<span data-ttu-id="c77fb-167">Notebook</span><span class="sxs-lookup"><span data-stu-id="c77fb-167">Notebook</span></span>](notebook.md)|<span data-ttu-id="c77fb-168">Записная книжка, содержащая раздел.</span><span class="sxs-lookup"><span data-stu-id="c77fb-168">The notebook that contains the section.</span></span>  <span data-ttu-id="c77fb-169">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c77fb-169">Read-only.</span></span>|
|<span data-ttu-id="c77fb-170">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="c77fb-170">parentSectionGroup</span></span>|[<span data-ttu-id="c77fb-171">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="c77fb-171">SectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="c77fb-172">Группа разделов, содержащая раздел.</span><span class="sxs-lookup"><span data-stu-id="c77fb-172">The section group that contains the section.</span></span>  <span data-ttu-id="c77fb-173">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c77fb-173">Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="c77fb-174">Методы</span><span class="sxs-lookup"><span data-stu-id="c77fb-174">Methods</span></span>

| <span data-ttu-id="c77fb-175">Метод</span><span class="sxs-lookup"><span data-stu-id="c77fb-175">Method</span></span>           | <span data-ttu-id="c77fb-176">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c77fb-176">Return Type</span></span>    |<span data-ttu-id="c77fb-177">Описание</span><span class="sxs-lookup"><span data-stu-id="c77fb-177">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c77fb-178">Получение раздела</span><span class="sxs-lookup"><span data-stu-id="c77fb-178">Get section</span></span>](../api/section-get.md) | [<span data-ttu-id="c77fb-179">Section</span><span class="sxs-lookup"><span data-stu-id="c77fb-179">Section</span></span>](section.md) |<span data-ttu-id="c77fb-180">Прочитайте свойства и связи раздела.</span><span class="sxs-lookup"><span data-stu-id="c77fb-180">Read the properties and relationships of the section.</span></span>|
|[<span data-ttu-id="c77fb-181">Создание страницы</span><span class="sxs-lookup"><span data-stu-id="c77fb-181">Create page</span></span>](../api/section-post-pages.md) |[<span data-ttu-id="c77fb-182">Page</span><span class="sxs-lookup"><span data-stu-id="c77fb-182">Page</span></span>](page.md)| <span data-ttu-id="c77fb-183">Создание страницы путем публикации в коллекции страниц в указанном разделе.</span><span class="sxs-lookup"><span data-stu-id="c77fb-183">Create a page by posting to the pages collection in the specified section.</span></span>|
|[<span data-ttu-id="c77fb-184">Перечисление страниц</span><span class="sxs-lookup"><span data-stu-id="c77fb-184">List pages</span></span>](../api/section-list-pages.md) |<span data-ttu-id="c77fb-185">Коллекция [страниц](page.md)</span><span class="sxs-lookup"><span data-stu-id="c77fb-185">[Page](page.md) collection</span></span>| <span data-ttu-id="c77fb-186">Получение коллекции страниц в указанном разделе.</span><span class="sxs-lookup"><span data-stu-id="c77fb-186">Get a collection of pages in the specified section.</span></span>|
|[<span data-ttu-id="c77fb-187">copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="c77fb-187">copyToNotebook</span></span>](../api/section-copytonotebook.md)|<span data-ttu-id="c77fb-188">Нет</span><span class="sxs-lookup"><span data-stu-id="c77fb-188">None</span></span>|<span data-ttu-id="c77fb-189">Скопируйте раздел в указанную записную книжку.</span><span class="sxs-lookup"><span data-stu-id="c77fb-189">Copy the section to a specific notebook.</span></span>|
|[<span data-ttu-id="c77fb-190">copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="c77fb-190">copyToSectionGroup</span></span>](../api/section-copytosectiongroup.md)|<span data-ttu-id="c77fb-191">Нет</span><span class="sxs-lookup"><span data-stu-id="c77fb-191">None</span></span>|<span data-ttu-id="c77fb-192">Скопируйте раздел в определенную группу разделов.</span><span class="sxs-lookup"><span data-stu-id="c77fb-192">Copy the section to a specific section group.</span></span>|

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
