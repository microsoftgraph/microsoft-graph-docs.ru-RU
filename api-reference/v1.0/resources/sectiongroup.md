---
title: тип ресурсов sectionGroup
description: Группа разделов в записной книжке OneNote. Группы разделов могут содержать разделы и группы разделов.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 5968a327800c823cd5767a382d019fba39f66927
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722008"
---
# <a name="sectiongroup-resource-type"></a><span data-ttu-id="392e1-104">тип ресурсов sectionGroup</span><span class="sxs-lookup"><span data-stu-id="392e1-104">sectionGroup resource type</span></span>

<span data-ttu-id="392e1-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="392e1-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="392e1-106">Группа разделов в записной книжке OneNote.</span><span class="sxs-lookup"><span data-stu-id="392e1-106">A section group in a OneNote notebook.</span></span> <span data-ttu-id="392e1-107">Группы разделов могут содержать разделы и группы разделов.</span><span class="sxs-lookup"><span data-stu-id="392e1-107">Section groups can contain sections and section groups.</span></span>

## <a name="json-representation"></a><span data-ttu-id="392e1-108">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="392e1-108">JSON representation</span></span>

<span data-ttu-id="392e1-109">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="392e1-109">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="392e1-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="392e1-110">Properties</span></span>
| <span data-ttu-id="392e1-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="392e1-111">Property</span></span>     | <span data-ttu-id="392e1-112">Тип</span><span class="sxs-lookup"><span data-stu-id="392e1-112">Type</span></span>   |<span data-ttu-id="392e1-113">Описание</span><span class="sxs-lookup"><span data-stu-id="392e1-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="392e1-114">createdBy</span><span class="sxs-lookup"><span data-stu-id="392e1-114">createdBy</span></span>|[<span data-ttu-id="392e1-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="392e1-115">identitySet</span></span>](identityset.md)|<span data-ttu-id="392e1-p103">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="392e1-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="392e1-118">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="392e1-118">createdDateTime</span></span>|<span data-ttu-id="392e1-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="392e1-119">DateTimeOffset</span></span>|<span data-ttu-id="392e1-120">Дата и время создания группы разделов.</span><span class="sxs-lookup"><span data-stu-id="392e1-120">The date and time when the section group was created.</span></span> <span data-ttu-id="392e1-121">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="392e1-121">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="392e1-122">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="392e1-122">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="392e1-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="392e1-123">Read-only.</span></span>|
|<span data-ttu-id="392e1-124">id</span><span class="sxs-lookup"><span data-stu-id="392e1-124">id</span></span>|<span data-ttu-id="392e1-125">String</span><span class="sxs-lookup"><span data-stu-id="392e1-125">String</span></span>|<span data-ttu-id="392e1-126">Уникальный идентификатор группы разделов.</span><span class="sxs-lookup"><span data-stu-id="392e1-126">The unique identifier of the section group.</span></span> <span data-ttu-id="392e1-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="392e1-127">Read-only.</span></span>|
|<span data-ttu-id="392e1-128">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="392e1-128">lastModifiedBy</span></span>|[<span data-ttu-id="392e1-129">identitySet</span><span class="sxs-lookup"><span data-stu-id="392e1-129">identitySet</span></span>](identityset.md)|<span data-ttu-id="392e1-p106">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="392e1-p106">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="392e1-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="392e1-132">lastModifiedDateTime</span></span>|<span data-ttu-id="392e1-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="392e1-133">DateTimeOffset</span></span>|<span data-ttu-id="392e1-134">Дата и время последнего изменения группы разделов.</span><span class="sxs-lookup"><span data-stu-id="392e1-134">The date and time when the section group was last modified.</span></span> <span data-ttu-id="392e1-135">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="392e1-135">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="392e1-136">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="392e1-136">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="392e1-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="392e1-137">Read-only.</span></span>|
|<span data-ttu-id="392e1-138">displayName</span><span class="sxs-lookup"><span data-stu-id="392e1-138">displayName</span></span>|<span data-ttu-id="392e1-139">String</span><span class="sxs-lookup"><span data-stu-id="392e1-139">String</span></span>|<span data-ttu-id="392e1-140">Имя группы разделов.</span><span class="sxs-lookup"><span data-stu-id="392e1-140">The name of the section group.</span></span>|
|<span data-ttu-id="392e1-141">sectionGroupsUrl</span><span class="sxs-lookup"><span data-stu-id="392e1-141">sectionGroupsUrl</span></span>|<span data-ttu-id="392e1-142">String</span><span class="sxs-lookup"><span data-stu-id="392e1-142">String</span></span>|<span data-ttu-id="392e1-143">URL-адрес `sectionGroups` свойства навигации, который возвращает все группы разделов в группе разделов.</span><span class="sxs-lookup"><span data-stu-id="392e1-143">The URL for the `sectionGroups` navigation property, which returns all the section groups in the section group.</span></span> <span data-ttu-id="392e1-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="392e1-144">Read-only.</span></span>|
|<span data-ttu-id="392e1-145">sectionsUrl</span><span class="sxs-lookup"><span data-stu-id="392e1-145">sectionsUrl</span></span>|<span data-ttu-id="392e1-146">String</span><span class="sxs-lookup"><span data-stu-id="392e1-146">String</span></span>|<span data-ttu-id="392e1-147">URL-адрес `sections` свойства навигации, который возвращает все разделы в группе разделов.</span><span class="sxs-lookup"><span data-stu-id="392e1-147">The URL for the `sections` navigation property, which returns all the sections in the section group.</span></span> <span data-ttu-id="392e1-148">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="392e1-148">Read-only.</span></span>|
|<span data-ttu-id="392e1-149">self</span><span class="sxs-lookup"><span data-stu-id="392e1-149">self</span></span>|<span data-ttu-id="392e1-150">String</span><span class="sxs-lookup"><span data-stu-id="392e1-150">String</span></span>|<span data-ttu-id="392e1-151">Конечная точка, где можно получить сведения о группе разделов.</span><span class="sxs-lookup"><span data-stu-id="392e1-151">The endpoint where you can get details about the section group.</span></span> <span data-ttu-id="392e1-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="392e1-152">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="392e1-153">Связи</span><span class="sxs-lookup"><span data-stu-id="392e1-153">Relationships</span></span>
| <span data-ttu-id="392e1-154">Связь</span><span class="sxs-lookup"><span data-stu-id="392e1-154">Relationship</span></span> | <span data-ttu-id="392e1-155">Тип</span><span class="sxs-lookup"><span data-stu-id="392e1-155">Type</span></span>   |<span data-ttu-id="392e1-156">Описание</span><span class="sxs-lookup"><span data-stu-id="392e1-156">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="392e1-157">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="392e1-157">parentNotebook</span></span>|[<span data-ttu-id="392e1-158">Notebook</span><span class="sxs-lookup"><span data-stu-id="392e1-158">Notebook</span></span>](notebook.md)|<span data-ttu-id="392e1-159">Блокнот, содержащий группу разделов.</span><span class="sxs-lookup"><span data-stu-id="392e1-159">The notebook that contains the section group.</span></span> <span data-ttu-id="392e1-160">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="392e1-160">Read-only.</span></span>|
|<span data-ttu-id="392e1-161">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="392e1-161">parentSectionGroup</span></span>|[<span data-ttu-id="392e1-162">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="392e1-162">SectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="392e1-163">Группа разделов, которая содержит группу разделов.</span><span class="sxs-lookup"><span data-stu-id="392e1-163">The section group that contains the section group.</span></span> <span data-ttu-id="392e1-164">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="392e1-164">Read-only.</span></span>|
|<span data-ttu-id="392e1-165">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="392e1-165">sectionGroups</span></span>|<span data-ttu-id="392e1-166">Коллекция [SectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="392e1-166">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="392e1-167">Раздел групп в разделе.</span><span class="sxs-lookup"><span data-stu-id="392e1-167">The section groups in the section.</span></span> <span data-ttu-id="392e1-168">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="392e1-168">Read-only.</span></span> <span data-ttu-id="392e1-169">Допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="392e1-169">Nullable.</span></span>|
|<span data-ttu-id="392e1-170">sections</span><span class="sxs-lookup"><span data-stu-id="392e1-170">sections</span></span>|<span data-ttu-id="392e1-171">Коллекция [OnenoteSection](section.md)</span><span class="sxs-lookup"><span data-stu-id="392e1-171">[OnenoteSection](section.md) collection</span></span>|<span data-ttu-id="392e1-172">Разделы в группе разделов.</span><span class="sxs-lookup"><span data-stu-id="392e1-172">The sections in the section group.</span></span> <span data-ttu-id="392e1-173">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="392e1-173">Read-only.</span></span> <span data-ttu-id="392e1-174">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="392e1-174">Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="392e1-175">Методы</span><span class="sxs-lookup"><span data-stu-id="392e1-175">Methods</span></span>

| <span data-ttu-id="392e1-176">Метод</span><span class="sxs-lookup"><span data-stu-id="392e1-176">Method</span></span>           | <span data-ttu-id="392e1-177">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="392e1-177">Return Type</span></span>    |<span data-ttu-id="392e1-178">Описание</span><span class="sxs-lookup"><span data-stu-id="392e1-178">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="392e1-179">Вывод группы разделов</span><span class="sxs-lookup"><span data-stu-id="392e1-179">Get section group</span></span>](../api/sectiongroup-get.md) | [<span data-ttu-id="392e1-180">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="392e1-180">SectionGroup</span></span>](sectiongroup.md) |<span data-ttu-id="392e1-181">Ознакомьтесь с свойствами и отношениями группы разделов.</span><span class="sxs-lookup"><span data-stu-id="392e1-181">Read the properties and relationships of the section group.</span></span>|
|[<span data-ttu-id="392e1-182">Создание группы разделов</span><span class="sxs-lookup"><span data-stu-id="392e1-182">Create section group</span></span>](../api/sectiongroup-post-sectiongroups.md) |[<span data-ttu-id="392e1-183">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="392e1-183">SectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="392e1-184">Создайте группу разделов, разместив в разделеGroups коллекцию в указанной группе раздела.</span><span class="sxs-lookup"><span data-stu-id="392e1-184">Create a section group by posting to the sectionGroups collection in the specified section group.</span></span>|
|[<span data-ttu-id="392e1-185">Перечисление групп разделов</span><span class="sxs-lookup"><span data-stu-id="392e1-185">List section groups</span></span>](../api/sectiongroup-list-sectiongroups.md) |<span data-ttu-id="392e1-186">Коллекция [SectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="392e1-186">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="392e1-187">Получите коллекцию групп разделов в указанной группе раздела.</span><span class="sxs-lookup"><span data-stu-id="392e1-187">Get collection of section groups in the specified section group.</span></span>|
|[<span data-ttu-id="392e1-188">Создание раздела</span><span class="sxs-lookup"><span data-stu-id="392e1-188">Create section</span></span>](../api/sectiongroup-post-sections.md) |[<span data-ttu-id="392e1-189">OnenoteSection</span><span class="sxs-lookup"><span data-stu-id="392e1-189">OnenoteSection</span></span>](section.md)| <span data-ttu-id="392e1-190">Создайте раздел, разместив в коллекции разделов в указанной группе разделов.</span><span class="sxs-lookup"><span data-stu-id="392e1-190">Create a section by posting to the sections collection in the specified section group.</span></span>|
|[<span data-ttu-id="392e1-191">Перечисление разделов</span><span class="sxs-lookup"><span data-stu-id="392e1-191">List sections</span></span>](../api/sectiongroup-list-sections.md) |<span data-ttu-id="392e1-192">Коллекция [OnenoteSection](section.md)</span><span class="sxs-lookup"><span data-stu-id="392e1-192">[OnenoteSection](section.md) collection</span></span>| <span data-ttu-id="392e1-193">Получите коллекцию разделов в указанной группе раздела.</span><span class="sxs-lookup"><span data-stu-id="392e1-193">Get a collection of sections in the specified section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sectionGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

