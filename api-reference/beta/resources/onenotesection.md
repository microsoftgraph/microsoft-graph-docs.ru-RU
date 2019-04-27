---
title: Тип ресурса Оненотесектион
description: Раздел в записной книжке OneNote. Разделы могут содержать страницы.
localization_priority: Normal
ms.openlocfilehash: d262065f46052c1cae55b42babaa91a2e065d3ef
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348949"
---
# <a name="onenotesection-resource-type"></a><span data-ttu-id="80f6c-104">Тип ресурса Оненотесектион</span><span class="sxs-lookup"><span data-stu-id="80f6c-104">onenoteSection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80f6c-105">Раздел в записной книжке OneNote.</span><span class="sxs-lookup"><span data-stu-id="80f6c-105">A section in a OneNote notebook.</span></span> <span data-ttu-id="80f6c-106">Разделы могут содержать страницы.</span><span class="sxs-lookup"><span data-stu-id="80f6c-106">Sections can contain pages.</span></span>

## <a name="properties"></a><span data-ttu-id="80f6c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="80f6c-107">Properties</span></span>
| <span data-ttu-id="80f6c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="80f6c-108">Property</span></span>     | <span data-ttu-id="80f6c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="80f6c-109">Type</span></span>   |<span data-ttu-id="80f6c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="80f6c-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="80f6c-111">createdBy</span><span class="sxs-lookup"><span data-stu-id="80f6c-111">createdBy</span></span>|[<span data-ttu-id="80f6c-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="80f6c-112">identitySet</span></span>](identityset.md)|<span data-ttu-id="80f6c-p103">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="80f6c-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="80f6c-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="80f6c-115">createdDateTime</span></span>|<span data-ttu-id="80f6c-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80f6c-116">DateTimeOffset</span></span>|<span data-ttu-id="80f6c-117">Дата и время создания раздела.</span><span class="sxs-lookup"><span data-stu-id="80f6c-117">The date and time when the section was created.</span></span> <span data-ttu-id="80f6c-118">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="80f6c-118">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="80f6c-119">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="80f6c-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="80f6c-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="80f6c-120">Read-only.</span></span>|
|<span data-ttu-id="80f6c-121">id</span><span class="sxs-lookup"><span data-stu-id="80f6c-121">id</span></span>|<span data-ttu-id="80f6c-122">String</span><span class="sxs-lookup"><span data-stu-id="80f6c-122">String</span></span>|<span data-ttu-id="80f6c-123">Уникальный идентификатор раздела.</span><span class="sxs-lookup"><span data-stu-id="80f6c-123">The unique identifier of the section.</span></span>  <span data-ttu-id="80f6c-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="80f6c-124">Read-only.</span></span>|
|<span data-ttu-id="80f6c-125">isDefault</span><span class="sxs-lookup"><span data-stu-id="80f6c-125">isDefault</span></span>|<span data-ttu-id="80f6c-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="80f6c-126">Boolean</span></span>|<span data-ttu-id="80f6c-127">Указывает, является ли этот раздел разделом пользователя по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="80f6c-127">Indicates whether this is the user's default section.</span></span> <span data-ttu-id="80f6c-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="80f6c-128">Read-only.</span></span>|
|<span data-ttu-id="80f6c-129">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="80f6c-129">lastModifiedBy</span></span>|[<span data-ttu-id="80f6c-130">identitySet</span><span class="sxs-lookup"><span data-stu-id="80f6c-130">identitySet</span></span>](identityset.md)|<span data-ttu-id="80f6c-p107">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="80f6c-p107">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="80f6c-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="80f6c-133">lastModifiedDateTime</span></span>|<span data-ttu-id="80f6c-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80f6c-134">DateTimeOffset</span></span>|<span data-ttu-id="80f6c-135">Дата и время последнего изменения раздела.</span><span class="sxs-lookup"><span data-stu-id="80f6c-135">The date and time when the section was last modified.</span></span> <span data-ttu-id="80f6c-136">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="80f6c-136">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="80f6c-137">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="80f6c-137">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="80f6c-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="80f6c-138">Read-only.</span></span>|
|<span data-ttu-id="80f6c-139">links</span><span class="sxs-lookup"><span data-stu-id="80f6c-139">links</span></span>|[<span data-ttu-id="80f6c-140">Сектионлинкс</span><span class="sxs-lookup"><span data-stu-id="80f6c-140">sectionLinks</span></span>](sectionlinks.md)|<span data-ttu-id="80f6c-141">Ссылки для открытия раздела.</span><span class="sxs-lookup"><span data-stu-id="80f6c-141">Links for opening the section.</span></span> <span data-ttu-id="80f6c-142">`oneNoteClientURL` Ссылка открывает раздел в собственном клиенте OneNote, если он установлен.</span><span class="sxs-lookup"><span data-stu-id="80f6c-142">The `oneNoteClientURL` link opens the section in the OneNote native client if it's installed.</span></span> <span data-ttu-id="80f6c-143">`oneNoteWebURL` Ссылка открывает раздел в OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="80f6c-143">The `oneNoteWebURL` link opens the section in OneNote Online.</span></span>|
|<span data-ttu-id="80f6c-144">displayName</span><span class="sxs-lookup"><span data-stu-id="80f6c-144">displayName</span></span>|<span data-ttu-id="80f6c-145">String</span><span class="sxs-lookup"><span data-stu-id="80f6c-145">String</span></span>|<span data-ttu-id="80f6c-146">Имя раздела.</span><span class="sxs-lookup"><span data-stu-id="80f6c-146">The name of the section.</span></span> |
|<span data-ttu-id="80f6c-147">Ссылки pagesurl</span><span class="sxs-lookup"><span data-stu-id="80f6c-147">pagesUrl</span></span>|<span data-ttu-id="80f6c-148">String</span><span class="sxs-lookup"><span data-stu-id="80f6c-148">String</span></span>|<span data-ttu-id="80f6c-149">Конечная точка, `pages` в которой можно получить сведения обо всех страницах в разделе.</span><span class="sxs-lookup"><span data-stu-id="80f6c-149">The `pages` endpoint where you can get details for all the pages in the section.</span></span> <span data-ttu-id="80f6c-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="80f6c-150">Read-only.</span></span>|
|<span data-ttu-id="80f6c-151">Self</span><span class="sxs-lookup"><span data-stu-id="80f6c-151">self</span></span>|<span data-ttu-id="80f6c-152">String</span><span class="sxs-lookup"><span data-stu-id="80f6c-152">String</span></span>|<span data-ttu-id="80f6c-153">Конечная точка, где можно получить сведения о разделе.</span><span class="sxs-lookup"><span data-stu-id="80f6c-153">The endpoint where you can get details about the section.</span></span> <span data-ttu-id="80f6c-154">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="80f6c-154">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="80f6c-155">Отношения</span><span class="sxs-lookup"><span data-stu-id="80f6c-155">Relationships</span></span>
| <span data-ttu-id="80f6c-156">Отношение</span><span class="sxs-lookup"><span data-stu-id="80f6c-156">Relationship</span></span> | <span data-ttu-id="80f6c-157">Тип</span><span class="sxs-lookup"><span data-stu-id="80f6c-157">Type</span></span>   |<span data-ttu-id="80f6c-158">Описание</span><span class="sxs-lookup"><span data-stu-id="80f6c-158">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="80f6c-159">pages</span><span class="sxs-lookup"><span data-stu-id="80f6c-159">pages</span></span>|<span data-ttu-id="80f6c-160">Коллекция [оненотепаже](onenotepage.md)</span><span class="sxs-lookup"><span data-stu-id="80f6c-160">[onenotePage](onenotepage.md) collection</span></span>|<span data-ttu-id="80f6c-161">Коллекция страниц в разделе.</span><span class="sxs-lookup"><span data-stu-id="80f6c-161">The collection of pages in the section.</span></span>  <span data-ttu-id="80f6c-162">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="80f6c-162">Read-only.</span></span> <span data-ttu-id="80f6c-163">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="80f6c-163">Nullable.</span></span>|
|<span data-ttu-id="80f6c-164">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="80f6c-164">parentNotebook</span></span>|[<span data-ttu-id="80f6c-165">записной книжки</span><span class="sxs-lookup"><span data-stu-id="80f6c-165">notebook</span></span>](notebook.md)|<span data-ttu-id="80f6c-166">Записная книжка, содержащая раздел.</span><span class="sxs-lookup"><span data-stu-id="80f6c-166">The notebook that contains the section.</span></span>  <span data-ttu-id="80f6c-167">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="80f6c-167">Read-only.</span></span>|
|<span data-ttu-id="80f6c-168">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="80f6c-168">parentSectionGroup</span></span>|[<span data-ttu-id="80f6c-169">sectionGroup</span><span class="sxs-lookup"><span data-stu-id="80f6c-169">sectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="80f6c-170">Группа разделов, содержащая раздел.</span><span class="sxs-lookup"><span data-stu-id="80f6c-170">The section group that contains the section.</span></span>  <span data-ttu-id="80f6c-171">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="80f6c-171">Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="80f6c-172">Методы</span><span class="sxs-lookup"><span data-stu-id="80f6c-172">Methods</span></span>

| <span data-ttu-id="80f6c-173">Метод</span><span class="sxs-lookup"><span data-stu-id="80f6c-173">Method</span></span>           | <span data-ttu-id="80f6c-174">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="80f6c-174">Return Type</span></span>    |<span data-ttu-id="80f6c-175">Описание</span><span class="sxs-lookup"><span data-stu-id="80f6c-175">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="80f6c-176">Получение раздела</span><span class="sxs-lookup"><span data-stu-id="80f6c-176">Get section</span></span>](../api/section-get.md) | [<span data-ttu-id="80f6c-177">Оненотесектион</span><span class="sxs-lookup"><span data-stu-id="80f6c-177">onenoteSection</span></span>](onenotesection.md) |<span data-ttu-id="80f6c-178">Прочитайте свойства и связи раздела.</span><span class="sxs-lookup"><span data-stu-id="80f6c-178">Read the properties and relationships of the section.</span></span>|
|[<span data-ttu-id="80f6c-179">Создание страницы</span><span class="sxs-lookup"><span data-stu-id="80f6c-179">Create page</span></span>](../api/section-post-pages.md) |[<span data-ttu-id="80f6c-180">Оненотепаже</span><span class="sxs-lookup"><span data-stu-id="80f6c-180">onenotePage</span></span>](onenotepage.md)| <span data-ttu-id="80f6c-181">Создание страницы путем публикации в коллекции страниц в указанном разделе.</span><span class="sxs-lookup"><span data-stu-id="80f6c-181">Create a page by posting to the pages collection in the specified section.</span></span>|
|[<span data-ttu-id="80f6c-182">Перечисление страниц</span><span class="sxs-lookup"><span data-stu-id="80f6c-182">List pages</span></span>](../api/section-list-pages.md) |<span data-ttu-id="80f6c-183">Коллекция [оненотепаже](onenotepage.md)</span><span class="sxs-lookup"><span data-stu-id="80f6c-183">[onenotePage](onenotepage.md) collection</span></span>| <span data-ttu-id="80f6c-184">Получение коллекции страниц в указанном разделе.</span><span class="sxs-lookup"><span data-stu-id="80f6c-184">Get a collection of pages in the specified section.</span></span>|
|[<span data-ttu-id="80f6c-185">copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="80f6c-185">copyToNotebook</span></span>](../api/section-copytonotebook.md)|<span data-ttu-id="80f6c-186">Отсутствует</span><span class="sxs-lookup"><span data-stu-id="80f6c-186">None</span></span>|<span data-ttu-id="80f6c-187">Скопируйте раздел в указанную записную книжку.</span><span class="sxs-lookup"><span data-stu-id="80f6c-187">Copy the section to a specific notebook.</span></span>|
|[<span data-ttu-id="80f6c-188">copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="80f6c-188">copyToSectionGroup</span></span>](../api/section-copytosectiongroup.md)|<span data-ttu-id="80f6c-189">Отсутствует</span><span class="sxs-lookup"><span data-stu-id="80f6c-189">None</span></span>|<span data-ttu-id="80f6c-190">Скопируйте раздел в определенную группу разделов.</span><span class="sxs-lookup"><span data-stu-id="80f6c-190">Copy the section to a specific section group.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="80f6c-191">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="80f6c-191">JSON representation</span></span>

<span data-ttu-id="80f6c-192">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="80f6c-192">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "pages",
    "parentNotebook",
    "parentSectionGroup"
  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
  "@odata.type": "microsoft.graph.onenoteSection"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "isDefault": true,
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "links": {"@odata.type": "microsoft.graph.sectionLinks"},
  "displayName": "string",
  "pagesUrl": "string",
  "self": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onenoteSection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
