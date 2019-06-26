---
title: Тип ресурса Page
description: Страница в записной книжке OneNote.
localization_priority: Normal
ms.openlocfilehash: 99807ff781aa3682fd3e310c19208378d457d391
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2019
ms.locfileid: "35236589"
---
# <a name="page-resource-type"></a><span data-ttu-id="2b4b6-103">Тип ресурса Page</span><span class="sxs-lookup"><span data-stu-id="2b4b6-103">page resource type</span></span>

<span data-ttu-id="2b4b6-104">Страница в записной книжке OneNote.</span><span class="sxs-lookup"><span data-stu-id="2b4b6-104">A page in a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2b4b6-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2b4b6-105">JSON representation</span></span>

<span data-ttu-id="2b4b6-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2b4b6-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="2b4b6-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2b4b6-107">Properties</span></span>
| <span data-ttu-id="2b4b6-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="2b4b6-108">Property</span></span>     | <span data-ttu-id="2b4b6-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2b4b6-109">Type</span></span>   |<span data-ttu-id="2b4b6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2b4b6-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2b4b6-111">содержимое</span><span class="sxs-lookup"><span data-stu-id="2b4b6-111">content</span></span>|<span data-ttu-id="2b4b6-112">Поток</span><span class="sxs-lookup"><span data-stu-id="2b4b6-112">Stream</span></span>|<span data-ttu-id="2b4b6-113">HTML-контент страницы.</span><span class="sxs-lookup"><span data-stu-id="2b4b6-113">The page's HTML content.</span></span>|
|<span data-ttu-id="2b4b6-114">contentUrl</span><span class="sxs-lookup"><span data-stu-id="2b4b6-114">contentUrl</span></span>|<span data-ttu-id="2b4b6-115">String</span><span class="sxs-lookup"><span data-stu-id="2b4b6-115">String</span></span>|<span data-ttu-id="2b4b6-116">URL-адрес HTML-содержимого страницы.</span><span class="sxs-lookup"><span data-stu-id="2b4b6-116">The URL for the page's HTML content.</span></span>  <span data-ttu-id="2b4b6-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2b4b6-117">Read-only.</span></span>|
|<span data-ttu-id="2b4b6-118">Креатедбяппид</span><span class="sxs-lookup"><span data-stu-id="2b4b6-118">createdByAppId</span></span>|<span data-ttu-id="2b4b6-119">String</span><span class="sxs-lookup"><span data-stu-id="2b4b6-119">String</span></span>|<span data-ttu-id="2b4b6-120">Уникальный идентификатор приложения, создавшего страницу.</span><span class="sxs-lookup"><span data-stu-id="2b4b6-120">The unique identifier of the application that created the page.</span></span> <span data-ttu-id="2b4b6-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2b4b6-121">Read-only.</span></span>|
|<span data-ttu-id="2b4b6-122">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2b4b6-122">createdDateTime</span></span>|<span data-ttu-id="2b4b6-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b4b6-123">DateTimeOffset</span></span>|<span data-ttu-id="2b4b6-124">Дата и время создания страницы.</span><span class="sxs-lookup"><span data-stu-id="2b4b6-124">The date and time when the page was created.</span></span> <span data-ttu-id="2b4b6-125">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="2b4b6-125">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2b4b6-126">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="2b4b6-126">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="2b4b6-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2b4b6-127">Read-only.</span></span>|
|<span data-ttu-id="2b4b6-128">id</span><span class="sxs-lookup"><span data-stu-id="2b4b6-128">id</span></span>|<span data-ttu-id="2b4b6-129">String</span><span class="sxs-lookup"><span data-stu-id="2b4b6-129">String</span></span>|<span data-ttu-id="2b4b6-130">Уникальный идентификатор страницы.</span><span class="sxs-lookup"><span data-stu-id="2b4b6-130">The unique identifier of the page.</span></span>  <span data-ttu-id="2b4b6-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2b4b6-131">Read-only.</span></span>|
|<span data-ttu-id="2b4b6-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2b4b6-132">lastModifiedDateTime</span></span>|<span data-ttu-id="2b4b6-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b4b6-133">DateTimeOffset</span></span>|<span data-ttu-id="2b4b6-134">Дата и время последнего изменения страницы.</span><span class="sxs-lookup"><span data-stu-id="2b4b6-134">The date and time when the page was last modified.</span></span> <span data-ttu-id="2b4b6-135">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="2b4b6-135">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2b4b6-136">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="2b4b6-136">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="2b4b6-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2b4b6-137">Read-only.</span></span>|
|<span data-ttu-id="2b4b6-138">level</span><span class="sxs-lookup"><span data-stu-id="2b4b6-138">level</span></span>|<span data-ttu-id="2b4b6-139">Int32</span><span class="sxs-lookup"><span data-stu-id="2b4b6-139">Int32</span></span>|<span data-ttu-id="2b4b6-140">Уровень отступа страницы.</span><span class="sxs-lookup"><span data-stu-id="2b4b6-140">The indentation level of the page.</span></span> <span data-ttu-id="2b4b6-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2b4b6-141">Read-only.</span></span>|
|<span data-ttu-id="2b4b6-142">links</span><span class="sxs-lookup"><span data-stu-id="2b4b6-142">links</span></span>|[<span data-ttu-id="2b4b6-143">Пажелинкс</span><span class="sxs-lookup"><span data-stu-id="2b4b6-143">PageLinks</span></span>](pagelinks.md)|<span data-ttu-id="2b4b6-144">Ссылки для открытия страницы.</span><span class="sxs-lookup"><span data-stu-id="2b4b6-144">Links for opening the page.</span></span> <span data-ttu-id="2b4b6-145">`oneNoteClientURL` Ссылка открывает страницу в собственном клиенте OneNote, если она установлена.</span><span class="sxs-lookup"><span data-stu-id="2b4b6-145">The `oneNoteClientURL` link opens the page in the OneNote native client if it 's installed.</span></span> <span data-ttu-id="2b4b6-146">`oneNoteWebUrl` Ссылка открывает страницу в OneNote в Интернете.</span><span class="sxs-lookup"><span data-stu-id="2b4b6-146">The `oneNoteWebUrl` link opens the page in OneNote on the web.</span></span> <span data-ttu-id="2b4b6-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2b4b6-147">Read-only.</span></span>|
|<span data-ttu-id="2b4b6-148">порядке</span><span class="sxs-lookup"><span data-stu-id="2b4b6-148">order</span></span>|<span data-ttu-id="2b4b6-149">Int32</span><span class="sxs-lookup"><span data-stu-id="2b4b6-149">Int32</span></span>|<span data-ttu-id="2b4b6-150">Порядок страницы в родительском разделе.</span><span class="sxs-lookup"><span data-stu-id="2b4b6-150">The order of the page within its parent section.</span></span> <span data-ttu-id="2b4b6-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2b4b6-151">Read-only.</span></span>|
|<span data-ttu-id="2b4b6-152">Self</span><span class="sxs-lookup"><span data-stu-id="2b4b6-152">self</span></span>|<span data-ttu-id="2b4b6-153">String</span><span class="sxs-lookup"><span data-stu-id="2b4b6-153">String</span></span>|<span data-ttu-id="2b4b6-154">Конечная точка, в которой можно получить сведения о странице.</span><span class="sxs-lookup"><span data-stu-id="2b4b6-154">The endpoint where you can get details about the page.</span></span> <span data-ttu-id="2b4b6-155">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2b4b6-155">Read-only.</span></span>|
|<span data-ttu-id="2b4b6-156">title</span><span class="sxs-lookup"><span data-stu-id="2b4b6-156">title</span></span>|<span data-ttu-id="2b4b6-157">String</span><span class="sxs-lookup"><span data-stu-id="2b4b6-157">String</span></span>|<span data-ttu-id="2b4b6-158">Заголовок страницы.</span><span class="sxs-lookup"><span data-stu-id="2b4b6-158">The title of the page.</span></span> |

## <a name="relationships"></a><span data-ttu-id="2b4b6-159">Отношения</span><span class="sxs-lookup"><span data-stu-id="2b4b6-159">Relationships</span></span>
| <span data-ttu-id="2b4b6-160">Отношение</span><span class="sxs-lookup"><span data-stu-id="2b4b6-160">Relationship</span></span> | <span data-ttu-id="2b4b6-161">Тип</span><span class="sxs-lookup"><span data-stu-id="2b4b6-161">Type</span></span>   |<span data-ttu-id="2b4b6-162">Описание</span><span class="sxs-lookup"><span data-stu-id="2b4b6-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2b4b6-163">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="2b4b6-163">parentNotebook</span></span>|[<span data-ttu-id="2b4b6-164">Notebook</span><span class="sxs-lookup"><span data-stu-id="2b4b6-164">Notebook</span></span>](notebook.md)|<span data-ttu-id="2b4b6-165">Записная книжка, содержащая страницу.</span><span class="sxs-lookup"><span data-stu-id="2b4b6-165">The notebook that contains the page.</span></span>  <span data-ttu-id="2b4b6-166">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2b4b6-166">Read-only.</span></span>|
|<span data-ttu-id="2b4b6-167">parentSection</span><span class="sxs-lookup"><span data-stu-id="2b4b6-167">parentSection</span></span>|[<span data-ttu-id="2b4b6-168">Оненотесектион</span><span class="sxs-lookup"><span data-stu-id="2b4b6-168">OnenoteSection</span></span>](section.md)|<span data-ttu-id="2b4b6-169">Раздел, содержащий страницу.</span><span class="sxs-lookup"><span data-stu-id="2b4b6-169">The section that contains the page.</span></span> <span data-ttu-id="2b4b6-170">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2b4b6-170">Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="2b4b6-171">Методы</span><span class="sxs-lookup"><span data-stu-id="2b4b6-171">Methods</span></span>

| <span data-ttu-id="2b4b6-172">Метод</span><span class="sxs-lookup"><span data-stu-id="2b4b6-172">Method</span></span>           | <span data-ttu-id="2b4b6-173">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2b4b6-173">Return Type</span></span>    |<span data-ttu-id="2b4b6-174">Описание</span><span class="sxs-lookup"><span data-stu-id="2b4b6-174">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2b4b6-175">Вывод страницы</span><span class="sxs-lookup"><span data-stu-id="2b4b6-175">Get page</span></span>](../api/page-get.md) | [<span data-ttu-id="2b4b6-176">Page</span><span class="sxs-lookup"><span data-stu-id="2b4b6-176">Page</span></span>](page.md) |<span data-ttu-id="2b4b6-177">Чтение свойств и связей страницы.</span><span class="sxs-lookup"><span data-stu-id="2b4b6-177">Read the properties and relationships of the page.</span></span>|
|[<span data-ttu-id="2b4b6-178">Обновление содержимого страницы</span><span class="sxs-lookup"><span data-stu-id="2b4b6-178">Update page content</span></span>](../api/page-update.md) | <span data-ttu-id="2b4b6-179">Нет</span><span class="sxs-lookup"><span data-stu-id="2b4b6-179">None</span></span> |<span data-ttu-id="2b4b6-180">Обновление HTML-содержимого страницы.</span><span class="sxs-lookup"><span data-stu-id="2b4b6-180">Update the HTML content of the page.</span></span> |
|[<span data-ttu-id="2b4b6-181">Удаление страницы</span><span class="sxs-lookup"><span data-stu-id="2b4b6-181">Delete page</span></span>](../api/page-delete.md) | <span data-ttu-id="2b4b6-182">Нет</span><span class="sxs-lookup"><span data-stu-id="2b4b6-182">None</span></span> |<span data-ttu-id="2b4b6-183">Удаление страницы.</span><span class="sxs-lookup"><span data-stu-id="2b4b6-183">Delete the page.</span></span> |
|[<span data-ttu-id="2b4b6-184">copyToSection</span><span class="sxs-lookup"><span data-stu-id="2b4b6-184">copyToSection</span></span>](../api/page-copytosection.md)| <span data-ttu-id="2b4b6-185">Нет</span><span class="sxs-lookup"><span data-stu-id="2b4b6-185">None</span></span> |<span data-ttu-id="2b4b6-186">Копирует страницу в определенный раздел.</span><span class="sxs-lookup"><span data-stu-id="2b4b6-186">Copies the page to a specific section.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
