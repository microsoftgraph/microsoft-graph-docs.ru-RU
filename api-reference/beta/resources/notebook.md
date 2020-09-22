---
title: Тип ресурса для записной книжки
description: Записная книжка OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 1fff6f16c111d8036eae5fcb1705d7e5b59d7893
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078327"
---
# <a name="notebook-resource-type"></a><span data-ttu-id="9cbdd-103">Тип ресурса для записной книжки</span><span class="sxs-lookup"><span data-stu-id="9cbdd-103">notebook resource type</span></span>

<span data-ttu-id="9cbdd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9cbdd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9cbdd-105">Записная книжка OneNote.</span><span class="sxs-lookup"><span data-stu-id="9cbdd-105">A OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9cbdd-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9cbdd-106">JSON representation</span></span>

<span data-ttu-id="9cbdd-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="9cbdd-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [
    "sectionGroups",
    "sections"
  ],
  "@odata.type": "microsoft.graph.notebook"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "isDefault": true,
  "isShared": true,
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "links": {"@odata.type": "microsoft.graph.notebookLinks"},
  "displayName": "string",
  "sectionGroupsUrl": "string",
  "sectionsUrl": "string",
  "self": "string",
  "userRole": "String"
}

```
## <a name="properties"></a><span data-ttu-id="9cbdd-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="9cbdd-108">Properties</span></span>
| <span data-ttu-id="9cbdd-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="9cbdd-109">Property</span></span>     | <span data-ttu-id="9cbdd-110">Тип</span><span class="sxs-lookup"><span data-stu-id="9cbdd-110">Type</span></span>   |<span data-ttu-id="9cbdd-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9cbdd-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9cbdd-112">createdBy</span><span class="sxs-lookup"><span data-stu-id="9cbdd-112">createdBy</span></span>|[<span data-ttu-id="9cbdd-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="9cbdd-113">identitySet</span></span>](identityset.md)|<span data-ttu-id="9cbdd-p101">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9cbdd-p101">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="9cbdd-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9cbdd-116">createdDateTime</span></span>|<span data-ttu-id="9cbdd-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9cbdd-117">DateTimeOffset</span></span>|<span data-ttu-id="9cbdd-118">Дата и время создания записной книжки.</span><span class="sxs-lookup"><span data-stu-id="9cbdd-118">The date and time when the notebook was created.</span></span> <span data-ttu-id="9cbdd-119">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="9cbdd-119">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9cbdd-120">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="9cbdd-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="9cbdd-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9cbdd-121">Read-only.</span></span>|
|<span data-ttu-id="9cbdd-122">id</span><span class="sxs-lookup"><span data-stu-id="9cbdd-122">id</span></span>|<span data-ttu-id="9cbdd-123">String</span><span class="sxs-lookup"><span data-stu-id="9cbdd-123">String</span></span>|<span data-ttu-id="9cbdd-124">Уникальный идентификатор записной книжки.</span><span class="sxs-lookup"><span data-stu-id="9cbdd-124">The unique identifier of the notebook.</span></span> <span data-ttu-id="9cbdd-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9cbdd-125">Read-only.</span></span>|
|<span data-ttu-id="9cbdd-126">isDefault</span><span class="sxs-lookup"><span data-stu-id="9cbdd-126">isDefault</span></span>|<span data-ttu-id="9cbdd-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="9cbdd-127">Boolean</span></span>|<span data-ttu-id="9cbdd-128">Указывает, является ли Записная книжка пользователя по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="9cbdd-128">Indicates whether this is the user's default notebook.</span></span> <span data-ttu-id="9cbdd-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9cbdd-129">Read-only.</span></span>|
|<span data-ttu-id="9cbdd-130">IsShared</span><span class="sxs-lookup"><span data-stu-id="9cbdd-130">isShared</span></span>|<span data-ttu-id="9cbdd-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="9cbdd-131">Boolean</span></span>|<span data-ttu-id="9cbdd-132">Указывает, является ли записная книжка общей.</span><span class="sxs-lookup"><span data-stu-id="9cbdd-132">Indicates whether the notebook is shared.</span></span> <span data-ttu-id="9cbdd-133">Если да, ее содержимое, кроме владельца, могут видеть другие люди.</span><span class="sxs-lookup"><span data-stu-id="9cbdd-133">If true, the contents of the notebook can be seen by people other than the owner.</span></span> <span data-ttu-id="9cbdd-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9cbdd-134">Read-only.</span></span>|
|<span data-ttu-id="9cbdd-135">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="9cbdd-135">lastModifiedBy</span></span>|[<span data-ttu-id="9cbdd-136">identitySet</span><span class="sxs-lookup"><span data-stu-id="9cbdd-136">identitySet</span></span>](identityset.md)|<span data-ttu-id="9cbdd-p106">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9cbdd-p106">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="9cbdd-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9cbdd-139">lastModifiedDateTime</span></span>|<span data-ttu-id="9cbdd-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9cbdd-140">DateTimeOffset</span></span>|<span data-ttu-id="9cbdd-141">Дата и время последнего изменения записной книжки.</span><span class="sxs-lookup"><span data-stu-id="9cbdd-141">The date and time when the notebook was last modified.</span></span> <span data-ttu-id="9cbdd-142">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="9cbdd-142">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9cbdd-143">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="9cbdd-143">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="9cbdd-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9cbdd-144">Read-only.</span></span>|
|<span data-ttu-id="9cbdd-145">links</span><span class="sxs-lookup"><span data-stu-id="9cbdd-145">links</span></span>|[<span data-ttu-id="9cbdd-146">нотебуклинкс</span><span class="sxs-lookup"><span data-stu-id="9cbdd-146">notebookLinks</span></span>](notebooklinks.md)|<span data-ttu-id="9cbdd-147">Ссылки для открытия записной книжки.</span><span class="sxs-lookup"><span data-stu-id="9cbdd-147">Links for opening the notebook.</span></span> <span data-ttu-id="9cbdd-148">`oneNoteClientURL`Ссылка открывает записную книжку в собственном клиенте OneNote, если она установлена.</span><span class="sxs-lookup"><span data-stu-id="9cbdd-148">The `oneNoteClientURL` link opens the notebook in the OneNote native client if it's installed.</span></span> <span data-ttu-id="9cbdd-149">`oneNoteWebURL`Ссылка открывает записную книжку в OneNote в Интернете.</span><span class="sxs-lookup"><span data-stu-id="9cbdd-149">The `oneNoteWebURL` link opens the notebook in OneNote on the web.</span></span>|
|<span data-ttu-id="9cbdd-150">displayName</span><span class="sxs-lookup"><span data-stu-id="9cbdd-150">displayName</span></span>|<span data-ttu-id="9cbdd-151">String</span><span class="sxs-lookup"><span data-stu-id="9cbdd-151">String</span></span>|<span data-ttu-id="9cbdd-152">Имя записной книжки.</span><span class="sxs-lookup"><span data-stu-id="9cbdd-152">The name of the notebook.</span></span>|
|<span data-ttu-id="9cbdd-153">сектионграупсурл</span><span class="sxs-lookup"><span data-stu-id="9cbdd-153">sectionGroupsUrl</span></span>|<span data-ttu-id="9cbdd-154">String</span><span class="sxs-lookup"><span data-stu-id="9cbdd-154">String</span></span>|<span data-ttu-id="9cbdd-155">URL-адрес для `sectionGroups` Свойства навигации, который возвращает все группы разделов в записной книжке.</span><span class="sxs-lookup"><span data-stu-id="9cbdd-155">The URL for the `sectionGroups` navigation property, which returns all the section groups in the notebook.</span></span> <span data-ttu-id="9cbdd-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9cbdd-156">Read-only.</span></span>|
|<span data-ttu-id="9cbdd-157">сектионсурл</span><span class="sxs-lookup"><span data-stu-id="9cbdd-157">sectionsUrl</span></span>|<span data-ttu-id="9cbdd-158">String</span><span class="sxs-lookup"><span data-stu-id="9cbdd-158">String</span></span>|<span data-ttu-id="9cbdd-159">URL-адрес для `sections` Свойства навигации, который возвращает все разделы записной книжки.</span><span class="sxs-lookup"><span data-stu-id="9cbdd-159">The URL for the `sections` navigation property, which returns all the sections in the notebook.</span></span> <span data-ttu-id="9cbdd-160">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9cbdd-160">Read-only.</span></span>|
|<span data-ttu-id="9cbdd-161">Self</span><span class="sxs-lookup"><span data-stu-id="9cbdd-161">self</span></span>|<span data-ttu-id="9cbdd-162">String</span><span class="sxs-lookup"><span data-stu-id="9cbdd-162">String</span></span>|<span data-ttu-id="9cbdd-163">Конечная точка, где можно получить сведения о записной книжке.</span><span class="sxs-lookup"><span data-stu-id="9cbdd-163">The endpoint where you can get details about the notebook.</span></span> <span data-ttu-id="9cbdd-164">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9cbdd-164">Read-only.</span></span>|
|<span data-ttu-id="9cbdd-165">userRole</span><span class="sxs-lookup"><span data-stu-id="9cbdd-165">userRole</span></span>|<span data-ttu-id="9cbdd-166">String</span><span class="sxs-lookup"><span data-stu-id="9cbdd-166">String</span></span>|<span data-ttu-id="9cbdd-167">Возможные значения: `Owner`, `Contributor`, `Reader`, `None`.</span><span class="sxs-lookup"><span data-stu-id="9cbdd-167">Possible values are: `Owner`, `Contributor`, `Reader`, `None`.</span></span> <span data-ttu-id="9cbdd-168">Owner — это доступ к записной книжке на уровне владельца.</span><span class="sxs-lookup"><span data-stu-id="9cbdd-168">Owner represents owner-level access to the notebook.</span></span> <span data-ttu-id="9cbdd-169">Участник представляет доступ к записной книжке для чтения и записи.</span><span class="sxs-lookup"><span data-stu-id="9cbdd-169">Contributor represents read/write access to the notebook.</span></span> <span data-ttu-id="9cbdd-170">Читатель предоставляет доступ только для чтения к записной книжке.</span><span class="sxs-lookup"><span data-stu-id="9cbdd-170">Reader represents read-only access to the notebook.</span></span> <span data-ttu-id="9cbdd-171">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9cbdd-171">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9cbdd-172">Отношения</span><span class="sxs-lookup"><span data-stu-id="9cbdd-172">Relationships</span></span>
| <span data-ttu-id="9cbdd-173">Связь</span><span class="sxs-lookup"><span data-stu-id="9cbdd-173">Relationship</span></span> | <span data-ttu-id="9cbdd-174">Тип</span><span class="sxs-lookup"><span data-stu-id="9cbdd-174">Type</span></span>   |<span data-ttu-id="9cbdd-175">Описание</span><span class="sxs-lookup"><span data-stu-id="9cbdd-175">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9cbdd-176">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="9cbdd-176">sectionGroups</span></span>|<span data-ttu-id="9cbdd-177">Коллекция [sectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="9cbdd-177">[sectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="9cbdd-178">Группы разделов в записной книжке.</span><span class="sxs-lookup"><span data-stu-id="9cbdd-178">The section groups in the notebook.</span></span> <span data-ttu-id="9cbdd-179">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9cbdd-179">Read-only.</span></span> <span data-ttu-id="9cbdd-180">Допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="9cbdd-180">Nullable.</span></span>|
|<span data-ttu-id="9cbdd-181">sections</span><span class="sxs-lookup"><span data-stu-id="9cbdd-181">sections</span></span>|<span data-ttu-id="9cbdd-182">Коллекция [оненотесектион](onenotesection.md)</span><span class="sxs-lookup"><span data-stu-id="9cbdd-182">[onenoteSection](onenotesection.md) collection</span></span>|<span data-ttu-id="9cbdd-183">Разделы записной книжки.</span><span class="sxs-lookup"><span data-stu-id="9cbdd-183">The sections in the notebook.</span></span> <span data-ttu-id="9cbdd-184">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9cbdd-184">Read-only.</span></span> <span data-ttu-id="9cbdd-185">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="9cbdd-185">Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="9cbdd-186">Методы</span><span class="sxs-lookup"><span data-stu-id="9cbdd-186">Methods</span></span>

| <span data-ttu-id="9cbdd-187">Метод</span><span class="sxs-lookup"><span data-stu-id="9cbdd-187">Method</span></span>           | <span data-ttu-id="9cbdd-188">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9cbdd-188">Return Type</span></span>    |<span data-ttu-id="9cbdd-189">Описание</span><span class="sxs-lookup"><span data-stu-id="9cbdd-189">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9cbdd-190">Вывод записной книжки</span><span class="sxs-lookup"><span data-stu-id="9cbdd-190">Get notebook</span></span>](../api/notebook-get.md) | [<span data-ttu-id="9cbdd-191">notebook</span><span class="sxs-lookup"><span data-stu-id="9cbdd-191">notebook</span></span>](notebook.md) |<span data-ttu-id="9cbdd-192">Прочитайте свойства и связи записной книжки.</span><span class="sxs-lookup"><span data-stu-id="9cbdd-192">Read the properties and relationships of the notebook.</span></span>|
|[<span data-ttu-id="9cbdd-193">getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="9cbdd-193">getRecentNotebooks</span></span>](../api/notebook-getrecentnotebooks.md) | <span data-ttu-id="9cbdd-194">Коллекция [recentNotebook](recentnotebook.md)</span><span class="sxs-lookup"><span data-stu-id="9cbdd-194">[recentNotebook](recentnotebook.md) collection</span></span> | <span data-ttu-id="9cbdd-195">Получите коллекцию записных книжек, которые недавно открывал пользователь.</span><span class="sxs-lookup"><span data-stu-id="9cbdd-195">Get a collection of the most recently accessed notebooks for the user.</span></span> |
|[<span data-ttu-id="9cbdd-196">жетнотебукфромвебурл</span><span class="sxs-lookup"><span data-stu-id="9cbdd-196">getNotebookFromWebUrl</span></span>](../api/notebook-getnotebookfromweburl.md) | [<span data-ttu-id="9cbdd-197">notebook</span><span class="sxs-lookup"><span data-stu-id="9cbdd-197">notebook</span></span>](notebook.md) | <span data-ttu-id="9cbdd-198">Получение свойств и связей объекта записной книжки с помощью URL-пути.</span><span class="sxs-lookup"><span data-stu-id="9cbdd-198">Retrieve the properties and relationships of a notebook object using its URL path.</span></span> |
|[<span data-ttu-id="9cbdd-199">Создание группы разделов</span><span class="sxs-lookup"><span data-stu-id="9cbdd-199">Create section group</span></span>](../api/notebook-post-sectiongroups.md) |[<span data-ttu-id="9cbdd-200">sectionGroup</span><span class="sxs-lookup"><span data-stu-id="9cbdd-200">sectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="9cbdd-201">Создание группы разделов путем отправки в коллекцию sectionGroups в указанной записной книжке.</span><span class="sxs-lookup"><span data-stu-id="9cbdd-201">Create a section group by posting to the sectionGroups collection in the specified notebook.</span></span>|
|[<span data-ttu-id="9cbdd-202">Перечисление групп разделов</span><span class="sxs-lookup"><span data-stu-id="9cbdd-202">List section groups</span></span>](../api/notebook-list-sectiongroups.md) |<span data-ttu-id="9cbdd-203">Коллекция [sectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="9cbdd-203">[sectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="9cbdd-204">Получение коллекции групп разделов в указанной записной книжке.</span><span class="sxs-lookup"><span data-stu-id="9cbdd-204">Get a collection of section groups in the specified notebook.</span></span>|
|[<span data-ttu-id="9cbdd-205">Создание раздела</span><span class="sxs-lookup"><span data-stu-id="9cbdd-205">Create section</span></span>](../api/notebook-post-sections.md) |[<span data-ttu-id="9cbdd-206">оненотесектион</span><span class="sxs-lookup"><span data-stu-id="9cbdd-206">onenoteSection</span></span>](onenotesection.md)| <span data-ttu-id="9cbdd-207">Создание раздела путем публикации в коллекции разделов в указанной записной книжке.</span><span class="sxs-lookup"><span data-stu-id="9cbdd-207">Create a section by posting to the sections collection in the specified notebook.</span></span>|
|[<span data-ttu-id="9cbdd-208">Перечисление разделов</span><span class="sxs-lookup"><span data-stu-id="9cbdd-208">List sections</span></span>](../api/notebook-list-sections.md) |<span data-ttu-id="9cbdd-209">Коллекция [оненотесектион](onenotesection.md)</span><span class="sxs-lookup"><span data-stu-id="9cbdd-209">[onenoteSection](onenotesection.md) collection</span></span>| <span data-ttu-id="9cbdd-210">Получение коллекции разделов в указанной записной книжке.</span><span class="sxs-lookup"><span data-stu-id="9cbdd-210">Get a collection of sections in the specified notebook.</span></span>|
|[<span data-ttu-id="9cbdd-211">Включеныcopynotebook</span><span class="sxs-lookup"><span data-stu-id="9cbdd-211">copyNotebook</span></span>](../api/notebook-copynotebook.md)| <span data-ttu-id="9cbdd-212">Нет</span><span class="sxs-lookup"><span data-stu-id="9cbdd-212">None</span></span> | <span data-ttu-id="9cbdd-213">Копирует записную книжку.</span><span class="sxs-lookup"><span data-stu-id="9cbdd-213">Copies a notebook.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "notebook resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


