---
author: JeremyKelley
description: Сложный тип listInfo используется для хранения дополнительных сведений о списке.
ms.date: 09/11/2017
title: ListInfo
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 3a066505348b1a1014b27ca3c83e0ee2f97f41a5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522955"
---
# <a name="listinfo-resource"></a><span data-ttu-id="c4d3a-103">Ресурс listInfo</span><span class="sxs-lookup"><span data-stu-id="c4d3a-103">ListInfo resource</span></span>

<span data-ttu-id="c4d3a-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c4d3a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4d3a-105">Сложный тип **listInfo** используется для хранения дополнительных сведений о [списке][].</span><span class="sxs-lookup"><span data-stu-id="c4d3a-105">The **listInfo** complex type provides additional information about a [list][].</span></span>

[списке]: list.md
[list]: list.md

## <a name="json-representation"></a><span data-ttu-id="c4d3a-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c4d3a-107">JSON representation</span></span>

<span data-ttu-id="c4d3a-108">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c4d3a-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="c4d3a-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="c4d3a-109">Properties</span></span>

| <span data-ttu-id="c4d3a-110">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="c4d3a-110">Property name</span></span>           | <span data-ttu-id="c4d3a-111">Тип</span><span class="sxs-lookup"><span data-stu-id="c4d3a-111">Type</span></span>    | <span data-ttu-id="c4d3a-112">Описание</span><span class="sxs-lookup"><span data-stu-id="c4d3a-112">Description</span></span>
|:------------------------|:--------|:------------------------------------------------
| <span data-ttu-id="c4d3a-113">**contentTypesEnabled**</span><span class="sxs-lookup"><span data-stu-id="c4d3a-113">**contentTypesEnabled**</span></span> | <span data-ttu-id="c4d3a-114">Логический</span><span class="sxs-lookup"><span data-stu-id="c4d3a-114">Boolean</span></span> | <span data-ttu-id="c4d3a-115">Если свойство имеет значение `true`, это указывает на то, что для этого списка разрешено использовать типы контента.</span><span class="sxs-lookup"><span data-stu-id="c4d3a-115">If `true`, indicates that content types are enabled for this list.</span></span>
| <span data-ttu-id="c4d3a-116">**hidden**</span><span class="sxs-lookup"><span data-stu-id="c4d3a-116">**hidden**</span></span>              | <span data-ttu-id="c4d3a-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="c4d3a-117">Boolean</span></span> | <span data-ttu-id="c4d3a-118">Если это свойство имеет значение `true`, это указывает на то, что список обычно не отображается в пользовательском интерфейсе SharePoint.</span><span class="sxs-lookup"><span data-stu-id="c4d3a-118">If `true`, indicates that the list is not normally visible in the SharePoint user experience.</span></span>
| <span data-ttu-id="c4d3a-119">**template**</span><span class="sxs-lookup"><span data-stu-id="c4d3a-119">**template**</span></span>            | <span data-ttu-id="c4d3a-120">String</span><span class="sxs-lookup"><span data-stu-id="c4d3a-120">String</span></span>  | <span data-ttu-id="c4d3a-121">Перечислимое значение, которое представляет базовый шаблон списка, используемый при создании списка.</span><span class="sxs-lookup"><span data-stu-id="c4d3a-121">An enumerated value that represents the base list template used in creating the list.</span></span> <span data-ttu-id="c4d3a-122">Возможные значения: `documentLibrary`, `genericList`, `task`, `survey`, `announcements`, `contacts` и другие.</span><span class="sxs-lookup"><span data-stu-id="c4d3a-122">Possible values include `documentLibrary`, `genericList`, `task`, `survey`, `announcements`, `contacts`, and more.</span></span>

### <a name="remarks"></a><span data-ttu-id="c4d3a-123">Замечания</span><span class="sxs-lookup"><span data-stu-id="c4d3a-123">Remarks</span></span>

<span data-ttu-id="c4d3a-124">Большинство списков, создаваемых пользователями, будут иметь одно из указанных выше значений, но можно также использовать и другие значения.</span><span class="sxs-lookup"><span data-stu-id="c4d3a-124">While most lists created by users will have one of the values listed above, other values are possible as well.</span></span>
<span data-ttu-id="c4d3a-125">Ваше приложение должно быть способно обрабатывать любые значения, которые не указаны здесь.</span><span class="sxs-lookup"><span data-stu-id="c4d3a-125">Your app should be prepared to handle any values that are not listed here.</span></span>
<span data-ttu-id="c4d3a-126">Для разработчиков, знакомых с API CSOM в SharePoint, значение `template` соответствует перечислению `SPListTemplateType`.</span><span class="sxs-lookup"><span data-stu-id="c4d3a-126">For developers familiar with SharePoint's CSOM APIs, the `template` value corresponds to the `SPListTemplateType` enumeration.</span></span>

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
