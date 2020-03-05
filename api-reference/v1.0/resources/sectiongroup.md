---
title: Тип ресурса sectionGroup
description: Группа разделов в записной книжке OneNote. Группы разделов могут содержать разделы и группы разделов.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 2e0d9b3b963e02bf017630ad898501518449a20f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446942"
---
# <a name="sectiongroup-resource-type"></a><span data-ttu-id="53423-104">Тип ресурса sectionGroup</span><span class="sxs-lookup"><span data-stu-id="53423-104">sectionGroup resource type</span></span>

<span data-ttu-id="53423-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="53423-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="53423-106">Группа разделов в записной книжке OneNote.</span><span class="sxs-lookup"><span data-stu-id="53423-106">A section group in a OneNote notebook.</span></span> <span data-ttu-id="53423-107">Группы разделов могут содержать разделы и группы разделов.</span><span class="sxs-lookup"><span data-stu-id="53423-107">Section groups can contain sections and section groups.</span></span>

## <a name="json-representation"></a><span data-ttu-id="53423-108">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="53423-108">JSON representation</span></span>

<span data-ttu-id="53423-109">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="53423-109">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.onenoteEntityHierarchyModel",
  "optionalProperties": [
    "parentNotebook",
    "parentSectionGroup",
    "sectionGroups",
    "sections"
  ],
  "@odata.type": "microsoft.graph.sectionGroup"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "string",
  "sectionGroupsUrl": "string",
  "sectionsUrl": "string",
  "self": "string"
}

```
## <a name="properties"></a><span data-ttu-id="53423-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="53423-110">Properties</span></span>
| <span data-ttu-id="53423-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="53423-111">Property</span></span>     | <span data-ttu-id="53423-112">Тип</span><span class="sxs-lookup"><span data-stu-id="53423-112">Type</span></span>   |<span data-ttu-id="53423-113">Описание</span><span class="sxs-lookup"><span data-stu-id="53423-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="53423-114">createdBy</span><span class="sxs-lookup"><span data-stu-id="53423-114">createdBy</span></span>|[<span data-ttu-id="53423-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="53423-115">identitySet</span></span>](identityset.md)|<span data-ttu-id="53423-p103">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="53423-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="53423-118">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="53423-118">createdDateTime</span></span>|<span data-ttu-id="53423-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53423-119">DateTimeOffset</span></span>|<span data-ttu-id="53423-120">Дата и время создания группы разделов.</span><span class="sxs-lookup"><span data-stu-id="53423-120">The date and time when the section group was created.</span></span> <span data-ttu-id="53423-121">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="53423-121">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="53423-122">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="53423-122">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="53423-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="53423-123">Read-only.</span></span>|
|<span data-ttu-id="53423-124">id</span><span class="sxs-lookup"><span data-stu-id="53423-124">id</span></span>|<span data-ttu-id="53423-125">String</span><span class="sxs-lookup"><span data-stu-id="53423-125">String</span></span>|<span data-ttu-id="53423-126">Уникальный идентификатор группы разделов.</span><span class="sxs-lookup"><span data-stu-id="53423-126">The unique identifier of the section group.</span></span> <span data-ttu-id="53423-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="53423-127">Read-only.</span></span>|
|<span data-ttu-id="53423-128">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="53423-128">lastModifiedBy</span></span>|[<span data-ttu-id="53423-129">identitySet</span><span class="sxs-lookup"><span data-stu-id="53423-129">identitySet</span></span>](identityset.md)|<span data-ttu-id="53423-p106">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="53423-p106">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="53423-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="53423-132">lastModifiedDateTime</span></span>|<span data-ttu-id="53423-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53423-133">DateTimeOffset</span></span>|<span data-ttu-id="53423-134">Дата и время последнего изменения группы разделов.</span><span class="sxs-lookup"><span data-stu-id="53423-134">The date and time when the section group was last modified.</span></span> <span data-ttu-id="53423-135">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="53423-135">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="53423-136">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="53423-136">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="53423-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="53423-137">Read-only.</span></span>|
|<span data-ttu-id="53423-138">displayName</span><span class="sxs-lookup"><span data-stu-id="53423-138">displayName</span></span>|<span data-ttu-id="53423-139">Строка</span><span class="sxs-lookup"><span data-stu-id="53423-139">String</span></span>|<span data-ttu-id="53423-140">Имя группы разделов.</span><span class="sxs-lookup"><span data-stu-id="53423-140">The name of the section group.</span></span>|
|<span data-ttu-id="53423-141">сектионграупсурл</span><span class="sxs-lookup"><span data-stu-id="53423-141">sectionGroupsUrl</span></span>|<span data-ttu-id="53423-142">String</span><span class="sxs-lookup"><span data-stu-id="53423-142">String</span></span>|<span data-ttu-id="53423-143">URL-адрес для `sectionGroups` свойства навигации, который возвращает все группы разделов в группе разделов.</span><span class="sxs-lookup"><span data-stu-id="53423-143">The URL for the `sectionGroups` navigation property, which returns all the section groups in the section group.</span></span> <span data-ttu-id="53423-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="53423-144">Read-only.</span></span>|
|<span data-ttu-id="53423-145">сектионсурл</span><span class="sxs-lookup"><span data-stu-id="53423-145">sectionsUrl</span></span>|<span data-ttu-id="53423-146">String</span><span class="sxs-lookup"><span data-stu-id="53423-146">String</span></span>|<span data-ttu-id="53423-147">URL-адрес для `sections` свойства навигации, который возвращает все разделы в группе разделов.</span><span class="sxs-lookup"><span data-stu-id="53423-147">The URL for the `sections` navigation property, which returns all the sections in the section group.</span></span> <span data-ttu-id="53423-148">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="53423-148">Read-only.</span></span>|
|<span data-ttu-id="53423-149">Self</span><span class="sxs-lookup"><span data-stu-id="53423-149">self</span></span>|<span data-ttu-id="53423-150">String</span><span class="sxs-lookup"><span data-stu-id="53423-150">String</span></span>|<span data-ttu-id="53423-151">Конечная точка, где можно получить сведения о группе разделов.</span><span class="sxs-lookup"><span data-stu-id="53423-151">The endpoint where you can get details about the section group.</span></span> <span data-ttu-id="53423-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="53423-152">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="53423-153">Отношения</span><span class="sxs-lookup"><span data-stu-id="53423-153">Relationships</span></span>
| <span data-ttu-id="53423-154">Связь</span><span class="sxs-lookup"><span data-stu-id="53423-154">Relationship</span></span> | <span data-ttu-id="53423-155">Тип</span><span class="sxs-lookup"><span data-stu-id="53423-155">Type</span></span>   |<span data-ttu-id="53423-156">Описание</span><span class="sxs-lookup"><span data-stu-id="53423-156">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="53423-157">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="53423-157">parentNotebook</span></span>|[<span data-ttu-id="53423-158">Notebook</span><span class="sxs-lookup"><span data-stu-id="53423-158">Notebook</span></span>](notebook.md)|<span data-ttu-id="53423-159">Записная книжка, содержащая группу разделов.</span><span class="sxs-lookup"><span data-stu-id="53423-159">The notebook that contains the section group.</span></span> <span data-ttu-id="53423-160">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="53423-160">Read-only.</span></span>|
|<span data-ttu-id="53423-161">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="53423-161">parentSectionGroup</span></span>|[<span data-ttu-id="53423-162">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="53423-162">SectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="53423-163">Группа разделов, содержащая группу разделов.</span><span class="sxs-lookup"><span data-stu-id="53423-163">The section group that contains the section group.</span></span> <span data-ttu-id="53423-164">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="53423-164">Read-only.</span></span>|
|<span data-ttu-id="53423-165">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="53423-165">sectionGroups</span></span>|<span data-ttu-id="53423-166">Коллекция [SectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="53423-166">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="53423-167">Группы разделов в разделе.</span><span class="sxs-lookup"><span data-stu-id="53423-167">The section groups in the section.</span></span> <span data-ttu-id="53423-168">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="53423-168">Read-only.</span></span> <span data-ttu-id="53423-169">Допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="53423-169">Nullable.</span></span>|
|<span data-ttu-id="53423-170">sections</span><span class="sxs-lookup"><span data-stu-id="53423-170">sections</span></span>|<span data-ttu-id="53423-171">Коллекция [OnenoteSection](section.md)</span><span class="sxs-lookup"><span data-stu-id="53423-171">[OnenoteSection](section.md) collection</span></span>|<span data-ttu-id="53423-172">Разделы в группе разделов.</span><span class="sxs-lookup"><span data-stu-id="53423-172">The sections in the section group.</span></span> <span data-ttu-id="53423-173">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="53423-173">Read-only.</span></span> <span data-ttu-id="53423-174">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="53423-174">Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="53423-175">Методы</span><span class="sxs-lookup"><span data-stu-id="53423-175">Methods</span></span>

| <span data-ttu-id="53423-176">Метод</span><span class="sxs-lookup"><span data-stu-id="53423-176">Method</span></span>           | <span data-ttu-id="53423-177">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="53423-177">Return Type</span></span>    |<span data-ttu-id="53423-178">Описание</span><span class="sxs-lookup"><span data-stu-id="53423-178">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="53423-179">Вывод группы разделов</span><span class="sxs-lookup"><span data-stu-id="53423-179">Get section group</span></span>](../api/sectiongroup-get.md) | [<span data-ttu-id="53423-180">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="53423-180">SectionGroup</span></span>](sectiongroup.md) |<span data-ttu-id="53423-181">Прочитайте свойства и связи группы разделов.</span><span class="sxs-lookup"><span data-stu-id="53423-181">Read the properties and relationships of the section group.</span></span>|
|[<span data-ttu-id="53423-182">Создание группы разделов</span><span class="sxs-lookup"><span data-stu-id="53423-182">Create section group</span></span>](../api/sectiongroup-post-sectiongroups.md) |[<span data-ttu-id="53423-183">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="53423-183">SectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="53423-184">Создание группы разделов путем отправки в коллекцию sectionGroups в указанной группе разделов.</span><span class="sxs-lookup"><span data-stu-id="53423-184">Create a section group by posting to the sectionGroups collection in the specified section group.</span></span>|
|[<span data-ttu-id="53423-185">Перечисление групп разделов</span><span class="sxs-lookup"><span data-stu-id="53423-185">List section groups</span></span>](../api/sectiongroup-list-sectiongroups.md) |<span data-ttu-id="53423-186">Коллекция [SectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="53423-186">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="53423-187">Получение коллекции групп разделов в указанной группе разделов.</span><span class="sxs-lookup"><span data-stu-id="53423-187">Get collection of section groups in the specified section group.</span></span>|
|[<span data-ttu-id="53423-188">Создание раздела</span><span class="sxs-lookup"><span data-stu-id="53423-188">Create section</span></span>](../api/sectiongroup-post-sections.md) |[<span data-ttu-id="53423-189">оненотесектион</span><span class="sxs-lookup"><span data-stu-id="53423-189">OnenoteSection</span></span>](section.md)| <span data-ttu-id="53423-190">Создание раздела путем публикации в коллекции разделов в указанной группе разделов.</span><span class="sxs-lookup"><span data-stu-id="53423-190">Create a section by posting to the sections collection in the specified section group.</span></span>|
|[<span data-ttu-id="53423-191">Перечисление разделов</span><span class="sxs-lookup"><span data-stu-id="53423-191">List sections</span></span>](../api/sectiongroup-list-sections.md) |<span data-ttu-id="53423-192">Коллекция [OnenoteSection](section.md)</span><span class="sxs-lookup"><span data-stu-id="53423-192">[OnenoteSection](section.md) collection</span></span>| <span data-ttu-id="53423-193">Получение коллекции разделов в указанной группе разделов.</span><span class="sxs-lookup"><span data-stu-id="53423-193">Get a collection of sections in the specified section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sectionGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
