---
title: Тип ресурса sectionGroup
description: Группа разделов в записной книжке OneNote. Группы разделов могут содержать разделы и группы разделов.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 0b7368f18058c0c8b00c5b34e5a804521dc64682
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575522"
---
# <a name="sectiongroup-resource-type"></a><span data-ttu-id="ee8ca-104">Тип ресурса sectionGroup</span><span class="sxs-lookup"><span data-stu-id="ee8ca-104">sectionGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee8ca-p102">Группа разделов в записной книжке OneNote. Группы разделов могут содержать разделы и группы разделов.</span><span class="sxs-lookup"><span data-stu-id="ee8ca-p102">A section group in a OneNote notebook. Section groups can contain sections and section groups.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ee8ca-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ee8ca-107">JSON representation</span></span>

<span data-ttu-id="ee8ca-108">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ee8ca-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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
## <a name="properties"></a><span data-ttu-id="ee8ca-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="ee8ca-109">Properties</span></span>
| <span data-ttu-id="ee8ca-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="ee8ca-110">Property</span></span>     | <span data-ttu-id="ee8ca-111">Тип</span><span class="sxs-lookup"><span data-stu-id="ee8ca-111">Type</span></span>   |<span data-ttu-id="ee8ca-112">Описание</span><span class="sxs-lookup"><span data-stu-id="ee8ca-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ee8ca-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="ee8ca-113">createdBy</span></span>|[<span data-ttu-id="ee8ca-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="ee8ca-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="ee8ca-p103">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ee8ca-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="ee8ca-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ee8ca-117">createdDateTime</span></span>|<span data-ttu-id="ee8ca-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee8ca-118">DateTimeOffset</span></span>|<span data-ttu-id="ee8ca-p104">Дата и время создания группы разделов. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ee8ca-p104">The date and time when the section group was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="ee8ca-123">id</span><span class="sxs-lookup"><span data-stu-id="ee8ca-123">id</span></span>|<span data-ttu-id="ee8ca-124">Строка</span><span class="sxs-lookup"><span data-stu-id="ee8ca-124">String</span></span>|<span data-ttu-id="ee8ca-p105">Уникальный идентификатор группы разделов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ee8ca-p105">The unique identifier of the section group. Read-only.</span></span>|
|<span data-ttu-id="ee8ca-127">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="ee8ca-127">lastModifiedBy</span></span>|[<span data-ttu-id="ee8ca-128">identitySet</span><span class="sxs-lookup"><span data-stu-id="ee8ca-128">identitySet</span></span>](identityset.md)|<span data-ttu-id="ee8ca-p106">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ee8ca-p106">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="ee8ca-131">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ee8ca-131">lastModifiedDateTime</span></span>|<span data-ttu-id="ee8ca-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee8ca-132">DateTimeOffset</span></span>|<span data-ttu-id="ee8ca-p107">Дата и время последнего изменения группы разделов. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ee8ca-p107">The date and time when the section group was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="ee8ca-137">displayName</span><span class="sxs-lookup"><span data-stu-id="ee8ca-137">displayName</span></span>|<span data-ttu-id="ee8ca-138">Строка</span><span class="sxs-lookup"><span data-stu-id="ee8ca-138">String</span></span>|<span data-ttu-id="ee8ca-139">Имя группы разделов.</span><span class="sxs-lookup"><span data-stu-id="ee8ca-139">The name of the section group.</span></span>|
|<span data-ttu-id="ee8ca-140">sectionGroupsUrl</span><span class="sxs-lookup"><span data-stu-id="ee8ca-140">sectionGroupsUrl</span></span>|<span data-ttu-id="ee8ca-141">Строка</span><span class="sxs-lookup"><span data-stu-id="ee8ca-141">String</span></span>|<span data-ttu-id="ee8ca-p108">URL-адрес для свойства навигации `sectionGroups`, который возвращает все группы разделов в группе разделов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ee8ca-p108">The URL for the `sectionGroups` navigation property, which returns all the section groups in the section group. Read-only.</span></span>|
|<span data-ttu-id="ee8ca-144">sectionsUrl</span><span class="sxs-lookup"><span data-stu-id="ee8ca-144">sectionsUrl</span></span>|<span data-ttu-id="ee8ca-145">Строка</span><span class="sxs-lookup"><span data-stu-id="ee8ca-145">String</span></span>|<span data-ttu-id="ee8ca-p109">URL-адрес для свойства навигации `sections`, который возвращает все разделы в группе разделов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ee8ca-p109">The URL for the `sections` navigation property, which returns all the sections in the section group. Read-only.</span></span>|
|<span data-ttu-id="ee8ca-148">self</span><span class="sxs-lookup"><span data-stu-id="ee8ca-148">self</span></span>|<span data-ttu-id="ee8ca-149">Строка</span><span class="sxs-lookup"><span data-stu-id="ee8ca-149">String</span></span>|<span data-ttu-id="ee8ca-p110">Конечная точка, в которой можно получить сведения о группе разделов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ee8ca-p110">The endpoint where you can get details about the section group. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ee8ca-152">Связи</span><span class="sxs-lookup"><span data-stu-id="ee8ca-152">Relationships</span></span>
| <span data-ttu-id="ee8ca-153">Связь</span><span class="sxs-lookup"><span data-stu-id="ee8ca-153">Relationship</span></span> | <span data-ttu-id="ee8ca-154">Тип</span><span class="sxs-lookup"><span data-stu-id="ee8ca-154">Type</span></span>   |<span data-ttu-id="ee8ca-155">Описание</span><span class="sxs-lookup"><span data-stu-id="ee8ca-155">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ee8ca-156">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="ee8ca-156">parentNotebook</span></span>|[<span data-ttu-id="ee8ca-157">записная книжка</span><span class="sxs-lookup"><span data-stu-id="ee8ca-157">notebook</span></span>](notebook.md)|<span data-ttu-id="ee8ca-p111">Записная книжка, содержащая группу разделов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ee8ca-p111">The notebook that contains the section group. Read-only.</span></span>|
|<span data-ttu-id="ee8ca-160">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="ee8ca-160">parentSectionGroup</span></span>|[<span data-ttu-id="ee8ca-161">sectionGroup</span><span class="sxs-lookup"><span data-stu-id="ee8ca-161">sectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="ee8ca-p112">Группа разделов, содержащая группу разделов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ee8ca-p112">The section group that contains the section group. Read-only.</span></span>|
|<span data-ttu-id="ee8ca-164">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="ee8ca-164">sectionGroups</span></span>|<span data-ttu-id="ee8ca-165">[sectionGroup](sectiongroup.md) семейства сайтов</span><span class="sxs-lookup"><span data-stu-id="ee8ca-165">[sectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="ee8ca-p113">Группы разделов в разделе. Только для чтения. Допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="ee8ca-p113">The section groups in the section. Read-only. Nullable.</span></span>|
|<span data-ttu-id="ee8ca-169">sections</span><span class="sxs-lookup"><span data-stu-id="ee8ca-169">sections</span></span>|<span data-ttu-id="ee8ca-170">[onenoteSection](section.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="ee8ca-170">[onenoteSection](section.md) collection</span></span>|<span data-ttu-id="ee8ca-p114">Разделы в группе разделов. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="ee8ca-p114">The sections in the section group. Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="ee8ca-174">Методы</span><span class="sxs-lookup"><span data-stu-id="ee8ca-174">Methods</span></span>

| <span data-ttu-id="ee8ca-175">Метод</span><span class="sxs-lookup"><span data-stu-id="ee8ca-175">Method</span></span>           | <span data-ttu-id="ee8ca-176">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ee8ca-176">Return Type</span></span>    |<span data-ttu-id="ee8ca-177">Описание</span><span class="sxs-lookup"><span data-stu-id="ee8ca-177">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ee8ca-178">Получение группы разделов</span><span class="sxs-lookup"><span data-stu-id="ee8ca-178">Get section group</span></span>](../api/sectiongroup-get.md) | [<span data-ttu-id="ee8ca-179">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="ee8ca-179">SectionGroup</span></span>](sectiongroup.md) |<span data-ttu-id="ee8ca-180">Чтение свойств и отношений группы разделов.</span><span class="sxs-lookup"><span data-stu-id="ee8ca-180">Read the properties and relationships of the section group.</span></span>|
|[<span data-ttu-id="ee8ca-181">Создание группы разделов</span><span class="sxs-lookup"><span data-stu-id="ee8ca-181">Create section group</span></span>](../api/sectiongroup-post-sectiongroups.md) |[<span data-ttu-id="ee8ca-182">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="ee8ca-182">SectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="ee8ca-183">Создайте группу разделов, отправив запрос POST в коллекцию sectionGroups в указанной группе разделов.</span><span class="sxs-lookup"><span data-stu-id="ee8ca-183">Create a section group by posting to the sectionGroups collection in the specified section group.</span></span>|
|[<span data-ttu-id="ee8ca-184">Перечисление групп разделов</span><span class="sxs-lookup"><span data-stu-id="ee8ca-184">List section groups</span></span>](../api/sectiongroup-list-sectiongroups.md) |<span data-ttu-id="ee8ca-185">Коллекция объектов [SectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="ee8ca-185">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="ee8ca-186">Получение коллекции групп разделов в указанной группе разделов.</span><span class="sxs-lookup"><span data-stu-id="ee8ca-186">Get collection of section groups in the specified section group.</span></span>|
|[<span data-ttu-id="ee8ca-187">Создание раздела</span><span class="sxs-lookup"><span data-stu-id="ee8ca-187">Create section</span></span>](../api/sectiongroup-post-sections.md) |[<span data-ttu-id="ee8ca-188">Section</span><span class="sxs-lookup"><span data-stu-id="ee8ca-188">Section</span></span>](section.md)| <span data-ttu-id="ee8ca-189">Создайте раздел, отправив запрос POST в коллекцию sections в указанной группе разделов.</span><span class="sxs-lookup"><span data-stu-id="ee8ca-189">Create a section by posting to the sections collection in the specified section group.</span></span>|
|[<span data-ttu-id="ee8ca-190">Перечисление разделов</span><span class="sxs-lookup"><span data-stu-id="ee8ca-190">List sections</span></span>](../api/sectiongroup-list-sections.md) |<span data-ttu-id="ee8ca-191">Коллекция объектов [Section](section.md)</span><span class="sxs-lookup"><span data-stu-id="ee8ca-191">[Section](section.md) collection</span></span>| <span data-ttu-id="ee8ca-192">Получение коллекции разделов в указанной группе разделов.</span><span class="sxs-lookup"><span data-stu-id="ee8ca-192">Get a collection of sections in the specified section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "sectionGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/sectiongroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
