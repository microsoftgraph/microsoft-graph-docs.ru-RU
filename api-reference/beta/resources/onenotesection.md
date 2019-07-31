---
title: Тип ресурса Оненотесектион
description: Раздел в записной книжке OneNote. Разделы могут содержать страницы.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: ed90d29e0441544bffd2576a255acf17e6cb3996
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966407"
---
# <a name="onenotesection-resource-type"></a><span data-ttu-id="40022-104">Тип ресурса Оненотесектион</span><span class="sxs-lookup"><span data-stu-id="40022-104">onenoteSection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40022-105">Раздел в записной книжке OneNote.</span><span class="sxs-lookup"><span data-stu-id="40022-105">A section in a OneNote notebook.</span></span> <span data-ttu-id="40022-106">Разделы могут содержать страницы.</span><span class="sxs-lookup"><span data-stu-id="40022-106">Sections can contain pages.</span></span>

## <a name="properties"></a><span data-ttu-id="40022-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="40022-107">Properties</span></span>
| <span data-ttu-id="40022-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="40022-108">Property</span></span>     | <span data-ttu-id="40022-109">Тип</span><span class="sxs-lookup"><span data-stu-id="40022-109">Type</span></span>   |<span data-ttu-id="40022-110">Описание</span><span class="sxs-lookup"><span data-stu-id="40022-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="40022-111">createdBy</span><span class="sxs-lookup"><span data-stu-id="40022-111">createdBy</span></span>|[<span data-ttu-id="40022-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="40022-112">identitySet</span></span>](identityset.md)|<span data-ttu-id="40022-p103">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="40022-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="40022-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="40022-115">createdDateTime</span></span>|<span data-ttu-id="40022-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40022-116">DateTimeOffset</span></span>|<span data-ttu-id="40022-117">Дата и время создания раздела.</span><span class="sxs-lookup"><span data-stu-id="40022-117">The date and time when the section was created.</span></span> <span data-ttu-id="40022-118">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="40022-118">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="40022-119">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="40022-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="40022-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="40022-120">Read-only.</span></span>|
|<span data-ttu-id="40022-121">id</span><span class="sxs-lookup"><span data-stu-id="40022-121">id</span></span>|<span data-ttu-id="40022-122">String</span><span class="sxs-lookup"><span data-stu-id="40022-122">String</span></span>|<span data-ttu-id="40022-123">Уникальный идентификатор раздела.</span><span class="sxs-lookup"><span data-stu-id="40022-123">The unique identifier of the section.</span></span>  <span data-ttu-id="40022-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="40022-124">Read-only.</span></span>|
|<span data-ttu-id="40022-125">isDefault</span><span class="sxs-lookup"><span data-stu-id="40022-125">isDefault</span></span>|<span data-ttu-id="40022-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="40022-126">Boolean</span></span>|<span data-ttu-id="40022-127">Указывает, является ли этот раздел разделом пользователя по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="40022-127">Indicates whether this is the user's default section.</span></span> <span data-ttu-id="40022-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="40022-128">Read-only.</span></span>|
|<span data-ttu-id="40022-129">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="40022-129">lastModifiedBy</span></span>|[<span data-ttu-id="40022-130">identitySet</span><span class="sxs-lookup"><span data-stu-id="40022-130">identitySet</span></span>](identityset.md)|<span data-ttu-id="40022-p107">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="40022-p107">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="40022-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="40022-133">lastModifiedDateTime</span></span>|<span data-ttu-id="40022-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40022-134">DateTimeOffset</span></span>|<span data-ttu-id="40022-135">Дата и время последнего изменения раздела.</span><span class="sxs-lookup"><span data-stu-id="40022-135">The date and time when the section was last modified.</span></span> <span data-ttu-id="40022-136">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="40022-136">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="40022-137">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="40022-137">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="40022-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="40022-138">Read-only.</span></span>|
|<span data-ttu-id="40022-139">links</span><span class="sxs-lookup"><span data-stu-id="40022-139">links</span></span>|[<span data-ttu-id="40022-140">Сектионлинкс</span><span class="sxs-lookup"><span data-stu-id="40022-140">sectionLinks</span></span>](sectionlinks.md)|<span data-ttu-id="40022-141">Ссылки для открытия раздела.</span><span class="sxs-lookup"><span data-stu-id="40022-141">Links for opening the section.</span></span> <span data-ttu-id="40022-142">`oneNoteClientURL` Ссылка открывает раздел в собственном клиенте OneNote, если он установлен.</span><span class="sxs-lookup"><span data-stu-id="40022-142">The `oneNoteClientURL` link opens the section in the OneNote native client if it's installed.</span></span> <span data-ttu-id="40022-143">`oneNoteWebURL` Ссылка открывает раздел в OneNote в Интернете.</span><span class="sxs-lookup"><span data-stu-id="40022-143">The `oneNoteWebURL` link opens the section in OneNote on the web.</span></span>|
|<span data-ttu-id="40022-144">displayName</span><span class="sxs-lookup"><span data-stu-id="40022-144">displayName</span></span>|<span data-ttu-id="40022-145">Строка</span><span class="sxs-lookup"><span data-stu-id="40022-145">String</span></span>|<span data-ttu-id="40022-146">Имя раздела.</span><span class="sxs-lookup"><span data-stu-id="40022-146">The name of the section.</span></span> |
|<span data-ttu-id="40022-147">Ссылки pagesurl</span><span class="sxs-lookup"><span data-stu-id="40022-147">pagesUrl</span></span>|<span data-ttu-id="40022-148">String</span><span class="sxs-lookup"><span data-stu-id="40022-148">String</span></span>|<span data-ttu-id="40022-149">Конечная точка, `pages` в которой можно получить сведения обо всех страницах в разделе.</span><span class="sxs-lookup"><span data-stu-id="40022-149">The `pages` endpoint where you can get details for all the pages in the section.</span></span> <span data-ttu-id="40022-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="40022-150">Read-only.</span></span>|
|<span data-ttu-id="40022-151">Self</span><span class="sxs-lookup"><span data-stu-id="40022-151">self</span></span>|<span data-ttu-id="40022-152">String</span><span class="sxs-lookup"><span data-stu-id="40022-152">String</span></span>|<span data-ttu-id="40022-153">Конечная точка, где можно получить сведения о разделе.</span><span class="sxs-lookup"><span data-stu-id="40022-153">The endpoint where you can get details about the section.</span></span> <span data-ttu-id="40022-154">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="40022-154">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="40022-155">Отношения</span><span class="sxs-lookup"><span data-stu-id="40022-155">Relationships</span></span>
| <span data-ttu-id="40022-156">Отношение</span><span class="sxs-lookup"><span data-stu-id="40022-156">Relationship</span></span> | <span data-ttu-id="40022-157">Тип</span><span class="sxs-lookup"><span data-stu-id="40022-157">Type</span></span>   |<span data-ttu-id="40022-158">Описание</span><span class="sxs-lookup"><span data-stu-id="40022-158">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="40022-159">pages</span><span class="sxs-lookup"><span data-stu-id="40022-159">pages</span></span>|<span data-ttu-id="40022-160">Коллекция [оненотепаже](onenotepage.md)</span><span class="sxs-lookup"><span data-stu-id="40022-160">[onenotePage](onenotepage.md) collection</span></span>|<span data-ttu-id="40022-161">Коллекция страниц в разделе.</span><span class="sxs-lookup"><span data-stu-id="40022-161">The collection of pages in the section.</span></span>  <span data-ttu-id="40022-162">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="40022-162">Read-only.</span></span> <span data-ttu-id="40022-163">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="40022-163">Nullable.</span></span>|
|<span data-ttu-id="40022-164">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="40022-164">parentNotebook</span></span>|[<span data-ttu-id="40022-165">записной книжки</span><span class="sxs-lookup"><span data-stu-id="40022-165">notebook</span></span>](notebook.md)|<span data-ttu-id="40022-166">Записная книжка, содержащая раздел.</span><span class="sxs-lookup"><span data-stu-id="40022-166">The notebook that contains the section.</span></span>  <span data-ttu-id="40022-167">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="40022-167">Read-only.</span></span>|
|<span data-ttu-id="40022-168">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="40022-168">parentSectionGroup</span></span>|[<span data-ttu-id="40022-169">sectionGroup</span><span class="sxs-lookup"><span data-stu-id="40022-169">sectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="40022-170">Группа разделов, содержащая раздел.</span><span class="sxs-lookup"><span data-stu-id="40022-170">The section group that contains the section.</span></span>  <span data-ttu-id="40022-171">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="40022-171">Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="40022-172">Методы</span><span class="sxs-lookup"><span data-stu-id="40022-172">Methods</span></span>

| <span data-ttu-id="40022-173">Метод</span><span class="sxs-lookup"><span data-stu-id="40022-173">Method</span></span>           | <span data-ttu-id="40022-174">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="40022-174">Return Type</span></span>    |<span data-ttu-id="40022-175">Описание</span><span class="sxs-lookup"><span data-stu-id="40022-175">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="40022-176">Получение раздела</span><span class="sxs-lookup"><span data-stu-id="40022-176">Get section</span></span>](../api/section-get.md) | [<span data-ttu-id="40022-177">Оненотесектион</span><span class="sxs-lookup"><span data-stu-id="40022-177">onenoteSection</span></span>](onenotesection.md) |<span data-ttu-id="40022-178">Прочитайте свойства и связи раздела.</span><span class="sxs-lookup"><span data-stu-id="40022-178">Read the properties and relationships of the section.</span></span>|
|[<span data-ttu-id="40022-179">Создание страницы</span><span class="sxs-lookup"><span data-stu-id="40022-179">Create page</span></span>](../api/section-post-pages.md) |[<span data-ttu-id="40022-180">Оненотепаже</span><span class="sxs-lookup"><span data-stu-id="40022-180">onenotePage</span></span>](onenotepage.md)| <span data-ttu-id="40022-181">Создание страницы путем публикации в коллекции страниц в указанном разделе.</span><span class="sxs-lookup"><span data-stu-id="40022-181">Create a page by posting to the pages collection in the specified section.</span></span>|
|[<span data-ttu-id="40022-182">Перечисление страниц</span><span class="sxs-lookup"><span data-stu-id="40022-182">List pages</span></span>](../api/section-list-pages.md) |<span data-ttu-id="40022-183">Коллекция [оненотепаже](onenotepage.md)</span><span class="sxs-lookup"><span data-stu-id="40022-183">[onenotePage](onenotepage.md) collection</span></span>| <span data-ttu-id="40022-184">Получение коллекции страниц в указанном разделе.</span><span class="sxs-lookup"><span data-stu-id="40022-184">Get a collection of pages in the specified section.</span></span>|
|[<span data-ttu-id="40022-185">copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="40022-185">copyToNotebook</span></span>](../api/section-copytonotebook.md)|<span data-ttu-id="40022-186">Нет</span><span class="sxs-lookup"><span data-stu-id="40022-186">None</span></span>|<span data-ttu-id="40022-187">Скопируйте раздел в указанную записную книжку.</span><span class="sxs-lookup"><span data-stu-id="40022-187">Copy the section to a specific notebook.</span></span>|
|[<span data-ttu-id="40022-188">copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="40022-188">copyToSectionGroup</span></span>](../api/section-copytosectiongroup.md)|<span data-ttu-id="40022-189">Нет</span><span class="sxs-lookup"><span data-stu-id="40022-189">None</span></span>|<span data-ttu-id="40022-190">Скопируйте раздел в определенную группу разделов.</span><span class="sxs-lookup"><span data-stu-id="40022-190">Copy the section to a specific section group.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="40022-191">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="40022-191">JSON representation</span></span>

<span data-ttu-id="40022-192">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="40022-192">Here is a JSON representation of the resource.</span></span>

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
