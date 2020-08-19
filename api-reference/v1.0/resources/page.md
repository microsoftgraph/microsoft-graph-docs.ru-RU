---
title: Тип ресурса Page
description: Страница в записной книжке OneNote.
localization_priority: Normal
author: jewan-microsoft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 33fbbb150908bf5b3c472cf02b971da60f1aa014
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811933"
---
# <a name="page-resource-type"></a><span data-ttu-id="cdf6f-103">Тип ресурса Page</span><span class="sxs-lookup"><span data-stu-id="cdf6f-103">page resource type</span></span>

<span data-ttu-id="cdf6f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cdf6f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cdf6f-105">Страница в записной книжке OneNote.</span><span class="sxs-lookup"><span data-stu-id="cdf6f-105">A page in a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cdf6f-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="cdf6f-106">JSON representation</span></span>

<span data-ttu-id="cdf6f-107">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cdf6f-107">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="cdf6f-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="cdf6f-108">Properties</span></span>
| <span data-ttu-id="cdf6f-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="cdf6f-109">Property</span></span>     | <span data-ttu-id="cdf6f-110">Тип</span><span class="sxs-lookup"><span data-stu-id="cdf6f-110">Type</span></span>   |<span data-ttu-id="cdf6f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="cdf6f-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cdf6f-112">содержимое</span><span class="sxs-lookup"><span data-stu-id="cdf6f-112">content</span></span>|<span data-ttu-id="cdf6f-113">Поток</span><span class="sxs-lookup"><span data-stu-id="cdf6f-113">Stream</span></span>|<span data-ttu-id="cdf6f-114">HTML-контент страницы.</span><span class="sxs-lookup"><span data-stu-id="cdf6f-114">The page's HTML content.</span></span>|
|<span data-ttu-id="cdf6f-115">contentUrl</span><span class="sxs-lookup"><span data-stu-id="cdf6f-115">contentUrl</span></span>|<span data-ttu-id="cdf6f-116">String</span><span class="sxs-lookup"><span data-stu-id="cdf6f-116">String</span></span>|<span data-ttu-id="cdf6f-117">URL-адрес HTML-содержимого страницы.</span><span class="sxs-lookup"><span data-stu-id="cdf6f-117">The URL for the page's HTML content.</span></span>  <span data-ttu-id="cdf6f-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cdf6f-118">Read-only.</span></span>|
|<span data-ttu-id="cdf6f-119">createdByAppId</span><span class="sxs-lookup"><span data-stu-id="cdf6f-119">createdByAppId</span></span>|<span data-ttu-id="cdf6f-120">String</span><span class="sxs-lookup"><span data-stu-id="cdf6f-120">String</span></span>|<span data-ttu-id="cdf6f-121">Уникальный идентификатор приложения, создавшего страницу.</span><span class="sxs-lookup"><span data-stu-id="cdf6f-121">The unique identifier of the application that created the page.</span></span> <span data-ttu-id="cdf6f-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cdf6f-122">Read-only.</span></span>|
|<span data-ttu-id="cdf6f-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cdf6f-123">createdDateTime</span></span>|<span data-ttu-id="cdf6f-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cdf6f-124">DateTimeOffset</span></span>|<span data-ttu-id="cdf6f-125">Дата и время создания страницы.</span><span class="sxs-lookup"><span data-stu-id="cdf6f-125">The date and time when the page was created.</span></span> <span data-ttu-id="cdf6f-126">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="cdf6f-126">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="cdf6f-127">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="cdf6f-127">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="cdf6f-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cdf6f-128">Read-only.</span></span>|
|<span data-ttu-id="cdf6f-129">id</span><span class="sxs-lookup"><span data-stu-id="cdf6f-129">id</span></span>|<span data-ttu-id="cdf6f-130">String</span><span class="sxs-lookup"><span data-stu-id="cdf6f-130">String</span></span>|<span data-ttu-id="cdf6f-131">Уникальный идентификатор страницы.</span><span class="sxs-lookup"><span data-stu-id="cdf6f-131">The unique identifier of the page.</span></span>  <span data-ttu-id="cdf6f-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cdf6f-132">Read-only.</span></span>|
|<span data-ttu-id="cdf6f-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cdf6f-133">lastModifiedDateTime</span></span>|<span data-ttu-id="cdf6f-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cdf6f-134">DateTimeOffset</span></span>|<span data-ttu-id="cdf6f-135">Дата и время последнего изменения страницы.</span><span class="sxs-lookup"><span data-stu-id="cdf6f-135">The date and time when the page was last modified.</span></span> <span data-ttu-id="cdf6f-136">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="cdf6f-136">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="cdf6f-137">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="cdf6f-137">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="cdf6f-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cdf6f-138">Read-only.</span></span>|
|<span data-ttu-id="cdf6f-139">степень</span><span class="sxs-lookup"><span data-stu-id="cdf6f-139">level</span></span>|<span data-ttu-id="cdf6f-140">Int32</span><span class="sxs-lookup"><span data-stu-id="cdf6f-140">Int32</span></span>|<span data-ttu-id="cdf6f-141">Уровень отступа страницы.</span><span class="sxs-lookup"><span data-stu-id="cdf6f-141">The indentation level of the page.</span></span> <span data-ttu-id="cdf6f-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cdf6f-142">Read-only.</span></span>|
|<span data-ttu-id="cdf6f-143">links</span><span class="sxs-lookup"><span data-stu-id="cdf6f-143">links</span></span>|[<span data-ttu-id="cdf6f-144">пажелинкс</span><span class="sxs-lookup"><span data-stu-id="cdf6f-144">PageLinks</span></span>](pagelinks.md)|<span data-ttu-id="cdf6f-145">Ссылки для открытия страницы.</span><span class="sxs-lookup"><span data-stu-id="cdf6f-145">Links for opening the page.</span></span> <span data-ttu-id="cdf6f-146">`oneNoteClientURL`Ссылка открывает страницу в собственном клиенте OneNote, если она установлена.</span><span class="sxs-lookup"><span data-stu-id="cdf6f-146">The `oneNoteClientURL` link opens the page in the OneNote native client if it 's installed.</span></span> <span data-ttu-id="cdf6f-147">`oneNoteWebUrl`Ссылка открывает страницу в OneNote в Интернете.</span><span class="sxs-lookup"><span data-stu-id="cdf6f-147">The `oneNoteWebUrl` link opens the page in OneNote on the web.</span></span> <span data-ttu-id="cdf6f-148">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cdf6f-148">Read-only.</span></span>|
|<span data-ttu-id="cdf6f-149">порядке</span><span class="sxs-lookup"><span data-stu-id="cdf6f-149">order</span></span>|<span data-ttu-id="cdf6f-150">Int32</span><span class="sxs-lookup"><span data-stu-id="cdf6f-150">Int32</span></span>|<span data-ttu-id="cdf6f-151">Порядок страницы в родительском разделе.</span><span class="sxs-lookup"><span data-stu-id="cdf6f-151">The order of the page within its parent section.</span></span> <span data-ttu-id="cdf6f-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cdf6f-152">Read-only.</span></span>|
|<span data-ttu-id="cdf6f-153">Self</span><span class="sxs-lookup"><span data-stu-id="cdf6f-153">self</span></span>|<span data-ttu-id="cdf6f-154">String</span><span class="sxs-lookup"><span data-stu-id="cdf6f-154">String</span></span>|<span data-ttu-id="cdf6f-155">Конечная точка, в которой можно получить сведения о странице.</span><span class="sxs-lookup"><span data-stu-id="cdf6f-155">The endpoint where you can get details about the page.</span></span> <span data-ttu-id="cdf6f-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cdf6f-156">Read-only.</span></span>|
|<span data-ttu-id="cdf6f-157">title</span><span class="sxs-lookup"><span data-stu-id="cdf6f-157">title</span></span>|<span data-ttu-id="cdf6f-158">String</span><span class="sxs-lookup"><span data-stu-id="cdf6f-158">String</span></span>|<span data-ttu-id="cdf6f-159">Заголовок страницы.</span><span class="sxs-lookup"><span data-stu-id="cdf6f-159">The title of the page.</span></span> |

## <a name="relationships"></a><span data-ttu-id="cdf6f-160">Отношения</span><span class="sxs-lookup"><span data-stu-id="cdf6f-160">Relationships</span></span>
| <span data-ttu-id="cdf6f-161">Связь</span><span class="sxs-lookup"><span data-stu-id="cdf6f-161">Relationship</span></span> | <span data-ttu-id="cdf6f-162">Тип</span><span class="sxs-lookup"><span data-stu-id="cdf6f-162">Type</span></span>   |<span data-ttu-id="cdf6f-163">Описание</span><span class="sxs-lookup"><span data-stu-id="cdf6f-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cdf6f-164">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="cdf6f-164">parentNotebook</span></span>|[<span data-ttu-id="cdf6f-165">Notebook</span><span class="sxs-lookup"><span data-stu-id="cdf6f-165">Notebook</span></span>](notebook.md)|<span data-ttu-id="cdf6f-166">Записная книжка, содержащая страницу.</span><span class="sxs-lookup"><span data-stu-id="cdf6f-166">The notebook that contains the page.</span></span>  <span data-ttu-id="cdf6f-167">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cdf6f-167">Read-only.</span></span>|
|<span data-ttu-id="cdf6f-168">parentSection</span><span class="sxs-lookup"><span data-stu-id="cdf6f-168">parentSection</span></span>|[<span data-ttu-id="cdf6f-169">оненотесектион</span><span class="sxs-lookup"><span data-stu-id="cdf6f-169">OnenoteSection</span></span>](section.md)|<span data-ttu-id="cdf6f-170">Раздел, содержащий страницу.</span><span class="sxs-lookup"><span data-stu-id="cdf6f-170">The section that contains the page.</span></span> <span data-ttu-id="cdf6f-171">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cdf6f-171">Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="cdf6f-172">Методы</span><span class="sxs-lookup"><span data-stu-id="cdf6f-172">Methods</span></span>

| <span data-ttu-id="cdf6f-173">Метод</span><span class="sxs-lookup"><span data-stu-id="cdf6f-173">Method</span></span>           | <span data-ttu-id="cdf6f-174">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="cdf6f-174">Return Type</span></span>    |<span data-ttu-id="cdf6f-175">Описание</span><span class="sxs-lookup"><span data-stu-id="cdf6f-175">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cdf6f-176">Вывод страницы</span><span class="sxs-lookup"><span data-stu-id="cdf6f-176">Get page</span></span>](../api/page-get.md) | [<span data-ttu-id="cdf6f-177">Page</span><span class="sxs-lookup"><span data-stu-id="cdf6f-177">Page</span></span>](page.md) |<span data-ttu-id="cdf6f-178">Чтение свойств и связей страницы.</span><span class="sxs-lookup"><span data-stu-id="cdf6f-178">Read the properties and relationships of the page.</span></span>|
|[<span data-ttu-id="cdf6f-179">Обновление содержимого страницы</span><span class="sxs-lookup"><span data-stu-id="cdf6f-179">Update page content</span></span>](../api/page-update.md) | <span data-ttu-id="cdf6f-180">Нет</span><span class="sxs-lookup"><span data-stu-id="cdf6f-180">None</span></span> |<span data-ttu-id="cdf6f-181">Обновление HTML-содержимого страницы.</span><span class="sxs-lookup"><span data-stu-id="cdf6f-181">Update the HTML content of the page.</span></span> |
|[<span data-ttu-id="cdf6f-182">Удаление страницы</span><span class="sxs-lookup"><span data-stu-id="cdf6f-182">Delete page</span></span>](../api/page-delete.md) | <span data-ttu-id="cdf6f-183">Нет</span><span class="sxs-lookup"><span data-stu-id="cdf6f-183">None</span></span> |<span data-ttu-id="cdf6f-184">Удаление страницы.</span><span class="sxs-lookup"><span data-stu-id="cdf6f-184">Delete the page.</span></span> |
|[<span data-ttu-id="cdf6f-185">copyToSection</span><span class="sxs-lookup"><span data-stu-id="cdf6f-185">copyToSection</span></span>](../api/page-copytosection.md)| <span data-ttu-id="cdf6f-186">Нет</span><span class="sxs-lookup"><span data-stu-id="cdf6f-186">None</span></span> |<span data-ttu-id="cdf6f-187">Копирует страницу в определенный раздел.</span><span class="sxs-lookup"><span data-stu-id="cdf6f-187">Copies the page to a specific section.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
