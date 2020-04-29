---
title: Тип ресурса "раздел"
description: Раздел в записной книжке OneNote. Разделы могут содержать страницы.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a701fbe2cea27db97bb7d95911c0c0ee1140b55c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533783"
---
# <a name="section-resource-type"></a><span data-ttu-id="b8c22-104">Тип ресурса "раздел"</span><span class="sxs-lookup"><span data-stu-id="b8c22-104">section resource type</span></span>

<span data-ttu-id="b8c22-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8c22-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b8c22-106">Раздел в записной книжке OneNote.</span><span class="sxs-lookup"><span data-stu-id="b8c22-106">A section in a OneNote notebook.</span></span> <span data-ttu-id="b8c22-107">Разделы могут содержать страницы.</span><span class="sxs-lookup"><span data-stu-id="b8c22-107">Sections can contain pages.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b8c22-108">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b8c22-108">JSON representation</span></span>

<span data-ttu-id="b8c22-109">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b8c22-109">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="b8c22-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="b8c22-110">Properties</span></span>
| <span data-ttu-id="b8c22-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="b8c22-111">Property</span></span>     | <span data-ttu-id="b8c22-112">Тип</span><span class="sxs-lookup"><span data-stu-id="b8c22-112">Type</span></span>   |<span data-ttu-id="b8c22-113">Описание</span><span class="sxs-lookup"><span data-stu-id="b8c22-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b8c22-114">createdBy</span><span class="sxs-lookup"><span data-stu-id="b8c22-114">createdBy</span></span>|[<span data-ttu-id="b8c22-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="b8c22-115">identitySet</span></span>](identityset.md)|<span data-ttu-id="b8c22-p103">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8c22-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="b8c22-118">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b8c22-118">createdDateTime</span></span>|<span data-ttu-id="b8c22-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8c22-119">DateTimeOffset</span></span>|<span data-ttu-id="b8c22-120">Дата и время создания раздела.</span><span class="sxs-lookup"><span data-stu-id="b8c22-120">The date and time when the section was created.</span></span> <span data-ttu-id="b8c22-121">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="b8c22-121">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b8c22-122">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="b8c22-122">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="b8c22-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8c22-123">Read-only.</span></span>|
|<span data-ttu-id="b8c22-124">id</span><span class="sxs-lookup"><span data-stu-id="b8c22-124">id</span></span>|<span data-ttu-id="b8c22-125">String</span><span class="sxs-lookup"><span data-stu-id="b8c22-125">String</span></span>|<span data-ttu-id="b8c22-126">Уникальный идентификатор раздела.</span><span class="sxs-lookup"><span data-stu-id="b8c22-126">The unique identifier of the section.</span></span>  <span data-ttu-id="b8c22-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8c22-127">Read-only.</span></span>|
|<span data-ttu-id="b8c22-128">isDefault</span><span class="sxs-lookup"><span data-stu-id="b8c22-128">isDefault</span></span>|<span data-ttu-id="b8c22-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="b8c22-129">Boolean</span></span>|<span data-ttu-id="b8c22-130">Указывает, является ли этот раздел разделом пользователя по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b8c22-130">Indicates whether this is the user's default section.</span></span> <span data-ttu-id="b8c22-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8c22-131">Read-only.</span></span>|
|<span data-ttu-id="b8c22-132">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="b8c22-132">lastModifiedBy</span></span>|[<span data-ttu-id="b8c22-133">identitySet</span><span class="sxs-lookup"><span data-stu-id="b8c22-133">identitySet</span></span>](identityset.md)|<span data-ttu-id="b8c22-p107">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8c22-p107">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="b8c22-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b8c22-136">lastModifiedDateTime</span></span>|<span data-ttu-id="b8c22-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8c22-137">DateTimeOffset</span></span>|<span data-ttu-id="b8c22-138">Дата и время последнего изменения раздела.</span><span class="sxs-lookup"><span data-stu-id="b8c22-138">The date and time when the section was last modified.</span></span> <span data-ttu-id="b8c22-139">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="b8c22-139">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b8c22-140">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="b8c22-140">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="b8c22-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8c22-141">Read-only.</span></span>|
|<span data-ttu-id="b8c22-142">links</span><span class="sxs-lookup"><span data-stu-id="b8c22-142">links</span></span>|[<span data-ttu-id="b8c22-143">сектионлинкс</span><span class="sxs-lookup"><span data-stu-id="b8c22-143">SectionLinks</span></span>](sectionlinks.md)|<span data-ttu-id="b8c22-144">Ссылки для открытия раздела.</span><span class="sxs-lookup"><span data-stu-id="b8c22-144">Links for opening the section.</span></span> <span data-ttu-id="b8c22-145">`oneNoteClientURL` Ссылка открывает раздел в собственном клиенте OneNote, если он установлен.</span><span class="sxs-lookup"><span data-stu-id="b8c22-145">The `oneNoteClientURL` link opens the section in the OneNote native client if it's installed.</span></span> <span data-ttu-id="b8c22-146">`oneNoteWebURL` Ссылка открывает раздел в OneNote в Интернете.</span><span class="sxs-lookup"><span data-stu-id="b8c22-146">The `oneNoteWebURL` link opens the section in OneNote on the web.</span></span>|
|<span data-ttu-id="b8c22-147">displayName</span><span class="sxs-lookup"><span data-stu-id="b8c22-147">displayName</span></span>|<span data-ttu-id="b8c22-148">Строка</span><span class="sxs-lookup"><span data-stu-id="b8c22-148">String</span></span>|<span data-ttu-id="b8c22-149">Имя раздела.</span><span class="sxs-lookup"><span data-stu-id="b8c22-149">The name of the section.</span></span> |
|<span data-ttu-id="b8c22-150">Ссылки pagesurl</span><span class="sxs-lookup"><span data-stu-id="b8c22-150">pagesUrl</span></span>|<span data-ttu-id="b8c22-151">String</span><span class="sxs-lookup"><span data-stu-id="b8c22-151">String</span></span>|<span data-ttu-id="b8c22-152">Конечная точка, `pages` в которой можно получить сведения обо всех страницах в разделе.</span><span class="sxs-lookup"><span data-stu-id="b8c22-152">The `pages` endpoint where you can get details for all the pages in the section.</span></span> <span data-ttu-id="b8c22-153">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8c22-153">Read-only.</span></span>|
|<span data-ttu-id="b8c22-154">Self</span><span class="sxs-lookup"><span data-stu-id="b8c22-154">self</span></span>|<span data-ttu-id="b8c22-155">String</span><span class="sxs-lookup"><span data-stu-id="b8c22-155">String</span></span>|<span data-ttu-id="b8c22-156">Конечная точка, где можно получить сведения о разделе.</span><span class="sxs-lookup"><span data-stu-id="b8c22-156">The endpoint where you can get details about the section.</span></span> <span data-ttu-id="b8c22-157">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8c22-157">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8c22-158">Отношения</span><span class="sxs-lookup"><span data-stu-id="b8c22-158">Relationships</span></span>
| <span data-ttu-id="b8c22-159">Связь</span><span class="sxs-lookup"><span data-stu-id="b8c22-159">Relationship</span></span> | <span data-ttu-id="b8c22-160">Тип</span><span class="sxs-lookup"><span data-stu-id="b8c22-160">Type</span></span>   |<span data-ttu-id="b8c22-161">Описание</span><span class="sxs-lookup"><span data-stu-id="b8c22-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b8c22-162">pages</span><span class="sxs-lookup"><span data-stu-id="b8c22-162">pages</span></span>|<span data-ttu-id="b8c22-163">Коллекция [OnenotePage](page.md)</span><span class="sxs-lookup"><span data-stu-id="b8c22-163">[OnenotePage](page.md) collection</span></span>|<span data-ttu-id="b8c22-164">Коллекция страниц в разделе.</span><span class="sxs-lookup"><span data-stu-id="b8c22-164">The collection of pages in the section.</span></span>  <span data-ttu-id="b8c22-165">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8c22-165">Read-only.</span></span> <span data-ttu-id="b8c22-166">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="b8c22-166">Nullable.</span></span>|
|<span data-ttu-id="b8c22-167">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="b8c22-167">parentNotebook</span></span>|[<span data-ttu-id="b8c22-168">Notebook</span><span class="sxs-lookup"><span data-stu-id="b8c22-168">Notebook</span></span>](notebook.md)|<span data-ttu-id="b8c22-169">Записная книжка, содержащая раздел.</span><span class="sxs-lookup"><span data-stu-id="b8c22-169">The notebook that contains the section.</span></span>  <span data-ttu-id="b8c22-170">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8c22-170">Read-only.</span></span>|
|<span data-ttu-id="b8c22-171">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="b8c22-171">parentSectionGroup</span></span>|[<span data-ttu-id="b8c22-172">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="b8c22-172">SectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="b8c22-173">Группа разделов, содержащая раздел.</span><span class="sxs-lookup"><span data-stu-id="b8c22-173">The section group that contains the section.</span></span>  <span data-ttu-id="b8c22-174">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8c22-174">Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="b8c22-175">Методы</span><span class="sxs-lookup"><span data-stu-id="b8c22-175">Methods</span></span>

| <span data-ttu-id="b8c22-176">Метод</span><span class="sxs-lookup"><span data-stu-id="b8c22-176">Method</span></span>           | <span data-ttu-id="b8c22-177">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b8c22-177">Return Type</span></span>    |<span data-ttu-id="b8c22-178">Описание</span><span class="sxs-lookup"><span data-stu-id="b8c22-178">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b8c22-179">Получение раздела</span><span class="sxs-lookup"><span data-stu-id="b8c22-179">Get section</span></span>](../api/section-get.md) | [<span data-ttu-id="b8c22-180">оненотесектион</span><span class="sxs-lookup"><span data-stu-id="b8c22-180">OnenoteSection</span></span>](section.md) |<span data-ttu-id="b8c22-181">Прочитайте свойства и связи раздела.</span><span class="sxs-lookup"><span data-stu-id="b8c22-181">Read the properties and relationships of the section.</span></span>|
|[<span data-ttu-id="b8c22-182">Создание страницы</span><span class="sxs-lookup"><span data-stu-id="b8c22-182">Create page</span></span>](../api/section-post-pages.md) |[<span data-ttu-id="b8c22-183">Page</span><span class="sxs-lookup"><span data-stu-id="b8c22-183">Page</span></span>](page.md)| <span data-ttu-id="b8c22-184">Создание страницы путем публикации в коллекции страниц в указанном разделе.</span><span class="sxs-lookup"><span data-stu-id="b8c22-184">Create a page by posting to the pages collection in the specified section.</span></span>|
|[<span data-ttu-id="b8c22-185">Перечисление страниц</span><span class="sxs-lookup"><span data-stu-id="b8c22-185">List pages</span></span>](../api/section-list-pages.md) |<span data-ttu-id="b8c22-186">Коллекция [Page](page.md)</span><span class="sxs-lookup"><span data-stu-id="b8c22-186">[Page](page.md) collection</span></span>| <span data-ttu-id="b8c22-187">Получение коллекции страниц в указанном разделе.</span><span class="sxs-lookup"><span data-stu-id="b8c22-187">Get a collection of pages in the specified section.</span></span>|
|[<span data-ttu-id="b8c22-188">copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="b8c22-188">copyToNotebook</span></span>](../api/section-copytonotebook.md)|<span data-ttu-id="b8c22-189">Нет</span><span class="sxs-lookup"><span data-stu-id="b8c22-189">None</span></span>|<span data-ttu-id="b8c22-190">Скопируйте раздел в указанную записную книжку.</span><span class="sxs-lookup"><span data-stu-id="b8c22-190">Copy the section to a specific notebook.</span></span>|
|[<span data-ttu-id="b8c22-191">copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="b8c22-191">copyToSectionGroup</span></span>](../api/section-copytosectiongroup.md)|<span data-ttu-id="b8c22-192">Нет</span><span class="sxs-lookup"><span data-stu-id="b8c22-192">None</span></span>|<span data-ttu-id="b8c22-193">Скопируйте раздел в определенную группу разделов.</span><span class="sxs-lookup"><span data-stu-id="b8c22-193">Copy the section to a specific section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteSection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
