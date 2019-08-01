---
title: Тип ресурса Page
description: Страница в записной книжке OneNote.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 4a8ff5f6d0d9ed435d51d005df21a73bcb25a930
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035639"
---
# <a name="page-resource-type"></a><span data-ttu-id="30daf-103">Тип ресурса Page</span><span class="sxs-lookup"><span data-stu-id="30daf-103">page resource type</span></span>

<span data-ttu-id="30daf-104">Страница в записной книжке OneNote.</span><span class="sxs-lookup"><span data-stu-id="30daf-104">A page in a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="30daf-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="30daf-105">JSON representation</span></span>

<span data-ttu-id="30daf-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="30daf-106">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.onenoteEntitySchemaObjectModel",
  "optionalProperties": [
    "parentNotebook",
    "parentSection"
  ],
  "isMediaEntity": true,
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
## <a name="properties"></a><span data-ttu-id="30daf-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="30daf-107">Properties</span></span>
| <span data-ttu-id="30daf-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="30daf-108">Property</span></span>     | <span data-ttu-id="30daf-109">Тип</span><span class="sxs-lookup"><span data-stu-id="30daf-109">Type</span></span>   |<span data-ttu-id="30daf-110">Описание</span><span class="sxs-lookup"><span data-stu-id="30daf-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="30daf-111">содержимое</span><span class="sxs-lookup"><span data-stu-id="30daf-111">content</span></span>|<span data-ttu-id="30daf-112">Поток</span><span class="sxs-lookup"><span data-stu-id="30daf-112">Stream</span></span>|<span data-ttu-id="30daf-113">HTML-контент страницы.</span><span class="sxs-lookup"><span data-stu-id="30daf-113">The page's HTML content.</span></span>|
|<span data-ttu-id="30daf-114">contentUrl</span><span class="sxs-lookup"><span data-stu-id="30daf-114">contentUrl</span></span>|<span data-ttu-id="30daf-115">String</span><span class="sxs-lookup"><span data-stu-id="30daf-115">String</span></span>|<span data-ttu-id="30daf-116">URL-адрес HTML-содержимого страницы.</span><span class="sxs-lookup"><span data-stu-id="30daf-116">The URL for the page's HTML content.</span></span>  <span data-ttu-id="30daf-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="30daf-117">Read-only.</span></span>|
|<span data-ttu-id="30daf-118">Креатедбяппид</span><span class="sxs-lookup"><span data-stu-id="30daf-118">createdByAppId</span></span>|<span data-ttu-id="30daf-119">String</span><span class="sxs-lookup"><span data-stu-id="30daf-119">String</span></span>|<span data-ttu-id="30daf-120">Уникальный идентификатор приложения, создавшего страницу.</span><span class="sxs-lookup"><span data-stu-id="30daf-120">The unique identifier of the application that created the page.</span></span> <span data-ttu-id="30daf-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="30daf-121">Read-only.</span></span>|
|<span data-ttu-id="30daf-122">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="30daf-122">createdDateTime</span></span>|<span data-ttu-id="30daf-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30daf-123">DateTimeOffset</span></span>|<span data-ttu-id="30daf-124">Дата и время создания страницы.</span><span class="sxs-lookup"><span data-stu-id="30daf-124">The date and time when the page was created.</span></span> <span data-ttu-id="30daf-125">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="30daf-125">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="30daf-126">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="30daf-126">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="30daf-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="30daf-127">Read-only.</span></span>|
|<span data-ttu-id="30daf-128">id</span><span class="sxs-lookup"><span data-stu-id="30daf-128">id</span></span>|<span data-ttu-id="30daf-129">String</span><span class="sxs-lookup"><span data-stu-id="30daf-129">String</span></span>|<span data-ttu-id="30daf-130">Уникальный идентификатор страницы.</span><span class="sxs-lookup"><span data-stu-id="30daf-130">The unique identifier of the page.</span></span>  <span data-ttu-id="30daf-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="30daf-131">Read-only.</span></span>|
|<span data-ttu-id="30daf-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="30daf-132">lastModifiedDateTime</span></span>|<span data-ttu-id="30daf-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30daf-133">DateTimeOffset</span></span>|<span data-ttu-id="30daf-134">Дата и время последнего изменения страницы.</span><span class="sxs-lookup"><span data-stu-id="30daf-134">The date and time when the page was last modified.</span></span> <span data-ttu-id="30daf-135">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="30daf-135">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="30daf-136">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="30daf-136">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="30daf-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="30daf-137">Read-only.</span></span>|
|<span data-ttu-id="30daf-138">level</span><span class="sxs-lookup"><span data-stu-id="30daf-138">level</span></span>|<span data-ttu-id="30daf-139">Int32</span><span class="sxs-lookup"><span data-stu-id="30daf-139">Int32</span></span>|<span data-ttu-id="30daf-140">Уровень отступа страницы.</span><span class="sxs-lookup"><span data-stu-id="30daf-140">The indentation level of the page.</span></span> <span data-ttu-id="30daf-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="30daf-141">Read-only.</span></span>|
|<span data-ttu-id="30daf-142">links</span><span class="sxs-lookup"><span data-stu-id="30daf-142">links</span></span>|[<span data-ttu-id="30daf-143">Пажелинкс</span><span class="sxs-lookup"><span data-stu-id="30daf-143">PageLinks</span></span>](pagelinks.md)|<span data-ttu-id="30daf-144">Ссылки для открытия страницы.</span><span class="sxs-lookup"><span data-stu-id="30daf-144">Links for opening the page.</span></span> <span data-ttu-id="30daf-145">`oneNoteClientURL` Ссылка открывает страницу в собственном клиенте OneNote, если она установлена.</span><span class="sxs-lookup"><span data-stu-id="30daf-145">The `oneNoteClientURL` link opens the page in the OneNote native client if it 's installed.</span></span> <span data-ttu-id="30daf-146">`oneNoteWebUrl` Ссылка открывает страницу в OneNote в Интернете.</span><span class="sxs-lookup"><span data-stu-id="30daf-146">The `oneNoteWebUrl` link opens the page in OneNote on the web.</span></span> <span data-ttu-id="30daf-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="30daf-147">Read-only.</span></span>|
|<span data-ttu-id="30daf-148">порядке</span><span class="sxs-lookup"><span data-stu-id="30daf-148">order</span></span>|<span data-ttu-id="30daf-149">Int32</span><span class="sxs-lookup"><span data-stu-id="30daf-149">Int32</span></span>|<span data-ttu-id="30daf-150">Порядок страницы в родительском разделе.</span><span class="sxs-lookup"><span data-stu-id="30daf-150">The order of the page within its parent section.</span></span> <span data-ttu-id="30daf-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="30daf-151">Read-only.</span></span>|
|<span data-ttu-id="30daf-152">Self</span><span class="sxs-lookup"><span data-stu-id="30daf-152">self</span></span>|<span data-ttu-id="30daf-153">String</span><span class="sxs-lookup"><span data-stu-id="30daf-153">String</span></span>|<span data-ttu-id="30daf-154">Конечная точка, в которой можно получить сведения о странице.</span><span class="sxs-lookup"><span data-stu-id="30daf-154">The endpoint where you can get details about the page.</span></span> <span data-ttu-id="30daf-155">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="30daf-155">Read-only.</span></span>|
|<span data-ttu-id="30daf-156">title</span><span class="sxs-lookup"><span data-stu-id="30daf-156">title</span></span>|<span data-ttu-id="30daf-157">String</span><span class="sxs-lookup"><span data-stu-id="30daf-157">String</span></span>|<span data-ttu-id="30daf-158">Заголовок страницы.</span><span class="sxs-lookup"><span data-stu-id="30daf-158">The title of the page.</span></span> |

## <a name="relationships"></a><span data-ttu-id="30daf-159">Отношения</span><span class="sxs-lookup"><span data-stu-id="30daf-159">Relationships</span></span>
| <span data-ttu-id="30daf-160">Отношение</span><span class="sxs-lookup"><span data-stu-id="30daf-160">Relationship</span></span> | <span data-ttu-id="30daf-161">Тип</span><span class="sxs-lookup"><span data-stu-id="30daf-161">Type</span></span>   |<span data-ttu-id="30daf-162">Описание</span><span class="sxs-lookup"><span data-stu-id="30daf-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="30daf-163">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="30daf-163">parentNotebook</span></span>|[<span data-ttu-id="30daf-164">Notebook</span><span class="sxs-lookup"><span data-stu-id="30daf-164">Notebook</span></span>](notebook.md)|<span data-ttu-id="30daf-165">Записная книжка, содержащая страницу.</span><span class="sxs-lookup"><span data-stu-id="30daf-165">The notebook that contains the page.</span></span>  <span data-ttu-id="30daf-166">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="30daf-166">Read-only.</span></span>|
|<span data-ttu-id="30daf-167">parentSection</span><span class="sxs-lookup"><span data-stu-id="30daf-167">parentSection</span></span>|[<span data-ttu-id="30daf-168">Оненотесектион</span><span class="sxs-lookup"><span data-stu-id="30daf-168">OnenoteSection</span></span>](section.md)|<span data-ttu-id="30daf-169">Раздел, содержащий страницу.</span><span class="sxs-lookup"><span data-stu-id="30daf-169">The section that contains the page.</span></span> <span data-ttu-id="30daf-170">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="30daf-170">Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="30daf-171">Методы</span><span class="sxs-lookup"><span data-stu-id="30daf-171">Methods</span></span>

| <span data-ttu-id="30daf-172">Метод</span><span class="sxs-lookup"><span data-stu-id="30daf-172">Method</span></span>           | <span data-ttu-id="30daf-173">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="30daf-173">Return Type</span></span>    |<span data-ttu-id="30daf-174">Описание</span><span class="sxs-lookup"><span data-stu-id="30daf-174">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="30daf-175">Вывод страницы</span><span class="sxs-lookup"><span data-stu-id="30daf-175">Get page</span></span>](../api/page-get.md) | [<span data-ttu-id="30daf-176">Page</span><span class="sxs-lookup"><span data-stu-id="30daf-176">Page</span></span>](page.md) |<span data-ttu-id="30daf-177">Чтение свойств и связей страницы.</span><span class="sxs-lookup"><span data-stu-id="30daf-177">Read the properties and relationships of the page.</span></span>|
|[<span data-ttu-id="30daf-178">Обновление содержимого страницы</span><span class="sxs-lookup"><span data-stu-id="30daf-178">Update page content</span></span>](../api/page-update.md) | <span data-ttu-id="30daf-179">Нет</span><span class="sxs-lookup"><span data-stu-id="30daf-179">None</span></span> |<span data-ttu-id="30daf-180">Обновление HTML-содержимого страницы.</span><span class="sxs-lookup"><span data-stu-id="30daf-180">Update the HTML content of the page.</span></span> |
|[<span data-ttu-id="30daf-181">Удаление страницы</span><span class="sxs-lookup"><span data-stu-id="30daf-181">Delete page</span></span>](../api/page-delete.md) | <span data-ttu-id="30daf-182">Нет</span><span class="sxs-lookup"><span data-stu-id="30daf-182">None</span></span> |<span data-ttu-id="30daf-183">Удаление страницы.</span><span class="sxs-lookup"><span data-stu-id="30daf-183">Delete the page.</span></span> |
|[<span data-ttu-id="30daf-184">copyToSection</span><span class="sxs-lookup"><span data-stu-id="30daf-184">copyToSection</span></span>](../api/page-copytosection.md)| <span data-ttu-id="30daf-185">Нет</span><span class="sxs-lookup"><span data-stu-id="30daf-185">None</span></span> |<span data-ttu-id="30daf-186">Копирует страницу в определенный раздел.</span><span class="sxs-lookup"><span data-stu-id="30daf-186">Copies the page to a specific section.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
