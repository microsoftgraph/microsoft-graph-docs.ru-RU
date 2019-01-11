---
title: Тип ресурса sectionGroup
description: Группа разделов в записной книжке OneNote. Группы разделов могут содержать разделы и группы разделов.
localization_priority: Normal
ms.openlocfilehash: f204c5422eb5f0f2580bfbed82ed28306dd0618f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806309"
---
# <a name="sectiongroup-resource-type"></a><span data-ttu-id="8b5dc-104">Тип ресурса sectionGroup</span><span class="sxs-lookup"><span data-stu-id="8b5dc-104">sectionGroup resource type</span></span>

<span data-ttu-id="8b5dc-p102">Группа разделов в записной книжке OneNote. Группы разделов могут содержать разделы и группы разделов.</span><span class="sxs-lookup"><span data-stu-id="8b5dc-p102">A section group in a OneNote notebook. Section groups can contain sections and section groups.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8b5dc-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8b5dc-107">JSON representation</span></span>

<span data-ttu-id="8b5dc-108">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8b5dc-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="8b5dc-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="8b5dc-109">Properties</span></span>
| <span data-ttu-id="8b5dc-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="8b5dc-110">Property</span></span>     | <span data-ttu-id="8b5dc-111">Тип</span><span class="sxs-lookup"><span data-stu-id="8b5dc-111">Type</span></span>   |<span data-ttu-id="8b5dc-112">Описание</span><span class="sxs-lookup"><span data-stu-id="8b5dc-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8b5dc-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="8b5dc-113">createdBy</span></span>|[<span data-ttu-id="8b5dc-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="8b5dc-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="8b5dc-p103">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8b5dc-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="8b5dc-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8b5dc-117">createdDateTime</span></span>|<span data-ttu-id="8b5dc-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8b5dc-118">DateTimeOffset</span></span>|<span data-ttu-id="8b5dc-p104">Дата и время создания группы разделов. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8b5dc-p104">The date and time when the section group was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="8b5dc-123">id</span><span class="sxs-lookup"><span data-stu-id="8b5dc-123">id</span></span>|<span data-ttu-id="8b5dc-124">Строка</span><span class="sxs-lookup"><span data-stu-id="8b5dc-124">String</span></span>|<span data-ttu-id="8b5dc-p105">Уникальный идентификатор группы разделов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8b5dc-p105">The unique identifier of the section group. Read-only.</span></span>|
|<span data-ttu-id="8b5dc-127">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="8b5dc-127">lastModifiedBy</span></span>|[<span data-ttu-id="8b5dc-128">identitySet</span><span class="sxs-lookup"><span data-stu-id="8b5dc-128">identitySet</span></span>](identityset.md)|<span data-ttu-id="8b5dc-p106">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8b5dc-p106">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="8b5dc-131">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8b5dc-131">lastModifiedDateTime</span></span>|<span data-ttu-id="8b5dc-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8b5dc-132">DateTimeOffset</span></span>|<span data-ttu-id="8b5dc-p107">Дата и время последнего изменения группы разделов. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8b5dc-p107">The date and time when the section group was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="8b5dc-137">displayName</span><span class="sxs-lookup"><span data-stu-id="8b5dc-137">displayName</span></span>|<span data-ttu-id="8b5dc-138">Строка</span><span class="sxs-lookup"><span data-stu-id="8b5dc-138">String</span></span>|<span data-ttu-id="8b5dc-139">Имя группы разделов.</span><span class="sxs-lookup"><span data-stu-id="8b5dc-139">The name of the section group.</span></span>|
|<span data-ttu-id="8b5dc-140">sectionGroupsUrl</span><span class="sxs-lookup"><span data-stu-id="8b5dc-140">sectionGroupsUrl</span></span>|<span data-ttu-id="8b5dc-141">Строка</span><span class="sxs-lookup"><span data-stu-id="8b5dc-141">String</span></span>|<span data-ttu-id="8b5dc-p108">URL-адрес для свойства навигации `sectionGroups`, который возвращает все группы разделов в группе разделов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8b5dc-p108">The URL for the `sectionGroups` navigation property, which returns all the section groups in the section group. Read-only.</span></span>|
|<span data-ttu-id="8b5dc-144">sectionsUrl</span><span class="sxs-lookup"><span data-stu-id="8b5dc-144">sectionsUrl</span></span>|<span data-ttu-id="8b5dc-145">Строка</span><span class="sxs-lookup"><span data-stu-id="8b5dc-145">String</span></span>|<span data-ttu-id="8b5dc-p109">URL-адрес для свойства навигации `sections`, который возвращает все разделы в группе разделов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8b5dc-p109">The URL for the `sections` navigation property, which returns all the sections in the section group. Read-only.</span></span>|
|<span data-ttu-id="8b5dc-148">self</span><span class="sxs-lookup"><span data-stu-id="8b5dc-148">self</span></span>|<span data-ttu-id="8b5dc-149">Строка</span><span class="sxs-lookup"><span data-stu-id="8b5dc-149">String</span></span>|<span data-ttu-id="8b5dc-p110">Конечная точка, в которой можно получить сведения о группе разделов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8b5dc-p110">The endpoint where you can get details about the section group. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8b5dc-152">Связи</span><span class="sxs-lookup"><span data-stu-id="8b5dc-152">Relationships</span></span>
| <span data-ttu-id="8b5dc-153">Связь</span><span class="sxs-lookup"><span data-stu-id="8b5dc-153">Relationship</span></span> | <span data-ttu-id="8b5dc-154">Тип</span><span class="sxs-lookup"><span data-stu-id="8b5dc-154">Type</span></span>   |<span data-ttu-id="8b5dc-155">Описание</span><span class="sxs-lookup"><span data-stu-id="8b5dc-155">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8b5dc-156">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="8b5dc-156">parentNotebook</span></span>|[<span data-ttu-id="8b5dc-157">Notebook</span><span class="sxs-lookup"><span data-stu-id="8b5dc-157">Notebook</span></span>](notebook.md)|<span data-ttu-id="8b5dc-p111">Записная книжка, содержащая группу разделов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8b5dc-p111">The notebook that contains the section group. Read-only.</span></span>|
|<span data-ttu-id="8b5dc-160">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="8b5dc-160">parentSectionGroup</span></span>|[<span data-ttu-id="8b5dc-161">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="8b5dc-161">SectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="8b5dc-p112">Группа разделов, содержащая группу разделов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8b5dc-p112">The section group that contains the section group. Read-only.</span></span>|
|<span data-ttu-id="8b5dc-164">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="8b5dc-164">sectionGroups</span></span>|<span data-ttu-id="8b5dc-165">Коллекция объектов [SectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="8b5dc-165">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="8b5dc-p113">Группы разделов в разделе. Только для чтения. Допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="8b5dc-p113">The section groups in the section. Read-only. Nullable.</span></span>|
|<span data-ttu-id="8b5dc-169">sections</span><span class="sxs-lookup"><span data-stu-id="8b5dc-169">sections</span></span>|<span data-ttu-id="8b5dc-170">[OnenoteSection](section.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="8b5dc-170">[OnenoteSection](section.md) collection</span></span>|<span data-ttu-id="8b5dc-p114">Разделы в группе разделов. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="8b5dc-p114">The sections in the section group. Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="8b5dc-174">Методы</span><span class="sxs-lookup"><span data-stu-id="8b5dc-174">Methods</span></span>

| <span data-ttu-id="8b5dc-175">Метод</span><span class="sxs-lookup"><span data-stu-id="8b5dc-175">Method</span></span>           | <span data-ttu-id="8b5dc-176">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8b5dc-176">Return Type</span></span>    |<span data-ttu-id="8b5dc-177">Описание</span><span class="sxs-lookup"><span data-stu-id="8b5dc-177">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8b5dc-178">Получение группы разделов</span><span class="sxs-lookup"><span data-stu-id="8b5dc-178">Get section group</span></span>](../api/sectiongroup-get.md) | [<span data-ttu-id="8b5dc-179">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="8b5dc-179">SectionGroup</span></span>](sectiongroup.md) |<span data-ttu-id="8b5dc-180">Чтение свойств и отношений группы разделов.</span><span class="sxs-lookup"><span data-stu-id="8b5dc-180">Read the properties and relationships of the section group.</span></span>|
|[<span data-ttu-id="8b5dc-181">Создание группы разделов</span><span class="sxs-lookup"><span data-stu-id="8b5dc-181">Create section group</span></span>](../api/sectiongroup-post-sectiongroups.md) |[<span data-ttu-id="8b5dc-182">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="8b5dc-182">SectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="8b5dc-183">Создайте группу разделов, отправив запрос POST в коллекцию sectionGroups в указанной группе разделов.</span><span class="sxs-lookup"><span data-stu-id="8b5dc-183">Create a section group by posting to the sectionGroups collection in the specified section group.</span></span>|
|[<span data-ttu-id="8b5dc-184">Перечисление групп разделов</span><span class="sxs-lookup"><span data-stu-id="8b5dc-184">List section groups</span></span>](../api/sectiongroup-list-sectiongroups.md) |<span data-ttu-id="8b5dc-185">Коллекция объектов [SectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="8b5dc-185">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="8b5dc-186">Получение коллекции групп разделов в указанной группе разделов.</span><span class="sxs-lookup"><span data-stu-id="8b5dc-186">Get collection of section groups in the specified section group.</span></span>|
|[<span data-ttu-id="8b5dc-187">Создание раздела</span><span class="sxs-lookup"><span data-stu-id="8b5dc-187">Create section</span></span>](../api/sectiongroup-post-sections.md) |[<span data-ttu-id="8b5dc-188">OnenoteSection</span><span class="sxs-lookup"><span data-stu-id="8b5dc-188">OnenoteSection</span></span>](section.md)| <span data-ttu-id="8b5dc-189">Создайте раздел, отправив запрос POST в коллекцию sections в указанной группе разделов.</span><span class="sxs-lookup"><span data-stu-id="8b5dc-189">Create a section by posting to the sections collection in the specified section group.</span></span>|
|[<span data-ttu-id="8b5dc-190">Перечисление разделов</span><span class="sxs-lookup"><span data-stu-id="8b5dc-190">List sections</span></span>](../api/sectiongroup-list-sections.md) |<span data-ttu-id="8b5dc-191">[OnenoteSection](section.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="8b5dc-191">[OnenoteSection](section.md) collection</span></span>| <span data-ttu-id="8b5dc-192">Получение коллекции разделов в указанной группе разделов.</span><span class="sxs-lookup"><span data-stu-id="8b5dc-192">Get a collection of sections in the specified section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sectionGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
