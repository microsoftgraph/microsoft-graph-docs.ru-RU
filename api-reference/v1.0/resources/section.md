---
title: Тип ресурса "раздел"
description: Раздел в записной книжке OneNote. Разделы могут содержать страницы.
localization_priority: Normal
ms.openlocfilehash: 8cb7869c914d53e92cc62546ef0936ecb70e8735
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2019
ms.locfileid: "35236645"
---
# <a name="section-resource-type"></a><span data-ttu-id="00138-104">Тип ресурса "раздел"</span><span class="sxs-lookup"><span data-stu-id="00138-104">section resource type</span></span>

<span data-ttu-id="00138-105">Раздел в записной книжке OneNote.</span><span class="sxs-lookup"><span data-stu-id="00138-105">A section in a OneNote notebook.</span></span> <span data-ttu-id="00138-106">Разделы могут содержать страницы.</span><span class="sxs-lookup"><span data-stu-id="00138-106">Sections can contain pages.</span></span>

## <a name="json-representation"></a><span data-ttu-id="00138-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="00138-107">JSON representation</span></span>

<span data-ttu-id="00138-108">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="00138-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="00138-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="00138-109">Properties</span></span>
| <span data-ttu-id="00138-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="00138-110">Property</span></span>     | <span data-ttu-id="00138-111">Тип</span><span class="sxs-lookup"><span data-stu-id="00138-111">Type</span></span>   |<span data-ttu-id="00138-112">Описание</span><span class="sxs-lookup"><span data-stu-id="00138-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="00138-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="00138-113">createdBy</span></span>|[<span data-ttu-id="00138-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="00138-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="00138-p103">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="00138-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="00138-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="00138-117">createdDateTime</span></span>|<span data-ttu-id="00138-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00138-118">DateTimeOffset</span></span>|<span data-ttu-id="00138-119">Дата и время создания раздела.</span><span class="sxs-lookup"><span data-stu-id="00138-119">The date and time when the section was created.</span></span> <span data-ttu-id="00138-120">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="00138-120">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="00138-121">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="00138-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="00138-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="00138-122">Read-only.</span></span>|
|<span data-ttu-id="00138-123">id</span><span class="sxs-lookup"><span data-stu-id="00138-123">id</span></span>|<span data-ttu-id="00138-124">String</span><span class="sxs-lookup"><span data-stu-id="00138-124">String</span></span>|<span data-ttu-id="00138-125">Уникальный идентификатор раздела.</span><span class="sxs-lookup"><span data-stu-id="00138-125">The unique identifier of the section.</span></span>  <span data-ttu-id="00138-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="00138-126">Read-only.</span></span>|
|<span data-ttu-id="00138-127">isDefault</span><span class="sxs-lookup"><span data-stu-id="00138-127">isDefault</span></span>|<span data-ttu-id="00138-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="00138-128">Boolean</span></span>|<span data-ttu-id="00138-129">Указывает, является ли этот раздел разделом пользователя по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="00138-129">Indicates whether this is the user's default section.</span></span> <span data-ttu-id="00138-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="00138-130">Read-only.</span></span>|
|<span data-ttu-id="00138-131">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="00138-131">lastModifiedBy</span></span>|[<span data-ttu-id="00138-132">identitySet</span><span class="sxs-lookup"><span data-stu-id="00138-132">identitySet</span></span>](identityset.md)|<span data-ttu-id="00138-p107">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="00138-p107">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="00138-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="00138-135">lastModifiedDateTime</span></span>|<span data-ttu-id="00138-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00138-136">DateTimeOffset</span></span>|<span data-ttu-id="00138-137">Дата и время последнего изменения раздела.</span><span class="sxs-lookup"><span data-stu-id="00138-137">The date and time when the section was last modified.</span></span> <span data-ttu-id="00138-138">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="00138-138">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="00138-139">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="00138-139">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="00138-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="00138-140">Read-only.</span></span>|
|<span data-ttu-id="00138-141">links</span><span class="sxs-lookup"><span data-stu-id="00138-141">links</span></span>|[<span data-ttu-id="00138-142">Сектионлинкс</span><span class="sxs-lookup"><span data-stu-id="00138-142">SectionLinks</span></span>](sectionlinks.md)|<span data-ttu-id="00138-143">Ссылки для открытия раздела.</span><span class="sxs-lookup"><span data-stu-id="00138-143">Links for opening the section.</span></span> <span data-ttu-id="00138-144">`oneNoteClientURL` Ссылка открывает раздел в собственном клиенте OneNote, если он установлен.</span><span class="sxs-lookup"><span data-stu-id="00138-144">The `oneNoteClientURL` link opens the section in the OneNote native client if it's installed.</span></span> <span data-ttu-id="00138-145">`oneNoteWebURL` Ссылка открывает раздел в OneNote в Интернете.</span><span class="sxs-lookup"><span data-stu-id="00138-145">The `oneNoteWebURL` link opens the section in OneNote on the web.</span></span>|
|<span data-ttu-id="00138-146">displayName</span><span class="sxs-lookup"><span data-stu-id="00138-146">displayName</span></span>|<span data-ttu-id="00138-147">Строка</span><span class="sxs-lookup"><span data-stu-id="00138-147">String</span></span>|<span data-ttu-id="00138-148">Имя раздела.</span><span class="sxs-lookup"><span data-stu-id="00138-148">The name of the section.</span></span> |
|<span data-ttu-id="00138-149">Ссылки pagesurl</span><span class="sxs-lookup"><span data-stu-id="00138-149">pagesUrl</span></span>|<span data-ttu-id="00138-150">String</span><span class="sxs-lookup"><span data-stu-id="00138-150">String</span></span>|<span data-ttu-id="00138-151">Конечная точка, `pages` в которой можно получить сведения обо всех страницах в разделе.</span><span class="sxs-lookup"><span data-stu-id="00138-151">The `pages` endpoint where you can get details for all the pages in the section.</span></span> <span data-ttu-id="00138-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="00138-152">Read-only.</span></span>|
|<span data-ttu-id="00138-153">Self</span><span class="sxs-lookup"><span data-stu-id="00138-153">self</span></span>|<span data-ttu-id="00138-154">String</span><span class="sxs-lookup"><span data-stu-id="00138-154">String</span></span>|<span data-ttu-id="00138-155">Конечная точка, где можно получить сведения о разделе.</span><span class="sxs-lookup"><span data-stu-id="00138-155">The endpoint where you can get details about the section.</span></span> <span data-ttu-id="00138-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="00138-156">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="00138-157">Отношения</span><span class="sxs-lookup"><span data-stu-id="00138-157">Relationships</span></span>
| <span data-ttu-id="00138-158">Отношение</span><span class="sxs-lookup"><span data-stu-id="00138-158">Relationship</span></span> | <span data-ttu-id="00138-159">Тип</span><span class="sxs-lookup"><span data-stu-id="00138-159">Type</span></span>   |<span data-ttu-id="00138-160">Описание</span><span class="sxs-lookup"><span data-stu-id="00138-160">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="00138-161">pages</span><span class="sxs-lookup"><span data-stu-id="00138-161">pages</span></span>|<span data-ttu-id="00138-162">Коллекция [OnenotePage](page.md)</span><span class="sxs-lookup"><span data-stu-id="00138-162">[OnenotePage](page.md) collection</span></span>|<span data-ttu-id="00138-163">Коллекция страниц в разделе.</span><span class="sxs-lookup"><span data-stu-id="00138-163">The collection of pages in the section.</span></span>  <span data-ttu-id="00138-164">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="00138-164">Read-only.</span></span> <span data-ttu-id="00138-165">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="00138-165">Nullable.</span></span>|
|<span data-ttu-id="00138-166">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="00138-166">parentNotebook</span></span>|[<span data-ttu-id="00138-167">Notebook</span><span class="sxs-lookup"><span data-stu-id="00138-167">Notebook</span></span>](notebook.md)|<span data-ttu-id="00138-168">Записная книжка, содержащая раздел.</span><span class="sxs-lookup"><span data-stu-id="00138-168">The notebook that contains the section.</span></span>  <span data-ttu-id="00138-169">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="00138-169">Read-only.</span></span>|
|<span data-ttu-id="00138-170">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="00138-170">parentSectionGroup</span></span>|[<span data-ttu-id="00138-171">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="00138-171">SectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="00138-172">Группа разделов, содержащая раздел.</span><span class="sxs-lookup"><span data-stu-id="00138-172">The section group that contains the section.</span></span>  <span data-ttu-id="00138-173">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="00138-173">Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="00138-174">Методы</span><span class="sxs-lookup"><span data-stu-id="00138-174">Methods</span></span>

| <span data-ttu-id="00138-175">Метод</span><span class="sxs-lookup"><span data-stu-id="00138-175">Method</span></span>           | <span data-ttu-id="00138-176">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="00138-176">Return Type</span></span>    |<span data-ttu-id="00138-177">Описание</span><span class="sxs-lookup"><span data-stu-id="00138-177">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="00138-178">Получение раздела</span><span class="sxs-lookup"><span data-stu-id="00138-178">Get section</span></span>](../api/section-get.md) | [<span data-ttu-id="00138-179">Оненотесектион</span><span class="sxs-lookup"><span data-stu-id="00138-179">OnenoteSection</span></span>](section.md) |<span data-ttu-id="00138-180">Прочитайте свойства и связи раздела.</span><span class="sxs-lookup"><span data-stu-id="00138-180">Read the properties and relationships of the section.</span></span>|
|[<span data-ttu-id="00138-181">Создание страницы</span><span class="sxs-lookup"><span data-stu-id="00138-181">Create page</span></span>](../api/section-post-pages.md) |[<span data-ttu-id="00138-182">Page</span><span class="sxs-lookup"><span data-stu-id="00138-182">Page</span></span>](page.md)| <span data-ttu-id="00138-183">Создание страницы путем публикации в коллекции страниц в указанном разделе.</span><span class="sxs-lookup"><span data-stu-id="00138-183">Create a page by posting to the pages collection in the specified section.</span></span>|
|[<span data-ttu-id="00138-184">Перечисление страниц</span><span class="sxs-lookup"><span data-stu-id="00138-184">List pages</span></span>](../api/section-list-pages.md) |<span data-ttu-id="00138-185">Коллекция [Page](page.md)</span><span class="sxs-lookup"><span data-stu-id="00138-185">[Page](page.md) collection</span></span>| <span data-ttu-id="00138-186">Получение коллекции страниц в указанном разделе.</span><span class="sxs-lookup"><span data-stu-id="00138-186">Get a collection of pages in the specified section.</span></span>|
|[<span data-ttu-id="00138-187">copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="00138-187">copyToNotebook</span></span>](../api/section-copytonotebook.md)|<span data-ttu-id="00138-188">Нет</span><span class="sxs-lookup"><span data-stu-id="00138-188">None</span></span>|<span data-ttu-id="00138-189">Скопируйте раздел в указанную записную книжку.</span><span class="sxs-lookup"><span data-stu-id="00138-189">Copy the section to a specific notebook.</span></span>|
|[<span data-ttu-id="00138-190">copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="00138-190">copyToSectionGroup</span></span>](../api/section-copytosectiongroup.md)|<span data-ttu-id="00138-191">Нет</span><span class="sxs-lookup"><span data-stu-id="00138-191">None</span></span>|<span data-ttu-id="00138-192">Скопируйте раздел в определенную группу разделов.</span><span class="sxs-lookup"><span data-stu-id="00138-192">Copy the section to a specific section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteSection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
