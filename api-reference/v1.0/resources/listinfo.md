---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: listInfo
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 459e51af92e01d10edd2ec1d86f3c288b125e1d6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957468"
---
# <a name="listinfo-resource"></a><span data-ttu-id="6e9d6-102">Ресурс listInfo</span><span class="sxs-lookup"><span data-stu-id="6e9d6-102">ListInfo resource</span></span>

<span data-ttu-id="6e9d6-103">Сложный тип **listInfo** используется для хранения дополнительных сведений о [списке][].</span><span class="sxs-lookup"><span data-stu-id="6e9d6-103">The **listInfo** complex type provides additional information about a [list][].</span></span>

[списке]: list.md
[list]: list.md

## <a name="json-representation"></a><span data-ttu-id="6e9d6-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="6e9d6-105">JSON representation</span></span>

<span data-ttu-id="6e9d6-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6e9d6-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="6e9d6-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6e9d6-107">Properties</span></span>

| <span data-ttu-id="6e9d6-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="6e9d6-108">Property name</span></span>           | <span data-ttu-id="6e9d6-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6e9d6-109">Type</span></span>    | <span data-ttu-id="6e9d6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6e9d6-110">Description</span></span>
|:------------------------|:--------|:------------------------------------------------
| <span data-ttu-id="6e9d6-111">**contentTypesEnabled**</span><span class="sxs-lookup"><span data-stu-id="6e9d6-111">**contentTypesEnabled**</span></span> | <span data-ttu-id="6e9d6-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e9d6-112">Boolean</span></span> | <span data-ttu-id="6e9d6-113">Если свойство имеет значение `true`, это указывает на то, что для этого списка разрешено использовать типы контента.</span><span class="sxs-lookup"><span data-stu-id="6e9d6-113">If `true`, indicates that content types are enabled for this list.</span></span>
| <span data-ttu-id="6e9d6-114">**hidden**</span><span class="sxs-lookup"><span data-stu-id="6e9d6-114">**hidden**</span></span>              | <span data-ttu-id="6e9d6-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e9d6-115">Boolean</span></span> | <span data-ttu-id="6e9d6-116">Если это свойство имеет значение `true`, это указывает на то, что список обычно не отображается в пользовательском интерфейсе SharePoint.</span><span class="sxs-lookup"><span data-stu-id="6e9d6-116">If `true`, indicates that the list is not normally visible in the SharePoint user experience.</span></span>
| <span data-ttu-id="6e9d6-117">**template**</span><span class="sxs-lookup"><span data-stu-id="6e9d6-117">**template**</span></span>            | <span data-ttu-id="6e9d6-118">String</span><span class="sxs-lookup"><span data-stu-id="6e9d6-118">String</span></span>  | <span data-ttu-id="6e9d6-119">Перечислимое значение, которое представляет базовый шаблон списка, используемый при создании списка.</span><span class="sxs-lookup"><span data-stu-id="6e9d6-119">An enumerated value that represents the base list template used in creating the list.</span></span> <span data-ttu-id="6e9d6-120">Возможные значения: `documentLibrary`, `genericList`, `task`, `survey`, `announcements`, `contacts` и другие.</span><span class="sxs-lookup"><span data-stu-id="6e9d6-120">Possible values include `documentLibrary`, `genericList`, `task`, `survey`, `announcements`, `contacts`, and more.</span></span>

### <a name="remarks"></a><span data-ttu-id="6e9d6-121">Замечания</span><span class="sxs-lookup"><span data-stu-id="6e9d6-121">Remarks</span></span>

<span data-ttu-id="6e9d6-122">Большинство списков, создаваемых пользователями, будут иметь одно из указанных выше значений, но можно также использовать и другие значения.</span><span class="sxs-lookup"><span data-stu-id="6e9d6-122">While most lists created by users will have one of the values listed above, other values are possible as well.</span></span>
<span data-ttu-id="6e9d6-123">Ваше приложение должно быть способно обрабатывать любые значения, которые не указаны здесь.</span><span class="sxs-lookup"><span data-stu-id="6e9d6-123">Your app should be prepared to handle any values that are not listed here.</span></span>
<span data-ttu-id="6e9d6-124">Для разработчиков, знакомых с API CSOM в SharePoint, значение `template` соответствует перечислению `SPListTemplateType`.</span><span class="sxs-lookup"><span data-stu-id="6e9d6-124">For developers familiar with SharePoint's CSOM APIs, the `template` value corresponds to the `SPListTemplateType` enumeration.</span></span>

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
