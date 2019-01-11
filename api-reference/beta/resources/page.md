---
title: Тип ресурса page
description: Страница в записной книжке OneNote.
localization_priority: Normal
ms.openlocfilehash: 5928f430fcbfe9f41c6aa83e99d7dfe737e8e1c7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27850136"
---
# <a name="page-resource-type"></a><span data-ttu-id="f4512-103">Тип ресурса page</span><span class="sxs-lookup"><span data-stu-id="f4512-103">page resource type</span></span>

> <span data-ttu-id="f4512-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f4512-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f4512-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4512-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f4512-106">Страница в записной книжке OneNote.</span><span class="sxs-lookup"><span data-stu-id="f4512-106">A page in a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f4512-107">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f4512-107">JSON representation</span></span>

<span data-ttu-id="f4512-108">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f4512-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="f4512-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="f4512-109">Properties</span></span>
| <span data-ttu-id="f4512-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="f4512-110">Property</span></span>     | <span data-ttu-id="f4512-111">Тип</span><span class="sxs-lookup"><span data-stu-id="f4512-111">Type</span></span>   |<span data-ttu-id="f4512-112">Описание</span><span class="sxs-lookup"><span data-stu-id="f4512-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f4512-113">content</span><span class="sxs-lookup"><span data-stu-id="f4512-113">content</span></span>|<span data-ttu-id="f4512-114">Поток</span><span class="sxs-lookup"><span data-stu-id="f4512-114">Stream</span></span>|<span data-ttu-id="f4512-115">HTML-содержимое страницы.</span><span class="sxs-lookup"><span data-stu-id="f4512-115">The page's HTML content.</span></span>|
|<span data-ttu-id="f4512-116">contentUrl</span><span class="sxs-lookup"><span data-stu-id="f4512-116">contentUrl</span></span>|<span data-ttu-id="f4512-117">Строка</span><span class="sxs-lookup"><span data-stu-id="f4512-117">String</span></span>|<span data-ttu-id="f4512-p102">URL-адрес HTML-содержимого страницы.  Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f4512-p102">The URL for the page's HTML content.  Read-only.</span></span>|
|<span data-ttu-id="f4512-120">createdByAppId</span><span class="sxs-lookup"><span data-stu-id="f4512-120">createdByAppId</span></span>|<span data-ttu-id="f4512-121">Строка</span><span class="sxs-lookup"><span data-stu-id="f4512-121">String</span></span>|<span data-ttu-id="f4512-p103">Уникальный идентификатор приложения, которое создало страницу. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f4512-p103">The unique identifier of the application that created the page. Read-only.</span></span>|
|<span data-ttu-id="f4512-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f4512-124">createdDateTime</span></span>|<span data-ttu-id="f4512-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4512-125">DateTimeOffset</span></span>|<span data-ttu-id="f4512-p104">Дата и время создания страницы. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f4512-p104">The date and time when the page was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="f4512-130">id</span><span class="sxs-lookup"><span data-stu-id="f4512-130">id</span></span>|<span data-ttu-id="f4512-131">Строка</span><span class="sxs-lookup"><span data-stu-id="f4512-131">String</span></span>|<span data-ttu-id="f4512-p105">Уникальный идентификатор страницы.  Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f4512-p105">The unique identifier of the page.  Read-only.</span></span>|
|<span data-ttu-id="f4512-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f4512-134">lastModifiedDateTime</span></span>|<span data-ttu-id="f4512-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4512-135">DateTimeOffset</span></span>|<span data-ttu-id="f4512-p106">Дата и время последнего изменения страницы. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f4512-p106">The date and time when the page was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="f4512-140">level</span><span class="sxs-lookup"><span data-stu-id="f4512-140">level</span></span>|<span data-ttu-id="f4512-141">Int32</span><span class="sxs-lookup"><span data-stu-id="f4512-141">Int32</span></span>|<span data-ttu-id="f4512-p107">Уровень отступа для страницы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f4512-p107">The indentation level of the page. Read-only.</span></span>|
|<span data-ttu-id="f4512-144">links</span><span class="sxs-lookup"><span data-stu-id="f4512-144">links</span></span>|[<span data-ttu-id="f4512-145">PageLinks</span><span class="sxs-lookup"><span data-stu-id="f4512-145">PageLinks</span></span>](pagelinks.md)|<span data-ttu-id="f4512-p108">Ссылки для открытия страницы. Ссылка `oneNoteClientURL` открывает страницу в клиенте OneNote, если он установлен. Ссылка `oneNoteWebUrl` открывает страницу в OneNote Online. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f4512-p108">Links for opening the page. The `oneNoteClientURL` link opens the page in the OneNote native client if it 's installed. The `oneNoteWebUrl` link opens the page in OneNote Online. Read-only.</span></span>|
|<span data-ttu-id="f4512-150">order</span><span class="sxs-lookup"><span data-stu-id="f4512-150">order</span></span>|<span data-ttu-id="f4512-151">Int32</span><span class="sxs-lookup"><span data-stu-id="f4512-151">Int32</span></span>|<span data-ttu-id="f4512-p109">Расположение страницы в родительском разделе. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f4512-p109">The order of the page within its parent section. Read-only.</span></span>|
|<span data-ttu-id="f4512-154">self</span><span class="sxs-lookup"><span data-stu-id="f4512-154">self</span></span>|<span data-ttu-id="f4512-155">Строка</span><span class="sxs-lookup"><span data-stu-id="f4512-155">String</span></span>|<span data-ttu-id="f4512-p110">Конечная точка, в которой можно получить сведения о странице. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f4512-p110">The endpoint where you can get details about the page. Read-only.</span></span>|
|<span data-ttu-id="f4512-158">title</span><span class="sxs-lookup"><span data-stu-id="f4512-158">title</span></span>|<span data-ttu-id="f4512-159">Строка</span><span class="sxs-lookup"><span data-stu-id="f4512-159">String</span></span>|<span data-ttu-id="f4512-160">Заголовок страницы.</span><span class="sxs-lookup"><span data-stu-id="f4512-160">The title of the page.</span></span> |

## <a name="relationships"></a><span data-ttu-id="f4512-161">Отношения</span><span class="sxs-lookup"><span data-stu-id="f4512-161">Relationships</span></span>
| <span data-ttu-id="f4512-162">Связь</span><span class="sxs-lookup"><span data-stu-id="f4512-162">Relationship</span></span> | <span data-ttu-id="f4512-163">Тип</span><span class="sxs-lookup"><span data-stu-id="f4512-163">Type</span></span>   |<span data-ttu-id="f4512-164">Описание</span><span class="sxs-lookup"><span data-stu-id="f4512-164">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f4512-165">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="f4512-165">parentNotebook</span></span>|[<span data-ttu-id="f4512-166">Notebook</span><span class="sxs-lookup"><span data-stu-id="f4512-166">Notebook</span></span>](notebook.md)|<span data-ttu-id="f4512-p111">Записная книжка, содержащая страницу.  Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f4512-p111">The notebook that contains the page.  Read-only.</span></span>|
|<span data-ttu-id="f4512-169">parentSection</span><span class="sxs-lookup"><span data-stu-id="f4512-169">parentSection</span></span>|[<span data-ttu-id="f4512-170">Section</span><span class="sxs-lookup"><span data-stu-id="f4512-170">Section</span></span>](section.md)|<span data-ttu-id="f4512-p112">Раздел, содержащий страницу. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f4512-p112">The section that contains the page. Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="f4512-173">Методы</span><span class="sxs-lookup"><span data-stu-id="f4512-173">Methods</span></span>

| <span data-ttu-id="f4512-174">Метод</span><span class="sxs-lookup"><span data-stu-id="f4512-174">Method</span></span>           | <span data-ttu-id="f4512-175">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f4512-175">Return Type</span></span>    |<span data-ttu-id="f4512-176">Описание</span><span class="sxs-lookup"><span data-stu-id="f4512-176">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f4512-177">Получение страницы</span><span class="sxs-lookup"><span data-stu-id="f4512-177">Get page</span></span>](../api/page-get.md) | [<span data-ttu-id="f4512-178">Page</span><span class="sxs-lookup"><span data-stu-id="f4512-178">Page</span></span>](page.md) |<span data-ttu-id="f4512-179">Чтение свойств и отношений страницы.</span><span class="sxs-lookup"><span data-stu-id="f4512-179">Read the properties and relationships of the page.</span></span>|
|[<span data-ttu-id="f4512-180">Обновление содержимого страницы</span><span class="sxs-lookup"><span data-stu-id="f4512-180">Update page content</span></span>](../api/page-update.md) | <span data-ttu-id="f4512-181">Нет</span><span class="sxs-lookup"><span data-stu-id="f4512-181">None</span></span> |<span data-ttu-id="f4512-182">Обновление HTML-содержимого страницы.</span><span class="sxs-lookup"><span data-stu-id="f4512-182">Update the HTML content of the page.</span></span> |
|[<span data-ttu-id="f4512-183">Удаление страницы</span><span class="sxs-lookup"><span data-stu-id="f4512-183">Delete page</span></span>](../api/page-delete.md) | <span data-ttu-id="f4512-184">Нет</span><span class="sxs-lookup"><span data-stu-id="f4512-184">None</span></span> |<span data-ttu-id="f4512-185">Удаление страницы.</span><span class="sxs-lookup"><span data-stu-id="f4512-185">Delete the page.</span></span> |
|[<span data-ttu-id="f4512-186">copyToSection</span><span class="sxs-lookup"><span data-stu-id="f4512-186">copyToSection</span></span>](../api/page-copytosection.md)| <span data-ttu-id="f4512-187">Нет</span><span class="sxs-lookup"><span data-stu-id="f4512-187">None</span></span> |<span data-ttu-id="f4512-188">Копирование страницы в определенный раздел.</span><span class="sxs-lookup"><span data-stu-id="f4512-188">Copies the page to a specific section.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
