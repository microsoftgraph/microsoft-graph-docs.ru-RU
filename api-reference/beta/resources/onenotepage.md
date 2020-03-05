---
title: Тип ресурса Оненотепаже
description: Страница в записной книжке OneNote.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: bf3410923cdcc7d48c78d6872e5fc6c20f4cf619
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522332"
---
# <a name="onenotepage-resource-type"></a><span data-ttu-id="e2aef-103">Тип ресурса Оненотепаже</span><span class="sxs-lookup"><span data-stu-id="e2aef-103">onenotePage resource type</span></span>

<span data-ttu-id="e2aef-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e2aef-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2aef-105">Страница в записной книжке OneNote.</span><span class="sxs-lookup"><span data-stu-id="e2aef-105">A page in a OneNote notebook.</span></span>

## <a name="properties"></a><span data-ttu-id="e2aef-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e2aef-106">Properties</span></span>
| <span data-ttu-id="e2aef-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="e2aef-107">Property</span></span>     | <span data-ttu-id="e2aef-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e2aef-108">Type</span></span>   |<span data-ttu-id="e2aef-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e2aef-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e2aef-110">содержимое</span><span class="sxs-lookup"><span data-stu-id="e2aef-110">content</span></span>|<span data-ttu-id="e2aef-111">Поток</span><span class="sxs-lookup"><span data-stu-id="e2aef-111">Stream</span></span>|<span data-ttu-id="e2aef-112">HTML-контент страницы.</span><span class="sxs-lookup"><span data-stu-id="e2aef-112">The page's HTML content.</span></span>|
|<span data-ttu-id="e2aef-113">contentUrl</span><span class="sxs-lookup"><span data-stu-id="e2aef-113">contentUrl</span></span>|<span data-ttu-id="e2aef-114">String</span><span class="sxs-lookup"><span data-stu-id="e2aef-114">String</span></span>|<span data-ttu-id="e2aef-115">URL-адрес HTML-содержимого страницы.</span><span class="sxs-lookup"><span data-stu-id="e2aef-115">The URL for the page's HTML content.</span></span>  <span data-ttu-id="e2aef-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e2aef-116">Read-only.</span></span>|
|<span data-ttu-id="e2aef-117">креатедбяппид</span><span class="sxs-lookup"><span data-stu-id="e2aef-117">createdByAppId</span></span>|<span data-ttu-id="e2aef-118">String</span><span class="sxs-lookup"><span data-stu-id="e2aef-118">String</span></span>|<span data-ttu-id="e2aef-119">Уникальный идентификатор приложения, создавшего страницу.</span><span class="sxs-lookup"><span data-stu-id="e2aef-119">The unique identifier of the application that created the page.</span></span> <span data-ttu-id="e2aef-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e2aef-120">Read-only.</span></span>|
|<span data-ttu-id="e2aef-121">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e2aef-121">createdDateTime</span></span>|<span data-ttu-id="e2aef-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2aef-122">DateTimeOffset</span></span>|<span data-ttu-id="e2aef-123">Дата и время создания страницы.</span><span class="sxs-lookup"><span data-stu-id="e2aef-123">The date and time when the page was created.</span></span> <span data-ttu-id="e2aef-124">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="e2aef-124">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e2aef-125">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="e2aef-125">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="e2aef-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e2aef-126">Read-only.</span></span>|
|<span data-ttu-id="e2aef-127">id</span><span class="sxs-lookup"><span data-stu-id="e2aef-127">id</span></span>|<span data-ttu-id="e2aef-128">String</span><span class="sxs-lookup"><span data-stu-id="e2aef-128">String</span></span>|<span data-ttu-id="e2aef-129">Уникальный идентификатор страницы.</span><span class="sxs-lookup"><span data-stu-id="e2aef-129">The unique identifier of the page.</span></span>  <span data-ttu-id="e2aef-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e2aef-130">Read-only.</span></span>|
|<span data-ttu-id="e2aef-131">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e2aef-131">lastModifiedDateTime</span></span>|<span data-ttu-id="e2aef-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2aef-132">DateTimeOffset</span></span>|<span data-ttu-id="e2aef-133">Дата и время последнего изменения страницы.</span><span class="sxs-lookup"><span data-stu-id="e2aef-133">The date and time when the page was last modified.</span></span> <span data-ttu-id="e2aef-134">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="e2aef-134">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e2aef-135">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="e2aef-135">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="e2aef-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e2aef-136">Read-only.</span></span>|
|<span data-ttu-id="e2aef-137">степень</span><span class="sxs-lookup"><span data-stu-id="e2aef-137">level</span></span>|<span data-ttu-id="e2aef-138">Int32</span><span class="sxs-lookup"><span data-stu-id="e2aef-138">Int32</span></span>|<span data-ttu-id="e2aef-139">Уровень отступа страницы.</span><span class="sxs-lookup"><span data-stu-id="e2aef-139">The indentation level of the page.</span></span> <span data-ttu-id="e2aef-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e2aef-140">Read-only.</span></span>|
|<span data-ttu-id="e2aef-141">links</span><span class="sxs-lookup"><span data-stu-id="e2aef-141">links</span></span>|[<span data-ttu-id="e2aef-142">пажелинкс</span><span class="sxs-lookup"><span data-stu-id="e2aef-142">pageLinks</span></span>](pagelinks.md)|<span data-ttu-id="e2aef-143">Ссылки для открытия страницы.</span><span class="sxs-lookup"><span data-stu-id="e2aef-143">Links for opening the page.</span></span> <span data-ttu-id="e2aef-144">`oneNoteClientURL` Ссылка открывает страницу в собственном клиенте OneNote, если она установлена.</span><span class="sxs-lookup"><span data-stu-id="e2aef-144">The `oneNoteClientURL` link opens the page in the OneNote native client if it 's installed.</span></span> <span data-ttu-id="e2aef-145">`oneNoteWebUrl` Ссылка открывает страницу в OneNote в Интернете.</span><span class="sxs-lookup"><span data-stu-id="e2aef-145">The `oneNoteWebUrl` link opens the page in OneNote on the web.</span></span> <span data-ttu-id="e2aef-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e2aef-146">Read-only.</span></span>|
|<span data-ttu-id="e2aef-147">порядке</span><span class="sxs-lookup"><span data-stu-id="e2aef-147">order</span></span>|<span data-ttu-id="e2aef-148">Int32</span><span class="sxs-lookup"><span data-stu-id="e2aef-148">Int32</span></span>|<span data-ttu-id="e2aef-149">Порядок страницы в родительском разделе.</span><span class="sxs-lookup"><span data-stu-id="e2aef-149">The order of the page within its parent section.</span></span> <span data-ttu-id="e2aef-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e2aef-150">Read-only.</span></span>|
|<span data-ttu-id="e2aef-151">Self</span><span class="sxs-lookup"><span data-stu-id="e2aef-151">self</span></span>|<span data-ttu-id="e2aef-152">String</span><span class="sxs-lookup"><span data-stu-id="e2aef-152">String</span></span>|<span data-ttu-id="e2aef-153">Конечная точка, в которой можно получить сведения о странице.</span><span class="sxs-lookup"><span data-stu-id="e2aef-153">The endpoint where you can get details about the page.</span></span> <span data-ttu-id="e2aef-154">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e2aef-154">Read-only.</span></span>|
|<span data-ttu-id="e2aef-155">title</span><span class="sxs-lookup"><span data-stu-id="e2aef-155">title</span></span>|<span data-ttu-id="e2aef-156">String</span><span class="sxs-lookup"><span data-stu-id="e2aef-156">String</span></span>|<span data-ttu-id="e2aef-157">Заголовок страницы.</span><span class="sxs-lookup"><span data-stu-id="e2aef-157">The title of the page.</span></span> |

## <a name="relationships"></a><span data-ttu-id="e2aef-158">Связи</span><span class="sxs-lookup"><span data-stu-id="e2aef-158">Relationships</span></span>
| <span data-ttu-id="e2aef-159">Связь</span><span class="sxs-lookup"><span data-stu-id="e2aef-159">Relationship</span></span> | <span data-ttu-id="e2aef-160">Тип</span><span class="sxs-lookup"><span data-stu-id="e2aef-160">Type</span></span>   |<span data-ttu-id="e2aef-161">Описание</span><span class="sxs-lookup"><span data-stu-id="e2aef-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e2aef-162">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="e2aef-162">parentNotebook</span></span>|[<span data-ttu-id="e2aef-163">notebook</span><span class="sxs-lookup"><span data-stu-id="e2aef-163">notebook</span></span>](notebook.md)|<span data-ttu-id="e2aef-164">Записная книжка, содержащая страницу.</span><span class="sxs-lookup"><span data-stu-id="e2aef-164">The notebook that contains the page.</span></span>  <span data-ttu-id="e2aef-165">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e2aef-165">Read-only.</span></span>|
|<span data-ttu-id="e2aef-166">parentSection</span><span class="sxs-lookup"><span data-stu-id="e2aef-166">parentSection</span></span>|[<span data-ttu-id="e2aef-167">оненотесектион</span><span class="sxs-lookup"><span data-stu-id="e2aef-167">onenoteSection</span></span>](onenotesection.md)|<span data-ttu-id="e2aef-168">Раздел, содержащий страницу.</span><span class="sxs-lookup"><span data-stu-id="e2aef-168">The section that contains the page.</span></span> <span data-ttu-id="e2aef-169">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e2aef-169">Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="e2aef-170">Методы</span><span class="sxs-lookup"><span data-stu-id="e2aef-170">Methods</span></span>

| <span data-ttu-id="e2aef-171">Метод</span><span class="sxs-lookup"><span data-stu-id="e2aef-171">Method</span></span>           | <span data-ttu-id="e2aef-172">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e2aef-172">Return Type</span></span>    |<span data-ttu-id="e2aef-173">Описание</span><span class="sxs-lookup"><span data-stu-id="e2aef-173">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e2aef-174">Вывод страницы</span><span class="sxs-lookup"><span data-stu-id="e2aef-174">Get page</span></span>](../api/page-get.md) | [<span data-ttu-id="e2aef-175">оненотепаже</span><span class="sxs-lookup"><span data-stu-id="e2aef-175">onenotePage</span></span>](onenotepage.md) |<span data-ttu-id="e2aef-176">Чтение свойств и связей страницы.</span><span class="sxs-lookup"><span data-stu-id="e2aef-176">Read the properties and relationships of the page.</span></span>|
|[<span data-ttu-id="e2aef-177">Обновление содержимого страницы</span><span class="sxs-lookup"><span data-stu-id="e2aef-177">Update page content</span></span>](../api/page-update.md) | <span data-ttu-id="e2aef-178">Нет</span><span class="sxs-lookup"><span data-stu-id="e2aef-178">None</span></span> |<span data-ttu-id="e2aef-179">Обновление HTML-содержимого страницы.</span><span class="sxs-lookup"><span data-stu-id="e2aef-179">Update the HTML content of the page.</span></span> |
|[<span data-ttu-id="e2aef-180">Удаление страницы</span><span class="sxs-lookup"><span data-stu-id="e2aef-180">Delete page</span></span>](../api/page-delete.md) | <span data-ttu-id="e2aef-181">Нет</span><span class="sxs-lookup"><span data-stu-id="e2aef-181">None</span></span> |<span data-ttu-id="e2aef-182">Удаление страницы.</span><span class="sxs-lookup"><span data-stu-id="e2aef-182">Delete the page.</span></span> |
|[<span data-ttu-id="e2aef-183">copyToSection</span><span class="sxs-lookup"><span data-stu-id="e2aef-183">copyToSection</span></span>](../api/page-copytosection.md)| <span data-ttu-id="e2aef-184">Нет</span><span class="sxs-lookup"><span data-stu-id="e2aef-184">None</span></span> |<span data-ttu-id="e2aef-185">Копирует страницу в определенный раздел.</span><span class="sxs-lookup"><span data-stu-id="e2aef-185">Copies the page to a specific section.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e2aef-186">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e2aef-186">JSON representation</span></span>

<span data-ttu-id="e2aef-187">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e2aef-187">Here is a JSON representation of the resource.</span></span>

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
