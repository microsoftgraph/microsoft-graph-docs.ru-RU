---
author: JeremyKelley
ms.date: 09/11/2017
title: ListInfo
localization_priority: Normal
ms.prod: sharepoint
description: Сложный тип listInfo используется для хранения дополнительных сведений о списке.
doc_type: resourcePageType
ms.openlocfilehash: c5d84f5fae89e6ecf433dad20a959f9846f58006
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239361"
---
# <a name="listinfo-resource"></a><span data-ttu-id="cb4e3-103">Ресурс listInfo</span><span class="sxs-lookup"><span data-stu-id="cb4e3-103">ListInfo resource</span></span>

<span data-ttu-id="cb4e3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb4e3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cb4e3-105">Сложный тип **listInfo** используется для хранения дополнительных сведений о [списке][].</span><span class="sxs-lookup"><span data-stu-id="cb4e3-105">The **listInfo** complex type provides additional information about a [list][].</span></span>

[списке]: list.md
[list]: list.md

## <a name="json-representation"></a><span data-ttu-id="cb4e3-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cb4e3-107">JSON representation</span></span>

<span data-ttu-id="cb4e3-108">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cb4e3-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.listInfo"
}-->

```json
{
  "contentTypesEnabled": false,
  "hidden": false,
  "template": "documentLibrary | genericList | tasks | survey | links | announcements | contacts | ..."
}
```

## <a name="properties"></a><span data-ttu-id="cb4e3-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="cb4e3-109">Properties</span></span>

| <span data-ttu-id="cb4e3-110">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="cb4e3-110">Property name</span></span>           | <span data-ttu-id="cb4e3-111">Тип</span><span class="sxs-lookup"><span data-stu-id="cb4e3-111">Type</span></span>    | <span data-ttu-id="cb4e3-112">Описание</span><span class="sxs-lookup"><span data-stu-id="cb4e3-112">Description</span></span>
|:------------------------|:--------|:------------------------------------------------
| <span data-ttu-id="cb4e3-113">**contentTypesEnabled**</span><span class="sxs-lookup"><span data-stu-id="cb4e3-113">**contentTypesEnabled**</span></span> | <span data-ttu-id="cb4e3-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb4e3-114">Boolean</span></span> | <span data-ttu-id="cb4e3-115">Если свойство имеет значение `true`, это указывает на то, что для этого списка разрешено использовать типы контента.</span><span class="sxs-lookup"><span data-stu-id="cb4e3-115">If `true`, indicates that content types are enabled for this list.</span></span>
| <span data-ttu-id="cb4e3-116">**hidden**</span><span class="sxs-lookup"><span data-stu-id="cb4e3-116">**hidden**</span></span>              | <span data-ttu-id="cb4e3-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb4e3-117">Boolean</span></span> | <span data-ttu-id="cb4e3-118">Если это свойство имеет значение `true`, это указывает на то, что список обычно не отображается в пользовательском интерфейсе SharePoint.</span><span class="sxs-lookup"><span data-stu-id="cb4e3-118">If `true`, indicates that the list is not normally visible in the SharePoint user experience.</span></span>
| <span data-ttu-id="cb4e3-119">**template**</span><span class="sxs-lookup"><span data-stu-id="cb4e3-119">**template**</span></span>            | <span data-ttu-id="cb4e3-120">String</span><span class="sxs-lookup"><span data-stu-id="cb4e3-120">String</span></span>  | <span data-ttu-id="cb4e3-121">Перечислимое значение, которое представляет базовый шаблон списка, используемый при создании списка.</span><span class="sxs-lookup"><span data-stu-id="cb4e3-121">An enumerated value that represents the base list template used in creating the list.</span></span> <span data-ttu-id="cb4e3-122">Возможные значения: `documentLibrary`, `genericList`, `task`, `survey`, `announcements`, `contacts` и другие.</span><span class="sxs-lookup"><span data-stu-id="cb4e3-122">Possible values include `documentLibrary`, `genericList`, `task`, `survey`, `announcements`, `contacts`, and more.</span></span>

### <a name="remarks"></a><span data-ttu-id="cb4e3-123">Замечания</span><span class="sxs-lookup"><span data-stu-id="cb4e3-123">Remarks</span></span>

<span data-ttu-id="cb4e3-124">Большинство списков, создаваемых пользователями, будут иметь одно из указанных выше значений, но можно также использовать и другие значения.</span><span class="sxs-lookup"><span data-stu-id="cb4e3-124">While most lists created by users will have one of the values listed above, other values are possible as well.</span></span>
<span data-ttu-id="cb4e3-125">Ваше приложение должно быть способно обрабатывать любые значения, которые не указаны здесь.</span><span class="sxs-lookup"><span data-stu-id="cb4e3-125">Your app should be prepared to handle any values that are not listed here.</span></span>
<span data-ttu-id="cb4e3-126">Для разработчиков, знакомых с API CSOM в SharePoint, значение `template` соответствует перечислению `SPListTemplateType`.</span><span class="sxs-lookup"><span data-stu-id="cb4e3-126">For developers familiar with SharePoint's CSOM APIs, the `template` value corresponds to the `SPListTemplateType` enumeration.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/listinfo.md:
      Found potential enums in resource example that weren't defined in a table:(documentLibrary,genericList,tasks,survey,links,announcements,contacts,...) are in resource, but () are in table"
  ],
  "tocPath": ""
}-->

