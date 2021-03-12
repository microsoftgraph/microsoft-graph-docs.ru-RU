---
title: Тип ресурса страницы
description: Страница в записной книжке OneNote.
localization_priority: Normal
author: jewan-microsoft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 6adb0197b5e8fbcaa71e88f66481ca18a11bbfeb
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721532"
---
# <a name="page-resource-type"></a><span data-ttu-id="373a9-103">Тип ресурса страницы</span><span class="sxs-lookup"><span data-stu-id="373a9-103">page resource type</span></span>

<span data-ttu-id="373a9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="373a9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="373a9-105">Страница в записной книжке OneNote.</span><span class="sxs-lookup"><span data-stu-id="373a9-105">A page in a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="373a9-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="373a9-106">JSON representation</span></span>

<span data-ttu-id="373a9-107">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="373a9-107">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="373a9-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="373a9-108">Properties</span></span>
| <span data-ttu-id="373a9-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="373a9-109">Property</span></span>     | <span data-ttu-id="373a9-110">Тип</span><span class="sxs-lookup"><span data-stu-id="373a9-110">Type</span></span>   |<span data-ttu-id="373a9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="373a9-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="373a9-112">содержимое</span><span class="sxs-lookup"><span data-stu-id="373a9-112">content</span></span>|<span data-ttu-id="373a9-113">Поток</span><span class="sxs-lookup"><span data-stu-id="373a9-113">Stream</span></span>|<span data-ttu-id="373a9-114">HTML-контент страницы.</span><span class="sxs-lookup"><span data-stu-id="373a9-114">The page's HTML content.</span></span>|
|<span data-ttu-id="373a9-115">contentUrl</span><span class="sxs-lookup"><span data-stu-id="373a9-115">contentUrl</span></span>|<span data-ttu-id="373a9-116">String</span><span class="sxs-lookup"><span data-stu-id="373a9-116">String</span></span>|<span data-ttu-id="373a9-117">URL-адрес HTML-контента страницы.</span><span class="sxs-lookup"><span data-stu-id="373a9-117">The URL for the page's HTML content.</span></span>  <span data-ttu-id="373a9-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="373a9-118">Read-only.</span></span>|
|<span data-ttu-id="373a9-119">createdByAppId</span><span class="sxs-lookup"><span data-stu-id="373a9-119">createdByAppId</span></span>|<span data-ttu-id="373a9-120">String</span><span class="sxs-lookup"><span data-stu-id="373a9-120">String</span></span>|<span data-ttu-id="373a9-121">Уникальный идентификатор приложения, создавшего страницу.</span><span class="sxs-lookup"><span data-stu-id="373a9-121">The unique identifier of the application that created the page.</span></span> <span data-ttu-id="373a9-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="373a9-122">Read-only.</span></span>|
|<span data-ttu-id="373a9-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="373a9-123">createdDateTime</span></span>|<span data-ttu-id="373a9-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="373a9-124">DateTimeOffset</span></span>|<span data-ttu-id="373a9-125">Дата и время создания страницы.</span><span class="sxs-lookup"><span data-stu-id="373a9-125">The date and time when the page was created.</span></span> <span data-ttu-id="373a9-126">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="373a9-126">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="373a9-127">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="373a9-127">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="373a9-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="373a9-128">Read-only.</span></span>|
|<span data-ttu-id="373a9-129">id</span><span class="sxs-lookup"><span data-stu-id="373a9-129">id</span></span>|<span data-ttu-id="373a9-130">String</span><span class="sxs-lookup"><span data-stu-id="373a9-130">String</span></span>|<span data-ttu-id="373a9-131">Уникальный идентификатор страницы.</span><span class="sxs-lookup"><span data-stu-id="373a9-131">The unique identifier of the page.</span></span>  <span data-ttu-id="373a9-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="373a9-132">Read-only.</span></span>|
|<span data-ttu-id="373a9-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="373a9-133">lastModifiedDateTime</span></span>|<span data-ttu-id="373a9-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="373a9-134">DateTimeOffset</span></span>|<span data-ttu-id="373a9-135">Дата и время последнего изменения страницы.</span><span class="sxs-lookup"><span data-stu-id="373a9-135">The date and time when the page was last modified.</span></span> <span data-ttu-id="373a9-136">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="373a9-136">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="373a9-137">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="373a9-137">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="373a9-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="373a9-138">Read-only.</span></span>|
|<span data-ttu-id="373a9-139">уровень</span><span class="sxs-lookup"><span data-stu-id="373a9-139">level</span></span>|<span data-ttu-id="373a9-140">Int32</span><span class="sxs-lookup"><span data-stu-id="373a9-140">Int32</span></span>|<span data-ttu-id="373a9-141">Уровень отступа страницы.</span><span class="sxs-lookup"><span data-stu-id="373a9-141">The indentation level of the page.</span></span> <span data-ttu-id="373a9-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="373a9-142">Read-only.</span></span>|
|<span data-ttu-id="373a9-143">links</span><span class="sxs-lookup"><span data-stu-id="373a9-143">links</span></span>|[<span data-ttu-id="373a9-144">PageLinks</span><span class="sxs-lookup"><span data-stu-id="373a9-144">PageLinks</span></span>](pagelinks.md)|<span data-ttu-id="373a9-145">Ссылки для открытия страницы.</span><span class="sxs-lookup"><span data-stu-id="373a9-145">Links for opening the page.</span></span> <span data-ttu-id="373a9-146">Ссылка `oneNoteClientURL` открывает страницу в родном клиенте OneNote, если она установлена.</span><span class="sxs-lookup"><span data-stu-id="373a9-146">The `oneNoteClientURL` link opens the page in the OneNote native client if it 's installed.</span></span> <span data-ttu-id="373a9-147">Ссылка `oneNoteWebUrl` открывает страницу в OneNote в Интернете.</span><span class="sxs-lookup"><span data-stu-id="373a9-147">The `oneNoteWebUrl` link opens the page in OneNote on the web.</span></span> <span data-ttu-id="373a9-148">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="373a9-148">Read-only.</span></span>|
|<span data-ttu-id="373a9-149">порядок</span><span class="sxs-lookup"><span data-stu-id="373a9-149">order</span></span>|<span data-ttu-id="373a9-150">Int32</span><span class="sxs-lookup"><span data-stu-id="373a9-150">Int32</span></span>|<span data-ttu-id="373a9-151">Порядок страницы в родительском разделе.</span><span class="sxs-lookup"><span data-stu-id="373a9-151">The order of the page within its parent section.</span></span> <span data-ttu-id="373a9-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="373a9-152">Read-only.</span></span>|
|<span data-ttu-id="373a9-153">self</span><span class="sxs-lookup"><span data-stu-id="373a9-153">self</span></span>|<span data-ttu-id="373a9-154">String</span><span class="sxs-lookup"><span data-stu-id="373a9-154">String</span></span>|<span data-ttu-id="373a9-155">Конечная точка, в которой можно получить сведения о странице.</span><span class="sxs-lookup"><span data-stu-id="373a9-155">The endpoint where you can get details about the page.</span></span> <span data-ttu-id="373a9-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="373a9-156">Read-only.</span></span>|
|<span data-ttu-id="373a9-157">title</span><span class="sxs-lookup"><span data-stu-id="373a9-157">title</span></span>|<span data-ttu-id="373a9-158">String</span><span class="sxs-lookup"><span data-stu-id="373a9-158">String</span></span>|<span data-ttu-id="373a9-159">Заголовок страницы.</span><span class="sxs-lookup"><span data-stu-id="373a9-159">The title of the page.</span></span> |

## <a name="relationships"></a><span data-ttu-id="373a9-160">Связи</span><span class="sxs-lookup"><span data-stu-id="373a9-160">Relationships</span></span>
| <span data-ttu-id="373a9-161">Связь</span><span class="sxs-lookup"><span data-stu-id="373a9-161">Relationship</span></span> | <span data-ttu-id="373a9-162">Тип</span><span class="sxs-lookup"><span data-stu-id="373a9-162">Type</span></span>   |<span data-ttu-id="373a9-163">Описание</span><span class="sxs-lookup"><span data-stu-id="373a9-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="373a9-164">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="373a9-164">parentNotebook</span></span>|[<span data-ttu-id="373a9-165">Notebook</span><span class="sxs-lookup"><span data-stu-id="373a9-165">Notebook</span></span>](notebook.md)|<span data-ttu-id="373a9-166">Блокнот, содержащий страницу.</span><span class="sxs-lookup"><span data-stu-id="373a9-166">The notebook that contains the page.</span></span>  <span data-ttu-id="373a9-167">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="373a9-167">Read-only.</span></span>|
|<span data-ttu-id="373a9-168">parentSection</span><span class="sxs-lookup"><span data-stu-id="373a9-168">parentSection</span></span>|[<span data-ttu-id="373a9-169">OnenoteSection</span><span class="sxs-lookup"><span data-stu-id="373a9-169">OnenoteSection</span></span>](section.md)|<span data-ttu-id="373a9-170">Раздел, содержащий страницу.</span><span class="sxs-lookup"><span data-stu-id="373a9-170">The section that contains the page.</span></span> <span data-ttu-id="373a9-171">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="373a9-171">Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="373a9-172">Методы</span><span class="sxs-lookup"><span data-stu-id="373a9-172">Methods</span></span>

| <span data-ttu-id="373a9-173">Метод</span><span class="sxs-lookup"><span data-stu-id="373a9-173">Method</span></span>           | <span data-ttu-id="373a9-174">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="373a9-174">Return Type</span></span>    |<span data-ttu-id="373a9-175">Описание</span><span class="sxs-lookup"><span data-stu-id="373a9-175">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="373a9-176">Вывод страницы</span><span class="sxs-lookup"><span data-stu-id="373a9-176">Get page</span></span>](../api/page-get.md) | [<span data-ttu-id="373a9-177">Page</span><span class="sxs-lookup"><span data-stu-id="373a9-177">Page</span></span>](page.md) |<span data-ttu-id="373a9-178">Ознакомьтесь с свойствами и отношениями страницы.</span><span class="sxs-lookup"><span data-stu-id="373a9-178">Read the properties and relationships of the page.</span></span>|
|[<span data-ttu-id="373a9-179">Обновление содержимого страницы</span><span class="sxs-lookup"><span data-stu-id="373a9-179">Update page content</span></span>](../api/page-update.md) | <span data-ttu-id="373a9-180">Нет</span><span class="sxs-lookup"><span data-stu-id="373a9-180">None</span></span> |<span data-ttu-id="373a9-181">Обновление HTML-контента страницы.</span><span class="sxs-lookup"><span data-stu-id="373a9-181">Update the HTML content of the page.</span></span> |
|[<span data-ttu-id="373a9-182">Удаление страницы</span><span class="sxs-lookup"><span data-stu-id="373a9-182">Delete page</span></span>](../api/page-delete.md) | <span data-ttu-id="373a9-183">Нет</span><span class="sxs-lookup"><span data-stu-id="373a9-183">None</span></span> |<span data-ttu-id="373a9-184">Удалите страницу.</span><span class="sxs-lookup"><span data-stu-id="373a9-184">Delete the page.</span></span> |
|[<span data-ttu-id="373a9-185">copyToSection</span><span class="sxs-lookup"><span data-stu-id="373a9-185">copyToSection</span></span>](../api/page-copytosection.md)| <span data-ttu-id="373a9-186">Нет</span><span class="sxs-lookup"><span data-stu-id="373a9-186">None</span></span> |<span data-ttu-id="373a9-187">Копирует страницу в определенный раздел.</span><span class="sxs-lookup"><span data-stu-id="373a9-187">Copies the page to a specific section.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

