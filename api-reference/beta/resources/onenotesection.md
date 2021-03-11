---
title: тип ресурса onenoteSection
description: Раздел в записной книжке OneNote. Разделы могут содержать страницы.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: jewan-microsoft
ms.openlocfilehash: 7a87c2f7cfb253acd3bee714dc28ae685a9559a6
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50718494"
---
# <a name="onenotesection-resource-type"></a><span data-ttu-id="69ba9-104">тип ресурса onenoteSection</span><span class="sxs-lookup"><span data-stu-id="69ba9-104">onenoteSection resource type</span></span>

<span data-ttu-id="69ba9-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69ba9-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69ba9-106">Раздел в записной книжке OneNote.</span><span class="sxs-lookup"><span data-stu-id="69ba9-106">A section in a OneNote notebook.</span></span> <span data-ttu-id="69ba9-107">Разделы могут содержать страницы.</span><span class="sxs-lookup"><span data-stu-id="69ba9-107">Sections can contain pages.</span></span>

## <a name="properties"></a><span data-ttu-id="69ba9-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="69ba9-108">Properties</span></span>
| <span data-ttu-id="69ba9-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="69ba9-109">Property</span></span>     | <span data-ttu-id="69ba9-110">Тип</span><span class="sxs-lookup"><span data-stu-id="69ba9-110">Type</span></span>   |<span data-ttu-id="69ba9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="69ba9-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="69ba9-112">createdBy</span><span class="sxs-lookup"><span data-stu-id="69ba9-112">createdBy</span></span>|[<span data-ttu-id="69ba9-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="69ba9-113">identitySet</span></span>](identityset.md)|<span data-ttu-id="69ba9-p103">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="69ba9-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="69ba9-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="69ba9-116">createdDateTime</span></span>|<span data-ttu-id="69ba9-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69ba9-117">DateTimeOffset</span></span>|<span data-ttu-id="69ba9-118">Дата и время создания раздела.</span><span class="sxs-lookup"><span data-stu-id="69ba9-118">The date and time when the section was created.</span></span> <span data-ttu-id="69ba9-119">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="69ba9-119">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="69ba9-120">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="69ba9-120">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="69ba9-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="69ba9-121">Read-only.</span></span>|
|<span data-ttu-id="69ba9-122">id</span><span class="sxs-lookup"><span data-stu-id="69ba9-122">id</span></span>|<span data-ttu-id="69ba9-123">String</span><span class="sxs-lookup"><span data-stu-id="69ba9-123">String</span></span>|<span data-ttu-id="69ba9-124">Уникальный идентификатор раздела.</span><span class="sxs-lookup"><span data-stu-id="69ba9-124">The unique identifier of the section.</span></span>  <span data-ttu-id="69ba9-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="69ba9-125">Read-only.</span></span>|
|<span data-ttu-id="69ba9-126">isDefault</span><span class="sxs-lookup"><span data-stu-id="69ba9-126">isDefault</span></span>|<span data-ttu-id="69ba9-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="69ba9-127">Boolean</span></span>|<span data-ttu-id="69ba9-128">Указывает, является ли это разделом по умолчанию пользователя.</span><span class="sxs-lookup"><span data-stu-id="69ba9-128">Indicates whether this is the user's default section.</span></span> <span data-ttu-id="69ba9-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="69ba9-129">Read-only.</span></span>|
|<span data-ttu-id="69ba9-130">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="69ba9-130">lastModifiedBy</span></span>|[<span data-ttu-id="69ba9-131">identitySet</span><span class="sxs-lookup"><span data-stu-id="69ba9-131">identitySet</span></span>](identityset.md)|<span data-ttu-id="69ba9-p107">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="69ba9-p107">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="69ba9-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="69ba9-134">lastModifiedDateTime</span></span>|<span data-ttu-id="69ba9-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69ba9-135">DateTimeOffset</span></span>|<span data-ttu-id="69ba9-136">Дата и время последнего изменения раздела.</span><span class="sxs-lookup"><span data-stu-id="69ba9-136">The date and time when the section was last modified.</span></span> <span data-ttu-id="69ba9-137">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="69ba9-137">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="69ba9-138">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="69ba9-138">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="69ba9-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="69ba9-139">Read-only.</span></span>|
|<span data-ttu-id="69ba9-140">links</span><span class="sxs-lookup"><span data-stu-id="69ba9-140">links</span></span>|[<span data-ttu-id="69ba9-141">sectionLinks</span><span class="sxs-lookup"><span data-stu-id="69ba9-141">sectionLinks</span></span>](sectionlinks.md)|<span data-ttu-id="69ba9-142">Ссылки для открытия раздела.</span><span class="sxs-lookup"><span data-stu-id="69ba9-142">Links for opening the section.</span></span> <span data-ttu-id="69ba9-143">Ссылка открывает раздел в родном клиенте `oneNoteClientURL` OneNote, если он установлен.</span><span class="sxs-lookup"><span data-stu-id="69ba9-143">The `oneNoteClientURL` link opens the section in the OneNote native client if it's installed.</span></span> <span data-ttu-id="69ba9-144">Ссылка `oneNoteWebURL` открывает раздел в OneNote в Интернете.</span><span class="sxs-lookup"><span data-stu-id="69ba9-144">The `oneNoteWebURL` link opens the section in OneNote on the web.</span></span>|
|<span data-ttu-id="69ba9-145">displayName</span><span class="sxs-lookup"><span data-stu-id="69ba9-145">displayName</span></span>|<span data-ttu-id="69ba9-146">String</span><span class="sxs-lookup"><span data-stu-id="69ba9-146">String</span></span>|<span data-ttu-id="69ba9-147">Имя раздела.</span><span class="sxs-lookup"><span data-stu-id="69ba9-147">The name of the section.</span></span> |
|<span data-ttu-id="69ba9-148">pagesUrl</span><span class="sxs-lookup"><span data-stu-id="69ba9-148">pagesUrl</span></span>|<span data-ttu-id="69ba9-149">String</span><span class="sxs-lookup"><span data-stu-id="69ba9-149">String</span></span>|<span data-ttu-id="69ba9-150">Конечная точка, где можно получить сведения `pages` для всех страниц в разделе.</span><span class="sxs-lookup"><span data-stu-id="69ba9-150">The `pages` endpoint where you can get details for all the pages in the section.</span></span> <span data-ttu-id="69ba9-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="69ba9-151">Read-only.</span></span>|
|<span data-ttu-id="69ba9-152">self</span><span class="sxs-lookup"><span data-stu-id="69ba9-152">self</span></span>|<span data-ttu-id="69ba9-153">String</span><span class="sxs-lookup"><span data-stu-id="69ba9-153">String</span></span>|<span data-ttu-id="69ba9-154">Конечная точка, где можно получить сведения о разделе.</span><span class="sxs-lookup"><span data-stu-id="69ba9-154">The endpoint where you can get details about the section.</span></span> <span data-ttu-id="69ba9-155">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="69ba9-155">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="69ba9-156">Связи</span><span class="sxs-lookup"><span data-stu-id="69ba9-156">Relationships</span></span>
| <span data-ttu-id="69ba9-157">Связь</span><span class="sxs-lookup"><span data-stu-id="69ba9-157">Relationship</span></span> | <span data-ttu-id="69ba9-158">Тип</span><span class="sxs-lookup"><span data-stu-id="69ba9-158">Type</span></span>   |<span data-ttu-id="69ba9-159">Описание</span><span class="sxs-lookup"><span data-stu-id="69ba9-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="69ba9-160">pages</span><span class="sxs-lookup"><span data-stu-id="69ba9-160">pages</span></span>|<span data-ttu-id="69ba9-161">[коллекция onenotePage](onenotepage.md)</span><span class="sxs-lookup"><span data-stu-id="69ba9-161">[onenotePage](onenotepage.md) collection</span></span>|<span data-ttu-id="69ba9-162">Коллекция страниц в разделе.</span><span class="sxs-lookup"><span data-stu-id="69ba9-162">The collection of pages in the section.</span></span>  <span data-ttu-id="69ba9-163">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="69ba9-163">Read-only.</span></span> <span data-ttu-id="69ba9-164">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="69ba9-164">Nullable.</span></span>|
|<span data-ttu-id="69ba9-165">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="69ba9-165">parentNotebook</span></span>|[<span data-ttu-id="69ba9-166">notebook</span><span class="sxs-lookup"><span data-stu-id="69ba9-166">notebook</span></span>](notebook.md)|<span data-ttu-id="69ba9-167">Блокнот, содержащий раздел.</span><span class="sxs-lookup"><span data-stu-id="69ba9-167">The notebook that contains the section.</span></span>  <span data-ttu-id="69ba9-168">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="69ba9-168">Read-only.</span></span>|
|<span data-ttu-id="69ba9-169">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="69ba9-169">parentSectionGroup</span></span>|[<span data-ttu-id="69ba9-170">sectionGroup</span><span class="sxs-lookup"><span data-stu-id="69ba9-170">sectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="69ba9-171">Группа разделов, которая содержит раздел.</span><span class="sxs-lookup"><span data-stu-id="69ba9-171">The section group that contains the section.</span></span>  <span data-ttu-id="69ba9-172">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="69ba9-172">Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="69ba9-173">Методы</span><span class="sxs-lookup"><span data-stu-id="69ba9-173">Methods</span></span>

| <span data-ttu-id="69ba9-174">Метод</span><span class="sxs-lookup"><span data-stu-id="69ba9-174">Method</span></span>           | <span data-ttu-id="69ba9-175">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="69ba9-175">Return Type</span></span>    |<span data-ttu-id="69ba9-176">Описание</span><span class="sxs-lookup"><span data-stu-id="69ba9-176">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="69ba9-177">Получение раздела</span><span class="sxs-lookup"><span data-stu-id="69ba9-177">Get section</span></span>](../api/section-get.md) | [<span data-ttu-id="69ba9-178">onenoteSection</span><span class="sxs-lookup"><span data-stu-id="69ba9-178">onenoteSection</span></span>](onenotesection.md) |<span data-ttu-id="69ba9-179">Ознакомьтесь с свойствами и отношениями раздела.</span><span class="sxs-lookup"><span data-stu-id="69ba9-179">Read the properties and relationships of the section.</span></span>|
|[<span data-ttu-id="69ba9-180">Создание страницы</span><span class="sxs-lookup"><span data-stu-id="69ba9-180">Create page</span></span>](../api/section-post-pages.md) |[<span data-ttu-id="69ba9-181">onenotePage</span><span class="sxs-lookup"><span data-stu-id="69ba9-181">onenotePage</span></span>](onenotepage.md)| <span data-ttu-id="69ba9-182">Создайте страницу, выложив ее в коллекцию страниц в указанном разделе.</span><span class="sxs-lookup"><span data-stu-id="69ba9-182">Create a page by posting to the pages collection in the specified section.</span></span>|
|[<span data-ttu-id="69ba9-183">Перечисление страниц</span><span class="sxs-lookup"><span data-stu-id="69ba9-183">List pages</span></span>](../api/section-list-pages.md) |<span data-ttu-id="69ba9-184">[коллекция onenotePage](onenotepage.md)</span><span class="sxs-lookup"><span data-stu-id="69ba9-184">[onenotePage](onenotepage.md) collection</span></span>| <span data-ttu-id="69ba9-185">Получите коллекцию страниц в указанном разделе.</span><span class="sxs-lookup"><span data-stu-id="69ba9-185">Get a collection of pages in the specified section.</span></span>|
|[<span data-ttu-id="69ba9-186">copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="69ba9-186">copyToNotebook</span></span>](../api/section-copytonotebook.md)|<span data-ttu-id="69ba9-187">Нет</span><span class="sxs-lookup"><span data-stu-id="69ba9-187">None</span></span>|<span data-ttu-id="69ba9-188">Скопируйте раздел в определенный блокнот.</span><span class="sxs-lookup"><span data-stu-id="69ba9-188">Copy the section to a specific notebook.</span></span>|
|[<span data-ttu-id="69ba9-189">copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="69ba9-189">copyToSectionGroup</span></span>](../api/section-copytosectiongroup.md)|<span data-ttu-id="69ba9-190">Нет</span><span class="sxs-lookup"><span data-stu-id="69ba9-190">None</span></span>|<span data-ttu-id="69ba9-191">Скопируйте раздел в определенную группу разделов.</span><span class="sxs-lookup"><span data-stu-id="69ba9-191">Copy the section to a specific section group.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="69ba9-192">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="69ba9-192">JSON representation</span></span>

<span data-ttu-id="69ba9-193">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="69ba9-193">Here is a JSON representation of the resource.</span></span>

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


