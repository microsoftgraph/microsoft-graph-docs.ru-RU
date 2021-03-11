---
title: тип ресурса onenotePage
description: Страница в записной книжке OneNote.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: jewan-microsoft
ms.openlocfilehash: 2f8a93080b3eaa58be95e8721307cdde31b359ea
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50719453"
---
# <a name="onenotepage-resource-type"></a><span data-ttu-id="0f8b6-103">тип ресурса onenotePage</span><span class="sxs-lookup"><span data-stu-id="0f8b6-103">onenotePage resource type</span></span>

<span data-ttu-id="0f8b6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f8b6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f8b6-105">Страница в записной книжке OneNote.</span><span class="sxs-lookup"><span data-stu-id="0f8b6-105">A page in a OneNote notebook.</span></span>

## <a name="properties"></a><span data-ttu-id="0f8b6-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="0f8b6-106">Properties</span></span>
| <span data-ttu-id="0f8b6-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="0f8b6-107">Property</span></span>     | <span data-ttu-id="0f8b6-108">Тип</span><span class="sxs-lookup"><span data-stu-id="0f8b6-108">Type</span></span>   |<span data-ttu-id="0f8b6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0f8b6-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0f8b6-110">содержимое</span><span class="sxs-lookup"><span data-stu-id="0f8b6-110">content</span></span>|<span data-ttu-id="0f8b6-111">Поток</span><span class="sxs-lookup"><span data-stu-id="0f8b6-111">Stream</span></span>|<span data-ttu-id="0f8b6-112">HTML-контент страницы.</span><span class="sxs-lookup"><span data-stu-id="0f8b6-112">The page's HTML content.</span></span>|
|<span data-ttu-id="0f8b6-113">contentUrl</span><span class="sxs-lookup"><span data-stu-id="0f8b6-113">contentUrl</span></span>|<span data-ttu-id="0f8b6-114">String</span><span class="sxs-lookup"><span data-stu-id="0f8b6-114">String</span></span>|<span data-ttu-id="0f8b6-115">URL-адрес HTML-контента страницы.</span><span class="sxs-lookup"><span data-stu-id="0f8b6-115">The URL for the page's HTML content.</span></span>  <span data-ttu-id="0f8b6-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0f8b6-116">Read-only.</span></span>|
|<span data-ttu-id="0f8b6-117">createdByAppId</span><span class="sxs-lookup"><span data-stu-id="0f8b6-117">createdByAppId</span></span>|<span data-ttu-id="0f8b6-118">String</span><span class="sxs-lookup"><span data-stu-id="0f8b6-118">String</span></span>|<span data-ttu-id="0f8b6-119">Уникальный идентификатор приложения, создавшего страницу.</span><span class="sxs-lookup"><span data-stu-id="0f8b6-119">The unique identifier of the application that created the page.</span></span> <span data-ttu-id="0f8b6-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0f8b6-120">Read-only.</span></span>|
|<span data-ttu-id="0f8b6-121">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0f8b6-121">createdDateTime</span></span>|<span data-ttu-id="0f8b6-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f8b6-122">DateTimeOffset</span></span>|<span data-ttu-id="0f8b6-123">Дата и время создания страницы.</span><span class="sxs-lookup"><span data-stu-id="0f8b6-123">The date and time when the page was created.</span></span> <span data-ttu-id="0f8b6-124">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="0f8b6-124">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0f8b6-125">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="0f8b6-125">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="0f8b6-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0f8b6-126">Read-only.</span></span>|
|<span data-ttu-id="0f8b6-127">id</span><span class="sxs-lookup"><span data-stu-id="0f8b6-127">id</span></span>|<span data-ttu-id="0f8b6-128">String</span><span class="sxs-lookup"><span data-stu-id="0f8b6-128">String</span></span>|<span data-ttu-id="0f8b6-129">Уникальный идентификатор страницы.</span><span class="sxs-lookup"><span data-stu-id="0f8b6-129">The unique identifier of the page.</span></span>  <span data-ttu-id="0f8b6-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0f8b6-130">Read-only.</span></span>|
|<span data-ttu-id="0f8b6-131">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0f8b6-131">lastModifiedDateTime</span></span>|<span data-ttu-id="0f8b6-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f8b6-132">DateTimeOffset</span></span>|<span data-ttu-id="0f8b6-133">Дата и время последнего изменения страницы.</span><span class="sxs-lookup"><span data-stu-id="0f8b6-133">The date and time when the page was last modified.</span></span> <span data-ttu-id="0f8b6-134">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="0f8b6-134">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0f8b6-135">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="0f8b6-135">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="0f8b6-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0f8b6-136">Read-only.</span></span>|
|<span data-ttu-id="0f8b6-137">уровень</span><span class="sxs-lookup"><span data-stu-id="0f8b6-137">level</span></span>|<span data-ttu-id="0f8b6-138">Int32</span><span class="sxs-lookup"><span data-stu-id="0f8b6-138">Int32</span></span>|<span data-ttu-id="0f8b6-139">Уровень отступа страницы.</span><span class="sxs-lookup"><span data-stu-id="0f8b6-139">The indentation level of the page.</span></span> <span data-ttu-id="0f8b6-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0f8b6-140">Read-only.</span></span>|
|<span data-ttu-id="0f8b6-141">links</span><span class="sxs-lookup"><span data-stu-id="0f8b6-141">links</span></span>|[<span data-ttu-id="0f8b6-142">pageLinks</span><span class="sxs-lookup"><span data-stu-id="0f8b6-142">pageLinks</span></span>](pagelinks.md)|<span data-ttu-id="0f8b6-143">Ссылки для открытия страницы.</span><span class="sxs-lookup"><span data-stu-id="0f8b6-143">Links for opening the page.</span></span> <span data-ttu-id="0f8b6-144">Ссылка `oneNoteClientURL` открывает страницу в родном клиенте OneNote, если она установлена.</span><span class="sxs-lookup"><span data-stu-id="0f8b6-144">The `oneNoteClientURL` link opens the page in the OneNote native client if it 's installed.</span></span> <span data-ttu-id="0f8b6-145">Ссылка `oneNoteWebUrl` открывает страницу в OneNote в Интернете.</span><span class="sxs-lookup"><span data-stu-id="0f8b6-145">The `oneNoteWebUrl` link opens the page in OneNote on the web.</span></span> <span data-ttu-id="0f8b6-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0f8b6-146">Read-only.</span></span>|
|<span data-ttu-id="0f8b6-147">порядок</span><span class="sxs-lookup"><span data-stu-id="0f8b6-147">order</span></span>|<span data-ttu-id="0f8b6-148">Int32</span><span class="sxs-lookup"><span data-stu-id="0f8b6-148">Int32</span></span>|<span data-ttu-id="0f8b6-149">Порядок страницы в родительском разделе.</span><span class="sxs-lookup"><span data-stu-id="0f8b6-149">The order of the page within its parent section.</span></span> <span data-ttu-id="0f8b6-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0f8b6-150">Read-only.</span></span>|
|<span data-ttu-id="0f8b6-151">self</span><span class="sxs-lookup"><span data-stu-id="0f8b6-151">self</span></span>|<span data-ttu-id="0f8b6-152">String</span><span class="sxs-lookup"><span data-stu-id="0f8b6-152">String</span></span>|<span data-ttu-id="0f8b6-153">Конечная точка, в которой можно получить сведения о странице.</span><span class="sxs-lookup"><span data-stu-id="0f8b6-153">The endpoint where you can get details about the page.</span></span> <span data-ttu-id="0f8b6-154">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0f8b6-154">Read-only.</span></span>|
|<span data-ttu-id="0f8b6-155">title</span><span class="sxs-lookup"><span data-stu-id="0f8b6-155">title</span></span>|<span data-ttu-id="0f8b6-156">String</span><span class="sxs-lookup"><span data-stu-id="0f8b6-156">String</span></span>|<span data-ttu-id="0f8b6-157">Заголовок страницы.</span><span class="sxs-lookup"><span data-stu-id="0f8b6-157">The title of the page.</span></span> |

## <a name="relationships"></a><span data-ttu-id="0f8b6-158">Связи</span><span class="sxs-lookup"><span data-stu-id="0f8b6-158">Relationships</span></span>
| <span data-ttu-id="0f8b6-159">Связь</span><span class="sxs-lookup"><span data-stu-id="0f8b6-159">Relationship</span></span> | <span data-ttu-id="0f8b6-160">Тип</span><span class="sxs-lookup"><span data-stu-id="0f8b6-160">Type</span></span>   |<span data-ttu-id="0f8b6-161">Описание</span><span class="sxs-lookup"><span data-stu-id="0f8b6-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0f8b6-162">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="0f8b6-162">parentNotebook</span></span>|[<span data-ttu-id="0f8b6-163">notebook</span><span class="sxs-lookup"><span data-stu-id="0f8b6-163">notebook</span></span>](notebook.md)|<span data-ttu-id="0f8b6-164">Блокнот, содержащий страницу.</span><span class="sxs-lookup"><span data-stu-id="0f8b6-164">The notebook that contains the page.</span></span>  <span data-ttu-id="0f8b6-165">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0f8b6-165">Read-only.</span></span>|
|<span data-ttu-id="0f8b6-166">parentSection</span><span class="sxs-lookup"><span data-stu-id="0f8b6-166">parentSection</span></span>|[<span data-ttu-id="0f8b6-167">onenoteSection</span><span class="sxs-lookup"><span data-stu-id="0f8b6-167">onenoteSection</span></span>](onenotesection.md)|<span data-ttu-id="0f8b6-168">Раздел, содержащий страницу.</span><span class="sxs-lookup"><span data-stu-id="0f8b6-168">The section that contains the page.</span></span> <span data-ttu-id="0f8b6-169">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0f8b6-169">Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="0f8b6-170">Методы</span><span class="sxs-lookup"><span data-stu-id="0f8b6-170">Methods</span></span>

| <span data-ttu-id="0f8b6-171">Метод</span><span class="sxs-lookup"><span data-stu-id="0f8b6-171">Method</span></span>           | <span data-ttu-id="0f8b6-172">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0f8b6-172">Return Type</span></span>    |<span data-ttu-id="0f8b6-173">Описание</span><span class="sxs-lookup"><span data-stu-id="0f8b6-173">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0f8b6-174">Вывод страницы</span><span class="sxs-lookup"><span data-stu-id="0f8b6-174">Get page</span></span>](../api/page-get.md) | [<span data-ttu-id="0f8b6-175">onenotePage</span><span class="sxs-lookup"><span data-stu-id="0f8b6-175">onenotePage</span></span>](onenotepage.md) |<span data-ttu-id="0f8b6-176">Ознакомьтесь с свойствами и отношениями страницы.</span><span class="sxs-lookup"><span data-stu-id="0f8b6-176">Read the properties and relationships of the page.</span></span>|
|[<span data-ttu-id="0f8b6-177">Обновление содержимого страницы</span><span class="sxs-lookup"><span data-stu-id="0f8b6-177">Update page content</span></span>](../api/page-update.md) | <span data-ttu-id="0f8b6-178">Нет</span><span class="sxs-lookup"><span data-stu-id="0f8b6-178">None</span></span> |<span data-ttu-id="0f8b6-179">Обновление HTML-контента страницы.</span><span class="sxs-lookup"><span data-stu-id="0f8b6-179">Update the HTML content of the page.</span></span> |
|[<span data-ttu-id="0f8b6-180">Удаление страницы</span><span class="sxs-lookup"><span data-stu-id="0f8b6-180">Delete page</span></span>](../api/page-delete.md) | <span data-ttu-id="0f8b6-181">Нет</span><span class="sxs-lookup"><span data-stu-id="0f8b6-181">None</span></span> |<span data-ttu-id="0f8b6-182">Удалите страницу.</span><span class="sxs-lookup"><span data-stu-id="0f8b6-182">Delete the page.</span></span> |
|[<span data-ttu-id="0f8b6-183">copyToSection</span><span class="sxs-lookup"><span data-stu-id="0f8b6-183">copyToSection</span></span>](../api/page-copytosection.md)| <span data-ttu-id="0f8b6-184">Нет</span><span class="sxs-lookup"><span data-stu-id="0f8b6-184">None</span></span> |<span data-ttu-id="0f8b6-185">Копирует страницу в определенный раздел.</span><span class="sxs-lookup"><span data-stu-id="0f8b6-185">Copies the page to a specific section.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0f8b6-186">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0f8b6-186">JSON representation</span></span>

<span data-ttu-id="0f8b6-187">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0f8b6-187">Here is a JSON representation of the resource.</span></span>

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


