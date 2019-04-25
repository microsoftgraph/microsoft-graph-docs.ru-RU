---
title: Тип ресурса sectionGroup
description: Группа разделов в записной книжке OneNote. Группы разделов могут содержать разделы и группы разделов.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: ec27343121ba20ef65703f3df1d53e6c62ccc8e4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579144"
---
# <a name="sectiongroup-resource-type"></a><span data-ttu-id="2c701-104">Тип ресурса sectionGroup</span><span class="sxs-lookup"><span data-stu-id="2c701-104">sectionGroup resource type</span></span>

<span data-ttu-id="2c701-105">Группа разделов в записной книжке OneNote.</span><span class="sxs-lookup"><span data-stu-id="2c701-105">A section group in a OneNote notebook.</span></span> <span data-ttu-id="2c701-106">Группы разделов могут содержать разделы и группы разделов.</span><span class="sxs-lookup"><span data-stu-id="2c701-106">Section groups can contain sections and section groups.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2c701-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2c701-107">JSON representation</span></span>

<span data-ttu-id="2c701-108">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2c701-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="2c701-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="2c701-109">Properties</span></span>
| <span data-ttu-id="2c701-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="2c701-110">Property</span></span>     | <span data-ttu-id="2c701-111">Тип</span><span class="sxs-lookup"><span data-stu-id="2c701-111">Type</span></span>   |<span data-ttu-id="2c701-112">Описание</span><span class="sxs-lookup"><span data-stu-id="2c701-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2c701-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="2c701-113">createdBy</span></span>|[<span data-ttu-id="2c701-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="2c701-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="2c701-p103">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2c701-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="2c701-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2c701-117">createdDateTime</span></span>|<span data-ttu-id="2c701-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c701-118">DateTimeOffset</span></span>|<span data-ttu-id="2c701-119">Дата и время создания группы разделов.</span><span class="sxs-lookup"><span data-stu-id="2c701-119">The date and time when the section group was created.</span></span> <span data-ttu-id="2c701-120">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="2c701-120">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2c701-121">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="2c701-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="2c701-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2c701-122">Read-only.</span></span>|
|<span data-ttu-id="2c701-123">id</span><span class="sxs-lookup"><span data-stu-id="2c701-123">id</span></span>|<span data-ttu-id="2c701-124">String</span><span class="sxs-lookup"><span data-stu-id="2c701-124">String</span></span>|<span data-ttu-id="2c701-125">Уникальный идентификатор группы разделов.</span><span class="sxs-lookup"><span data-stu-id="2c701-125">The unique identifier of the section group.</span></span> <span data-ttu-id="2c701-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2c701-126">Read-only.</span></span>|
|<span data-ttu-id="2c701-127">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="2c701-127">lastModifiedBy</span></span>|[<span data-ttu-id="2c701-128">identitySet</span><span class="sxs-lookup"><span data-stu-id="2c701-128">identitySet</span></span>](identityset.md)|<span data-ttu-id="2c701-p106">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2c701-p106">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="2c701-131">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2c701-131">lastModifiedDateTime</span></span>|<span data-ttu-id="2c701-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c701-132">DateTimeOffset</span></span>|<span data-ttu-id="2c701-133">Дата и время последнего изменения группы разделов.</span><span class="sxs-lookup"><span data-stu-id="2c701-133">The date and time when the section group was last modified.</span></span> <span data-ttu-id="2c701-134">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="2c701-134">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2c701-135">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="2c701-135">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="2c701-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2c701-136">Read-only.</span></span>|
|<span data-ttu-id="2c701-137">displayName</span><span class="sxs-lookup"><span data-stu-id="2c701-137">displayName</span></span>|<span data-ttu-id="2c701-138">String</span><span class="sxs-lookup"><span data-stu-id="2c701-138">String</span></span>|<span data-ttu-id="2c701-139">Имя группы разделов.</span><span class="sxs-lookup"><span data-stu-id="2c701-139">The name of the section group.</span></span>|
|<span data-ttu-id="2c701-140">Сектионграупсурл</span><span class="sxs-lookup"><span data-stu-id="2c701-140">sectionGroupsUrl</span></span>|<span data-ttu-id="2c701-141">String</span><span class="sxs-lookup"><span data-stu-id="2c701-141">String</span></span>|<span data-ttu-id="2c701-142">URL-адрес для `sectionGroups` свойства навигации, который возвращает все группы разделов в группе разделов.</span><span class="sxs-lookup"><span data-stu-id="2c701-142">The URL for the `sectionGroups` navigation property, which returns all the section groups in the section group.</span></span> <span data-ttu-id="2c701-143">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2c701-143">Read-only.</span></span>|
|<span data-ttu-id="2c701-144">Сектионсурл</span><span class="sxs-lookup"><span data-stu-id="2c701-144">sectionsUrl</span></span>|<span data-ttu-id="2c701-145">String</span><span class="sxs-lookup"><span data-stu-id="2c701-145">String</span></span>|<span data-ttu-id="2c701-146">URL-адрес для `sections` свойства навигации, который возвращает все разделы в группе разделов.</span><span class="sxs-lookup"><span data-stu-id="2c701-146">The URL for the `sections` navigation property, which returns all the sections in the section group.</span></span> <span data-ttu-id="2c701-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2c701-147">Read-only.</span></span>|
|<span data-ttu-id="2c701-148">Self</span><span class="sxs-lookup"><span data-stu-id="2c701-148">self</span></span>|<span data-ttu-id="2c701-149">String</span><span class="sxs-lookup"><span data-stu-id="2c701-149">String</span></span>|<span data-ttu-id="2c701-150">Конечная точка, где можно получить сведения о группе разделов.</span><span class="sxs-lookup"><span data-stu-id="2c701-150">The endpoint where you can get details about the section group.</span></span> <span data-ttu-id="2c701-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2c701-151">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2c701-152">Отношения</span><span class="sxs-lookup"><span data-stu-id="2c701-152">Relationships</span></span>
| <span data-ttu-id="2c701-153">Отношение</span><span class="sxs-lookup"><span data-stu-id="2c701-153">Relationship</span></span> | <span data-ttu-id="2c701-154">Тип</span><span class="sxs-lookup"><span data-stu-id="2c701-154">Type</span></span>   |<span data-ttu-id="2c701-155">Описание</span><span class="sxs-lookup"><span data-stu-id="2c701-155">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2c701-156">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="2c701-156">parentNotebook</span></span>|[<span data-ttu-id="2c701-157">Notebook</span><span class="sxs-lookup"><span data-stu-id="2c701-157">Notebook</span></span>](notebook.md)|<span data-ttu-id="2c701-158">Записная книжка, содержащая группу разделов.</span><span class="sxs-lookup"><span data-stu-id="2c701-158">The notebook that contains the section group.</span></span> <span data-ttu-id="2c701-159">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2c701-159">Read-only.</span></span>|
|<span data-ttu-id="2c701-160">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="2c701-160">parentSectionGroup</span></span>|[<span data-ttu-id="2c701-161">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="2c701-161">SectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="2c701-162">Группа разделов, содержащая группу разделов.</span><span class="sxs-lookup"><span data-stu-id="2c701-162">The section group that contains the section group.</span></span> <span data-ttu-id="2c701-163">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2c701-163">Read-only.</span></span>|
|<span data-ttu-id="2c701-164">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="2c701-164">sectionGroups</span></span>|<span data-ttu-id="2c701-165">Коллекция [sectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="2c701-165">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="2c701-166">Группы разделов в разделе.</span><span class="sxs-lookup"><span data-stu-id="2c701-166">The section groups in the section.</span></span> <span data-ttu-id="2c701-167">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2c701-167">Read-only.</span></span> <span data-ttu-id="2c701-168">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="2c701-168">Nullable.</span></span>|
|<span data-ttu-id="2c701-169">sections</span><span class="sxs-lookup"><span data-stu-id="2c701-169">sections</span></span>|<span data-ttu-id="2c701-170">Коллекция [оненотесектион](section.md)</span><span class="sxs-lookup"><span data-stu-id="2c701-170">[OnenoteSection](section.md) collection</span></span>|<span data-ttu-id="2c701-171">Разделы в группе разделов.</span><span class="sxs-lookup"><span data-stu-id="2c701-171">The sections in the section group.</span></span> <span data-ttu-id="2c701-172">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2c701-172">Read-only.</span></span> <span data-ttu-id="2c701-173">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="2c701-173">Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="2c701-174">Методы</span><span class="sxs-lookup"><span data-stu-id="2c701-174">Methods</span></span>

| <span data-ttu-id="2c701-175">Метод</span><span class="sxs-lookup"><span data-stu-id="2c701-175">Method</span></span>           | <span data-ttu-id="2c701-176">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2c701-176">Return Type</span></span>    |<span data-ttu-id="2c701-177">Описание</span><span class="sxs-lookup"><span data-stu-id="2c701-177">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2c701-178">Вывод группы разделов</span><span class="sxs-lookup"><span data-stu-id="2c701-178">Get section group</span></span>](../api/sectiongroup-get.md) | [<span data-ttu-id="2c701-179">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="2c701-179">SectionGroup</span></span>](sectiongroup.md) |<span data-ttu-id="2c701-180">Прочитайте свойства и связи группы разделов.</span><span class="sxs-lookup"><span data-stu-id="2c701-180">Read the properties and relationships of the section group.</span></span>|
|[<span data-ttu-id="2c701-181">Создание группы разделов</span><span class="sxs-lookup"><span data-stu-id="2c701-181">Create section group</span></span>](../api/sectiongroup-post-sectiongroups.md) |[<span data-ttu-id="2c701-182">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="2c701-182">SectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="2c701-183">Создание группы разделов путем отправки в коллекцию sectionGroups в указанной группе разделов.</span><span class="sxs-lookup"><span data-stu-id="2c701-183">Create a section group by posting to the sectionGroups collection in the specified section group.</span></span>|
|[<span data-ttu-id="2c701-184">Список групп разделов</span><span class="sxs-lookup"><span data-stu-id="2c701-184">List section groups</span></span>](../api/sectiongroup-list-sectiongroups.md) |<span data-ttu-id="2c701-185">Коллекция [sectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="2c701-185">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="2c701-186">Получение коллекции групп разделов в указанной группе разделов.</span><span class="sxs-lookup"><span data-stu-id="2c701-186">Get collection of section groups in the specified section group.</span></span>|
|[<span data-ttu-id="2c701-187">Создание раздела</span><span class="sxs-lookup"><span data-stu-id="2c701-187">Create section</span></span>](../api/sectiongroup-post-sections.md) |[<span data-ttu-id="2c701-188">Оненотесектион</span><span class="sxs-lookup"><span data-stu-id="2c701-188">OnenoteSection</span></span>](section.md)| <span data-ttu-id="2c701-189">Создание раздела путем публикации в коллекции разделов в указанной группе разделов.</span><span class="sxs-lookup"><span data-stu-id="2c701-189">Create a section by posting to the sections collection in the specified section group.</span></span>|
|[<span data-ttu-id="2c701-190">Вывод списка разделов</span><span class="sxs-lookup"><span data-stu-id="2c701-190">List sections</span></span>](../api/sectiongroup-list-sections.md) |<span data-ttu-id="2c701-191">Коллекция [оненотесектион](section.md)</span><span class="sxs-lookup"><span data-stu-id="2c701-191">[OnenoteSection](section.md) collection</span></span>| <span data-ttu-id="2c701-192">Получение коллекции разделов в указанной группе разделов.</span><span class="sxs-lookup"><span data-stu-id="2c701-192">Get a collection of sections in the specified section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sectionGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
