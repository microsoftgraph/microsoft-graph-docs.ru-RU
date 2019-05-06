---
title: Тип ресурса Оненотепаже
description: Страница в записной книжке OneNote.
localization_priority: Normal
ms.openlocfilehash: 04e06fefd0b48a5d794f20733a4755e030cb7e0d
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630799"
---
# <a name="onenotepage-resource-type"></a><span data-ttu-id="03263-103">Тип ресурса Оненотепаже</span><span class="sxs-lookup"><span data-stu-id="03263-103">onenotePage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03263-104">Страница в записной книжке OneNote.</span><span class="sxs-lookup"><span data-stu-id="03263-104">A page in a OneNote notebook.</span></span>

## <a name="properties"></a><span data-ttu-id="03263-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="03263-105">Properties</span></span>
| <span data-ttu-id="03263-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="03263-106">Property</span></span>     | <span data-ttu-id="03263-107">Тип</span><span class="sxs-lookup"><span data-stu-id="03263-107">Type</span></span>   |<span data-ttu-id="03263-108">Описание</span><span class="sxs-lookup"><span data-stu-id="03263-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="03263-109">содержимое</span><span class="sxs-lookup"><span data-stu-id="03263-109">content</span></span>|<span data-ttu-id="03263-110">Поток</span><span class="sxs-lookup"><span data-stu-id="03263-110">Stream</span></span>|<span data-ttu-id="03263-111">HTML-контент страницы.</span><span class="sxs-lookup"><span data-stu-id="03263-111">The page's HTML content.</span></span>|
|<span data-ttu-id="03263-112">contentUrl</span><span class="sxs-lookup"><span data-stu-id="03263-112">contentUrl</span></span>|<span data-ttu-id="03263-113">String</span><span class="sxs-lookup"><span data-stu-id="03263-113">String</span></span>|<span data-ttu-id="03263-114">URL-адрес HTML-содержимого страницы.</span><span class="sxs-lookup"><span data-stu-id="03263-114">The URL for the page's HTML content.</span></span>  <span data-ttu-id="03263-115">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="03263-115">Read-only.</span></span>|
|<span data-ttu-id="03263-116">Креатедбяппид</span><span class="sxs-lookup"><span data-stu-id="03263-116">createdByAppId</span></span>|<span data-ttu-id="03263-117">String</span><span class="sxs-lookup"><span data-stu-id="03263-117">String</span></span>|<span data-ttu-id="03263-118">Уникальный идентификатор приложения, создавшего страницу.</span><span class="sxs-lookup"><span data-stu-id="03263-118">The unique identifier of the application that created the page.</span></span> <span data-ttu-id="03263-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="03263-119">Read-only.</span></span>|
|<span data-ttu-id="03263-120">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="03263-120">createdDateTime</span></span>|<span data-ttu-id="03263-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03263-121">DateTimeOffset</span></span>|<span data-ttu-id="03263-122">Дата и время создания страницы.</span><span class="sxs-lookup"><span data-stu-id="03263-122">The date and time when the page was created.</span></span> <span data-ttu-id="03263-123">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="03263-123">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="03263-124">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="03263-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="03263-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="03263-125">Read-only.</span></span>|
|<span data-ttu-id="03263-126">id</span><span class="sxs-lookup"><span data-stu-id="03263-126">id</span></span>|<span data-ttu-id="03263-127">String</span><span class="sxs-lookup"><span data-stu-id="03263-127">String</span></span>|<span data-ttu-id="03263-128">Уникальный идентификатор страницы.</span><span class="sxs-lookup"><span data-stu-id="03263-128">The unique identifier of the page.</span></span>  <span data-ttu-id="03263-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="03263-129">Read-only.</span></span>|
|<span data-ttu-id="03263-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="03263-130">lastModifiedDateTime</span></span>|<span data-ttu-id="03263-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03263-131">DateTimeOffset</span></span>|<span data-ttu-id="03263-132">Дата и время последнего изменения страницы.</span><span class="sxs-lookup"><span data-stu-id="03263-132">The date and time when the page was last modified.</span></span> <span data-ttu-id="03263-133">Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="03263-133">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="03263-134">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="03263-134">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="03263-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="03263-135">Read-only.</span></span>|
|<span data-ttu-id="03263-136">степень</span><span class="sxs-lookup"><span data-stu-id="03263-136">level</span></span>|<span data-ttu-id="03263-137">Int32</span><span class="sxs-lookup"><span data-stu-id="03263-137">Int32</span></span>|<span data-ttu-id="03263-138">Уровень отступа страницы.</span><span class="sxs-lookup"><span data-stu-id="03263-138">The indentation level of the page.</span></span> <span data-ttu-id="03263-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="03263-139">Read-only.</span></span>|
|<span data-ttu-id="03263-140">links</span><span class="sxs-lookup"><span data-stu-id="03263-140">links</span></span>|[<span data-ttu-id="03263-141">Пажелинкс</span><span class="sxs-lookup"><span data-stu-id="03263-141">pageLinks</span></span>](pagelinks.md)|<span data-ttu-id="03263-142">Ссылки для открытия страницы.</span><span class="sxs-lookup"><span data-stu-id="03263-142">Links for opening the page.</span></span> <span data-ttu-id="03263-143">`oneNoteClientURL` Ссылка открывает страницу в собственном клиенте OneNote, если она установлена.</span><span class="sxs-lookup"><span data-stu-id="03263-143">The `oneNoteClientURL` link opens the page in the OneNote native client if it 's installed.</span></span> <span data-ttu-id="03263-144">`oneNoteWebUrl` Ссылка открывает страницу в OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="03263-144">The `oneNoteWebUrl` link opens the page in OneNote Online.</span></span> <span data-ttu-id="03263-145">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="03263-145">Read-only.</span></span>|
|<span data-ttu-id="03263-146">порядке</span><span class="sxs-lookup"><span data-stu-id="03263-146">order</span></span>|<span data-ttu-id="03263-147">Int32</span><span class="sxs-lookup"><span data-stu-id="03263-147">Int32</span></span>|<span data-ttu-id="03263-148">Порядок страницы в родительском разделе.</span><span class="sxs-lookup"><span data-stu-id="03263-148">The order of the page within its parent section.</span></span> <span data-ttu-id="03263-149">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="03263-149">Read-only.</span></span>|
|<span data-ttu-id="03263-150">Self</span><span class="sxs-lookup"><span data-stu-id="03263-150">self</span></span>|<span data-ttu-id="03263-151">String</span><span class="sxs-lookup"><span data-stu-id="03263-151">String</span></span>|<span data-ttu-id="03263-152">Конечная точка, в которой можно получить сведения о странице.</span><span class="sxs-lookup"><span data-stu-id="03263-152">The endpoint where you can get details about the page.</span></span> <span data-ttu-id="03263-153">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="03263-153">Read-only.</span></span>|
|<span data-ttu-id="03263-154">title</span><span class="sxs-lookup"><span data-stu-id="03263-154">title</span></span>|<span data-ttu-id="03263-155">String</span><span class="sxs-lookup"><span data-stu-id="03263-155">String</span></span>|<span data-ttu-id="03263-156">Заголовок страницы.</span><span class="sxs-lookup"><span data-stu-id="03263-156">The title of the page.</span></span> |

## <a name="relationships"></a><span data-ttu-id="03263-157">Связи</span><span class="sxs-lookup"><span data-stu-id="03263-157">Relationships</span></span>
| <span data-ttu-id="03263-158">Отношение</span><span class="sxs-lookup"><span data-stu-id="03263-158">Relationship</span></span> | <span data-ttu-id="03263-159">Тип</span><span class="sxs-lookup"><span data-stu-id="03263-159">Type</span></span>   |<span data-ttu-id="03263-160">Описание</span><span class="sxs-lookup"><span data-stu-id="03263-160">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="03263-161">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="03263-161">parentNotebook</span></span>|[<span data-ttu-id="03263-162">записной книжки</span><span class="sxs-lookup"><span data-stu-id="03263-162">notebook</span></span>](notebook.md)|<span data-ttu-id="03263-163">Записная книжка, содержащая страницу.</span><span class="sxs-lookup"><span data-stu-id="03263-163">The notebook that contains the page.</span></span>  <span data-ttu-id="03263-164">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="03263-164">Read-only.</span></span>|
|<span data-ttu-id="03263-165">parentSection</span><span class="sxs-lookup"><span data-stu-id="03263-165">parentSection</span></span>|[<span data-ttu-id="03263-166">Оненотесектион</span><span class="sxs-lookup"><span data-stu-id="03263-166">onenoteSection</span></span>](onenotesection.md)|<span data-ttu-id="03263-167">Раздел, содержащий страницу.</span><span class="sxs-lookup"><span data-stu-id="03263-167">The section that contains the page.</span></span> <span data-ttu-id="03263-168">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="03263-168">Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="03263-169">Методы</span><span class="sxs-lookup"><span data-stu-id="03263-169">Methods</span></span>

| <span data-ttu-id="03263-170">Метод</span><span class="sxs-lookup"><span data-stu-id="03263-170">Method</span></span>           | <span data-ttu-id="03263-171">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="03263-171">Return Type</span></span>    |<span data-ttu-id="03263-172">Описание</span><span class="sxs-lookup"><span data-stu-id="03263-172">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="03263-173">Вывод страницы</span><span class="sxs-lookup"><span data-stu-id="03263-173">Get page</span></span>](../api/page-get.md) | [<span data-ttu-id="03263-174">Оненотепаже</span><span class="sxs-lookup"><span data-stu-id="03263-174">onenotePage</span></span>](onenotepage.md) |<span data-ttu-id="03263-175">Чтение свойств и связей страницы.</span><span class="sxs-lookup"><span data-stu-id="03263-175">Read the properties and relationships of the page.</span></span>|
|[<span data-ttu-id="03263-176">Обновление содержимого страницы</span><span class="sxs-lookup"><span data-stu-id="03263-176">Update page content</span></span>](../api/page-update.md) | <span data-ttu-id="03263-177">Нет</span><span class="sxs-lookup"><span data-stu-id="03263-177">None</span></span> |<span data-ttu-id="03263-178">Обновление HTML-содержимого страницы.</span><span class="sxs-lookup"><span data-stu-id="03263-178">Update the HTML content of the page.</span></span> |
|[<span data-ttu-id="03263-179">Удаление страницы</span><span class="sxs-lookup"><span data-stu-id="03263-179">Delete page</span></span>](../api/page-delete.md) | <span data-ttu-id="03263-180">Нет</span><span class="sxs-lookup"><span data-stu-id="03263-180">None</span></span> |<span data-ttu-id="03263-181">Удаление страницы.</span><span class="sxs-lookup"><span data-stu-id="03263-181">Delete the page.</span></span> |
|[<span data-ttu-id="03263-182">copyToSection</span><span class="sxs-lookup"><span data-stu-id="03263-182">copyToSection</span></span>](../api/page-copytosection.md)| <span data-ttu-id="03263-183">Нет</span><span class="sxs-lookup"><span data-stu-id="03263-183">None</span></span> |<span data-ttu-id="03263-184">Копирует страницу в определенный раздел.</span><span class="sxs-lookup"><span data-stu-id="03263-184">Copies the page to a specific section.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="03263-185">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="03263-185">JSON representation</span></span>

<span data-ttu-id="03263-186">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="03263-186">Here is a JSON representation of the resource.</span></span>

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
