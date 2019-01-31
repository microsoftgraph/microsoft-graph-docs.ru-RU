---
title: Тип ресурса page
description: Страница в записной книжке OneNote.
localization_priority: Normal
ms.openlocfilehash: d8c27cdc144e9b192bd0205f256653ff7f04df5f
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29649451"
---
# <a name="page-resource-type"></a><span data-ttu-id="f70b2-103">Тип ресурса page</span><span class="sxs-lookup"><span data-stu-id="f70b2-103">page resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f70b2-104">Страница в записной книжке OneNote.</span><span class="sxs-lookup"><span data-stu-id="f70b2-104">A page in a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f70b2-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f70b2-105">JSON representation</span></span>

<span data-ttu-id="f70b2-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f70b2-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "parentNotebook",
    "parentSection"
  ],
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
## <a name="properties"></a><span data-ttu-id="f70b2-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f70b2-107">Properties</span></span>
| <span data-ttu-id="f70b2-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f70b2-108">Property</span></span>     | <span data-ttu-id="f70b2-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f70b2-109">Type</span></span>   |<span data-ttu-id="f70b2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f70b2-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f70b2-111">content</span><span class="sxs-lookup"><span data-stu-id="f70b2-111">content</span></span>|<span data-ttu-id="f70b2-112">Поток</span><span class="sxs-lookup"><span data-stu-id="f70b2-112">Stream</span></span>|<span data-ttu-id="f70b2-113">HTML-содержимое страницы.</span><span class="sxs-lookup"><span data-stu-id="f70b2-113">The page's HTML content.</span></span>|
|<span data-ttu-id="f70b2-114">contentUrl</span><span class="sxs-lookup"><span data-stu-id="f70b2-114">contentUrl</span></span>|<span data-ttu-id="f70b2-115">String</span><span class="sxs-lookup"><span data-stu-id="f70b2-115">String</span></span>|<span data-ttu-id="f70b2-p101">URL-адрес HTML-содержимого страницы.  Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f70b2-p101">The URL for the page's HTML content.  Read-only.</span></span>|
|<span data-ttu-id="f70b2-118">createdByAppId</span><span class="sxs-lookup"><span data-stu-id="f70b2-118">createdByAppId</span></span>|<span data-ttu-id="f70b2-119">String</span><span class="sxs-lookup"><span data-stu-id="f70b2-119">String</span></span>|<span data-ttu-id="f70b2-p102">Уникальный идентификатор приложения, которое создало страницу. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f70b2-p102">The unique identifier of the application that created the page. Read-only.</span></span>|
|<span data-ttu-id="f70b2-122">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f70b2-122">createdDateTime</span></span>|<span data-ttu-id="f70b2-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f70b2-123">DateTimeOffset</span></span>|<span data-ttu-id="f70b2-p103">Дата и время создания страницы. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f70b2-p103">The date and time when the page was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="f70b2-128">id</span><span class="sxs-lookup"><span data-stu-id="f70b2-128">id</span></span>|<span data-ttu-id="f70b2-129">String</span><span class="sxs-lookup"><span data-stu-id="f70b2-129">String</span></span>|<span data-ttu-id="f70b2-p104">Уникальный идентификатор страницы.  Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f70b2-p104">The unique identifier of the page.  Read-only.</span></span>|
|<span data-ttu-id="f70b2-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f70b2-132">lastModifiedDateTime</span></span>|<span data-ttu-id="f70b2-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f70b2-133">DateTimeOffset</span></span>|<span data-ttu-id="f70b2-p105">Дата и время последнего изменения страницы. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f70b2-p105">The date and time when the page was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="f70b2-138">level</span><span class="sxs-lookup"><span data-stu-id="f70b2-138">level</span></span>|<span data-ttu-id="f70b2-139">Int32</span><span class="sxs-lookup"><span data-stu-id="f70b2-139">Int32</span></span>|<span data-ttu-id="f70b2-p106">Уровень отступа для страницы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f70b2-p106">The indentation level of the page. Read-only.</span></span>|
|<span data-ttu-id="f70b2-142">links</span><span class="sxs-lookup"><span data-stu-id="f70b2-142">links</span></span>|[<span data-ttu-id="f70b2-143">PageLinks</span><span class="sxs-lookup"><span data-stu-id="f70b2-143">PageLinks</span></span>](pagelinks.md)|<span data-ttu-id="f70b2-p107">Ссылки для открытия страницы. Ссылка `oneNoteClientURL` открывает страницу в клиенте OneNote, если он установлен. Ссылка `oneNoteWebUrl` открывает страницу в OneNote Online. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f70b2-p107">Links for opening the page. The `oneNoteClientURL` link opens the page in the OneNote native client if it 's installed. The `oneNoteWebUrl` link opens the page in OneNote Online. Read-only.</span></span>|
|<span data-ttu-id="f70b2-148">order</span><span class="sxs-lookup"><span data-stu-id="f70b2-148">order</span></span>|<span data-ttu-id="f70b2-149">Int32</span><span class="sxs-lookup"><span data-stu-id="f70b2-149">Int32</span></span>|<span data-ttu-id="f70b2-p108">Расположение страницы в родительском разделе. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f70b2-p108">The order of the page within its parent section. Read-only.</span></span>|
|<span data-ttu-id="f70b2-152">self</span><span class="sxs-lookup"><span data-stu-id="f70b2-152">self</span></span>|<span data-ttu-id="f70b2-153">String</span><span class="sxs-lookup"><span data-stu-id="f70b2-153">String</span></span>|<span data-ttu-id="f70b2-p109">Конечная точка, в которой можно получить сведения о странице. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f70b2-p109">The endpoint where you can get details about the page. Read-only.</span></span>|
|<span data-ttu-id="f70b2-156">title</span><span class="sxs-lookup"><span data-stu-id="f70b2-156">title</span></span>|<span data-ttu-id="f70b2-157">Строка</span><span class="sxs-lookup"><span data-stu-id="f70b2-157">String</span></span>|<span data-ttu-id="f70b2-158">Заголовок страницы.</span><span class="sxs-lookup"><span data-stu-id="f70b2-158">The title of the page.</span></span> |

## <a name="relationships"></a><span data-ttu-id="f70b2-159">Отношения</span><span class="sxs-lookup"><span data-stu-id="f70b2-159">Relationships</span></span>
| <span data-ttu-id="f70b2-160">Связь</span><span class="sxs-lookup"><span data-stu-id="f70b2-160">Relationship</span></span> | <span data-ttu-id="f70b2-161">Тип</span><span class="sxs-lookup"><span data-stu-id="f70b2-161">Type</span></span>   |<span data-ttu-id="f70b2-162">Описание</span><span class="sxs-lookup"><span data-stu-id="f70b2-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f70b2-163">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="f70b2-163">parentNotebook</span></span>|[<span data-ttu-id="f70b2-164">Notebook</span><span class="sxs-lookup"><span data-stu-id="f70b2-164">Notebook</span></span>](notebook.md)|<span data-ttu-id="f70b2-p110">Записная книжка, содержащая страницу.  Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f70b2-p110">The notebook that contains the page.  Read-only.</span></span>|
|<span data-ttu-id="f70b2-167">parentSection</span><span class="sxs-lookup"><span data-stu-id="f70b2-167">parentSection</span></span>|[<span data-ttu-id="f70b2-168">Section</span><span class="sxs-lookup"><span data-stu-id="f70b2-168">Section</span></span>](section.md)|<span data-ttu-id="f70b2-p111">Раздел, содержащий страницу. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f70b2-p111">The section that contains the page. Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="f70b2-171">Методы</span><span class="sxs-lookup"><span data-stu-id="f70b2-171">Methods</span></span>

| <span data-ttu-id="f70b2-172">Метод</span><span class="sxs-lookup"><span data-stu-id="f70b2-172">Method</span></span>           | <span data-ttu-id="f70b2-173">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f70b2-173">Return Type</span></span>    |<span data-ttu-id="f70b2-174">Описание</span><span class="sxs-lookup"><span data-stu-id="f70b2-174">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f70b2-175">Получение страницы</span><span class="sxs-lookup"><span data-stu-id="f70b2-175">Get page</span></span>](../api/page-get.md) | [<span data-ttu-id="f70b2-176">Page</span><span class="sxs-lookup"><span data-stu-id="f70b2-176">Page</span></span>](page.md) |<span data-ttu-id="f70b2-177">Чтение свойств и отношений страницы.</span><span class="sxs-lookup"><span data-stu-id="f70b2-177">Read the properties and relationships of the page.</span></span>|
|[<span data-ttu-id="f70b2-178">Обновление содержимого страницы</span><span class="sxs-lookup"><span data-stu-id="f70b2-178">Update page content</span></span>](../api/page-update.md) | <span data-ttu-id="f70b2-179">Нет</span><span class="sxs-lookup"><span data-stu-id="f70b2-179">None</span></span> |<span data-ttu-id="f70b2-180">Обновление HTML-содержимого страницы.</span><span class="sxs-lookup"><span data-stu-id="f70b2-180">Update the HTML content of the page.</span></span> |
|[<span data-ttu-id="f70b2-181">Удаление страницы</span><span class="sxs-lookup"><span data-stu-id="f70b2-181">Delete page</span></span>](../api/page-delete.md) | <span data-ttu-id="f70b2-182">Нет</span><span class="sxs-lookup"><span data-stu-id="f70b2-182">None</span></span> |<span data-ttu-id="f70b2-183">Удаление страницы.</span><span class="sxs-lookup"><span data-stu-id="f70b2-183">Delete the page.</span></span> |
|[<span data-ttu-id="f70b2-184">copyToSection</span><span class="sxs-lookup"><span data-stu-id="f70b2-184">copyToSection</span></span>](../api/page-copytosection.md)| <span data-ttu-id="f70b2-185">Нет</span><span class="sxs-lookup"><span data-stu-id="f70b2-185">None</span></span> |<span data-ttu-id="f70b2-186">Копирование страницы в определенный раздел.</span><span class="sxs-lookup"><span data-stu-id="f70b2-186">Copies the page to a specific section.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/page.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
