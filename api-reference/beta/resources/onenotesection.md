---
title: Тип ресурса Оненотесектион
description: Раздел в записной книжке OneNote. Разделы могут содержать страницы.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: f23017506208c1c0ff4f5a190eafe12079626d23
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522318"
---
# <a name="onenotesection-resource-type"></a><span data-ttu-id="92d0c-104">Тип ресурса Оненотесектион</span><span class="sxs-lookup"><span data-stu-id="92d0c-104">onenoteSection resource type</span></span>

<span data-ttu-id="92d0c-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="92d0c-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92d0c-106">Раздел в записной книжке OneNote.</span><span class="sxs-lookup"><span data-stu-id="92d0c-106">A section in a OneNote notebook.</span></span> <span data-ttu-id="92d0c-107">Разделы могут содержать страницы.</span><span class="sxs-lookup"><span data-stu-id="92d0c-107">Sections can contain pages.</span></span>

## <a name="properties"></a><span data-ttu-id="92d0c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="92d0c-108">Properties</span></span>
| <span data-ttu-id="92d0c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="92d0c-109">Property</span></span>     | <span data-ttu-id="92d0c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="92d0c-110">Type</span></span>   |<span data-ttu-id="92d0c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="92d0c-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="92d0c-112">createdBy</span><span class="sxs-lookup"><span data-stu-id="92d0c-112">createdBy</span></span>|[<span data-ttu-id="92d0c-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="92d0c-113">identitySet</span></span>](identityset.md)|<span data-ttu-id="92d0c-p103">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="92d0c-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="92d0c-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="92d0c-116">createdDateTime</span></span>|<span data-ttu-id="92d0c-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92d0c-117">DateTimeOffset</span></span>|<span data-ttu-id="92d0c-118">Дата и время создания раздела.</span><span class="sxs-lookup"><span data-stu-id="92d0c-118">The date and time when the section was created.</span></span> <span data-ttu-id="92d0c-119">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="92d0c-119">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="92d0c-120">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="92d0c-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="92d0c-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="92d0c-121">Read-only.</span></span>|
|<span data-ttu-id="92d0c-122">id</span><span class="sxs-lookup"><span data-stu-id="92d0c-122">id</span></span>|<span data-ttu-id="92d0c-123">String</span><span class="sxs-lookup"><span data-stu-id="92d0c-123">String</span></span>|<span data-ttu-id="92d0c-124">Уникальный идентификатор раздела.</span><span class="sxs-lookup"><span data-stu-id="92d0c-124">The unique identifier of the section.</span></span>  <span data-ttu-id="92d0c-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="92d0c-125">Read-only.</span></span>|
|<span data-ttu-id="92d0c-126">isDefault</span><span class="sxs-lookup"><span data-stu-id="92d0c-126">isDefault</span></span>|<span data-ttu-id="92d0c-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="92d0c-127">Boolean</span></span>|<span data-ttu-id="92d0c-128">Указывает, является ли этот раздел разделом пользователя по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="92d0c-128">Indicates whether this is the user's default section.</span></span> <span data-ttu-id="92d0c-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="92d0c-129">Read-only.</span></span>|
|<span data-ttu-id="92d0c-130">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="92d0c-130">lastModifiedBy</span></span>|[<span data-ttu-id="92d0c-131">identitySet</span><span class="sxs-lookup"><span data-stu-id="92d0c-131">identitySet</span></span>](identityset.md)|<span data-ttu-id="92d0c-p107">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="92d0c-p107">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="92d0c-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="92d0c-134">lastModifiedDateTime</span></span>|<span data-ttu-id="92d0c-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92d0c-135">DateTimeOffset</span></span>|<span data-ttu-id="92d0c-136">Дата и время последнего изменения раздела.</span><span class="sxs-lookup"><span data-stu-id="92d0c-136">The date and time when the section was last modified.</span></span> <span data-ttu-id="92d0c-137">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="92d0c-137">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="92d0c-138">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="92d0c-138">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="92d0c-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="92d0c-139">Read-only.</span></span>|
|<span data-ttu-id="92d0c-140">links</span><span class="sxs-lookup"><span data-stu-id="92d0c-140">links</span></span>|[<span data-ttu-id="92d0c-141">сектионлинкс</span><span class="sxs-lookup"><span data-stu-id="92d0c-141">sectionLinks</span></span>](sectionlinks.md)|<span data-ttu-id="92d0c-142">Ссылки для открытия раздела.</span><span class="sxs-lookup"><span data-stu-id="92d0c-142">Links for opening the section.</span></span> <span data-ttu-id="92d0c-143">`oneNoteClientURL` Ссылка открывает раздел в собственном клиенте OneNote, если он установлен.</span><span class="sxs-lookup"><span data-stu-id="92d0c-143">The `oneNoteClientURL` link opens the section in the OneNote native client if it's installed.</span></span> <span data-ttu-id="92d0c-144">`oneNoteWebURL` Ссылка открывает раздел в OneNote в Интернете.</span><span class="sxs-lookup"><span data-stu-id="92d0c-144">The `oneNoteWebURL` link opens the section in OneNote on the web.</span></span>|
|<span data-ttu-id="92d0c-145">displayName</span><span class="sxs-lookup"><span data-stu-id="92d0c-145">displayName</span></span>|<span data-ttu-id="92d0c-146">Строка</span><span class="sxs-lookup"><span data-stu-id="92d0c-146">String</span></span>|<span data-ttu-id="92d0c-147">Имя раздела.</span><span class="sxs-lookup"><span data-stu-id="92d0c-147">The name of the section.</span></span> |
|<span data-ttu-id="92d0c-148">Ссылки pagesurl</span><span class="sxs-lookup"><span data-stu-id="92d0c-148">pagesUrl</span></span>|<span data-ttu-id="92d0c-149">String</span><span class="sxs-lookup"><span data-stu-id="92d0c-149">String</span></span>|<span data-ttu-id="92d0c-150">Конечная точка, `pages` в которой можно получить сведения обо всех страницах в разделе.</span><span class="sxs-lookup"><span data-stu-id="92d0c-150">The `pages` endpoint where you can get details for all the pages in the section.</span></span> <span data-ttu-id="92d0c-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="92d0c-151">Read-only.</span></span>|
|<span data-ttu-id="92d0c-152">Self</span><span class="sxs-lookup"><span data-stu-id="92d0c-152">self</span></span>|<span data-ttu-id="92d0c-153">String</span><span class="sxs-lookup"><span data-stu-id="92d0c-153">String</span></span>|<span data-ttu-id="92d0c-154">Конечная точка, где можно получить сведения о разделе.</span><span class="sxs-lookup"><span data-stu-id="92d0c-154">The endpoint where you can get details about the section.</span></span> <span data-ttu-id="92d0c-155">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="92d0c-155">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="92d0c-156">Отношения</span><span class="sxs-lookup"><span data-stu-id="92d0c-156">Relationships</span></span>
| <span data-ttu-id="92d0c-157">Связь</span><span class="sxs-lookup"><span data-stu-id="92d0c-157">Relationship</span></span> | <span data-ttu-id="92d0c-158">Тип</span><span class="sxs-lookup"><span data-stu-id="92d0c-158">Type</span></span>   |<span data-ttu-id="92d0c-159">Описание</span><span class="sxs-lookup"><span data-stu-id="92d0c-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="92d0c-160">pages</span><span class="sxs-lookup"><span data-stu-id="92d0c-160">pages</span></span>|<span data-ttu-id="92d0c-161">Коллекция [оненотепаже](onenotepage.md)</span><span class="sxs-lookup"><span data-stu-id="92d0c-161">[onenotePage](onenotepage.md) collection</span></span>|<span data-ttu-id="92d0c-162">Коллекция страниц в разделе.</span><span class="sxs-lookup"><span data-stu-id="92d0c-162">The collection of pages in the section.</span></span>  <span data-ttu-id="92d0c-163">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="92d0c-163">Read-only.</span></span> <span data-ttu-id="92d0c-164">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="92d0c-164">Nullable.</span></span>|
|<span data-ttu-id="92d0c-165">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="92d0c-165">parentNotebook</span></span>|[<span data-ttu-id="92d0c-166">notebook</span><span class="sxs-lookup"><span data-stu-id="92d0c-166">notebook</span></span>](notebook.md)|<span data-ttu-id="92d0c-167">Записная книжка, содержащая раздел.</span><span class="sxs-lookup"><span data-stu-id="92d0c-167">The notebook that contains the section.</span></span>  <span data-ttu-id="92d0c-168">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="92d0c-168">Read-only.</span></span>|
|<span data-ttu-id="92d0c-169">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="92d0c-169">parentSectionGroup</span></span>|[<span data-ttu-id="92d0c-170">sectionGroup</span><span class="sxs-lookup"><span data-stu-id="92d0c-170">sectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="92d0c-171">Группа разделов, содержащая раздел.</span><span class="sxs-lookup"><span data-stu-id="92d0c-171">The section group that contains the section.</span></span>  <span data-ttu-id="92d0c-172">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="92d0c-172">Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="92d0c-173">Методы</span><span class="sxs-lookup"><span data-stu-id="92d0c-173">Methods</span></span>

| <span data-ttu-id="92d0c-174">Метод</span><span class="sxs-lookup"><span data-stu-id="92d0c-174">Method</span></span>           | <span data-ttu-id="92d0c-175">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="92d0c-175">Return Type</span></span>    |<span data-ttu-id="92d0c-176">Описание</span><span class="sxs-lookup"><span data-stu-id="92d0c-176">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="92d0c-177">Получение раздела</span><span class="sxs-lookup"><span data-stu-id="92d0c-177">Get section</span></span>](../api/section-get.md) | [<span data-ttu-id="92d0c-178">оненотесектион</span><span class="sxs-lookup"><span data-stu-id="92d0c-178">onenoteSection</span></span>](onenotesection.md) |<span data-ttu-id="92d0c-179">Прочитайте свойства и связи раздела.</span><span class="sxs-lookup"><span data-stu-id="92d0c-179">Read the properties and relationships of the section.</span></span>|
|[<span data-ttu-id="92d0c-180">Создание страницы</span><span class="sxs-lookup"><span data-stu-id="92d0c-180">Create page</span></span>](../api/section-post-pages.md) |[<span data-ttu-id="92d0c-181">оненотепаже</span><span class="sxs-lookup"><span data-stu-id="92d0c-181">onenotePage</span></span>](onenotepage.md)| <span data-ttu-id="92d0c-182">Создание страницы путем публикации в коллекции страниц в указанном разделе.</span><span class="sxs-lookup"><span data-stu-id="92d0c-182">Create a page by posting to the pages collection in the specified section.</span></span>|
|[<span data-ttu-id="92d0c-183">Перечисление страниц</span><span class="sxs-lookup"><span data-stu-id="92d0c-183">List pages</span></span>](../api/section-list-pages.md) |<span data-ttu-id="92d0c-184">Коллекция [оненотепаже](onenotepage.md)</span><span class="sxs-lookup"><span data-stu-id="92d0c-184">[onenotePage](onenotepage.md) collection</span></span>| <span data-ttu-id="92d0c-185">Получение коллекции страниц в указанном разделе.</span><span class="sxs-lookup"><span data-stu-id="92d0c-185">Get a collection of pages in the specified section.</span></span>|
|[<span data-ttu-id="92d0c-186">copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="92d0c-186">copyToNotebook</span></span>](../api/section-copytonotebook.md)|<span data-ttu-id="92d0c-187">Нет</span><span class="sxs-lookup"><span data-stu-id="92d0c-187">None</span></span>|<span data-ttu-id="92d0c-188">Скопируйте раздел в указанную записную книжку.</span><span class="sxs-lookup"><span data-stu-id="92d0c-188">Copy the section to a specific notebook.</span></span>|
|[<span data-ttu-id="92d0c-189">copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="92d0c-189">copyToSectionGroup</span></span>](../api/section-copytosectiongroup.md)|<span data-ttu-id="92d0c-190">Нет</span><span class="sxs-lookup"><span data-stu-id="92d0c-190">None</span></span>|<span data-ttu-id="92d0c-191">Скопируйте раздел в определенную группу разделов.</span><span class="sxs-lookup"><span data-stu-id="92d0c-191">Copy the section to a specific section group.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="92d0c-192">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="92d0c-192">JSON representation</span></span>

<span data-ttu-id="92d0c-193">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="92d0c-193">Here is a JSON representation of the resource.</span></span>

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
