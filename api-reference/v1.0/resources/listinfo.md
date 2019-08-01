---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: ListInfo
localization_priority: Normal
ms.prod: sharepoint
description: Сложный тип listInfo используется для хранения дополнительных сведений о списке.
doc_type: resourcePageType
ms.openlocfilehash: dd6b2d892746c5aafc599b988113aefaa0b9973d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036416"
---
# <a name="listinfo-resource"></a><span data-ttu-id="c5b4d-103">Ресурс listInfo</span><span class="sxs-lookup"><span data-stu-id="c5b4d-103">ListInfo resource</span></span>

<span data-ttu-id="c5b4d-104">Сложный тип **listInfo** используется для хранения дополнительных сведений о [списке][].</span><span class="sxs-lookup"><span data-stu-id="c5b4d-104">The **listInfo** complex type provides additional information about a [list][].</span></span>

[списке]: list.md
[list]: list.md

## <a name="json-representation"></a><span data-ttu-id="c5b4d-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c5b4d-106">JSON representation</span></span>

<span data-ttu-id="c5b4d-107">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c5b4d-107">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="c5b4d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c5b4d-108">Properties</span></span>

| <span data-ttu-id="c5b4d-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="c5b4d-109">Property name</span></span>           | <span data-ttu-id="c5b4d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c5b4d-110">Type</span></span>    | <span data-ttu-id="c5b4d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c5b4d-111">Description</span></span>
|:------------------------|:--------|:------------------------------------------------
| <span data-ttu-id="c5b4d-112">**contentTypesEnabled**</span><span class="sxs-lookup"><span data-stu-id="c5b4d-112">**contentTypesEnabled**</span></span> | <span data-ttu-id="c5b4d-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5b4d-113">Boolean</span></span> | <span data-ttu-id="c5b4d-114">Если свойство имеет значение `true`, это указывает на то, что для этого списка разрешено использовать типы контента.</span><span class="sxs-lookup"><span data-stu-id="c5b4d-114">If `true`, indicates that content types are enabled for this list.</span></span>
| <span data-ttu-id="c5b4d-115">**hidden**</span><span class="sxs-lookup"><span data-stu-id="c5b4d-115">**hidden**</span></span>              | <span data-ttu-id="c5b4d-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5b4d-116">Boolean</span></span> | <span data-ttu-id="c5b4d-117">Если это свойство имеет значение `true`, это указывает на то, что список обычно не отображается в пользовательском интерфейсе SharePoint.</span><span class="sxs-lookup"><span data-stu-id="c5b4d-117">If `true`, indicates that the list is not normally visible in the SharePoint user experience.</span></span>
| <span data-ttu-id="c5b4d-118">**template**</span><span class="sxs-lookup"><span data-stu-id="c5b4d-118">**template**</span></span>            | <span data-ttu-id="c5b4d-119">String</span><span class="sxs-lookup"><span data-stu-id="c5b4d-119">String</span></span>  | <span data-ttu-id="c5b4d-120">Перечислимое значение, которое представляет базовый шаблон списка, используемый при создании списка.</span><span class="sxs-lookup"><span data-stu-id="c5b4d-120">An enumerated value that represents the base list template used in creating the list.</span></span> <span data-ttu-id="c5b4d-121">Возможные значения: `documentLibrary`, `genericList`, `task`, `survey`, `announcements`, `contacts` и другие.</span><span class="sxs-lookup"><span data-stu-id="c5b4d-121">Possible values include `documentLibrary`, `genericList`, `task`, `survey`, `announcements`, `contacts`, and more.</span></span>

### <a name="remarks"></a><span data-ttu-id="c5b4d-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="c5b4d-122">Remarks</span></span>

<span data-ttu-id="c5b4d-123">Большинство списков, создаваемых пользователями, будут иметь одно из указанных выше значений, но можно также использовать и другие значения.</span><span class="sxs-lookup"><span data-stu-id="c5b4d-123">While most lists created by users will have one of the values listed above, other values are possible as well.</span></span>
<span data-ttu-id="c5b4d-124">Ваше приложение должно быть способно обрабатывать любые значения, которые не указаны здесь.</span><span class="sxs-lookup"><span data-stu-id="c5b4d-124">Your app should be prepared to handle any values that are not listed here.</span></span>
<span data-ttu-id="c5b4d-125">Для разработчиков, знакомых с API CSOM в SharePoint, значение `template` соответствует перечислению `SPListTemplateType`.</span><span class="sxs-lookup"><span data-stu-id="c5b4d-125">For developers familiar with SharePoint's CSOM APIs, the `template` value corresponds to the `SPListTemplateType` enumeration.</span></span>

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
