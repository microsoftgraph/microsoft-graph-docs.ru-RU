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
# <a name="onenotepage-resource-type"></a><span data-ttu-id="6494b-103">Тип ресурса Оненотепаже</span><span class="sxs-lookup"><span data-stu-id="6494b-103">onenotePage resource type</span></span>

<span data-ttu-id="6494b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6494b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6494b-105">Страница в записной книжке OneNote.</span><span class="sxs-lookup"><span data-stu-id="6494b-105">A page in a OneNote notebook.</span></span>

## <a name="properties"></a><span data-ttu-id="6494b-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="6494b-106">Properties</span></span>
| <span data-ttu-id="6494b-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="6494b-107">Property</span></span>     | <span data-ttu-id="6494b-108">Тип</span><span class="sxs-lookup"><span data-stu-id="6494b-108">Type</span></span>   |<span data-ttu-id="6494b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6494b-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6494b-110">содержимое</span><span class="sxs-lookup"><span data-stu-id="6494b-110">content</span></span>|<span data-ttu-id="6494b-111">Поток</span><span class="sxs-lookup"><span data-stu-id="6494b-111">Stream</span></span>|<span data-ttu-id="6494b-112">HTML-контент страницы.</span><span class="sxs-lookup"><span data-stu-id="6494b-112">The page's HTML content.</span></span>|
|<span data-ttu-id="6494b-113">contentUrl</span><span class="sxs-lookup"><span data-stu-id="6494b-113">contentUrl</span></span>|<span data-ttu-id="6494b-114">String</span><span class="sxs-lookup"><span data-stu-id="6494b-114">String</span></span>|<span data-ttu-id="6494b-115">URL-адрес HTML-содержимого страницы.</span><span class="sxs-lookup"><span data-stu-id="6494b-115">The URL for the page's HTML content.</span></span>  <span data-ttu-id="6494b-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6494b-116">Read-only.</span></span>|
|<span data-ttu-id="6494b-117">createdByAppId</span><span class="sxs-lookup"><span data-stu-id="6494b-117">createdByAppId</span></span>|<span data-ttu-id="6494b-118">String</span><span class="sxs-lookup"><span data-stu-id="6494b-118">String</span></span>|<span data-ttu-id="6494b-119">Уникальный идентификатор приложения, создавшего страницу.</span><span class="sxs-lookup"><span data-stu-id="6494b-119">The unique identifier of the application that created the page.</span></span> <span data-ttu-id="6494b-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6494b-120">Read-only.</span></span>|
|<span data-ttu-id="6494b-121">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6494b-121">createdDateTime</span></span>|<span data-ttu-id="6494b-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6494b-122">DateTimeOffset</span></span>|<span data-ttu-id="6494b-123">Дата и время создания страницы.</span><span class="sxs-lookup"><span data-stu-id="6494b-123">The date and time when the page was created.</span></span> <span data-ttu-id="6494b-124">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="6494b-124">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6494b-125">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="6494b-125">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="6494b-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6494b-126">Read-only.</span></span>|
|<span data-ttu-id="6494b-127">id</span><span class="sxs-lookup"><span data-stu-id="6494b-127">id</span></span>|<span data-ttu-id="6494b-128">String</span><span class="sxs-lookup"><span data-stu-id="6494b-128">String</span></span>|<span data-ttu-id="6494b-129">Уникальный идентификатор страницы.</span><span class="sxs-lookup"><span data-stu-id="6494b-129">The unique identifier of the page.</span></span>  <span data-ttu-id="6494b-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6494b-130">Read-only.</span></span>|
|<span data-ttu-id="6494b-131">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6494b-131">lastModifiedDateTime</span></span>|<span data-ttu-id="6494b-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6494b-132">DateTimeOffset</span></span>|<span data-ttu-id="6494b-133">Дата и время последнего изменения страницы.</span><span class="sxs-lookup"><span data-stu-id="6494b-133">The date and time when the page was last modified.</span></span> <span data-ttu-id="6494b-134">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="6494b-134">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6494b-135">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="6494b-135">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="6494b-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6494b-136">Read-only.</span></span>|
|<span data-ttu-id="6494b-137">степень</span><span class="sxs-lookup"><span data-stu-id="6494b-137">level</span></span>|<span data-ttu-id="6494b-138">Int32</span><span class="sxs-lookup"><span data-stu-id="6494b-138">Int32</span></span>|<span data-ttu-id="6494b-139">Уровень отступа страницы.</span><span class="sxs-lookup"><span data-stu-id="6494b-139">The indentation level of the page.</span></span> <span data-ttu-id="6494b-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6494b-140">Read-only.</span></span>|
|<span data-ttu-id="6494b-141">links</span><span class="sxs-lookup"><span data-stu-id="6494b-141">links</span></span>|[<span data-ttu-id="6494b-142">пажелинкс</span><span class="sxs-lookup"><span data-stu-id="6494b-142">pageLinks</span></span>](pagelinks.md)|<span data-ttu-id="6494b-143">Ссылки для открытия страницы.</span><span class="sxs-lookup"><span data-stu-id="6494b-143">Links for opening the page.</span></span> <span data-ttu-id="6494b-144">`oneNoteClientURL` Ссылка открывает страницу в собственном клиенте OneNote, если она установлена.</span><span class="sxs-lookup"><span data-stu-id="6494b-144">The `oneNoteClientURL` link opens the page in the OneNote native client if it 's installed.</span></span> <span data-ttu-id="6494b-145">`oneNoteWebUrl` Ссылка открывает страницу в OneNote в Интернете.</span><span class="sxs-lookup"><span data-stu-id="6494b-145">The `oneNoteWebUrl` link opens the page in OneNote on the web.</span></span> <span data-ttu-id="6494b-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6494b-146">Read-only.</span></span>|
|<span data-ttu-id="6494b-147">порядке</span><span class="sxs-lookup"><span data-stu-id="6494b-147">order</span></span>|<span data-ttu-id="6494b-148">Int32</span><span class="sxs-lookup"><span data-stu-id="6494b-148">Int32</span></span>|<span data-ttu-id="6494b-149">Порядок страницы в родительском разделе.</span><span class="sxs-lookup"><span data-stu-id="6494b-149">The order of the page within its parent section.</span></span> <span data-ttu-id="6494b-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6494b-150">Read-only.</span></span>|
|<span data-ttu-id="6494b-151">Self</span><span class="sxs-lookup"><span data-stu-id="6494b-151">self</span></span>|<span data-ttu-id="6494b-152">String</span><span class="sxs-lookup"><span data-stu-id="6494b-152">String</span></span>|<span data-ttu-id="6494b-153">Конечная точка, в которой можно получить сведения о странице.</span><span class="sxs-lookup"><span data-stu-id="6494b-153">The endpoint where you can get details about the page.</span></span> <span data-ttu-id="6494b-154">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6494b-154">Read-only.</span></span>|
|<span data-ttu-id="6494b-155">title</span><span class="sxs-lookup"><span data-stu-id="6494b-155">title</span></span>|<span data-ttu-id="6494b-156">Строка</span><span class="sxs-lookup"><span data-stu-id="6494b-156">String</span></span>|<span data-ttu-id="6494b-157">Заголовок страницы.</span><span class="sxs-lookup"><span data-stu-id="6494b-157">The title of the page.</span></span> |

## <a name="relationships"></a><span data-ttu-id="6494b-158">Связи</span><span class="sxs-lookup"><span data-stu-id="6494b-158">Relationships</span></span>
| <span data-ttu-id="6494b-159">Связь</span><span class="sxs-lookup"><span data-stu-id="6494b-159">Relationship</span></span> | <span data-ttu-id="6494b-160">Тип</span><span class="sxs-lookup"><span data-stu-id="6494b-160">Type</span></span>   |<span data-ttu-id="6494b-161">Описание</span><span class="sxs-lookup"><span data-stu-id="6494b-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6494b-162">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="6494b-162">parentNotebook</span></span>|[<span data-ttu-id="6494b-163">notebook</span><span class="sxs-lookup"><span data-stu-id="6494b-163">notebook</span></span>](notebook.md)|<span data-ttu-id="6494b-164">Записная книжка, содержащая страницу.</span><span class="sxs-lookup"><span data-stu-id="6494b-164">The notebook that contains the page.</span></span>  <span data-ttu-id="6494b-165">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6494b-165">Read-only.</span></span>|
|<span data-ttu-id="6494b-166">parentSection</span><span class="sxs-lookup"><span data-stu-id="6494b-166">parentSection</span></span>|[<span data-ttu-id="6494b-167">оненотесектион</span><span class="sxs-lookup"><span data-stu-id="6494b-167">onenoteSection</span></span>](onenotesection.md)|<span data-ttu-id="6494b-168">Раздел, содержащий страницу.</span><span class="sxs-lookup"><span data-stu-id="6494b-168">The section that contains the page.</span></span> <span data-ttu-id="6494b-169">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6494b-169">Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="6494b-170">Методы</span><span class="sxs-lookup"><span data-stu-id="6494b-170">Methods</span></span>

| <span data-ttu-id="6494b-171">Метод</span><span class="sxs-lookup"><span data-stu-id="6494b-171">Method</span></span>           | <span data-ttu-id="6494b-172">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6494b-172">Return Type</span></span>    |<span data-ttu-id="6494b-173">Описание</span><span class="sxs-lookup"><span data-stu-id="6494b-173">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6494b-174">Вывод страницы</span><span class="sxs-lookup"><span data-stu-id="6494b-174">Get page</span></span>](../api/page-get.md) | [<span data-ttu-id="6494b-175">оненотепаже</span><span class="sxs-lookup"><span data-stu-id="6494b-175">onenotePage</span></span>](onenotepage.md) |<span data-ttu-id="6494b-176">Чтение свойств и связей страницы.</span><span class="sxs-lookup"><span data-stu-id="6494b-176">Read the properties and relationships of the page.</span></span>|
|[<span data-ttu-id="6494b-177">Обновление содержимого страницы</span><span class="sxs-lookup"><span data-stu-id="6494b-177">Update page content</span></span>](../api/page-update.md) | <span data-ttu-id="6494b-178">Нет</span><span class="sxs-lookup"><span data-stu-id="6494b-178">None</span></span> |<span data-ttu-id="6494b-179">Обновление HTML-содержимого страницы.</span><span class="sxs-lookup"><span data-stu-id="6494b-179">Update the HTML content of the page.</span></span> |
|[<span data-ttu-id="6494b-180">Удаление страницы</span><span class="sxs-lookup"><span data-stu-id="6494b-180">Delete page</span></span>](../api/page-delete.md) | <span data-ttu-id="6494b-181">Нет</span><span class="sxs-lookup"><span data-stu-id="6494b-181">None</span></span> |<span data-ttu-id="6494b-182">Удаление страницы.</span><span class="sxs-lookup"><span data-stu-id="6494b-182">Delete the page.</span></span> |
|[<span data-ttu-id="6494b-183">copyToSection</span><span class="sxs-lookup"><span data-stu-id="6494b-183">copyToSection</span></span>](../api/page-copytosection.md)| <span data-ttu-id="6494b-184">Нет</span><span class="sxs-lookup"><span data-stu-id="6494b-184">None</span></span> |<span data-ttu-id="6494b-185">Копирует страницу в определенный раздел.</span><span class="sxs-lookup"><span data-stu-id="6494b-185">Copies the page to a specific section.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6494b-186">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6494b-186">JSON representation</span></span>

<span data-ttu-id="6494b-187">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6494b-187">Here is a JSON representation of the resource.</span></span>

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
