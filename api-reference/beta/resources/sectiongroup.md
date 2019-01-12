---
title: Тип ресурса sectionGroup
description: Группа разделов в записной книжке OneNote. Группы разделов могут содержать разделы и группы разделов.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 8ecd8633b3311459368a16477be391778087882c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976760"
---
# <a name="sectiongroup-resource-type"></a><span data-ttu-id="e0188-104">Тип ресурса sectionGroup</span><span class="sxs-lookup"><span data-stu-id="e0188-104">sectionGroup resource type</span></span>

> <span data-ttu-id="e0188-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e0188-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e0188-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0188-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e0188-p103">Группа разделов в записной книжке OneNote. Группы разделов могут содержать разделы и группы разделов.</span><span class="sxs-lookup"><span data-stu-id="e0188-p103">A section group in a OneNote notebook. Section groups can contain sections and section groups.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e0188-109">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e0188-109">JSON representation</span></span>

<span data-ttu-id="e0188-110">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e0188-110">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="e0188-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="e0188-111">Properties</span></span>
| <span data-ttu-id="e0188-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="e0188-112">Property</span></span>     | <span data-ttu-id="e0188-113">Тип</span><span class="sxs-lookup"><span data-stu-id="e0188-113">Type</span></span>   |<span data-ttu-id="e0188-114">Описание</span><span class="sxs-lookup"><span data-stu-id="e0188-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e0188-115">createdBy</span><span class="sxs-lookup"><span data-stu-id="e0188-115">createdBy</span></span>|[<span data-ttu-id="e0188-116">identitySet</span><span class="sxs-lookup"><span data-stu-id="e0188-116">identitySet</span></span>](identityset.md)|<span data-ttu-id="e0188-p104">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e0188-p104">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="e0188-119">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e0188-119">createdDateTime</span></span>|<span data-ttu-id="e0188-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0188-120">DateTimeOffset</span></span>|<span data-ttu-id="e0188-p105">Дата и время создания группы разделов. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e0188-p105">The date and time when the section group was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="e0188-125">id</span><span class="sxs-lookup"><span data-stu-id="e0188-125">id</span></span>|<span data-ttu-id="e0188-126">String</span><span class="sxs-lookup"><span data-stu-id="e0188-126">String</span></span>|<span data-ttu-id="e0188-p106">Уникальный идентификатор группы разделов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e0188-p106">The unique identifier of the section group. Read-only.</span></span>|
|<span data-ttu-id="e0188-129">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="e0188-129">lastModifiedBy</span></span>|[<span data-ttu-id="e0188-130">identitySet</span><span class="sxs-lookup"><span data-stu-id="e0188-130">identitySet</span></span>](identityset.md)|<span data-ttu-id="e0188-p107">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e0188-p107">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="e0188-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e0188-133">lastModifiedDateTime</span></span>|<span data-ttu-id="e0188-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0188-134">DateTimeOffset</span></span>|<span data-ttu-id="e0188-p108">Дата и время последнего изменения группы разделов. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e0188-p108">The date and time when the section group was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="e0188-139">displayName</span><span class="sxs-lookup"><span data-stu-id="e0188-139">displayName</span></span>|<span data-ttu-id="e0188-140">Строка</span><span class="sxs-lookup"><span data-stu-id="e0188-140">String</span></span>|<span data-ttu-id="e0188-141">Имя группы разделов.</span><span class="sxs-lookup"><span data-stu-id="e0188-141">The name of the section group.</span></span>|
|<span data-ttu-id="e0188-142">sectionGroupsUrl</span><span class="sxs-lookup"><span data-stu-id="e0188-142">sectionGroupsUrl</span></span>|<span data-ttu-id="e0188-143">Строка</span><span class="sxs-lookup"><span data-stu-id="e0188-143">String</span></span>|<span data-ttu-id="e0188-p109">URL-адрес для свойства навигации `sectionGroups`, который возвращает все группы разделов в группе разделов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e0188-p109">The URL for the `sectionGroups` navigation property, which returns all the section groups in the section group. Read-only.</span></span>|
|<span data-ttu-id="e0188-146">sectionsUrl</span><span class="sxs-lookup"><span data-stu-id="e0188-146">sectionsUrl</span></span>|<span data-ttu-id="e0188-147">Строка</span><span class="sxs-lookup"><span data-stu-id="e0188-147">String</span></span>|<span data-ttu-id="e0188-p110">URL-адрес для свойства навигации `sections`, который возвращает все разделы в группе разделов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e0188-p110">The URL for the `sections` navigation property, which returns all the sections in the section group. Read-only.</span></span>|
|<span data-ttu-id="e0188-150">self</span><span class="sxs-lookup"><span data-stu-id="e0188-150">self</span></span>|<span data-ttu-id="e0188-151">String</span><span class="sxs-lookup"><span data-stu-id="e0188-151">String</span></span>|<span data-ttu-id="e0188-p111">Конечная точка, в которой можно получить сведения о группе разделов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e0188-p111">The endpoint where you can get details about the section group. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e0188-154">Связи</span><span class="sxs-lookup"><span data-stu-id="e0188-154">Relationships</span></span>
| <span data-ttu-id="e0188-155">Связь</span><span class="sxs-lookup"><span data-stu-id="e0188-155">Relationship</span></span> | <span data-ttu-id="e0188-156">Тип</span><span class="sxs-lookup"><span data-stu-id="e0188-156">Type</span></span>   |<span data-ttu-id="e0188-157">Описание</span><span class="sxs-lookup"><span data-stu-id="e0188-157">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e0188-158">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="e0188-158">parentNotebook</span></span>|[<span data-ttu-id="e0188-159">Notebook</span><span class="sxs-lookup"><span data-stu-id="e0188-159">Notebook</span></span>](notebook.md)|<span data-ttu-id="e0188-p112">Записная книжка, содержащая группу разделов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e0188-p112">The notebook that contains the section group. Read-only.</span></span>|
|<span data-ttu-id="e0188-162">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="e0188-162">parentSectionGroup</span></span>|[<span data-ttu-id="e0188-163">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="e0188-163">SectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="e0188-p113">Группа разделов, содержащая группу разделов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e0188-p113">The section group that contains the section group. Read-only.</span></span>|
|<span data-ttu-id="e0188-166">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="e0188-166">sectionGroups</span></span>|<span data-ttu-id="e0188-167">Коллекция объектов [SectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="e0188-167">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="e0188-p114">Группы разделов в разделе. Только для чтения. Допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="e0188-p114">The section groups in the section. Read-only. Nullable.</span></span>|
|<span data-ttu-id="e0188-171">sections</span><span class="sxs-lookup"><span data-stu-id="e0188-171">sections</span></span>|<span data-ttu-id="e0188-172">Коллекция объектов [Section](section.md)</span><span class="sxs-lookup"><span data-stu-id="e0188-172">[Section](section.md) collection</span></span>|<span data-ttu-id="e0188-p115">Разделы в группе разделов. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="e0188-p115">The sections in the section group. Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="e0188-176">Методы</span><span class="sxs-lookup"><span data-stu-id="e0188-176">Methods</span></span>

| <span data-ttu-id="e0188-177">Метод</span><span class="sxs-lookup"><span data-stu-id="e0188-177">Method</span></span>           | <span data-ttu-id="e0188-178">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e0188-178">Return Type</span></span>    |<span data-ttu-id="e0188-179">Описание</span><span class="sxs-lookup"><span data-stu-id="e0188-179">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e0188-180">Получение группы разделов</span><span class="sxs-lookup"><span data-stu-id="e0188-180">Get section group</span></span>](../api/sectiongroup-get.md) | [<span data-ttu-id="e0188-181">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="e0188-181">SectionGroup</span></span>](sectiongroup.md) |<span data-ttu-id="e0188-182">Чтение свойств и отношений группы разделов.</span><span class="sxs-lookup"><span data-stu-id="e0188-182">Read the properties and relationships of the section group.</span></span>|
|[<span data-ttu-id="e0188-183">Создание группы разделов</span><span class="sxs-lookup"><span data-stu-id="e0188-183">Create section group</span></span>](../api/sectiongroup-post-sectiongroups.md) |[<span data-ttu-id="e0188-184">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="e0188-184">SectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="e0188-185">Создайте группу разделов, отправив запрос POST в коллекцию sectionGroups в указанной группе разделов.</span><span class="sxs-lookup"><span data-stu-id="e0188-185">Create a section group by posting to the sectionGroups collection in the specified section group.</span></span>|
|[<span data-ttu-id="e0188-186">Перечисление групп разделов</span><span class="sxs-lookup"><span data-stu-id="e0188-186">List section groups</span></span>](../api/sectiongroup-list-sectiongroups.md) |<span data-ttu-id="e0188-187">Коллекция объектов [SectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="e0188-187">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="e0188-188">Получение коллекции групп разделов в указанной группе разделов.</span><span class="sxs-lookup"><span data-stu-id="e0188-188">Get collection of section groups in the specified section group.</span></span>|
|[<span data-ttu-id="e0188-189">Создание раздела</span><span class="sxs-lookup"><span data-stu-id="e0188-189">Create section</span></span>](../api/sectiongroup-post-sections.md) |[<span data-ttu-id="e0188-190">Section</span><span class="sxs-lookup"><span data-stu-id="e0188-190">Section</span></span>](section.md)| <span data-ttu-id="e0188-191">Создайте раздел, отправив запрос POST в коллекцию sections в указанной группе разделов.</span><span class="sxs-lookup"><span data-stu-id="e0188-191">Create a section by posting to the sections collection in the specified section group.</span></span>|
|[<span data-ttu-id="e0188-192">Перечисление разделов</span><span class="sxs-lookup"><span data-stu-id="e0188-192">List sections</span></span>](../api/sectiongroup-list-sections.md) |<span data-ttu-id="e0188-193">Коллекция объектов [Section](section.md)</span><span class="sxs-lookup"><span data-stu-id="e0188-193">[Section](section.md) collection</span></span>| <span data-ttu-id="e0188-194">Получение коллекции разделов в указанной группе разделов.</span><span class="sxs-lookup"><span data-stu-id="e0188-194">Get a collection of sections in the specified section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sectionGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
