---
title: Тип ресурса sectionGroup
description: Группа разделов в записной книжке OneNote. Группы разделов могут содержать разделы и группы разделов.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: f1cd9757b0a58afb4183bd917a7a090b14502a36
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343403"
---
# <a name="sectiongroup-resource-type"></a><span data-ttu-id="77f2b-104">Тип ресурса sectionGroup</span><span class="sxs-lookup"><span data-stu-id="77f2b-104">sectionGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77f2b-105">Группа разделов в записной книжке OneNote.</span><span class="sxs-lookup"><span data-stu-id="77f2b-105">A section group in a OneNote notebook.</span></span> <span data-ttu-id="77f2b-106">Группы разделов могут содержать разделы и группы разделов.</span><span class="sxs-lookup"><span data-stu-id="77f2b-106">Section groups can contain sections and section groups.</span></span>

## <a name="json-representation"></a><span data-ttu-id="77f2b-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="77f2b-107">JSON representation</span></span>

<span data-ttu-id="77f2b-108">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="77f2b-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "parentNotebook",
    "parentSectionGroup",
    "sectionGroups",
    "sections"
  ],
  "keyProperty": "id",
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
## <a name="properties"></a><span data-ttu-id="77f2b-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="77f2b-109">Properties</span></span>
| <span data-ttu-id="77f2b-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="77f2b-110">Property</span></span>     | <span data-ttu-id="77f2b-111">Тип</span><span class="sxs-lookup"><span data-stu-id="77f2b-111">Type</span></span>   |<span data-ttu-id="77f2b-112">Описание</span><span class="sxs-lookup"><span data-stu-id="77f2b-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="77f2b-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="77f2b-113">createdBy</span></span>|[<span data-ttu-id="77f2b-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="77f2b-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="77f2b-p103">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="77f2b-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="77f2b-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="77f2b-117">createdDateTime</span></span>|<span data-ttu-id="77f2b-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77f2b-118">DateTimeOffset</span></span>|<span data-ttu-id="77f2b-119">Дата и время создания группы разделов.</span><span class="sxs-lookup"><span data-stu-id="77f2b-119">The date and time when the section group was created.</span></span> <span data-ttu-id="77f2b-120">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="77f2b-120">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="77f2b-121">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="77f2b-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="77f2b-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="77f2b-122">Read-only.</span></span>|
|<span data-ttu-id="77f2b-123">id</span><span class="sxs-lookup"><span data-stu-id="77f2b-123">id</span></span>|<span data-ttu-id="77f2b-124">String</span><span class="sxs-lookup"><span data-stu-id="77f2b-124">String</span></span>|<span data-ttu-id="77f2b-125">Уникальный идентификатор группы разделов.</span><span class="sxs-lookup"><span data-stu-id="77f2b-125">The unique identifier of the section group.</span></span> <span data-ttu-id="77f2b-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="77f2b-126">Read-only.</span></span>|
|<span data-ttu-id="77f2b-127">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="77f2b-127">lastModifiedBy</span></span>|[<span data-ttu-id="77f2b-128">identitySet</span><span class="sxs-lookup"><span data-stu-id="77f2b-128">identitySet</span></span>](identityset.md)|<span data-ttu-id="77f2b-p106">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="77f2b-p106">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="77f2b-131">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="77f2b-131">lastModifiedDateTime</span></span>|<span data-ttu-id="77f2b-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77f2b-132">DateTimeOffset</span></span>|<span data-ttu-id="77f2b-133">Дата и время последнего изменения группы разделов.</span><span class="sxs-lookup"><span data-stu-id="77f2b-133">The date and time when the section group was last modified.</span></span> <span data-ttu-id="77f2b-134">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="77f2b-134">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="77f2b-135">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="77f2b-135">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="77f2b-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="77f2b-136">Read-only.</span></span>|
|<span data-ttu-id="77f2b-137">displayName</span><span class="sxs-lookup"><span data-stu-id="77f2b-137">displayName</span></span>|<span data-ttu-id="77f2b-138">String</span><span class="sxs-lookup"><span data-stu-id="77f2b-138">String</span></span>|<span data-ttu-id="77f2b-139">Имя группы разделов.</span><span class="sxs-lookup"><span data-stu-id="77f2b-139">The name of the section group.</span></span>|
|<span data-ttu-id="77f2b-140">Сектионграупсурл</span><span class="sxs-lookup"><span data-stu-id="77f2b-140">sectionGroupsUrl</span></span>|<span data-ttu-id="77f2b-141">String</span><span class="sxs-lookup"><span data-stu-id="77f2b-141">String</span></span>|<span data-ttu-id="77f2b-142">URL-адрес для `sectionGroups` свойства навигации, который возвращает все группы разделов в группе разделов.</span><span class="sxs-lookup"><span data-stu-id="77f2b-142">The URL for the `sectionGroups` navigation property, which returns all the section groups in the section group.</span></span> <span data-ttu-id="77f2b-143">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="77f2b-143">Read-only.</span></span>|
|<span data-ttu-id="77f2b-144">Сектионсурл</span><span class="sxs-lookup"><span data-stu-id="77f2b-144">sectionsUrl</span></span>|<span data-ttu-id="77f2b-145">String</span><span class="sxs-lookup"><span data-stu-id="77f2b-145">String</span></span>|<span data-ttu-id="77f2b-146">URL-адрес для `sections` свойства навигации, который возвращает все разделы в группе разделов.</span><span class="sxs-lookup"><span data-stu-id="77f2b-146">The URL for the `sections` navigation property, which returns all the sections in the section group.</span></span> <span data-ttu-id="77f2b-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="77f2b-147">Read-only.</span></span>|
|<span data-ttu-id="77f2b-148">Self</span><span class="sxs-lookup"><span data-stu-id="77f2b-148">self</span></span>|<span data-ttu-id="77f2b-149">String</span><span class="sxs-lookup"><span data-stu-id="77f2b-149">String</span></span>|<span data-ttu-id="77f2b-150">Конечная точка, где можно получить сведения о группе разделов.</span><span class="sxs-lookup"><span data-stu-id="77f2b-150">The endpoint where you can get details about the section group.</span></span> <span data-ttu-id="77f2b-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="77f2b-151">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="77f2b-152">Отношения</span><span class="sxs-lookup"><span data-stu-id="77f2b-152">Relationships</span></span>
| <span data-ttu-id="77f2b-153">Отношение</span><span class="sxs-lookup"><span data-stu-id="77f2b-153">Relationship</span></span> | <span data-ttu-id="77f2b-154">Тип</span><span class="sxs-lookup"><span data-stu-id="77f2b-154">Type</span></span>   |<span data-ttu-id="77f2b-155">Описание</span><span class="sxs-lookup"><span data-stu-id="77f2b-155">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="77f2b-156">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="77f2b-156">parentNotebook</span></span>|[<span data-ttu-id="77f2b-157">записной книжки</span><span class="sxs-lookup"><span data-stu-id="77f2b-157">notebook</span></span>](notebook.md)|<span data-ttu-id="77f2b-158">Записная книжка, содержащая группу разделов.</span><span class="sxs-lookup"><span data-stu-id="77f2b-158">The notebook that contains the section group.</span></span> <span data-ttu-id="77f2b-159">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="77f2b-159">Read-only.</span></span>|
|<span data-ttu-id="77f2b-160">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="77f2b-160">parentSectionGroup</span></span>|[<span data-ttu-id="77f2b-161">sectionGroup</span><span class="sxs-lookup"><span data-stu-id="77f2b-161">sectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="77f2b-162">Группа разделов, содержащая группу разделов.</span><span class="sxs-lookup"><span data-stu-id="77f2b-162">The section group that contains the section group.</span></span> <span data-ttu-id="77f2b-163">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="77f2b-163">Read-only.</span></span>|
|<span data-ttu-id="77f2b-164">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="77f2b-164">sectionGroups</span></span>|<span data-ttu-id="77f2b-165">Коллекция [sectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="77f2b-165">[sectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="77f2b-166">Группы разделов в разделе.</span><span class="sxs-lookup"><span data-stu-id="77f2b-166">The section groups in the section.</span></span> <span data-ttu-id="77f2b-167">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="77f2b-167">Read-only.</span></span> <span data-ttu-id="77f2b-168">Допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="77f2b-168">Nullable.</span></span>|
|<span data-ttu-id="77f2b-169">sections</span><span class="sxs-lookup"><span data-stu-id="77f2b-169">sections</span></span>|<span data-ttu-id="77f2b-170">Коллекция [оненотесектион](onenotesection.md)</span><span class="sxs-lookup"><span data-stu-id="77f2b-170">[onenoteSection](onenotesection.md) collection</span></span>|<span data-ttu-id="77f2b-171">Разделы в группе разделов.</span><span class="sxs-lookup"><span data-stu-id="77f2b-171">The sections in the section group.</span></span> <span data-ttu-id="77f2b-172">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="77f2b-172">Read-only.</span></span> <span data-ttu-id="77f2b-173">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="77f2b-173">Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="77f2b-174">Методы</span><span class="sxs-lookup"><span data-stu-id="77f2b-174">Methods</span></span>

| <span data-ttu-id="77f2b-175">Метод</span><span class="sxs-lookup"><span data-stu-id="77f2b-175">Method</span></span>           | <span data-ttu-id="77f2b-176">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="77f2b-176">Return Type</span></span>    |<span data-ttu-id="77f2b-177">Описание</span><span class="sxs-lookup"><span data-stu-id="77f2b-177">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="77f2b-178">Вывод группы разделов</span><span class="sxs-lookup"><span data-stu-id="77f2b-178">Get section group</span></span>](../api/sectiongroup-get.md) | [<span data-ttu-id="77f2b-179">sectionGroup</span><span class="sxs-lookup"><span data-stu-id="77f2b-179">sectionGroup</span></span>](sectiongroup.md) |<span data-ttu-id="77f2b-180">Прочитайте свойства и связи группы разделов.</span><span class="sxs-lookup"><span data-stu-id="77f2b-180">Read the properties and relationships of the section group.</span></span>|
|[<span data-ttu-id="77f2b-181">Создание группы разделов</span><span class="sxs-lookup"><span data-stu-id="77f2b-181">Create section group</span></span>](../api/sectiongroup-post-sectiongroups.md) |[<span data-ttu-id="77f2b-182">sectionGroup</span><span class="sxs-lookup"><span data-stu-id="77f2b-182">sectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="77f2b-183">Создание группы разделов путем отправки в коллекцию sectionGroups в указанной группе разделов.</span><span class="sxs-lookup"><span data-stu-id="77f2b-183">Create a section group by posting to the sectionGroups collection in the specified section group.</span></span>|
|[<span data-ttu-id="77f2b-184">Перечисление групп разделов</span><span class="sxs-lookup"><span data-stu-id="77f2b-184">List section groups</span></span>](../api/sectiongroup-list-sectiongroups.md) |<span data-ttu-id="77f2b-185">Коллекция [sectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="77f2b-185">[sectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="77f2b-186">Получение коллекции групп разделов в указанной группе разделов.</span><span class="sxs-lookup"><span data-stu-id="77f2b-186">Get collection of section groups in the specified section group.</span></span>|
|[<span data-ttu-id="77f2b-187">Создание раздела</span><span class="sxs-lookup"><span data-stu-id="77f2b-187">Create section</span></span>](../api/sectiongroup-post-sections.md) |[<span data-ttu-id="77f2b-188">Оненотесектион</span><span class="sxs-lookup"><span data-stu-id="77f2b-188">onenoteSection</span></span>](onenotesection.md)| <span data-ttu-id="77f2b-189">Создание раздела путем публикации в коллекции разделов в указанной группе разделов.</span><span class="sxs-lookup"><span data-stu-id="77f2b-189">Create a section by posting to the sections collection in the specified section group.</span></span>|
|[<span data-ttu-id="77f2b-190">Перечисление разделов</span><span class="sxs-lookup"><span data-stu-id="77f2b-190">List sections</span></span>](../api/sectiongroup-list-sections.md) |<span data-ttu-id="77f2b-191">Коллекция [оненотесектион](onenotesection.md)</span><span class="sxs-lookup"><span data-stu-id="77f2b-191">[onenoteSection](onenotesection.md) collection</span></span>| <span data-ttu-id="77f2b-192">Получение коллекции разделов в указанной группе разделов.</span><span class="sxs-lookup"><span data-stu-id="77f2b-192">Get a collection of sections in the specified section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "sectionGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
