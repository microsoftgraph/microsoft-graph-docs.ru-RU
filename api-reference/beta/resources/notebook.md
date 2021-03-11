---
title: тип ресурса записной книжки
description: Блокнот OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 35c6ab2136f8a04be7edbc6170b4e7e0328b314c
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722107"
---
# <a name="notebook-resource-type"></a><span data-ttu-id="61804-103">тип ресурса записной книжки</span><span class="sxs-lookup"><span data-stu-id="61804-103">notebook resource type</span></span>

<span data-ttu-id="61804-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61804-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="61804-105">Блокнот OneNote.</span><span class="sxs-lookup"><span data-stu-id="61804-105">A OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="61804-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="61804-106">JSON representation</span></span>

<span data-ttu-id="61804-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="61804-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="61804-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="61804-108">Properties</span></span>
| <span data-ttu-id="61804-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="61804-109">Property</span></span>     | <span data-ttu-id="61804-110">Тип</span><span class="sxs-lookup"><span data-stu-id="61804-110">Type</span></span>   |<span data-ttu-id="61804-111">Описание</span><span class="sxs-lookup"><span data-stu-id="61804-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="61804-112">createdBy</span><span class="sxs-lookup"><span data-stu-id="61804-112">createdBy</span></span>|[<span data-ttu-id="61804-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="61804-113">identitySet</span></span>](identityset.md)|<span data-ttu-id="61804-p101">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="61804-p101">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="61804-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="61804-116">createdDateTime</span></span>|<span data-ttu-id="61804-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61804-117">DateTimeOffset</span></span>|<span data-ttu-id="61804-118">Дата и время создания записной книжки.</span><span class="sxs-lookup"><span data-stu-id="61804-118">The date and time when the notebook was created.</span></span> <span data-ttu-id="61804-119">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="61804-119">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="61804-120">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="61804-120">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="61804-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="61804-121">Read-only.</span></span>|
|<span data-ttu-id="61804-122">id</span><span class="sxs-lookup"><span data-stu-id="61804-122">id</span></span>|<span data-ttu-id="61804-123">String</span><span class="sxs-lookup"><span data-stu-id="61804-123">String</span></span>|<span data-ttu-id="61804-124">Уникальный идентификатор записной книжки.</span><span class="sxs-lookup"><span data-stu-id="61804-124">The unique identifier of the notebook.</span></span> <span data-ttu-id="61804-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="61804-125">Read-only.</span></span>|
|<span data-ttu-id="61804-126">isDefault</span><span class="sxs-lookup"><span data-stu-id="61804-126">isDefault</span></span>|<span data-ttu-id="61804-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="61804-127">Boolean</span></span>|<span data-ttu-id="61804-128">Указывает, является ли это ноутбук пользователя по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="61804-128">Indicates whether this is the user's default notebook.</span></span> <span data-ttu-id="61804-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="61804-129">Read-only.</span></span>|
|<span data-ttu-id="61804-130">IsShared</span><span class="sxs-lookup"><span data-stu-id="61804-130">isShared</span></span>|<span data-ttu-id="61804-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="61804-131">Boolean</span></span>|<span data-ttu-id="61804-132">Указывает, является ли записная книжка общей.</span><span class="sxs-lookup"><span data-stu-id="61804-132">Indicates whether the notebook is shared.</span></span> <span data-ttu-id="61804-133">Если да, ее содержимое, кроме владельца, могут видеть другие люди.</span><span class="sxs-lookup"><span data-stu-id="61804-133">If true, the contents of the notebook can be seen by people other than the owner.</span></span> <span data-ttu-id="61804-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="61804-134">Read-only.</span></span>|
|<span data-ttu-id="61804-135">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="61804-135">lastModifiedBy</span></span>|[<span data-ttu-id="61804-136">identitySet</span><span class="sxs-lookup"><span data-stu-id="61804-136">identitySet</span></span>](identityset.md)|<span data-ttu-id="61804-p106">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="61804-p106">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="61804-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="61804-139">lastModifiedDateTime</span></span>|<span data-ttu-id="61804-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61804-140">DateTimeOffset</span></span>|<span data-ttu-id="61804-141">Дата и время последнего изменения записной книжки.</span><span class="sxs-lookup"><span data-stu-id="61804-141">The date and time when the notebook was last modified.</span></span> <span data-ttu-id="61804-142">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="61804-142">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="61804-143">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="61804-143">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="61804-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="61804-144">Read-only.</span></span>|
|<span data-ttu-id="61804-145">links</span><span class="sxs-lookup"><span data-stu-id="61804-145">links</span></span>|[<span data-ttu-id="61804-146">notebookLinks</span><span class="sxs-lookup"><span data-stu-id="61804-146">notebookLinks</span></span>](notebooklinks.md)|<span data-ttu-id="61804-147">Ссылки для открытия записной книжки.</span><span class="sxs-lookup"><span data-stu-id="61804-147">Links for opening the notebook.</span></span> <span data-ttu-id="61804-148">Ссылка `oneNoteClientURL` открывает записную книжку в родном клиенте OneNote, если она установлена.</span><span class="sxs-lookup"><span data-stu-id="61804-148">The `oneNoteClientURL` link opens the notebook in the OneNote native client if it's installed.</span></span> <span data-ttu-id="61804-149">Ссылка `oneNoteWebURL` открывает записную книжку в OneNote в Интернете.</span><span class="sxs-lookup"><span data-stu-id="61804-149">The `oneNoteWebURL` link opens the notebook in OneNote on the web.</span></span>|
|<span data-ttu-id="61804-150">displayName</span><span class="sxs-lookup"><span data-stu-id="61804-150">displayName</span></span>|<span data-ttu-id="61804-151">String</span><span class="sxs-lookup"><span data-stu-id="61804-151">String</span></span>|<span data-ttu-id="61804-152">Имя записной книжки.</span><span class="sxs-lookup"><span data-stu-id="61804-152">The name of the notebook.</span></span>|
|<span data-ttu-id="61804-153">sectionGroupsUrl</span><span class="sxs-lookup"><span data-stu-id="61804-153">sectionGroupsUrl</span></span>|<span data-ttu-id="61804-154">String</span><span class="sxs-lookup"><span data-stu-id="61804-154">String</span></span>|<span data-ttu-id="61804-155">URL-адрес `sectionGroups` свойства навигации, который возвращает все группы разделов в записной книжке.</span><span class="sxs-lookup"><span data-stu-id="61804-155">The URL for the `sectionGroups` navigation property, which returns all the section groups in the notebook.</span></span> <span data-ttu-id="61804-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="61804-156">Read-only.</span></span>|
|<span data-ttu-id="61804-157">sectionsUrl</span><span class="sxs-lookup"><span data-stu-id="61804-157">sectionsUrl</span></span>|<span data-ttu-id="61804-158">String</span><span class="sxs-lookup"><span data-stu-id="61804-158">String</span></span>|<span data-ttu-id="61804-159">URL-адрес `sections` свойства навигации, который возвращает все разделы в записной книжке.</span><span class="sxs-lookup"><span data-stu-id="61804-159">The URL for the `sections` navigation property, which returns all the sections in the notebook.</span></span> <span data-ttu-id="61804-160">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="61804-160">Read-only.</span></span>|
|<span data-ttu-id="61804-161">self</span><span class="sxs-lookup"><span data-stu-id="61804-161">self</span></span>|<span data-ttu-id="61804-162">String</span><span class="sxs-lookup"><span data-stu-id="61804-162">String</span></span>|<span data-ttu-id="61804-163">Конечная точка, где можно получить сведения о записной книжке.</span><span class="sxs-lookup"><span data-stu-id="61804-163">The endpoint where you can get details about the notebook.</span></span> <span data-ttu-id="61804-164">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="61804-164">Read-only.</span></span>|
|<span data-ttu-id="61804-165">userRole</span><span class="sxs-lookup"><span data-stu-id="61804-165">userRole</span></span>|<span data-ttu-id="61804-166">String</span><span class="sxs-lookup"><span data-stu-id="61804-166">String</span></span>|<span data-ttu-id="61804-167">Возможные значения: `Owner`, `Contributor`, `Reader`, `None`.</span><span class="sxs-lookup"><span data-stu-id="61804-167">Possible values are: `Owner`, `Contributor`, `Reader`, `None`.</span></span> <span data-ttu-id="61804-168">Владелец представляет доступ к записной книжке на уровне владельца.</span><span class="sxs-lookup"><span data-stu-id="61804-168">Owner represents owner-level access to the notebook.</span></span> <span data-ttu-id="61804-169">Автор представляет доступ к записной книжке для чтения и записи.</span><span class="sxs-lookup"><span data-stu-id="61804-169">Contributor represents read/write access to the notebook.</span></span> <span data-ttu-id="61804-170">Reader представляет доступ только для чтения к записной книжке.</span><span class="sxs-lookup"><span data-stu-id="61804-170">Reader represents read-only access to the notebook.</span></span> <span data-ttu-id="61804-171">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="61804-171">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="61804-172">Связи</span><span class="sxs-lookup"><span data-stu-id="61804-172">Relationships</span></span>
| <span data-ttu-id="61804-173">Связь</span><span class="sxs-lookup"><span data-stu-id="61804-173">Relationship</span></span> | <span data-ttu-id="61804-174">Тип</span><span class="sxs-lookup"><span data-stu-id="61804-174">Type</span></span>   |<span data-ttu-id="61804-175">Описание</span><span class="sxs-lookup"><span data-stu-id="61804-175">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="61804-176">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="61804-176">sectionGroups</span></span>|<span data-ttu-id="61804-177">[коллекция sectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="61804-177">[sectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="61804-178">Группы разделов в записной книжке.</span><span class="sxs-lookup"><span data-stu-id="61804-178">The section groups in the notebook.</span></span> <span data-ttu-id="61804-179">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="61804-179">Read-only.</span></span> <span data-ttu-id="61804-180">Допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="61804-180">Nullable.</span></span>|
|<span data-ttu-id="61804-181">sections</span><span class="sxs-lookup"><span data-stu-id="61804-181">sections</span></span>|<span data-ttu-id="61804-182">[коллекция onenoteSection](onenotesection.md)</span><span class="sxs-lookup"><span data-stu-id="61804-182">[onenoteSection](onenotesection.md) collection</span></span>|<span data-ttu-id="61804-183">Разделы в записной книжке.</span><span class="sxs-lookup"><span data-stu-id="61804-183">The sections in the notebook.</span></span> <span data-ttu-id="61804-184">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="61804-184">Read-only.</span></span> <span data-ttu-id="61804-185">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="61804-185">Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="61804-186">Методы</span><span class="sxs-lookup"><span data-stu-id="61804-186">Methods</span></span>

| <span data-ttu-id="61804-187">Метод</span><span class="sxs-lookup"><span data-stu-id="61804-187">Method</span></span>           | <span data-ttu-id="61804-188">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="61804-188">Return Type</span></span>    |<span data-ttu-id="61804-189">Описание</span><span class="sxs-lookup"><span data-stu-id="61804-189">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="61804-190">Вывод записной книжки</span><span class="sxs-lookup"><span data-stu-id="61804-190">Get notebook</span></span>](../api/notebook-get.md) | [<span data-ttu-id="61804-191">notebook</span><span class="sxs-lookup"><span data-stu-id="61804-191">notebook</span></span>](notebook.md) |<span data-ttu-id="61804-192">Ознакомьтесь с свойствами и отношениями записной книжки.</span><span class="sxs-lookup"><span data-stu-id="61804-192">Read the properties and relationships of the notebook.</span></span>|
|[<span data-ttu-id="61804-193">getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="61804-193">getRecentNotebooks</span></span>](../api/notebook-getrecentnotebooks.md) | <span data-ttu-id="61804-194">[recentNotebook](recentnotebook.md) collection</span><span class="sxs-lookup"><span data-stu-id="61804-194">[recentNotebook](recentnotebook.md) collection</span></span> | <span data-ttu-id="61804-195">Получите коллекцию записных книжек, которые недавно открывал пользователь.</span><span class="sxs-lookup"><span data-stu-id="61804-195">Get a collection of the most recently accessed notebooks for the user.</span></span> |
|[<span data-ttu-id="61804-196">getNotebookFromWebUrl</span><span class="sxs-lookup"><span data-stu-id="61804-196">getNotebookFromWebUrl</span></span>](../api/notebook-getnotebookfromweburl.md) | [<span data-ttu-id="61804-197">notebook</span><span class="sxs-lookup"><span data-stu-id="61804-197">notebook</span></span>](notebook.md) | <span data-ttu-id="61804-198">Извлечение свойств и связей объекта записной книжки с помощью url-адреса.</span><span class="sxs-lookup"><span data-stu-id="61804-198">Retrieve the properties and relationships of a notebook object using its URL path.</span></span> |
|[<span data-ttu-id="61804-199">Создание группы разделов</span><span class="sxs-lookup"><span data-stu-id="61804-199">Create section group</span></span>](../api/notebook-post-sectiongroups.md) |[<span data-ttu-id="61804-200">sectionGroup</span><span class="sxs-lookup"><span data-stu-id="61804-200">sectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="61804-201">Создайте группу разделов, разместив в разделеGroups коллекцию в указанной записной книжке.</span><span class="sxs-lookup"><span data-stu-id="61804-201">Create a section group by posting to the sectionGroups collection in the specified notebook.</span></span>|
|[<span data-ttu-id="61804-202">Перечисление групп разделов</span><span class="sxs-lookup"><span data-stu-id="61804-202">List section groups</span></span>](../api/notebook-list-sectiongroups.md) |<span data-ttu-id="61804-203">[коллекция sectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="61804-203">[sectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="61804-204">Получите коллекцию групп разделов в указанной записной книжке.</span><span class="sxs-lookup"><span data-stu-id="61804-204">Get a collection of section groups in the specified notebook.</span></span>|
|[<span data-ttu-id="61804-205">Создание раздела</span><span class="sxs-lookup"><span data-stu-id="61804-205">Create section</span></span>](../api/notebook-post-sections.md) |[<span data-ttu-id="61804-206">onenoteSection</span><span class="sxs-lookup"><span data-stu-id="61804-206">onenoteSection</span></span>](onenotesection.md)| <span data-ttu-id="61804-207">Создайте раздел, разместив в коллекции разделов в указанной записной книжке.</span><span class="sxs-lookup"><span data-stu-id="61804-207">Create a section by posting to the sections collection in the specified notebook.</span></span>|
|[<span data-ttu-id="61804-208">Перечисление разделов</span><span class="sxs-lookup"><span data-stu-id="61804-208">List sections</span></span>](../api/notebook-list-sections.md) |<span data-ttu-id="61804-209">[коллекция onenoteSection](onenotesection.md)</span><span class="sxs-lookup"><span data-stu-id="61804-209">[onenoteSection](onenotesection.md) collection</span></span>| <span data-ttu-id="61804-210">Получите коллекцию разделов в указанной записной книжке.</span><span class="sxs-lookup"><span data-stu-id="61804-210">Get a collection of sections in the specified notebook.</span></span>|
|[<span data-ttu-id="61804-211">copyNotebook</span><span class="sxs-lookup"><span data-stu-id="61804-211">copyNotebook</span></span>](../api/notebook-copynotebook.md)| <span data-ttu-id="61804-212">Нет</span><span class="sxs-lookup"><span data-stu-id="61804-212">None</span></span> | <span data-ttu-id="61804-213">Копирует записную книжку.</span><span class="sxs-lookup"><span data-stu-id="61804-213">Copies a notebook.</span></span>|

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


