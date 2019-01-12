---
title: Тип ресурса sectionGroup
description: Группа разделов в записной книжке OneNote. Группы разделов могут содержать разделы и группы разделов.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: ec27343121ba20ef65703f3df1d53e6c62ccc8e4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961878"
---
# <a name="sectiongroup-resource-type"></a><span data-ttu-id="2feee-104">Тип ресурса sectionGroup</span><span class="sxs-lookup"><span data-stu-id="2feee-104">sectionGroup resource type</span></span>

<span data-ttu-id="2feee-p102">Группа разделов в записной книжке OneNote. Группы разделов могут содержать разделы и группы разделов.</span><span class="sxs-lookup"><span data-stu-id="2feee-p102">A section group in a OneNote notebook. Section groups can contain sections and section groups.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2feee-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2feee-107">JSON representation</span></span>

<span data-ttu-id="2feee-108">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2feee-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="2feee-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="2feee-109">Properties</span></span>
| <span data-ttu-id="2feee-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="2feee-110">Property</span></span>     | <span data-ttu-id="2feee-111">Тип</span><span class="sxs-lookup"><span data-stu-id="2feee-111">Type</span></span>   |<span data-ttu-id="2feee-112">Описание</span><span class="sxs-lookup"><span data-stu-id="2feee-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2feee-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="2feee-113">createdBy</span></span>|[<span data-ttu-id="2feee-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="2feee-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="2feee-p103">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2feee-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="2feee-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2feee-117">createdDateTime</span></span>|<span data-ttu-id="2feee-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2feee-118">DateTimeOffset</span></span>|<span data-ttu-id="2feee-p104">Дата и время создания группы разделов. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2feee-p104">The date and time when the section group was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="2feee-123">id</span><span class="sxs-lookup"><span data-stu-id="2feee-123">id</span></span>|<span data-ttu-id="2feee-124">String</span><span class="sxs-lookup"><span data-stu-id="2feee-124">String</span></span>|<span data-ttu-id="2feee-p105">Уникальный идентификатор группы разделов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2feee-p105">The unique identifier of the section group. Read-only.</span></span>|
|<span data-ttu-id="2feee-127">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="2feee-127">lastModifiedBy</span></span>|[<span data-ttu-id="2feee-128">identitySet</span><span class="sxs-lookup"><span data-stu-id="2feee-128">identitySet</span></span>](identityset.md)|<span data-ttu-id="2feee-p106">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2feee-p106">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="2feee-131">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2feee-131">lastModifiedDateTime</span></span>|<span data-ttu-id="2feee-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2feee-132">DateTimeOffset</span></span>|<span data-ttu-id="2feee-p107">Дата и время последнего изменения группы разделов. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2feee-p107">The date and time when the section group was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="2feee-137">displayName</span><span class="sxs-lookup"><span data-stu-id="2feee-137">displayName</span></span>|<span data-ttu-id="2feee-138">Строка</span><span class="sxs-lookup"><span data-stu-id="2feee-138">String</span></span>|<span data-ttu-id="2feee-139">Имя группы разделов.</span><span class="sxs-lookup"><span data-stu-id="2feee-139">The name of the section group.</span></span>|
|<span data-ttu-id="2feee-140">sectionGroupsUrl</span><span class="sxs-lookup"><span data-stu-id="2feee-140">sectionGroupsUrl</span></span>|<span data-ttu-id="2feee-141">Строка</span><span class="sxs-lookup"><span data-stu-id="2feee-141">String</span></span>|<span data-ttu-id="2feee-p108">URL-адрес для свойства навигации `sectionGroups`, который возвращает все группы разделов в группе разделов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2feee-p108">The URL for the `sectionGroups` navigation property, which returns all the section groups in the section group. Read-only.</span></span>|
|<span data-ttu-id="2feee-144">sectionsUrl</span><span class="sxs-lookup"><span data-stu-id="2feee-144">sectionsUrl</span></span>|<span data-ttu-id="2feee-145">Строка</span><span class="sxs-lookup"><span data-stu-id="2feee-145">String</span></span>|<span data-ttu-id="2feee-p109">URL-адрес для свойства навигации `sections`, который возвращает все разделы в группе разделов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2feee-p109">The URL for the `sections` navigation property, which returns all the sections in the section group. Read-only.</span></span>|
|<span data-ttu-id="2feee-148">self</span><span class="sxs-lookup"><span data-stu-id="2feee-148">self</span></span>|<span data-ttu-id="2feee-149">String</span><span class="sxs-lookup"><span data-stu-id="2feee-149">String</span></span>|<span data-ttu-id="2feee-p110">Конечная точка, в которой можно получить сведения о группе разделов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2feee-p110">The endpoint where you can get details about the section group. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2feee-152">Связи</span><span class="sxs-lookup"><span data-stu-id="2feee-152">Relationships</span></span>
| <span data-ttu-id="2feee-153">Связь</span><span class="sxs-lookup"><span data-stu-id="2feee-153">Relationship</span></span> | <span data-ttu-id="2feee-154">Тип</span><span class="sxs-lookup"><span data-stu-id="2feee-154">Type</span></span>   |<span data-ttu-id="2feee-155">Описание</span><span class="sxs-lookup"><span data-stu-id="2feee-155">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2feee-156">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="2feee-156">parentNotebook</span></span>|[<span data-ttu-id="2feee-157">Notebook</span><span class="sxs-lookup"><span data-stu-id="2feee-157">Notebook</span></span>](notebook.md)|<span data-ttu-id="2feee-p111">Записная книжка, содержащая группу разделов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2feee-p111">The notebook that contains the section group. Read-only.</span></span>|
|<span data-ttu-id="2feee-160">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="2feee-160">parentSectionGroup</span></span>|[<span data-ttu-id="2feee-161">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="2feee-161">SectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="2feee-p112">Группа разделов, содержащая группу разделов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2feee-p112">The section group that contains the section group. Read-only.</span></span>|
|<span data-ttu-id="2feee-164">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="2feee-164">sectionGroups</span></span>|<span data-ttu-id="2feee-165">Коллекция объектов [SectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="2feee-165">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="2feee-p113">Группы разделов в разделе. Только для чтения. Допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="2feee-p113">The section groups in the section. Read-only. Nullable.</span></span>|
|<span data-ttu-id="2feee-169">sections</span><span class="sxs-lookup"><span data-stu-id="2feee-169">sections</span></span>|<span data-ttu-id="2feee-170">[OnenoteSection](section.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="2feee-170">[OnenoteSection](section.md) collection</span></span>|<span data-ttu-id="2feee-p114">Разделы в группе разделов. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="2feee-p114">The sections in the section group. Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="2feee-174">Методы</span><span class="sxs-lookup"><span data-stu-id="2feee-174">Methods</span></span>

| <span data-ttu-id="2feee-175">Метод</span><span class="sxs-lookup"><span data-stu-id="2feee-175">Method</span></span>           | <span data-ttu-id="2feee-176">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2feee-176">Return Type</span></span>    |<span data-ttu-id="2feee-177">Описание</span><span class="sxs-lookup"><span data-stu-id="2feee-177">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2feee-178">Получение группы разделов</span><span class="sxs-lookup"><span data-stu-id="2feee-178">Get section group</span></span>](../api/sectiongroup-get.md) | [<span data-ttu-id="2feee-179">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="2feee-179">SectionGroup</span></span>](sectiongroup.md) |<span data-ttu-id="2feee-180">Чтение свойств и отношений группы разделов.</span><span class="sxs-lookup"><span data-stu-id="2feee-180">Read the properties and relationships of the section group.</span></span>|
|[<span data-ttu-id="2feee-181">Создание группы разделов</span><span class="sxs-lookup"><span data-stu-id="2feee-181">Create section group</span></span>](../api/sectiongroup-post-sectiongroups.md) |[<span data-ttu-id="2feee-182">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="2feee-182">SectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="2feee-183">Создайте группу разделов, отправив запрос POST в коллекцию sectionGroups в указанной группе разделов.</span><span class="sxs-lookup"><span data-stu-id="2feee-183">Create a section group by posting to the sectionGroups collection in the specified section group.</span></span>|
|[<span data-ttu-id="2feee-184">Перечисление групп разделов</span><span class="sxs-lookup"><span data-stu-id="2feee-184">List section groups</span></span>](../api/sectiongroup-list-sectiongroups.md) |<span data-ttu-id="2feee-185">Коллекция объектов [SectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="2feee-185">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="2feee-186">Получение коллекции групп разделов в указанной группе разделов.</span><span class="sxs-lookup"><span data-stu-id="2feee-186">Get collection of section groups in the specified section group.</span></span>|
|[<span data-ttu-id="2feee-187">Создание раздела</span><span class="sxs-lookup"><span data-stu-id="2feee-187">Create section</span></span>](../api/sectiongroup-post-sections.md) |[<span data-ttu-id="2feee-188">OnenoteSection</span><span class="sxs-lookup"><span data-stu-id="2feee-188">OnenoteSection</span></span>](section.md)| <span data-ttu-id="2feee-189">Создайте раздел, отправив запрос POST в коллекцию sections в указанной группе разделов.</span><span class="sxs-lookup"><span data-stu-id="2feee-189">Create a section by posting to the sections collection in the specified section group.</span></span>|
|[<span data-ttu-id="2feee-190">Перечисление разделов</span><span class="sxs-lookup"><span data-stu-id="2feee-190">List sections</span></span>](../api/sectiongroup-list-sections.md) |<span data-ttu-id="2feee-191">[OnenoteSection](section.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="2feee-191">[OnenoteSection](section.md) collection</span></span>| <span data-ttu-id="2feee-192">Получение коллекции разделов в указанной группе разделов.</span><span class="sxs-lookup"><span data-stu-id="2feee-192">Get a collection of sections in the specified section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sectionGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
