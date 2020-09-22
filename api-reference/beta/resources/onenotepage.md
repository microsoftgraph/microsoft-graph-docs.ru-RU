---
title: Тип ресурса Оненотепаже
description: Страница в записной книжке OneNote.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: jewan-microsoft
ms.openlocfilehash: 463ac02029753fcc99392fbc3db464989f5ae01a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971545"
---
# <a name="onenotepage-resource-type"></a><span data-ttu-id="fcc88-103">Тип ресурса Оненотепаже</span><span class="sxs-lookup"><span data-stu-id="fcc88-103">onenotePage resource type</span></span>

<span data-ttu-id="fcc88-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fcc88-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fcc88-105">Страница в записной книжке OneNote.</span><span class="sxs-lookup"><span data-stu-id="fcc88-105">A page in a OneNote notebook.</span></span>

## <a name="properties"></a><span data-ttu-id="fcc88-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="fcc88-106">Properties</span></span>
| <span data-ttu-id="fcc88-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="fcc88-107">Property</span></span>     | <span data-ttu-id="fcc88-108">Тип</span><span class="sxs-lookup"><span data-stu-id="fcc88-108">Type</span></span>   |<span data-ttu-id="fcc88-109">Описание</span><span class="sxs-lookup"><span data-stu-id="fcc88-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fcc88-110">содержимое</span><span class="sxs-lookup"><span data-stu-id="fcc88-110">content</span></span>|<span data-ttu-id="fcc88-111">Поток</span><span class="sxs-lookup"><span data-stu-id="fcc88-111">Stream</span></span>|<span data-ttu-id="fcc88-112">HTML-контент страницы.</span><span class="sxs-lookup"><span data-stu-id="fcc88-112">The page's HTML content.</span></span>|
|<span data-ttu-id="fcc88-113">contentUrl</span><span class="sxs-lookup"><span data-stu-id="fcc88-113">contentUrl</span></span>|<span data-ttu-id="fcc88-114">String</span><span class="sxs-lookup"><span data-stu-id="fcc88-114">String</span></span>|<span data-ttu-id="fcc88-115">URL-адрес HTML-содержимого страницы.</span><span class="sxs-lookup"><span data-stu-id="fcc88-115">The URL for the page's HTML content.</span></span>  <span data-ttu-id="fcc88-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fcc88-116">Read-only.</span></span>|
|<span data-ttu-id="fcc88-117">createdByAppId</span><span class="sxs-lookup"><span data-stu-id="fcc88-117">createdByAppId</span></span>|<span data-ttu-id="fcc88-118">String</span><span class="sxs-lookup"><span data-stu-id="fcc88-118">String</span></span>|<span data-ttu-id="fcc88-119">Уникальный идентификатор приложения, создавшего страницу.</span><span class="sxs-lookup"><span data-stu-id="fcc88-119">The unique identifier of the application that created the page.</span></span> <span data-ttu-id="fcc88-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fcc88-120">Read-only.</span></span>|
|<span data-ttu-id="fcc88-121">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fcc88-121">createdDateTime</span></span>|<span data-ttu-id="fcc88-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fcc88-122">DateTimeOffset</span></span>|<span data-ttu-id="fcc88-123">Дата и время создания страницы.</span><span class="sxs-lookup"><span data-stu-id="fcc88-123">The date and time when the page was created.</span></span> <span data-ttu-id="fcc88-124">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="fcc88-124">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fcc88-125">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="fcc88-125">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="fcc88-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fcc88-126">Read-only.</span></span>|
|<span data-ttu-id="fcc88-127">id</span><span class="sxs-lookup"><span data-stu-id="fcc88-127">id</span></span>|<span data-ttu-id="fcc88-128">String</span><span class="sxs-lookup"><span data-stu-id="fcc88-128">String</span></span>|<span data-ttu-id="fcc88-129">Уникальный идентификатор страницы.</span><span class="sxs-lookup"><span data-stu-id="fcc88-129">The unique identifier of the page.</span></span>  <span data-ttu-id="fcc88-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fcc88-130">Read-only.</span></span>|
|<span data-ttu-id="fcc88-131">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fcc88-131">lastModifiedDateTime</span></span>|<span data-ttu-id="fcc88-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fcc88-132">DateTimeOffset</span></span>|<span data-ttu-id="fcc88-133">Дата и время последнего изменения страницы.</span><span class="sxs-lookup"><span data-stu-id="fcc88-133">The date and time when the page was last modified.</span></span> <span data-ttu-id="fcc88-134">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="fcc88-134">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fcc88-135">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="fcc88-135">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="fcc88-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fcc88-136">Read-only.</span></span>|
|<span data-ttu-id="fcc88-137">степень</span><span class="sxs-lookup"><span data-stu-id="fcc88-137">level</span></span>|<span data-ttu-id="fcc88-138">Int32</span><span class="sxs-lookup"><span data-stu-id="fcc88-138">Int32</span></span>|<span data-ttu-id="fcc88-139">Уровень отступа страницы.</span><span class="sxs-lookup"><span data-stu-id="fcc88-139">The indentation level of the page.</span></span> <span data-ttu-id="fcc88-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fcc88-140">Read-only.</span></span>|
|<span data-ttu-id="fcc88-141">links</span><span class="sxs-lookup"><span data-stu-id="fcc88-141">links</span></span>|[<span data-ttu-id="fcc88-142">пажелинкс</span><span class="sxs-lookup"><span data-stu-id="fcc88-142">pageLinks</span></span>](pagelinks.md)|<span data-ttu-id="fcc88-143">Ссылки для открытия страницы.</span><span class="sxs-lookup"><span data-stu-id="fcc88-143">Links for opening the page.</span></span> <span data-ttu-id="fcc88-144">`oneNoteClientURL`Ссылка открывает страницу в собственном клиенте OneNote, если она установлена.</span><span class="sxs-lookup"><span data-stu-id="fcc88-144">The `oneNoteClientURL` link opens the page in the OneNote native client if it 's installed.</span></span> <span data-ttu-id="fcc88-145">`oneNoteWebUrl`Ссылка открывает страницу в OneNote в Интернете.</span><span class="sxs-lookup"><span data-stu-id="fcc88-145">The `oneNoteWebUrl` link opens the page in OneNote on the web.</span></span> <span data-ttu-id="fcc88-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fcc88-146">Read-only.</span></span>|
|<span data-ttu-id="fcc88-147">порядке</span><span class="sxs-lookup"><span data-stu-id="fcc88-147">order</span></span>|<span data-ttu-id="fcc88-148">Int32</span><span class="sxs-lookup"><span data-stu-id="fcc88-148">Int32</span></span>|<span data-ttu-id="fcc88-149">Порядок страницы в родительском разделе.</span><span class="sxs-lookup"><span data-stu-id="fcc88-149">The order of the page within its parent section.</span></span> <span data-ttu-id="fcc88-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fcc88-150">Read-only.</span></span>|
|<span data-ttu-id="fcc88-151">Self</span><span class="sxs-lookup"><span data-stu-id="fcc88-151">self</span></span>|<span data-ttu-id="fcc88-152">String</span><span class="sxs-lookup"><span data-stu-id="fcc88-152">String</span></span>|<span data-ttu-id="fcc88-153">Конечная точка, в которой можно получить сведения о странице.</span><span class="sxs-lookup"><span data-stu-id="fcc88-153">The endpoint where you can get details about the page.</span></span> <span data-ttu-id="fcc88-154">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fcc88-154">Read-only.</span></span>|
|<span data-ttu-id="fcc88-155">title</span><span class="sxs-lookup"><span data-stu-id="fcc88-155">title</span></span>|<span data-ttu-id="fcc88-156">String</span><span class="sxs-lookup"><span data-stu-id="fcc88-156">String</span></span>|<span data-ttu-id="fcc88-157">Заголовок страницы.</span><span class="sxs-lookup"><span data-stu-id="fcc88-157">The title of the page.</span></span> |

## <a name="relationships"></a><span data-ttu-id="fcc88-158">Связи</span><span class="sxs-lookup"><span data-stu-id="fcc88-158">Relationships</span></span>
| <span data-ttu-id="fcc88-159">Связь</span><span class="sxs-lookup"><span data-stu-id="fcc88-159">Relationship</span></span> | <span data-ttu-id="fcc88-160">Тип</span><span class="sxs-lookup"><span data-stu-id="fcc88-160">Type</span></span>   |<span data-ttu-id="fcc88-161">Описание</span><span class="sxs-lookup"><span data-stu-id="fcc88-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fcc88-162">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="fcc88-162">parentNotebook</span></span>|[<span data-ttu-id="fcc88-163">notebook</span><span class="sxs-lookup"><span data-stu-id="fcc88-163">notebook</span></span>](notebook.md)|<span data-ttu-id="fcc88-164">Записная книжка, содержащая страницу.</span><span class="sxs-lookup"><span data-stu-id="fcc88-164">The notebook that contains the page.</span></span>  <span data-ttu-id="fcc88-165">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fcc88-165">Read-only.</span></span>|
|<span data-ttu-id="fcc88-166">parentSection</span><span class="sxs-lookup"><span data-stu-id="fcc88-166">parentSection</span></span>|[<span data-ttu-id="fcc88-167">оненотесектион</span><span class="sxs-lookup"><span data-stu-id="fcc88-167">onenoteSection</span></span>](onenotesection.md)|<span data-ttu-id="fcc88-168">Раздел, содержащий страницу.</span><span class="sxs-lookup"><span data-stu-id="fcc88-168">The section that contains the page.</span></span> <span data-ttu-id="fcc88-169">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fcc88-169">Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="fcc88-170">Методы</span><span class="sxs-lookup"><span data-stu-id="fcc88-170">Methods</span></span>

| <span data-ttu-id="fcc88-171">Метод</span><span class="sxs-lookup"><span data-stu-id="fcc88-171">Method</span></span>           | <span data-ttu-id="fcc88-172">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="fcc88-172">Return Type</span></span>    |<span data-ttu-id="fcc88-173">Описание</span><span class="sxs-lookup"><span data-stu-id="fcc88-173">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fcc88-174">Вывод страницы</span><span class="sxs-lookup"><span data-stu-id="fcc88-174">Get page</span></span>](../api/page-get.md) | [<span data-ttu-id="fcc88-175">оненотепаже</span><span class="sxs-lookup"><span data-stu-id="fcc88-175">onenotePage</span></span>](onenotepage.md) |<span data-ttu-id="fcc88-176">Чтение свойств и связей страницы.</span><span class="sxs-lookup"><span data-stu-id="fcc88-176">Read the properties and relationships of the page.</span></span>|
|[<span data-ttu-id="fcc88-177">Обновление содержимого страницы</span><span class="sxs-lookup"><span data-stu-id="fcc88-177">Update page content</span></span>](../api/page-update.md) | <span data-ttu-id="fcc88-178">Нет</span><span class="sxs-lookup"><span data-stu-id="fcc88-178">None</span></span> |<span data-ttu-id="fcc88-179">Обновление HTML-содержимого страницы.</span><span class="sxs-lookup"><span data-stu-id="fcc88-179">Update the HTML content of the page.</span></span> |
|[<span data-ttu-id="fcc88-180">Удаление страницы</span><span class="sxs-lookup"><span data-stu-id="fcc88-180">Delete page</span></span>](../api/page-delete.md) | <span data-ttu-id="fcc88-181">Нет</span><span class="sxs-lookup"><span data-stu-id="fcc88-181">None</span></span> |<span data-ttu-id="fcc88-182">Удаление страницы.</span><span class="sxs-lookup"><span data-stu-id="fcc88-182">Delete the page.</span></span> |
|[<span data-ttu-id="fcc88-183">copyToSection</span><span class="sxs-lookup"><span data-stu-id="fcc88-183">copyToSection</span></span>](../api/page-copytosection.md)| <span data-ttu-id="fcc88-184">Нет</span><span class="sxs-lookup"><span data-stu-id="fcc88-184">None</span></span> |<span data-ttu-id="fcc88-185">Копирует страницу в определенный раздел.</span><span class="sxs-lookup"><span data-stu-id="fcc88-185">Copies the page to a specific section.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fcc88-186">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fcc88-186">JSON representation</span></span>

<span data-ttu-id="fcc88-187">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fcc88-187">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "parentNotebook",
    "parentSection"
  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.onenotePage"
}-->

```json
{
  "content": "stream",
  "contentUrl": "string",
  "createdByAppId": "string",
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "level": 1024,
  "links": {"@odata.type": "microsoft.graph.pageLinks"},
  "order": 1024,
  "self": "string",
  "title": "string"
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


