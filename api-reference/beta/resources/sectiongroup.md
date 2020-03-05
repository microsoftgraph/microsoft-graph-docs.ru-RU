---
title: Тип ресурса sectionGroup
description: Группа разделов в записной книжке OneNote. Группы разделов могут содержать разделы и группы разделов.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 5183affe44244ab5cdc5685dd1200443d583fcaa
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520880"
---
# <a name="sectiongroup-resource-type"></a><span data-ttu-id="346a5-104">Тип ресурса sectionGroup</span><span class="sxs-lookup"><span data-stu-id="346a5-104">sectionGroup resource type</span></span>

<span data-ttu-id="346a5-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="346a5-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="346a5-106">Группа разделов в записной книжке OneNote.</span><span class="sxs-lookup"><span data-stu-id="346a5-106">A section group in a OneNote notebook.</span></span> <span data-ttu-id="346a5-107">Группы разделов могут содержать разделы и группы разделов.</span><span class="sxs-lookup"><span data-stu-id="346a5-107">Section groups can contain sections and section groups.</span></span>

## <a name="json-representation"></a><span data-ttu-id="346a5-108">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="346a5-108">JSON representation</span></span>

<span data-ttu-id="346a5-109">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="346a5-109">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="346a5-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="346a5-110">Properties</span></span>
| <span data-ttu-id="346a5-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="346a5-111">Property</span></span>     | <span data-ttu-id="346a5-112">Тип</span><span class="sxs-lookup"><span data-stu-id="346a5-112">Type</span></span>   |<span data-ttu-id="346a5-113">Описание</span><span class="sxs-lookup"><span data-stu-id="346a5-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="346a5-114">createdBy</span><span class="sxs-lookup"><span data-stu-id="346a5-114">createdBy</span></span>|[<span data-ttu-id="346a5-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="346a5-115">identitySet</span></span>](identityset.md)|<span data-ttu-id="346a5-p103">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="346a5-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="346a5-118">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="346a5-118">createdDateTime</span></span>|<span data-ttu-id="346a5-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="346a5-119">DateTimeOffset</span></span>|<span data-ttu-id="346a5-120">Дата и время создания группы разделов.</span><span class="sxs-lookup"><span data-stu-id="346a5-120">The date and time when the section group was created.</span></span> <span data-ttu-id="346a5-121">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="346a5-121">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="346a5-122">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="346a5-122">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="346a5-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="346a5-123">Read-only.</span></span>|
|<span data-ttu-id="346a5-124">id</span><span class="sxs-lookup"><span data-stu-id="346a5-124">id</span></span>|<span data-ttu-id="346a5-125">String</span><span class="sxs-lookup"><span data-stu-id="346a5-125">String</span></span>|<span data-ttu-id="346a5-126">Уникальный идентификатор группы разделов.</span><span class="sxs-lookup"><span data-stu-id="346a5-126">The unique identifier of the section group.</span></span> <span data-ttu-id="346a5-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="346a5-127">Read-only.</span></span>|
|<span data-ttu-id="346a5-128">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="346a5-128">lastModifiedBy</span></span>|[<span data-ttu-id="346a5-129">identitySet</span><span class="sxs-lookup"><span data-stu-id="346a5-129">identitySet</span></span>](identityset.md)|<span data-ttu-id="346a5-p106">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="346a5-p106">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="346a5-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="346a5-132">lastModifiedDateTime</span></span>|<span data-ttu-id="346a5-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="346a5-133">DateTimeOffset</span></span>|<span data-ttu-id="346a5-134">Дата и время последнего изменения группы разделов.</span><span class="sxs-lookup"><span data-stu-id="346a5-134">The date and time when the section group was last modified.</span></span> <span data-ttu-id="346a5-135">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="346a5-135">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="346a5-136">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="346a5-136">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="346a5-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="346a5-137">Read-only.</span></span>|
|<span data-ttu-id="346a5-138">displayName</span><span class="sxs-lookup"><span data-stu-id="346a5-138">displayName</span></span>|<span data-ttu-id="346a5-139">Строка</span><span class="sxs-lookup"><span data-stu-id="346a5-139">String</span></span>|<span data-ttu-id="346a5-140">Имя группы разделов.</span><span class="sxs-lookup"><span data-stu-id="346a5-140">The name of the section group.</span></span>|
|<span data-ttu-id="346a5-141">сектионграупсурл</span><span class="sxs-lookup"><span data-stu-id="346a5-141">sectionGroupsUrl</span></span>|<span data-ttu-id="346a5-142">String</span><span class="sxs-lookup"><span data-stu-id="346a5-142">String</span></span>|<span data-ttu-id="346a5-143">URL-адрес для `sectionGroups` свойства навигации, который возвращает все группы разделов в группе разделов.</span><span class="sxs-lookup"><span data-stu-id="346a5-143">The URL for the `sectionGroups` navigation property, which returns all the section groups in the section group.</span></span> <span data-ttu-id="346a5-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="346a5-144">Read-only.</span></span>|
|<span data-ttu-id="346a5-145">сектионсурл</span><span class="sxs-lookup"><span data-stu-id="346a5-145">sectionsUrl</span></span>|<span data-ttu-id="346a5-146">String</span><span class="sxs-lookup"><span data-stu-id="346a5-146">String</span></span>|<span data-ttu-id="346a5-147">URL-адрес для `sections` свойства навигации, который возвращает все разделы в группе разделов.</span><span class="sxs-lookup"><span data-stu-id="346a5-147">The URL for the `sections` navigation property, which returns all the sections in the section group.</span></span> <span data-ttu-id="346a5-148">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="346a5-148">Read-only.</span></span>|
|<span data-ttu-id="346a5-149">Self</span><span class="sxs-lookup"><span data-stu-id="346a5-149">self</span></span>|<span data-ttu-id="346a5-150">String</span><span class="sxs-lookup"><span data-stu-id="346a5-150">String</span></span>|<span data-ttu-id="346a5-151">Конечная точка, где можно получить сведения о группе разделов.</span><span class="sxs-lookup"><span data-stu-id="346a5-151">The endpoint where you can get details about the section group.</span></span> <span data-ttu-id="346a5-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="346a5-152">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="346a5-153">Отношения</span><span class="sxs-lookup"><span data-stu-id="346a5-153">Relationships</span></span>
| <span data-ttu-id="346a5-154">Связь</span><span class="sxs-lookup"><span data-stu-id="346a5-154">Relationship</span></span> | <span data-ttu-id="346a5-155">Тип</span><span class="sxs-lookup"><span data-stu-id="346a5-155">Type</span></span>   |<span data-ttu-id="346a5-156">Описание</span><span class="sxs-lookup"><span data-stu-id="346a5-156">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="346a5-157">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="346a5-157">parentNotebook</span></span>|[<span data-ttu-id="346a5-158">notebook</span><span class="sxs-lookup"><span data-stu-id="346a5-158">notebook</span></span>](notebook.md)|<span data-ttu-id="346a5-159">Записная книжка, содержащая группу разделов.</span><span class="sxs-lookup"><span data-stu-id="346a5-159">The notebook that contains the section group.</span></span> <span data-ttu-id="346a5-160">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="346a5-160">Read-only.</span></span>|
|<span data-ttu-id="346a5-161">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="346a5-161">parentSectionGroup</span></span>|[<span data-ttu-id="346a5-162">sectionGroup</span><span class="sxs-lookup"><span data-stu-id="346a5-162">sectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="346a5-163">Группа разделов, содержащая группу разделов.</span><span class="sxs-lookup"><span data-stu-id="346a5-163">The section group that contains the section group.</span></span> <span data-ttu-id="346a5-164">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="346a5-164">Read-only.</span></span>|
|<span data-ttu-id="346a5-165">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="346a5-165">sectionGroups</span></span>|<span data-ttu-id="346a5-166">Коллекция [sectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="346a5-166">[sectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="346a5-167">Группы разделов в разделе.</span><span class="sxs-lookup"><span data-stu-id="346a5-167">The section groups in the section.</span></span> <span data-ttu-id="346a5-168">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="346a5-168">Read-only.</span></span> <span data-ttu-id="346a5-169">Допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="346a5-169">Nullable.</span></span>|
|<span data-ttu-id="346a5-170">sections</span><span class="sxs-lookup"><span data-stu-id="346a5-170">sections</span></span>|<span data-ttu-id="346a5-171">Коллекция [оненотесектион](onenotesection.md)</span><span class="sxs-lookup"><span data-stu-id="346a5-171">[onenoteSection](onenotesection.md) collection</span></span>|<span data-ttu-id="346a5-172">Разделы в группе разделов.</span><span class="sxs-lookup"><span data-stu-id="346a5-172">The sections in the section group.</span></span> <span data-ttu-id="346a5-173">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="346a5-173">Read-only.</span></span> <span data-ttu-id="346a5-174">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="346a5-174">Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="346a5-175">Методы</span><span class="sxs-lookup"><span data-stu-id="346a5-175">Methods</span></span>

| <span data-ttu-id="346a5-176">Метод</span><span class="sxs-lookup"><span data-stu-id="346a5-176">Method</span></span>           | <span data-ttu-id="346a5-177">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="346a5-177">Return Type</span></span>    |<span data-ttu-id="346a5-178">Описание</span><span class="sxs-lookup"><span data-stu-id="346a5-178">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="346a5-179">Вывод группы разделов</span><span class="sxs-lookup"><span data-stu-id="346a5-179">Get section group</span></span>](../api/sectiongroup-get.md) | [<span data-ttu-id="346a5-180">sectionGroup</span><span class="sxs-lookup"><span data-stu-id="346a5-180">sectionGroup</span></span>](sectiongroup.md) |<span data-ttu-id="346a5-181">Прочитайте свойства и связи группы разделов.</span><span class="sxs-lookup"><span data-stu-id="346a5-181">Read the properties and relationships of the section group.</span></span>|
|[<span data-ttu-id="346a5-182">Создание группы разделов</span><span class="sxs-lookup"><span data-stu-id="346a5-182">Create section group</span></span>](../api/sectiongroup-post-sectiongroups.md) |[<span data-ttu-id="346a5-183">sectionGroup</span><span class="sxs-lookup"><span data-stu-id="346a5-183">sectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="346a5-184">Создание группы разделов путем отправки в коллекцию sectionGroups в указанной группе разделов.</span><span class="sxs-lookup"><span data-stu-id="346a5-184">Create a section group by posting to the sectionGroups collection in the specified section group.</span></span>|
|[<span data-ttu-id="346a5-185">Перечисление групп разделов</span><span class="sxs-lookup"><span data-stu-id="346a5-185">List section groups</span></span>](../api/sectiongroup-list-sectiongroups.md) |<span data-ttu-id="346a5-186">Коллекция [sectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="346a5-186">[sectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="346a5-187">Получение коллекции групп разделов в указанной группе разделов.</span><span class="sxs-lookup"><span data-stu-id="346a5-187">Get collection of section groups in the specified section group.</span></span>|
|[<span data-ttu-id="346a5-188">Создание раздела</span><span class="sxs-lookup"><span data-stu-id="346a5-188">Create section</span></span>](../api/sectiongroup-post-sections.md) |[<span data-ttu-id="346a5-189">оненотесектион</span><span class="sxs-lookup"><span data-stu-id="346a5-189">onenoteSection</span></span>](onenotesection.md)| <span data-ttu-id="346a5-190">Создание раздела путем публикации в коллекции разделов в указанной группе разделов.</span><span class="sxs-lookup"><span data-stu-id="346a5-190">Create a section by posting to the sections collection in the specified section group.</span></span>|
|[<span data-ttu-id="346a5-191">Перечисление разделов</span><span class="sxs-lookup"><span data-stu-id="346a5-191">List sections</span></span>](../api/sectiongroup-list-sections.md) |<span data-ttu-id="346a5-192">Коллекция [оненотесектион](onenotesection.md)</span><span class="sxs-lookup"><span data-stu-id="346a5-192">[onenoteSection](onenotesection.md) collection</span></span>| <span data-ttu-id="346a5-193">Получение коллекции разделов в указанной группе разделов.</span><span class="sxs-lookup"><span data-stu-id="346a5-193">Get a collection of sections in the specified section group.</span></span>|

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
