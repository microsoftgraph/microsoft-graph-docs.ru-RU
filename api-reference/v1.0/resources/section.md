---
title: Тип ресурса раздела
description: Раздел в записной книжке OneNote. Разделы могут содержать страницы.
localization_priority: Normal
author: jewan-microsoft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 421d910a79dd04403f09b455417d5ad97eac5691
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722016"
---
# <a name="section-resource-type"></a><span data-ttu-id="35edb-104">Тип ресурса раздела</span><span class="sxs-lookup"><span data-stu-id="35edb-104">section resource type</span></span>

<span data-ttu-id="35edb-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35edb-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="35edb-106">Раздел в записной книжке OneNote.</span><span class="sxs-lookup"><span data-stu-id="35edb-106">A section in a OneNote notebook.</span></span> <span data-ttu-id="35edb-107">Разделы могут содержать страницы.</span><span class="sxs-lookup"><span data-stu-id="35edb-107">Sections can contain pages.</span></span>

## <a name="json-representation"></a><span data-ttu-id="35edb-108">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="35edb-108">JSON representation</span></span>

<span data-ttu-id="35edb-109">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="35edb-109">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="35edb-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="35edb-110">Properties</span></span>
| <span data-ttu-id="35edb-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="35edb-111">Property</span></span>     | <span data-ttu-id="35edb-112">Тип</span><span class="sxs-lookup"><span data-stu-id="35edb-112">Type</span></span>   |<span data-ttu-id="35edb-113">Описание</span><span class="sxs-lookup"><span data-stu-id="35edb-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="35edb-114">createdBy</span><span class="sxs-lookup"><span data-stu-id="35edb-114">createdBy</span></span>|[<span data-ttu-id="35edb-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="35edb-115">identitySet</span></span>](identityset.md)|<span data-ttu-id="35edb-p103">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="35edb-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="35edb-118">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="35edb-118">createdDateTime</span></span>|<span data-ttu-id="35edb-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35edb-119">DateTimeOffset</span></span>|<span data-ttu-id="35edb-120">Дата и время создания раздела.</span><span class="sxs-lookup"><span data-stu-id="35edb-120">The date and time when the section was created.</span></span> <span data-ttu-id="35edb-121">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="35edb-121">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="35edb-122">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="35edb-122">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="35edb-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="35edb-123">Read-only.</span></span>|
|<span data-ttu-id="35edb-124">id</span><span class="sxs-lookup"><span data-stu-id="35edb-124">id</span></span>|<span data-ttu-id="35edb-125">String</span><span class="sxs-lookup"><span data-stu-id="35edb-125">String</span></span>|<span data-ttu-id="35edb-126">Уникальный идентификатор раздела.</span><span class="sxs-lookup"><span data-stu-id="35edb-126">The unique identifier of the section.</span></span>  <span data-ttu-id="35edb-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="35edb-127">Read-only.</span></span>|
|<span data-ttu-id="35edb-128">isDefault</span><span class="sxs-lookup"><span data-stu-id="35edb-128">isDefault</span></span>|<span data-ttu-id="35edb-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="35edb-129">Boolean</span></span>|<span data-ttu-id="35edb-130">Указывает, является ли это разделом по умолчанию пользователя.</span><span class="sxs-lookup"><span data-stu-id="35edb-130">Indicates whether this is the user's default section.</span></span> <span data-ttu-id="35edb-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="35edb-131">Read-only.</span></span>|
|<span data-ttu-id="35edb-132">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="35edb-132">lastModifiedBy</span></span>|[<span data-ttu-id="35edb-133">identitySet</span><span class="sxs-lookup"><span data-stu-id="35edb-133">identitySet</span></span>](identityset.md)|<span data-ttu-id="35edb-p107">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="35edb-p107">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="35edb-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="35edb-136">lastModifiedDateTime</span></span>|<span data-ttu-id="35edb-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35edb-137">DateTimeOffset</span></span>|<span data-ttu-id="35edb-138">Дата и время последнего изменения раздела.</span><span class="sxs-lookup"><span data-stu-id="35edb-138">The date and time when the section was last modified.</span></span> <span data-ttu-id="35edb-139">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="35edb-139">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="35edb-140">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="35edb-140">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="35edb-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="35edb-141">Read-only.</span></span>|
|<span data-ttu-id="35edb-142">links</span><span class="sxs-lookup"><span data-stu-id="35edb-142">links</span></span>|[<span data-ttu-id="35edb-143">SectionLinks</span><span class="sxs-lookup"><span data-stu-id="35edb-143">SectionLinks</span></span>](sectionlinks.md)|<span data-ttu-id="35edb-144">Ссылки для открытия раздела.</span><span class="sxs-lookup"><span data-stu-id="35edb-144">Links for opening the section.</span></span> <span data-ttu-id="35edb-145">Ссылка открывает раздел в родном клиенте `oneNoteClientURL` OneNote, если он установлен.</span><span class="sxs-lookup"><span data-stu-id="35edb-145">The `oneNoteClientURL` link opens the section in the OneNote native client if it's installed.</span></span> <span data-ttu-id="35edb-146">Ссылка `oneNoteWebURL` открывает раздел в OneNote в Интернете.</span><span class="sxs-lookup"><span data-stu-id="35edb-146">The `oneNoteWebURL` link opens the section in OneNote on the web.</span></span>|
|<span data-ttu-id="35edb-147">displayName</span><span class="sxs-lookup"><span data-stu-id="35edb-147">displayName</span></span>|<span data-ttu-id="35edb-148">String</span><span class="sxs-lookup"><span data-stu-id="35edb-148">String</span></span>|<span data-ttu-id="35edb-149">Имя раздела.</span><span class="sxs-lookup"><span data-stu-id="35edb-149">The name of the section.</span></span> |
|<span data-ttu-id="35edb-150">pagesUrl</span><span class="sxs-lookup"><span data-stu-id="35edb-150">pagesUrl</span></span>|<span data-ttu-id="35edb-151">String</span><span class="sxs-lookup"><span data-stu-id="35edb-151">String</span></span>|<span data-ttu-id="35edb-152">Конечная точка, где можно получить сведения `pages` для всех страниц в разделе.</span><span class="sxs-lookup"><span data-stu-id="35edb-152">The `pages` endpoint where you can get details for all the pages in the section.</span></span> <span data-ttu-id="35edb-153">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="35edb-153">Read-only.</span></span>|
|<span data-ttu-id="35edb-154">self</span><span class="sxs-lookup"><span data-stu-id="35edb-154">self</span></span>|<span data-ttu-id="35edb-155">String</span><span class="sxs-lookup"><span data-stu-id="35edb-155">String</span></span>|<span data-ttu-id="35edb-156">Конечная точка, где можно получить сведения о разделе.</span><span class="sxs-lookup"><span data-stu-id="35edb-156">The endpoint where you can get details about the section.</span></span> <span data-ttu-id="35edb-157">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="35edb-157">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="35edb-158">Связи</span><span class="sxs-lookup"><span data-stu-id="35edb-158">Relationships</span></span>
| <span data-ttu-id="35edb-159">Связь</span><span class="sxs-lookup"><span data-stu-id="35edb-159">Relationship</span></span> | <span data-ttu-id="35edb-160">Тип</span><span class="sxs-lookup"><span data-stu-id="35edb-160">Type</span></span>   |<span data-ttu-id="35edb-161">Описание</span><span class="sxs-lookup"><span data-stu-id="35edb-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="35edb-162">pages</span><span class="sxs-lookup"><span data-stu-id="35edb-162">pages</span></span>|<span data-ttu-id="35edb-163">Коллекция [OnenotePage](page.md)</span><span class="sxs-lookup"><span data-stu-id="35edb-163">[OnenotePage](page.md) collection</span></span>|<span data-ttu-id="35edb-164">Коллекция страниц в разделе.</span><span class="sxs-lookup"><span data-stu-id="35edb-164">The collection of pages in the section.</span></span>  <span data-ttu-id="35edb-165">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="35edb-165">Read-only.</span></span> <span data-ttu-id="35edb-166">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="35edb-166">Nullable.</span></span>|
|<span data-ttu-id="35edb-167">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="35edb-167">parentNotebook</span></span>|[<span data-ttu-id="35edb-168">Notebook</span><span class="sxs-lookup"><span data-stu-id="35edb-168">Notebook</span></span>](notebook.md)|<span data-ttu-id="35edb-169">Блокнот, содержащий раздел.</span><span class="sxs-lookup"><span data-stu-id="35edb-169">The notebook that contains the section.</span></span>  <span data-ttu-id="35edb-170">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="35edb-170">Read-only.</span></span>|
|<span data-ttu-id="35edb-171">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="35edb-171">parentSectionGroup</span></span>|[<span data-ttu-id="35edb-172">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="35edb-172">SectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="35edb-173">Группа разделов, которая содержит раздел.</span><span class="sxs-lookup"><span data-stu-id="35edb-173">The section group that contains the section.</span></span>  <span data-ttu-id="35edb-174">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="35edb-174">Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="35edb-175">Методы</span><span class="sxs-lookup"><span data-stu-id="35edb-175">Methods</span></span>

| <span data-ttu-id="35edb-176">Метод</span><span class="sxs-lookup"><span data-stu-id="35edb-176">Method</span></span>           | <span data-ttu-id="35edb-177">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="35edb-177">Return Type</span></span>    |<span data-ttu-id="35edb-178">Описание</span><span class="sxs-lookup"><span data-stu-id="35edb-178">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="35edb-179">Получение раздела</span><span class="sxs-lookup"><span data-stu-id="35edb-179">Get section</span></span>](../api/section-get.md) | [<span data-ttu-id="35edb-180">OnenoteSection</span><span class="sxs-lookup"><span data-stu-id="35edb-180">OnenoteSection</span></span>](section.md) |<span data-ttu-id="35edb-181">Ознакомьтесь с свойствами и отношениями раздела.</span><span class="sxs-lookup"><span data-stu-id="35edb-181">Read the properties and relationships of the section.</span></span>|
|[<span data-ttu-id="35edb-182">Создание страницы</span><span class="sxs-lookup"><span data-stu-id="35edb-182">Create page</span></span>](../api/section-post-pages.md) |[<span data-ttu-id="35edb-183">Page</span><span class="sxs-lookup"><span data-stu-id="35edb-183">Page</span></span>](page.md)| <span data-ttu-id="35edb-184">Создайте страницу, выложив ее в коллекцию страниц в указанном разделе.</span><span class="sxs-lookup"><span data-stu-id="35edb-184">Create a page by posting to the pages collection in the specified section.</span></span>|
|[<span data-ttu-id="35edb-185">Перечисление страниц</span><span class="sxs-lookup"><span data-stu-id="35edb-185">List pages</span></span>](../api/section-list-pages.md) |<span data-ttu-id="35edb-186">Коллекция [Page](page.md)</span><span class="sxs-lookup"><span data-stu-id="35edb-186">[Page](page.md) collection</span></span>| <span data-ttu-id="35edb-187">Получите коллекцию страниц в указанном разделе.</span><span class="sxs-lookup"><span data-stu-id="35edb-187">Get a collection of pages in the specified section.</span></span>|
|[<span data-ttu-id="35edb-188">copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="35edb-188">copyToNotebook</span></span>](../api/section-copytonotebook.md)|<span data-ttu-id="35edb-189">Нет</span><span class="sxs-lookup"><span data-stu-id="35edb-189">None</span></span>|<span data-ttu-id="35edb-190">Скопируйте раздел в определенный блокнот.</span><span class="sxs-lookup"><span data-stu-id="35edb-190">Copy the section to a specific notebook.</span></span>|
|[<span data-ttu-id="35edb-191">copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="35edb-191">copyToSectionGroup</span></span>](../api/section-copytosectiongroup.md)|<span data-ttu-id="35edb-192">Нет</span><span class="sxs-lookup"><span data-stu-id="35edb-192">None</span></span>|<span data-ttu-id="35edb-193">Скопируйте раздел в определенную группу разделов.</span><span class="sxs-lookup"><span data-stu-id="35edb-193">Copy the section to a specific section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteSection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

