---
title: Тип ресурса Оненотепаже
description: Страница в записной книжке OneNote.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: jewan-microsoft
ms.openlocfilehash: d219677c70be566b5039a39c5421c91a9ab11c8c
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809376"
---
# <a name="onenotepage-resource-type"></a><span data-ttu-id="64f92-103">Тип ресурса Оненотепаже</span><span class="sxs-lookup"><span data-stu-id="64f92-103">onenotePage resource type</span></span>

<span data-ttu-id="64f92-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64f92-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64f92-105">Страница в записной книжке OneNote.</span><span class="sxs-lookup"><span data-stu-id="64f92-105">A page in a OneNote notebook.</span></span>

## <a name="properties"></a><span data-ttu-id="64f92-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="64f92-106">Properties</span></span>
| <span data-ttu-id="64f92-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="64f92-107">Property</span></span>     | <span data-ttu-id="64f92-108">Тип</span><span class="sxs-lookup"><span data-stu-id="64f92-108">Type</span></span>   |<span data-ttu-id="64f92-109">Описание</span><span class="sxs-lookup"><span data-stu-id="64f92-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="64f92-110">содержимое</span><span class="sxs-lookup"><span data-stu-id="64f92-110">content</span></span>|<span data-ttu-id="64f92-111">Поток</span><span class="sxs-lookup"><span data-stu-id="64f92-111">Stream</span></span>|<span data-ttu-id="64f92-112">HTML-контент страницы.</span><span class="sxs-lookup"><span data-stu-id="64f92-112">The page's HTML content.</span></span>|
|<span data-ttu-id="64f92-113">contentUrl</span><span class="sxs-lookup"><span data-stu-id="64f92-113">contentUrl</span></span>|<span data-ttu-id="64f92-114">String</span><span class="sxs-lookup"><span data-stu-id="64f92-114">String</span></span>|<span data-ttu-id="64f92-115">URL-адрес HTML-содержимого страницы.</span><span class="sxs-lookup"><span data-stu-id="64f92-115">The URL for the page's HTML content.</span></span>  <span data-ttu-id="64f92-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="64f92-116">Read-only.</span></span>|
|<span data-ttu-id="64f92-117">createdByAppId</span><span class="sxs-lookup"><span data-stu-id="64f92-117">createdByAppId</span></span>|<span data-ttu-id="64f92-118">String</span><span class="sxs-lookup"><span data-stu-id="64f92-118">String</span></span>|<span data-ttu-id="64f92-119">Уникальный идентификатор приложения, создавшего страницу.</span><span class="sxs-lookup"><span data-stu-id="64f92-119">The unique identifier of the application that created the page.</span></span> <span data-ttu-id="64f92-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="64f92-120">Read-only.</span></span>|
|<span data-ttu-id="64f92-121">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="64f92-121">createdDateTime</span></span>|<span data-ttu-id="64f92-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64f92-122">DateTimeOffset</span></span>|<span data-ttu-id="64f92-123">Дата и время создания страницы.</span><span class="sxs-lookup"><span data-stu-id="64f92-123">The date and time when the page was created.</span></span> <span data-ttu-id="64f92-124">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="64f92-124">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="64f92-125">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="64f92-125">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="64f92-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="64f92-126">Read-only.</span></span>|
|<span data-ttu-id="64f92-127">id</span><span class="sxs-lookup"><span data-stu-id="64f92-127">id</span></span>|<span data-ttu-id="64f92-128">String</span><span class="sxs-lookup"><span data-stu-id="64f92-128">String</span></span>|<span data-ttu-id="64f92-129">Уникальный идентификатор страницы.</span><span class="sxs-lookup"><span data-stu-id="64f92-129">The unique identifier of the page.</span></span>  <span data-ttu-id="64f92-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="64f92-130">Read-only.</span></span>|
|<span data-ttu-id="64f92-131">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="64f92-131">lastModifiedDateTime</span></span>|<span data-ttu-id="64f92-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64f92-132">DateTimeOffset</span></span>|<span data-ttu-id="64f92-133">Дата и время последнего изменения страницы.</span><span class="sxs-lookup"><span data-stu-id="64f92-133">The date and time when the page was last modified.</span></span> <span data-ttu-id="64f92-134">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="64f92-134">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="64f92-135">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="64f92-135">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="64f92-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="64f92-136">Read-only.</span></span>|
|<span data-ttu-id="64f92-137">степень</span><span class="sxs-lookup"><span data-stu-id="64f92-137">level</span></span>|<span data-ttu-id="64f92-138">Int32</span><span class="sxs-lookup"><span data-stu-id="64f92-138">Int32</span></span>|<span data-ttu-id="64f92-139">Уровень отступа страницы.</span><span class="sxs-lookup"><span data-stu-id="64f92-139">The indentation level of the page.</span></span> <span data-ttu-id="64f92-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="64f92-140">Read-only.</span></span>|
|<span data-ttu-id="64f92-141">links</span><span class="sxs-lookup"><span data-stu-id="64f92-141">links</span></span>|[<span data-ttu-id="64f92-142">пажелинкс</span><span class="sxs-lookup"><span data-stu-id="64f92-142">pageLinks</span></span>](pagelinks.md)|<span data-ttu-id="64f92-143">Ссылки для открытия страницы.</span><span class="sxs-lookup"><span data-stu-id="64f92-143">Links for opening the page.</span></span> <span data-ttu-id="64f92-144">`oneNoteClientURL`Ссылка открывает страницу в собственном клиенте OneNote, если она установлена.</span><span class="sxs-lookup"><span data-stu-id="64f92-144">The `oneNoteClientURL` link opens the page in the OneNote native client if it 's installed.</span></span> <span data-ttu-id="64f92-145">`oneNoteWebUrl`Ссылка открывает страницу в OneNote в Интернете.</span><span class="sxs-lookup"><span data-stu-id="64f92-145">The `oneNoteWebUrl` link opens the page in OneNote on the web.</span></span> <span data-ttu-id="64f92-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="64f92-146">Read-only.</span></span>|
|<span data-ttu-id="64f92-147">порядке</span><span class="sxs-lookup"><span data-stu-id="64f92-147">order</span></span>|<span data-ttu-id="64f92-148">Int32</span><span class="sxs-lookup"><span data-stu-id="64f92-148">Int32</span></span>|<span data-ttu-id="64f92-149">Порядок страницы в родительском разделе.</span><span class="sxs-lookup"><span data-stu-id="64f92-149">The order of the page within its parent section.</span></span> <span data-ttu-id="64f92-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="64f92-150">Read-only.</span></span>|
|<span data-ttu-id="64f92-151">Self</span><span class="sxs-lookup"><span data-stu-id="64f92-151">self</span></span>|<span data-ttu-id="64f92-152">String</span><span class="sxs-lookup"><span data-stu-id="64f92-152">String</span></span>|<span data-ttu-id="64f92-153">Конечная точка, в которой можно получить сведения о странице.</span><span class="sxs-lookup"><span data-stu-id="64f92-153">The endpoint where you can get details about the page.</span></span> <span data-ttu-id="64f92-154">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="64f92-154">Read-only.</span></span>|
|<span data-ttu-id="64f92-155">title</span><span class="sxs-lookup"><span data-stu-id="64f92-155">title</span></span>|<span data-ttu-id="64f92-156">String</span><span class="sxs-lookup"><span data-stu-id="64f92-156">String</span></span>|<span data-ttu-id="64f92-157">Заголовок страницы.</span><span class="sxs-lookup"><span data-stu-id="64f92-157">The title of the page.</span></span> |

## <a name="relationships"></a><span data-ttu-id="64f92-158">Отношения</span><span class="sxs-lookup"><span data-stu-id="64f92-158">Relationships</span></span>
| <span data-ttu-id="64f92-159">Связь</span><span class="sxs-lookup"><span data-stu-id="64f92-159">Relationship</span></span> | <span data-ttu-id="64f92-160">Тип</span><span class="sxs-lookup"><span data-stu-id="64f92-160">Type</span></span>   |<span data-ttu-id="64f92-161">Описание</span><span class="sxs-lookup"><span data-stu-id="64f92-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="64f92-162">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="64f92-162">parentNotebook</span></span>|[<span data-ttu-id="64f92-163">notebook</span><span class="sxs-lookup"><span data-stu-id="64f92-163">notebook</span></span>](notebook.md)|<span data-ttu-id="64f92-164">Записная книжка, содержащая страницу.</span><span class="sxs-lookup"><span data-stu-id="64f92-164">The notebook that contains the page.</span></span>  <span data-ttu-id="64f92-165">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="64f92-165">Read-only.</span></span>|
|<span data-ttu-id="64f92-166">parentSection</span><span class="sxs-lookup"><span data-stu-id="64f92-166">parentSection</span></span>|[<span data-ttu-id="64f92-167">оненотесектион</span><span class="sxs-lookup"><span data-stu-id="64f92-167">onenoteSection</span></span>](onenotesection.md)|<span data-ttu-id="64f92-168">Раздел, содержащий страницу.</span><span class="sxs-lookup"><span data-stu-id="64f92-168">The section that contains the page.</span></span> <span data-ttu-id="64f92-169">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="64f92-169">Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="64f92-170">Методы</span><span class="sxs-lookup"><span data-stu-id="64f92-170">Methods</span></span>

| <span data-ttu-id="64f92-171">Метод</span><span class="sxs-lookup"><span data-stu-id="64f92-171">Method</span></span>           | <span data-ttu-id="64f92-172">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="64f92-172">Return Type</span></span>    |<span data-ttu-id="64f92-173">Описание</span><span class="sxs-lookup"><span data-stu-id="64f92-173">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="64f92-174">Вывод страницы</span><span class="sxs-lookup"><span data-stu-id="64f92-174">Get page</span></span>](../api/page-get.md) | [<span data-ttu-id="64f92-175">оненотепаже</span><span class="sxs-lookup"><span data-stu-id="64f92-175">onenotePage</span></span>](onenotepage.md) |<span data-ttu-id="64f92-176">Чтение свойств и связей страницы.</span><span class="sxs-lookup"><span data-stu-id="64f92-176">Read the properties and relationships of the page.</span></span>|
|[<span data-ttu-id="64f92-177">Обновление содержимого страницы</span><span class="sxs-lookup"><span data-stu-id="64f92-177">Update page content</span></span>](../api/page-update.md) | <span data-ttu-id="64f92-178">Нет</span><span class="sxs-lookup"><span data-stu-id="64f92-178">None</span></span> |<span data-ttu-id="64f92-179">Обновление HTML-содержимого страницы.</span><span class="sxs-lookup"><span data-stu-id="64f92-179">Update the HTML content of the page.</span></span> |
|[<span data-ttu-id="64f92-180">Удаление страницы</span><span class="sxs-lookup"><span data-stu-id="64f92-180">Delete page</span></span>](../api/page-delete.md) | <span data-ttu-id="64f92-181">Нет</span><span class="sxs-lookup"><span data-stu-id="64f92-181">None</span></span> |<span data-ttu-id="64f92-182">Удаление страницы.</span><span class="sxs-lookup"><span data-stu-id="64f92-182">Delete the page.</span></span> |
|[<span data-ttu-id="64f92-183">copyToSection</span><span class="sxs-lookup"><span data-stu-id="64f92-183">copyToSection</span></span>](../api/page-copytosection.md)| <span data-ttu-id="64f92-184">Нет</span><span class="sxs-lookup"><span data-stu-id="64f92-184">None</span></span> |<span data-ttu-id="64f92-185">Копирует страницу в определенный раздел.</span><span class="sxs-lookup"><span data-stu-id="64f92-185">Copies the page to a specific section.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="64f92-186">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="64f92-186">JSON representation</span></span>

<span data-ttu-id="64f92-187">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="64f92-187">Here is a JSON representation of the resource.</span></span>

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
