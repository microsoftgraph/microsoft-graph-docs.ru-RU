---
author: JeremyKelley
description: Сложный тип listInfo используется для хранения дополнительных сведений о списке.
ms.date: 09/11/2017
title: ListInfo
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 962fc4928bac69489cf2ae2a4c77f3b72169ce0c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966947"
---
# <a name="listinfo-resource"></a><span data-ttu-id="fa33f-103">Ресурс listInfo</span><span class="sxs-lookup"><span data-stu-id="fa33f-103">ListInfo resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa33f-104">Сложный тип **listInfo** используется для хранения дополнительных сведений о [списке][].</span><span class="sxs-lookup"><span data-stu-id="fa33f-104">The **listInfo** complex type provides additional information about a [list][].</span></span>

[списке]: list.md
[list]: list.md

## <a name="json-representation"></a><span data-ttu-id="fa33f-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fa33f-106">JSON representation</span></span>

<span data-ttu-id="fa33f-107">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fa33f-107">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="fa33f-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="fa33f-108">Properties</span></span>

| <span data-ttu-id="fa33f-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="fa33f-109">Property name</span></span>           | <span data-ttu-id="fa33f-110">Тип</span><span class="sxs-lookup"><span data-stu-id="fa33f-110">Type</span></span>    | <span data-ttu-id="fa33f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="fa33f-111">Description</span></span>
|:------------------------|:--------|:------------------------------------------------
| <span data-ttu-id="fa33f-112">**contentTypesEnabled**</span><span class="sxs-lookup"><span data-stu-id="fa33f-112">**contentTypesEnabled**</span></span> | <span data-ttu-id="fa33f-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="fa33f-113">Boolean</span></span> | <span data-ttu-id="fa33f-114">Если свойство имеет значение `true`, это указывает на то, что для этого списка разрешено использовать типы контента.</span><span class="sxs-lookup"><span data-stu-id="fa33f-114">If `true`, indicates that content types are enabled for this list.</span></span>
| <span data-ttu-id="fa33f-115">**hidden**</span><span class="sxs-lookup"><span data-stu-id="fa33f-115">**hidden**</span></span>              | <span data-ttu-id="fa33f-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="fa33f-116">Boolean</span></span> | <span data-ttu-id="fa33f-117">Если это свойство имеет значение `true`, это указывает на то, что список обычно не отображается в пользовательском интерфейсе SharePoint.</span><span class="sxs-lookup"><span data-stu-id="fa33f-117">If `true`, indicates that the list is not normally visible in the SharePoint user experience.</span></span>
| <span data-ttu-id="fa33f-118">**template**</span><span class="sxs-lookup"><span data-stu-id="fa33f-118">**template**</span></span>            | <span data-ttu-id="fa33f-119">String</span><span class="sxs-lookup"><span data-stu-id="fa33f-119">String</span></span>  | <span data-ttu-id="fa33f-120">Перечислимое значение, которое представляет базовый шаблон списка, используемый при создании списка.</span><span class="sxs-lookup"><span data-stu-id="fa33f-120">An enumerated value that represents the base list template used in creating the list.</span></span> <span data-ttu-id="fa33f-121">Возможные значения: `documentLibrary`, `genericList`, `task`, `survey`, `announcements`, `contacts` и другие.</span><span class="sxs-lookup"><span data-stu-id="fa33f-121">Possible values include `documentLibrary`, `genericList`, `task`, `survey`, `announcements`, `contacts`, and more.</span></span>

### <a name="remarks"></a><span data-ttu-id="fa33f-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="fa33f-122">Remarks</span></span>

<span data-ttu-id="fa33f-123">Большинство списков, создаваемых пользователями, будут иметь одно из указанных выше значений, но можно также использовать и другие значения.</span><span class="sxs-lookup"><span data-stu-id="fa33f-123">While most lists created by users will have one of the values listed above, other values are possible as well.</span></span>
<span data-ttu-id="fa33f-124">Ваше приложение должно быть способно обрабатывать любые значения, которые не указаны здесь.</span><span class="sxs-lookup"><span data-stu-id="fa33f-124">Your app should be prepared to handle any values that are not listed here.</span></span>
<span data-ttu-id="fa33f-125">Для разработчиков, знакомых с API CSOM в SharePoint, значение `template` соответствует перечислению `SPListTemplateType`.</span><span class="sxs-lookup"><span data-stu-id="fa33f-125">For developers familiar with SharePoint's CSOM APIs, the `template` value corresponds to the `SPListTemplateType` enumeration.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
