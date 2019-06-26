---
title: Тип ресурса Оненотесектион
description: Раздел в записной книжке OneNote. Разделы могут содержать страницы.
localization_priority: Normal
ms.openlocfilehash: b07ea378a4338e22896d40065e35aa599db42832
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2019
ms.locfileid: "35236631"
---
# <a name="onenotesection-resource-type"></a><span data-ttu-id="29ece-104">Тип ресурса Оненотесектион</span><span class="sxs-lookup"><span data-stu-id="29ece-104">onenoteSection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29ece-105">Раздел в записной книжке OneNote.</span><span class="sxs-lookup"><span data-stu-id="29ece-105">A section in a OneNote notebook.</span></span> <span data-ttu-id="29ece-106">Разделы могут содержать страницы.</span><span class="sxs-lookup"><span data-stu-id="29ece-106">Sections can contain pages.</span></span>

## <a name="properties"></a><span data-ttu-id="29ece-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="29ece-107">Properties</span></span>
| <span data-ttu-id="29ece-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="29ece-108">Property</span></span>     | <span data-ttu-id="29ece-109">Тип</span><span class="sxs-lookup"><span data-stu-id="29ece-109">Type</span></span>   |<span data-ttu-id="29ece-110">Описание</span><span class="sxs-lookup"><span data-stu-id="29ece-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="29ece-111">createdBy</span><span class="sxs-lookup"><span data-stu-id="29ece-111">createdBy</span></span>|[<span data-ttu-id="29ece-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="29ece-112">identitySet</span></span>](identityset.md)|<span data-ttu-id="29ece-p103">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="29ece-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="29ece-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="29ece-115">createdDateTime</span></span>|<span data-ttu-id="29ece-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29ece-116">DateTimeOffset</span></span>|<span data-ttu-id="29ece-117">Дата и время создания раздела.</span><span class="sxs-lookup"><span data-stu-id="29ece-117">The date and time when the section was created.</span></span> <span data-ttu-id="29ece-118">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="29ece-118">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="29ece-119">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="29ece-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="29ece-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="29ece-120">Read-only.</span></span>|
|<span data-ttu-id="29ece-121">id</span><span class="sxs-lookup"><span data-stu-id="29ece-121">id</span></span>|<span data-ttu-id="29ece-122">String</span><span class="sxs-lookup"><span data-stu-id="29ece-122">String</span></span>|<span data-ttu-id="29ece-123">Уникальный идентификатор раздела.</span><span class="sxs-lookup"><span data-stu-id="29ece-123">The unique identifier of the section.</span></span>  <span data-ttu-id="29ece-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="29ece-124">Read-only.</span></span>|
|<span data-ttu-id="29ece-125">isDefault</span><span class="sxs-lookup"><span data-stu-id="29ece-125">isDefault</span></span>|<span data-ttu-id="29ece-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="29ece-126">Boolean</span></span>|<span data-ttu-id="29ece-127">Указывает, является ли этот раздел разделом пользователя по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="29ece-127">Indicates whether this is the user's default section.</span></span> <span data-ttu-id="29ece-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="29ece-128">Read-only.</span></span>|
|<span data-ttu-id="29ece-129">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="29ece-129">lastModifiedBy</span></span>|[<span data-ttu-id="29ece-130">identitySet</span><span class="sxs-lookup"><span data-stu-id="29ece-130">identitySet</span></span>](identityset.md)|<span data-ttu-id="29ece-p107">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="29ece-p107">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="29ece-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="29ece-133">lastModifiedDateTime</span></span>|<span data-ttu-id="29ece-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29ece-134">DateTimeOffset</span></span>|<span data-ttu-id="29ece-135">Дата и время последнего изменения раздела.</span><span class="sxs-lookup"><span data-stu-id="29ece-135">The date and time when the section was last modified.</span></span> <span data-ttu-id="29ece-136">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="29ece-136">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="29ece-137">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="29ece-137">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="29ece-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="29ece-138">Read-only.</span></span>|
|<span data-ttu-id="29ece-139">links</span><span class="sxs-lookup"><span data-stu-id="29ece-139">links</span></span>|[<span data-ttu-id="29ece-140">Сектионлинкс</span><span class="sxs-lookup"><span data-stu-id="29ece-140">sectionLinks</span></span>](sectionlinks.md)|<span data-ttu-id="29ece-141">Ссылки для открытия раздела.</span><span class="sxs-lookup"><span data-stu-id="29ece-141">Links for opening the section.</span></span> <span data-ttu-id="29ece-142">`oneNoteClientURL` Ссылка открывает раздел в собственном клиенте OneNote, если он установлен.</span><span class="sxs-lookup"><span data-stu-id="29ece-142">The `oneNoteClientURL` link opens the section in the OneNote native client if it's installed.</span></span> <span data-ttu-id="29ece-143">`oneNoteWebURL` Ссылка открывает раздел в OneNote в Интернете.</span><span class="sxs-lookup"><span data-stu-id="29ece-143">The `oneNoteWebURL` link opens the section in OneNote on the web.</span></span>|
|<span data-ttu-id="29ece-144">displayName</span><span class="sxs-lookup"><span data-stu-id="29ece-144">displayName</span></span>|<span data-ttu-id="29ece-145">Строка</span><span class="sxs-lookup"><span data-stu-id="29ece-145">String</span></span>|<span data-ttu-id="29ece-146">Имя раздела.</span><span class="sxs-lookup"><span data-stu-id="29ece-146">The name of the section.</span></span> |
|<span data-ttu-id="29ece-147">Ссылки pagesurl</span><span class="sxs-lookup"><span data-stu-id="29ece-147">pagesUrl</span></span>|<span data-ttu-id="29ece-148">String</span><span class="sxs-lookup"><span data-stu-id="29ece-148">String</span></span>|<span data-ttu-id="29ece-149">Конечная точка, `pages` в которой можно получить сведения обо всех страницах в разделе.</span><span class="sxs-lookup"><span data-stu-id="29ece-149">The `pages` endpoint where you can get details for all the pages in the section.</span></span> <span data-ttu-id="29ece-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="29ece-150">Read-only.</span></span>|
|<span data-ttu-id="29ece-151">Self</span><span class="sxs-lookup"><span data-stu-id="29ece-151">self</span></span>|<span data-ttu-id="29ece-152">String</span><span class="sxs-lookup"><span data-stu-id="29ece-152">String</span></span>|<span data-ttu-id="29ece-153">Конечная точка, где можно получить сведения о разделе.</span><span class="sxs-lookup"><span data-stu-id="29ece-153">The endpoint where you can get details about the section.</span></span> <span data-ttu-id="29ece-154">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="29ece-154">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="29ece-155">Отношения</span><span class="sxs-lookup"><span data-stu-id="29ece-155">Relationships</span></span>
| <span data-ttu-id="29ece-156">Отношение</span><span class="sxs-lookup"><span data-stu-id="29ece-156">Relationship</span></span> | <span data-ttu-id="29ece-157">Тип</span><span class="sxs-lookup"><span data-stu-id="29ece-157">Type</span></span>   |<span data-ttu-id="29ece-158">Описание</span><span class="sxs-lookup"><span data-stu-id="29ece-158">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="29ece-159">pages</span><span class="sxs-lookup"><span data-stu-id="29ece-159">pages</span></span>|<span data-ttu-id="29ece-160">Коллекция [оненотепаже](onenotepage.md)</span><span class="sxs-lookup"><span data-stu-id="29ece-160">[onenotePage](onenotepage.md) collection</span></span>|<span data-ttu-id="29ece-161">Коллекция страниц в разделе.</span><span class="sxs-lookup"><span data-stu-id="29ece-161">The collection of pages in the section.</span></span>  <span data-ttu-id="29ece-162">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="29ece-162">Read-only.</span></span> <span data-ttu-id="29ece-163">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="29ece-163">Nullable.</span></span>|
|<span data-ttu-id="29ece-164">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="29ece-164">parentNotebook</span></span>|[<span data-ttu-id="29ece-165">записной книжки</span><span class="sxs-lookup"><span data-stu-id="29ece-165">notebook</span></span>](notebook.md)|<span data-ttu-id="29ece-166">Записная книжка, содержащая раздел.</span><span class="sxs-lookup"><span data-stu-id="29ece-166">The notebook that contains the section.</span></span>  <span data-ttu-id="29ece-167">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="29ece-167">Read-only.</span></span>|
|<span data-ttu-id="29ece-168">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="29ece-168">parentSectionGroup</span></span>|[<span data-ttu-id="29ece-169">sectionGroup</span><span class="sxs-lookup"><span data-stu-id="29ece-169">sectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="29ece-170">Группа разделов, содержащая раздел.</span><span class="sxs-lookup"><span data-stu-id="29ece-170">The section group that contains the section.</span></span>  <span data-ttu-id="29ece-171">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="29ece-171">Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="29ece-172">Методы</span><span class="sxs-lookup"><span data-stu-id="29ece-172">Methods</span></span>

| <span data-ttu-id="29ece-173">Метод</span><span class="sxs-lookup"><span data-stu-id="29ece-173">Method</span></span>           | <span data-ttu-id="29ece-174">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="29ece-174">Return Type</span></span>    |<span data-ttu-id="29ece-175">Описание</span><span class="sxs-lookup"><span data-stu-id="29ece-175">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="29ece-176">Получение раздела</span><span class="sxs-lookup"><span data-stu-id="29ece-176">Get section</span></span>](../api/section-get.md) | [<span data-ttu-id="29ece-177">Оненотесектион</span><span class="sxs-lookup"><span data-stu-id="29ece-177">onenoteSection</span></span>](onenotesection.md) |<span data-ttu-id="29ece-178">Прочитайте свойства и связи раздела.</span><span class="sxs-lookup"><span data-stu-id="29ece-178">Read the properties and relationships of the section.</span></span>|
|[<span data-ttu-id="29ece-179">Создание страницы</span><span class="sxs-lookup"><span data-stu-id="29ece-179">Create page</span></span>](../api/section-post-pages.md) |[<span data-ttu-id="29ece-180">Оненотепаже</span><span class="sxs-lookup"><span data-stu-id="29ece-180">onenotePage</span></span>](onenotepage.md)| <span data-ttu-id="29ece-181">Создание страницы путем публикации в коллекции страниц в указанном разделе.</span><span class="sxs-lookup"><span data-stu-id="29ece-181">Create a page by posting to the pages collection in the specified section.</span></span>|
|[<span data-ttu-id="29ece-182">Перечисление страниц</span><span class="sxs-lookup"><span data-stu-id="29ece-182">List pages</span></span>](../api/section-list-pages.md) |<span data-ttu-id="29ece-183">Коллекция [оненотепаже](onenotepage.md)</span><span class="sxs-lookup"><span data-stu-id="29ece-183">[onenotePage](onenotepage.md) collection</span></span>| <span data-ttu-id="29ece-184">Получение коллекции страниц в указанном разделе.</span><span class="sxs-lookup"><span data-stu-id="29ece-184">Get a collection of pages in the specified section.</span></span>|
|[<span data-ttu-id="29ece-185">copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="29ece-185">copyToNotebook</span></span>](../api/section-copytonotebook.md)|<span data-ttu-id="29ece-186">Нет</span><span class="sxs-lookup"><span data-stu-id="29ece-186">None</span></span>|<span data-ttu-id="29ece-187">Скопируйте раздел в указанную записную книжку.</span><span class="sxs-lookup"><span data-stu-id="29ece-187">Copy the section to a specific notebook.</span></span>|
|[<span data-ttu-id="29ece-188">copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="29ece-188">copyToSectionGroup</span></span>](../api/section-copytosectiongroup.md)|<span data-ttu-id="29ece-189">Нет</span><span class="sxs-lookup"><span data-stu-id="29ece-189">None</span></span>|<span data-ttu-id="29ece-190">Скопируйте раздел в определенную группу разделов.</span><span class="sxs-lookup"><span data-stu-id="29ece-190">Copy the section to a specific section group.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="29ece-191">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="29ece-191">JSON representation</span></span>

<span data-ttu-id="29ece-192">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="29ece-192">Here is a JSON representation of the resource.</span></span>

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
