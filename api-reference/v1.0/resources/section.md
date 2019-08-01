---
title: Тип ресурса "раздел"
description: Раздел в записной книжке OneNote. Разделы могут содержать страницы.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 3246cd861d61130ea83ab8a02886a9f281603398
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034568"
---
# <a name="section-resource-type"></a><span data-ttu-id="5cfde-104">Тип ресурса "раздел"</span><span class="sxs-lookup"><span data-stu-id="5cfde-104">section resource type</span></span>

<span data-ttu-id="5cfde-105">Раздел в записной книжке OneNote.</span><span class="sxs-lookup"><span data-stu-id="5cfde-105">A section in a OneNote notebook.</span></span> <span data-ttu-id="5cfde-106">Разделы могут содержать страницы.</span><span class="sxs-lookup"><span data-stu-id="5cfde-106">Sections can contain pages.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5cfde-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5cfde-107">JSON representation</span></span>

<span data-ttu-id="5cfde-108">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5cfde-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="5cfde-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="5cfde-109">Properties</span></span>
| <span data-ttu-id="5cfde-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="5cfde-110">Property</span></span>     | <span data-ttu-id="5cfde-111">Тип</span><span class="sxs-lookup"><span data-stu-id="5cfde-111">Type</span></span>   |<span data-ttu-id="5cfde-112">Описание</span><span class="sxs-lookup"><span data-stu-id="5cfde-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5cfde-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="5cfde-113">createdBy</span></span>|[<span data-ttu-id="5cfde-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="5cfde-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="5cfde-p103">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5cfde-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="5cfde-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5cfde-117">createdDateTime</span></span>|<span data-ttu-id="5cfde-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5cfde-118">DateTimeOffset</span></span>|<span data-ttu-id="5cfde-119">Дата и время создания раздела.</span><span class="sxs-lookup"><span data-stu-id="5cfde-119">The date and time when the section was created.</span></span> <span data-ttu-id="5cfde-120">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="5cfde-120">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5cfde-121">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="5cfde-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="5cfde-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5cfde-122">Read-only.</span></span>|
|<span data-ttu-id="5cfde-123">id</span><span class="sxs-lookup"><span data-stu-id="5cfde-123">id</span></span>|<span data-ttu-id="5cfde-124">String</span><span class="sxs-lookup"><span data-stu-id="5cfde-124">String</span></span>|<span data-ttu-id="5cfde-125">Уникальный идентификатор раздела.</span><span class="sxs-lookup"><span data-stu-id="5cfde-125">The unique identifier of the section.</span></span>  <span data-ttu-id="5cfde-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5cfde-126">Read-only.</span></span>|
|<span data-ttu-id="5cfde-127">isDefault</span><span class="sxs-lookup"><span data-stu-id="5cfde-127">isDefault</span></span>|<span data-ttu-id="5cfde-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="5cfde-128">Boolean</span></span>|<span data-ttu-id="5cfde-129">Указывает, является ли этот раздел разделом пользователя по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5cfde-129">Indicates whether this is the user's default section.</span></span> <span data-ttu-id="5cfde-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5cfde-130">Read-only.</span></span>|
|<span data-ttu-id="5cfde-131">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="5cfde-131">lastModifiedBy</span></span>|[<span data-ttu-id="5cfde-132">identitySet</span><span class="sxs-lookup"><span data-stu-id="5cfde-132">identitySet</span></span>](identityset.md)|<span data-ttu-id="5cfde-p107">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5cfde-p107">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="5cfde-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5cfde-135">lastModifiedDateTime</span></span>|<span data-ttu-id="5cfde-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5cfde-136">DateTimeOffset</span></span>|<span data-ttu-id="5cfde-137">Дата и время последнего изменения раздела.</span><span class="sxs-lookup"><span data-stu-id="5cfde-137">The date and time when the section was last modified.</span></span> <span data-ttu-id="5cfde-138">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="5cfde-138">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5cfde-139">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="5cfde-139">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="5cfde-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5cfde-140">Read-only.</span></span>|
|<span data-ttu-id="5cfde-141">links</span><span class="sxs-lookup"><span data-stu-id="5cfde-141">links</span></span>|[<span data-ttu-id="5cfde-142">Сектионлинкс</span><span class="sxs-lookup"><span data-stu-id="5cfde-142">SectionLinks</span></span>](sectionlinks.md)|<span data-ttu-id="5cfde-143">Ссылки для открытия раздела.</span><span class="sxs-lookup"><span data-stu-id="5cfde-143">Links for opening the section.</span></span> <span data-ttu-id="5cfde-144">`oneNoteClientURL` Ссылка открывает раздел в собственном клиенте OneNote, если он установлен.</span><span class="sxs-lookup"><span data-stu-id="5cfde-144">The `oneNoteClientURL` link opens the section in the OneNote native client if it's installed.</span></span> <span data-ttu-id="5cfde-145">`oneNoteWebURL` Ссылка открывает раздел в OneNote в Интернете.</span><span class="sxs-lookup"><span data-stu-id="5cfde-145">The `oneNoteWebURL` link opens the section in OneNote on the web.</span></span>|
|<span data-ttu-id="5cfde-146">displayName</span><span class="sxs-lookup"><span data-stu-id="5cfde-146">displayName</span></span>|<span data-ttu-id="5cfde-147">Строка</span><span class="sxs-lookup"><span data-stu-id="5cfde-147">String</span></span>|<span data-ttu-id="5cfde-148">Имя раздела.</span><span class="sxs-lookup"><span data-stu-id="5cfde-148">The name of the section.</span></span> |
|<span data-ttu-id="5cfde-149">Ссылки pagesurl</span><span class="sxs-lookup"><span data-stu-id="5cfde-149">pagesUrl</span></span>|<span data-ttu-id="5cfde-150">String</span><span class="sxs-lookup"><span data-stu-id="5cfde-150">String</span></span>|<span data-ttu-id="5cfde-151">Конечная точка, `pages` в которой можно получить сведения обо всех страницах в разделе.</span><span class="sxs-lookup"><span data-stu-id="5cfde-151">The `pages` endpoint where you can get details for all the pages in the section.</span></span> <span data-ttu-id="5cfde-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5cfde-152">Read-only.</span></span>|
|<span data-ttu-id="5cfde-153">Self</span><span class="sxs-lookup"><span data-stu-id="5cfde-153">self</span></span>|<span data-ttu-id="5cfde-154">String</span><span class="sxs-lookup"><span data-stu-id="5cfde-154">String</span></span>|<span data-ttu-id="5cfde-155">Конечная точка, где можно получить сведения о разделе.</span><span class="sxs-lookup"><span data-stu-id="5cfde-155">The endpoint where you can get details about the section.</span></span> <span data-ttu-id="5cfde-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5cfde-156">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5cfde-157">Отношения</span><span class="sxs-lookup"><span data-stu-id="5cfde-157">Relationships</span></span>
| <span data-ttu-id="5cfde-158">Отношение</span><span class="sxs-lookup"><span data-stu-id="5cfde-158">Relationship</span></span> | <span data-ttu-id="5cfde-159">Тип</span><span class="sxs-lookup"><span data-stu-id="5cfde-159">Type</span></span>   |<span data-ttu-id="5cfde-160">Описание</span><span class="sxs-lookup"><span data-stu-id="5cfde-160">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5cfde-161">pages</span><span class="sxs-lookup"><span data-stu-id="5cfde-161">pages</span></span>|<span data-ttu-id="5cfde-162">Коллекция [OnenotePage](page.md)</span><span class="sxs-lookup"><span data-stu-id="5cfde-162">[OnenotePage](page.md) collection</span></span>|<span data-ttu-id="5cfde-163">Коллекция страниц в разделе.</span><span class="sxs-lookup"><span data-stu-id="5cfde-163">The collection of pages in the section.</span></span>  <span data-ttu-id="5cfde-164">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5cfde-164">Read-only.</span></span> <span data-ttu-id="5cfde-165">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="5cfde-165">Nullable.</span></span>|
|<span data-ttu-id="5cfde-166">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="5cfde-166">parentNotebook</span></span>|[<span data-ttu-id="5cfde-167">Notebook</span><span class="sxs-lookup"><span data-stu-id="5cfde-167">Notebook</span></span>](notebook.md)|<span data-ttu-id="5cfde-168">Записная книжка, содержащая раздел.</span><span class="sxs-lookup"><span data-stu-id="5cfde-168">The notebook that contains the section.</span></span>  <span data-ttu-id="5cfde-169">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5cfde-169">Read-only.</span></span>|
|<span data-ttu-id="5cfde-170">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="5cfde-170">parentSectionGroup</span></span>|[<span data-ttu-id="5cfde-171">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="5cfde-171">SectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="5cfde-172">Группа разделов, содержащая раздел.</span><span class="sxs-lookup"><span data-stu-id="5cfde-172">The section group that contains the section.</span></span>  <span data-ttu-id="5cfde-173">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5cfde-173">Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="5cfde-174">Методы</span><span class="sxs-lookup"><span data-stu-id="5cfde-174">Methods</span></span>

| <span data-ttu-id="5cfde-175">Метод</span><span class="sxs-lookup"><span data-stu-id="5cfde-175">Method</span></span>           | <span data-ttu-id="5cfde-176">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5cfde-176">Return Type</span></span>    |<span data-ttu-id="5cfde-177">Описание</span><span class="sxs-lookup"><span data-stu-id="5cfde-177">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5cfde-178">Получение раздела</span><span class="sxs-lookup"><span data-stu-id="5cfde-178">Get section</span></span>](../api/section-get.md) | [<span data-ttu-id="5cfde-179">Оненотесектион</span><span class="sxs-lookup"><span data-stu-id="5cfde-179">OnenoteSection</span></span>](section.md) |<span data-ttu-id="5cfde-180">Прочитайте свойства и связи раздела.</span><span class="sxs-lookup"><span data-stu-id="5cfde-180">Read the properties and relationships of the section.</span></span>|
|[<span data-ttu-id="5cfde-181">Создание страницы</span><span class="sxs-lookup"><span data-stu-id="5cfde-181">Create page</span></span>](../api/section-post-pages.md) |[<span data-ttu-id="5cfde-182">Page</span><span class="sxs-lookup"><span data-stu-id="5cfde-182">Page</span></span>](page.md)| <span data-ttu-id="5cfde-183">Создание страницы путем публикации в коллекции страниц в указанном разделе.</span><span class="sxs-lookup"><span data-stu-id="5cfde-183">Create a page by posting to the pages collection in the specified section.</span></span>|
|[<span data-ttu-id="5cfde-184">Перечисление страниц</span><span class="sxs-lookup"><span data-stu-id="5cfde-184">List pages</span></span>](../api/section-list-pages.md) |<span data-ttu-id="5cfde-185">Коллекция [Page](page.md)</span><span class="sxs-lookup"><span data-stu-id="5cfde-185">[Page](page.md) collection</span></span>| <span data-ttu-id="5cfde-186">Получение коллекции страниц в указанном разделе.</span><span class="sxs-lookup"><span data-stu-id="5cfde-186">Get a collection of pages in the specified section.</span></span>|
|[<span data-ttu-id="5cfde-187">copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="5cfde-187">copyToNotebook</span></span>](../api/section-copytonotebook.md)|<span data-ttu-id="5cfde-188">Нет</span><span class="sxs-lookup"><span data-stu-id="5cfde-188">None</span></span>|<span data-ttu-id="5cfde-189">Скопируйте раздел в указанную записную книжку.</span><span class="sxs-lookup"><span data-stu-id="5cfde-189">Copy the section to a specific notebook.</span></span>|
|[<span data-ttu-id="5cfde-190">copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="5cfde-190">copyToSectionGroup</span></span>](../api/section-copytosectiongroup.md)|<span data-ttu-id="5cfde-191">Нет</span><span class="sxs-lookup"><span data-stu-id="5cfde-191">None</span></span>|<span data-ttu-id="5cfde-192">Скопируйте раздел в определенную группу разделов.</span><span class="sxs-lookup"><span data-stu-id="5cfde-192">Copy the section to a specific section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteSection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
