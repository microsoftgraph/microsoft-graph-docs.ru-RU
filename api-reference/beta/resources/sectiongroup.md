---
title: Тип ресурса sectionGroup
description: Группа разделов в записной книжке OneNote. Группы разделов могут содержать разделы и группы разделов.
ms.openlocfilehash: e27f3f468d660b2ffe778a46078054751ed8063e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081668"
---
# <a name="sectiongroup-resource-type"></a><span data-ttu-id="3ffaa-104">Тип ресурса sectionGroup</span><span class="sxs-lookup"><span data-stu-id="3ffaa-104">sectionGroup resource type</span></span>

> <span data-ttu-id="3ffaa-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3ffaa-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3ffaa-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ffaa-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3ffaa-p103">Группа разделов в записной книжке OneNote. Группы разделов могут содержать разделы и группы разделов.</span><span class="sxs-lookup"><span data-stu-id="3ffaa-p103">A section group in a OneNote notebook. Section groups can contain sections and section groups.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3ffaa-109">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3ffaa-109">JSON representation</span></span>

<span data-ttu-id="3ffaa-110">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3ffaa-110">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "parentNotebook",
    "parentSectionGroup",
    "sectionGroups",
    "sections"
  ],
  "@odata.type": "microsoft.graph.sectiongroup"
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
## <a name="properties"></a><span data-ttu-id="3ffaa-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="3ffaa-111">Properties</span></span>
| <span data-ttu-id="3ffaa-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="3ffaa-112">Property</span></span>     | <span data-ttu-id="3ffaa-113">Тип</span><span class="sxs-lookup"><span data-stu-id="3ffaa-113">Type</span></span>   |<span data-ttu-id="3ffaa-114">Описание</span><span class="sxs-lookup"><span data-stu-id="3ffaa-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3ffaa-115">createdBy</span><span class="sxs-lookup"><span data-stu-id="3ffaa-115">createdBy</span></span>|[<span data-ttu-id="3ffaa-116">identitySet</span><span class="sxs-lookup"><span data-stu-id="3ffaa-116">identitySet</span></span>](identityset.md)|<span data-ttu-id="3ffaa-p104">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3ffaa-p104">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="3ffaa-119">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3ffaa-119">createdDateTime</span></span>|<span data-ttu-id="3ffaa-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ffaa-120">DateTimeOffset</span></span>|<span data-ttu-id="3ffaa-p105">Дата и время создания группы разделов. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3ffaa-p105">The date and time when the section group was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="3ffaa-125">id</span><span class="sxs-lookup"><span data-stu-id="3ffaa-125">id</span></span>|<span data-ttu-id="3ffaa-126">String</span><span class="sxs-lookup"><span data-stu-id="3ffaa-126">String</span></span>|<span data-ttu-id="3ffaa-p106">Уникальный идентификатор группы разделов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3ffaa-p106">The unique identifier of the section group. Read-only.</span></span>|
|<span data-ttu-id="3ffaa-129">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="3ffaa-129">lastModifiedBy</span></span>|[<span data-ttu-id="3ffaa-130">identitySet</span><span class="sxs-lookup"><span data-stu-id="3ffaa-130">identitySet</span></span>](identityset.md)|<span data-ttu-id="3ffaa-p107">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3ffaa-p107">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="3ffaa-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3ffaa-133">lastModifiedDateTime</span></span>|<span data-ttu-id="3ffaa-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ffaa-134">DateTimeOffset</span></span>|<span data-ttu-id="3ffaa-p108">Дата и время последнего изменения группы разделов. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3ffaa-p108">The date and time when the section group was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="3ffaa-139">displayName</span><span class="sxs-lookup"><span data-stu-id="3ffaa-139">displayName</span></span>|<span data-ttu-id="3ffaa-140">Строка</span><span class="sxs-lookup"><span data-stu-id="3ffaa-140">String</span></span>|<span data-ttu-id="3ffaa-141">Имя группы разделов.</span><span class="sxs-lookup"><span data-stu-id="3ffaa-141">The name of the section group.</span></span>|
|<span data-ttu-id="3ffaa-142">sectionGroupsUrl</span><span class="sxs-lookup"><span data-stu-id="3ffaa-142">sectionGroupsUrl</span></span>|<span data-ttu-id="3ffaa-143">Строка</span><span class="sxs-lookup"><span data-stu-id="3ffaa-143">String</span></span>|<span data-ttu-id="3ffaa-p109">URL-адрес для свойства навигации `sectionGroups`, который возвращает все группы разделов в группе разделов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3ffaa-p109">The URL for the `sectionGroups` navigation property, which returns all the section groups in the section group. Read-only.</span></span>|
|<span data-ttu-id="3ffaa-146">sectionsUrl</span><span class="sxs-lookup"><span data-stu-id="3ffaa-146">sectionsUrl</span></span>|<span data-ttu-id="3ffaa-147">Строка</span><span class="sxs-lookup"><span data-stu-id="3ffaa-147">String</span></span>|<span data-ttu-id="3ffaa-p110">URL-адрес для свойства навигации `sections`, который возвращает все разделы в группе разделов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3ffaa-p110">The URL for the `sections` navigation property, which returns all the sections in the section group. Read-only.</span></span>|
|<span data-ttu-id="3ffaa-150">self</span><span class="sxs-lookup"><span data-stu-id="3ffaa-150">self</span></span>|<span data-ttu-id="3ffaa-151">String</span><span class="sxs-lookup"><span data-stu-id="3ffaa-151">String</span></span>|<span data-ttu-id="3ffaa-p111">Конечная точка, в которой можно получить сведения о группе разделов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3ffaa-p111">The endpoint where you can get details about the section group. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3ffaa-154">Связи</span><span class="sxs-lookup"><span data-stu-id="3ffaa-154">Relationships</span></span>
| <span data-ttu-id="3ffaa-155">Связь</span><span class="sxs-lookup"><span data-stu-id="3ffaa-155">Relationship</span></span> | <span data-ttu-id="3ffaa-156">Тип</span><span class="sxs-lookup"><span data-stu-id="3ffaa-156">Type</span></span>   |<span data-ttu-id="3ffaa-157">Описание</span><span class="sxs-lookup"><span data-stu-id="3ffaa-157">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3ffaa-158">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="3ffaa-158">parentNotebook</span></span>|[<span data-ttu-id="3ffaa-159">Notebook</span><span class="sxs-lookup"><span data-stu-id="3ffaa-159">Notebook</span></span>](notebook.md)|<span data-ttu-id="3ffaa-p112">Записная книжка, содержащая группу разделов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3ffaa-p112">The notebook that contains the section group. Read-only.</span></span>|
|<span data-ttu-id="3ffaa-162">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="3ffaa-162">parentSectionGroup</span></span>|[<span data-ttu-id="3ffaa-163">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="3ffaa-163">SectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="3ffaa-p113">Группа разделов, содержащая группу разделов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3ffaa-p113">The section group that contains the section group. Read-only.</span></span>|
|<span data-ttu-id="3ffaa-166">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="3ffaa-166">sectionGroups</span></span>|<span data-ttu-id="3ffaa-167">Коллекция объектов [SectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="3ffaa-167">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="3ffaa-p114">Группы разделов в разделе. Только для чтения. Допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="3ffaa-p114">The section groups in the section. Read-only. Nullable.</span></span>|
|<span data-ttu-id="3ffaa-171">sections</span><span class="sxs-lookup"><span data-stu-id="3ffaa-171">sections</span></span>|<span data-ttu-id="3ffaa-172">Коллекция объектов [Section](section.md)</span><span class="sxs-lookup"><span data-stu-id="3ffaa-172">[Section](section.md) collection</span></span>|<span data-ttu-id="3ffaa-p115">Разделы в группе разделов. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="3ffaa-p115">The sections in the section group. Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="3ffaa-176">Методы</span><span class="sxs-lookup"><span data-stu-id="3ffaa-176">Methods</span></span>

| <span data-ttu-id="3ffaa-177">Метод</span><span class="sxs-lookup"><span data-stu-id="3ffaa-177">Method</span></span>           | <span data-ttu-id="3ffaa-178">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3ffaa-178">Return Type</span></span>    |<span data-ttu-id="3ffaa-179">Описание</span><span class="sxs-lookup"><span data-stu-id="3ffaa-179">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3ffaa-180">Получение группы разделов</span><span class="sxs-lookup"><span data-stu-id="3ffaa-180">Get section group</span></span>](../api/sectiongroup-get.md) | [<span data-ttu-id="3ffaa-181">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="3ffaa-181">SectionGroup</span></span>](sectiongroup.md) |<span data-ttu-id="3ffaa-182">Чтение свойств и отношений группы разделов.</span><span class="sxs-lookup"><span data-stu-id="3ffaa-182">Read the properties and relationships of the section group.</span></span>|
|[<span data-ttu-id="3ffaa-183">Создание группы разделов</span><span class="sxs-lookup"><span data-stu-id="3ffaa-183">Create section group</span></span>](../api/sectiongroup-post-sectiongroups.md) |[<span data-ttu-id="3ffaa-184">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="3ffaa-184">SectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="3ffaa-185">Создайте группу разделов, отправив запрос POST в коллекцию sectionGroups в указанной группе разделов.</span><span class="sxs-lookup"><span data-stu-id="3ffaa-185">Create a section group by posting to the sectionGroups collection in the specified section group.</span></span>|
|[<span data-ttu-id="3ffaa-186">Перечисление групп разделов</span><span class="sxs-lookup"><span data-stu-id="3ffaa-186">List section groups</span></span>](../api/sectiongroup-list-sectiongroups.md) |<span data-ttu-id="3ffaa-187">Коллекция объектов [SectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="3ffaa-187">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="3ffaa-188">Получение коллекции групп разделов в указанной группе разделов.</span><span class="sxs-lookup"><span data-stu-id="3ffaa-188">Get collection of section groups in the specified section group.</span></span>|
|[<span data-ttu-id="3ffaa-189">Создание раздела</span><span class="sxs-lookup"><span data-stu-id="3ffaa-189">Create section</span></span>](../api/sectiongroup-post-sections.md) |[<span data-ttu-id="3ffaa-190">Section</span><span class="sxs-lookup"><span data-stu-id="3ffaa-190">Section</span></span>](section.md)| <span data-ttu-id="3ffaa-191">Создайте раздел, отправив запрос POST в коллекцию sections в указанной группе разделов.</span><span class="sxs-lookup"><span data-stu-id="3ffaa-191">Create a section by posting to the sections collection in the specified section group.</span></span>|
|[<span data-ttu-id="3ffaa-192">Перечисление разделов</span><span class="sxs-lookup"><span data-stu-id="3ffaa-192">List sections</span></span>](../api/sectiongroup-list-sections.md) |<span data-ttu-id="3ffaa-193">Коллекция объектов [Section](section.md)</span><span class="sxs-lookup"><span data-stu-id="3ffaa-193">[Section](section.md) collection</span></span>| <span data-ttu-id="3ffaa-194">Получение коллекции разделов в указанной группе разделов.</span><span class="sxs-lookup"><span data-stu-id="3ffaa-194">Get a collection of sections in the specified section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sectionGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
