---
title: Тип ресурса "раздел"
description: Раздел в записной книжке OneNote. Разделы могут содержать страницы.
localization_priority: Normal
ms.openlocfilehash: f9cb5a8e3ddf9cf4a045103e4ecc7909653d797c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579159"
---
# <a name="section-resource-type"></a><span data-ttu-id="470ac-104">Тип ресурса "раздел"</span><span class="sxs-lookup"><span data-stu-id="470ac-104">section resource type</span></span>

<span data-ttu-id="470ac-105">Раздел в записной книжке OneNote.</span><span class="sxs-lookup"><span data-stu-id="470ac-105">A section in a OneNote notebook.</span></span> <span data-ttu-id="470ac-106">Разделы могут содержать страницы.</span><span class="sxs-lookup"><span data-stu-id="470ac-106">Sections can contain pages.</span></span>

## <a name="json-representation"></a><span data-ttu-id="470ac-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="470ac-107">JSON representation</span></span>

<span data-ttu-id="470ac-108">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="470ac-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="470ac-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="470ac-109">Properties</span></span>
| <span data-ttu-id="470ac-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="470ac-110">Property</span></span>     | <span data-ttu-id="470ac-111">Тип</span><span class="sxs-lookup"><span data-stu-id="470ac-111">Type</span></span>   |<span data-ttu-id="470ac-112">Описание</span><span class="sxs-lookup"><span data-stu-id="470ac-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="470ac-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="470ac-113">createdBy</span></span>|[<span data-ttu-id="470ac-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="470ac-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="470ac-p103">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="470ac-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="470ac-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="470ac-117">createdDateTime</span></span>|<span data-ttu-id="470ac-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="470ac-118">DateTimeOffset</span></span>|<span data-ttu-id="470ac-119">Дата и время создания раздела.</span><span class="sxs-lookup"><span data-stu-id="470ac-119">The date and time when the section was created.</span></span> <span data-ttu-id="470ac-120">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="470ac-120">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="470ac-121">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="470ac-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="470ac-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="470ac-122">Read-only.</span></span>|
|<span data-ttu-id="470ac-123">id</span><span class="sxs-lookup"><span data-stu-id="470ac-123">id</span></span>|<span data-ttu-id="470ac-124">String</span><span class="sxs-lookup"><span data-stu-id="470ac-124">String</span></span>|<span data-ttu-id="470ac-125">Уникальный идентификатор раздела.</span><span class="sxs-lookup"><span data-stu-id="470ac-125">The unique identifier of the section.</span></span>  <span data-ttu-id="470ac-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="470ac-126">Read-only.</span></span>|
|<span data-ttu-id="470ac-127">isDefault</span><span class="sxs-lookup"><span data-stu-id="470ac-127">isDefault</span></span>|<span data-ttu-id="470ac-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="470ac-128">Boolean</span></span>|<span data-ttu-id="470ac-129">Указывает, является ли этот раздел разделом пользователя по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="470ac-129">Indicates whether this is the user's default section.</span></span> <span data-ttu-id="470ac-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="470ac-130">Read-only.</span></span>|
|<span data-ttu-id="470ac-131">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="470ac-131">lastModifiedBy</span></span>|[<span data-ttu-id="470ac-132">identitySet</span><span class="sxs-lookup"><span data-stu-id="470ac-132">identitySet</span></span>](identityset.md)|<span data-ttu-id="470ac-p107">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="470ac-p107">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="470ac-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="470ac-135">lastModifiedDateTime</span></span>|<span data-ttu-id="470ac-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="470ac-136">DateTimeOffset</span></span>|<span data-ttu-id="470ac-137">Дата и время последнего изменения раздела.</span><span class="sxs-lookup"><span data-stu-id="470ac-137">The date and time when the section was last modified.</span></span> <span data-ttu-id="470ac-138">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="470ac-138">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="470ac-139">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="470ac-139">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="470ac-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="470ac-140">Read-only.</span></span>|
|<span data-ttu-id="470ac-141">links</span><span class="sxs-lookup"><span data-stu-id="470ac-141">links</span></span>|[<span data-ttu-id="470ac-142">Сектионлинкс</span><span class="sxs-lookup"><span data-stu-id="470ac-142">SectionLinks</span></span>](sectionlinks.md)|<span data-ttu-id="470ac-143">Ссылки для открытия раздела.</span><span class="sxs-lookup"><span data-stu-id="470ac-143">Links for opening the section.</span></span> <span data-ttu-id="470ac-144">`oneNoteClientURL` Ссылка открывает раздел в собственном клиенте OneNote, если он установлен.</span><span class="sxs-lookup"><span data-stu-id="470ac-144">The `oneNoteClientURL` link opens the section in the OneNote native client if it's installed.</span></span> <span data-ttu-id="470ac-145">`oneNoteWebURL` Ссылка открывает раздел в OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="470ac-145">The `oneNoteWebURL` link opens the section in OneNote Online.</span></span>|
|<span data-ttu-id="470ac-146">displayName</span><span class="sxs-lookup"><span data-stu-id="470ac-146">displayName</span></span>|<span data-ttu-id="470ac-147">String</span><span class="sxs-lookup"><span data-stu-id="470ac-147">String</span></span>|<span data-ttu-id="470ac-148">Имя раздела.</span><span class="sxs-lookup"><span data-stu-id="470ac-148">The name of the section.</span></span> |
|<span data-ttu-id="470ac-149">Ссылки pagesurl</span><span class="sxs-lookup"><span data-stu-id="470ac-149">pagesUrl</span></span>|<span data-ttu-id="470ac-150">String</span><span class="sxs-lookup"><span data-stu-id="470ac-150">String</span></span>|<span data-ttu-id="470ac-151">Конечная точка, `pages` в которой можно получить сведения обо всех страницах в разделе.</span><span class="sxs-lookup"><span data-stu-id="470ac-151">The `pages` endpoint where you can get details for all the pages in the section.</span></span> <span data-ttu-id="470ac-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="470ac-152">Read-only.</span></span>|
|<span data-ttu-id="470ac-153">Self</span><span class="sxs-lookup"><span data-stu-id="470ac-153">self</span></span>|<span data-ttu-id="470ac-154">String</span><span class="sxs-lookup"><span data-stu-id="470ac-154">String</span></span>|<span data-ttu-id="470ac-155">Конечная точка, где можно получить сведения о разделе.</span><span class="sxs-lookup"><span data-stu-id="470ac-155">The endpoint where you can get details about the section.</span></span> <span data-ttu-id="470ac-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="470ac-156">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="470ac-157">Отношения</span><span class="sxs-lookup"><span data-stu-id="470ac-157">Relationships</span></span>
| <span data-ttu-id="470ac-158">Отношение</span><span class="sxs-lookup"><span data-stu-id="470ac-158">Relationship</span></span> | <span data-ttu-id="470ac-159">Тип</span><span class="sxs-lookup"><span data-stu-id="470ac-159">Type</span></span>   |<span data-ttu-id="470ac-160">Описание</span><span class="sxs-lookup"><span data-stu-id="470ac-160">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="470ac-161">pages</span><span class="sxs-lookup"><span data-stu-id="470ac-161">pages</span></span>|<span data-ttu-id="470ac-162">Коллекция [оненотепаже](page.md)</span><span class="sxs-lookup"><span data-stu-id="470ac-162">[OnenotePage](page.md) collection</span></span>|<span data-ttu-id="470ac-163">Коллекция страниц в разделе.</span><span class="sxs-lookup"><span data-stu-id="470ac-163">The collection of pages in the section.</span></span>  <span data-ttu-id="470ac-164">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="470ac-164">Read-only.</span></span> <span data-ttu-id="470ac-165">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="470ac-165">Nullable.</span></span>|
|<span data-ttu-id="470ac-166">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="470ac-166">parentNotebook</span></span>|[<span data-ttu-id="470ac-167">Notebook</span><span class="sxs-lookup"><span data-stu-id="470ac-167">Notebook</span></span>](notebook.md)|<span data-ttu-id="470ac-168">Записная книжка, содержащая раздел.</span><span class="sxs-lookup"><span data-stu-id="470ac-168">The notebook that contains the section.</span></span>  <span data-ttu-id="470ac-169">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="470ac-169">Read-only.</span></span>|
|<span data-ttu-id="470ac-170">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="470ac-170">parentSectionGroup</span></span>|[<span data-ttu-id="470ac-171">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="470ac-171">SectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="470ac-172">Группа разделов, содержащая раздел.</span><span class="sxs-lookup"><span data-stu-id="470ac-172">The section group that contains the section.</span></span>  <span data-ttu-id="470ac-173">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="470ac-173">Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="470ac-174">Методы</span><span class="sxs-lookup"><span data-stu-id="470ac-174">Methods</span></span>

| <span data-ttu-id="470ac-175">Метод</span><span class="sxs-lookup"><span data-stu-id="470ac-175">Method</span></span>           | <span data-ttu-id="470ac-176">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="470ac-176">Return Type</span></span>    |<span data-ttu-id="470ac-177">Описание</span><span class="sxs-lookup"><span data-stu-id="470ac-177">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="470ac-178">Получение раздела</span><span class="sxs-lookup"><span data-stu-id="470ac-178">Get section</span></span>](../api/section-get.md) | [<span data-ttu-id="470ac-179">Оненотесектион</span><span class="sxs-lookup"><span data-stu-id="470ac-179">OnenoteSection</span></span>](section.md) |<span data-ttu-id="470ac-180">Прочитайте свойства и связи раздела.</span><span class="sxs-lookup"><span data-stu-id="470ac-180">Read the properties and relationships of the section.</span></span>|
|[<span data-ttu-id="470ac-181">Создание страницы</span><span class="sxs-lookup"><span data-stu-id="470ac-181">Create page</span></span>](../api/section-post-pages.md) |[<span data-ttu-id="470ac-182">Page</span><span class="sxs-lookup"><span data-stu-id="470ac-182">Page</span></span>](page.md)| <span data-ttu-id="470ac-183">Создание страницы путем публикации в коллекции страниц в указанном разделе.</span><span class="sxs-lookup"><span data-stu-id="470ac-183">Create a page by posting to the pages collection in the specified section.</span></span>|
|[<span data-ttu-id="470ac-184">Перечисление страниц</span><span class="sxs-lookup"><span data-stu-id="470ac-184">List pages</span></span>](../api/section-list-pages.md) |<span data-ttu-id="470ac-185">Коллекция [страниц](page.md)</span><span class="sxs-lookup"><span data-stu-id="470ac-185">[Page](page.md) collection</span></span>| <span data-ttu-id="470ac-186">Получение коллекции страниц в указанном разделе.</span><span class="sxs-lookup"><span data-stu-id="470ac-186">Get a collection of pages in the specified section.</span></span>|
|[<span data-ttu-id="470ac-187">copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="470ac-187">copyToNotebook</span></span>](../api/section-copytonotebook.md)|<span data-ttu-id="470ac-188">Нет</span><span class="sxs-lookup"><span data-stu-id="470ac-188">None</span></span>|<span data-ttu-id="470ac-189">Скопируйте раздел в указанную записную книжку.</span><span class="sxs-lookup"><span data-stu-id="470ac-189">Copy the section to a specific notebook.</span></span>|
|[<span data-ttu-id="470ac-190">copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="470ac-190">copyToSectionGroup</span></span>](../api/section-copytosectiongroup.md)|<span data-ttu-id="470ac-191">Нет</span><span class="sxs-lookup"><span data-stu-id="470ac-191">None</span></span>|<span data-ttu-id="470ac-192">Скопируйте раздел в определенную группу разделов.</span><span class="sxs-lookup"><span data-stu-id="470ac-192">Copy the section to a specific section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteSection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
