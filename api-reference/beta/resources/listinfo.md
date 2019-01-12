---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: listInfo
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 0e1106873a9f069870c981f6df3ae94412ca85de
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987771"
---
# <a name="listinfo-resource"></a><span data-ttu-id="67941-102">Ресурс listInfo</span><span class="sxs-lookup"><span data-stu-id="67941-102">ListInfo resource</span></span>

> <span data-ttu-id="67941-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="67941-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="67941-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67941-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="67941-105">Сложный тип **listInfo** используется для хранения дополнительных сведений о [списке][].</span><span class="sxs-lookup"><span data-stu-id="67941-105">The **listInfo** complex type provides additional information about a [list][].</span></span>

[list]: list.md

## <a name="json-representation"></a><span data-ttu-id="67941-107">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="67941-107">JSON representation</span></span>

<span data-ttu-id="67941-108">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="67941-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="67941-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="67941-109">Properties</span></span>

| <span data-ttu-id="67941-110">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="67941-110">Property name</span></span>           | <span data-ttu-id="67941-111">Тип</span><span class="sxs-lookup"><span data-stu-id="67941-111">Type</span></span>    | <span data-ttu-id="67941-112">Описание</span><span class="sxs-lookup"><span data-stu-id="67941-112">Description</span></span>
|:------------------------|:--------|:------------------------------------------------
| <span data-ttu-id="67941-113">**contentTypesEnabled**</span><span class="sxs-lookup"><span data-stu-id="67941-113">**contentTypesEnabled**</span></span> | <span data-ttu-id="67941-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="67941-114">Boolean</span></span> | <span data-ttu-id="67941-115">Если свойство имеет значение `true`, это указывает на то, что для этого списка разрешено использовать типы контента.</span><span class="sxs-lookup"><span data-stu-id="67941-115">If `true`, indicates that content types are enabled for this list.</span></span>
| <span data-ttu-id="67941-116">**hidden**</span><span class="sxs-lookup"><span data-stu-id="67941-116">**hidden**</span></span>              | <span data-ttu-id="67941-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="67941-117">Boolean</span></span> | <span data-ttu-id="67941-118">Если это свойство имеет значение `true`, это указывает на то, что список обычно не отображается в пользовательском интерфейсе SharePoint.</span><span class="sxs-lookup"><span data-stu-id="67941-118">If `true`, indicates that the list is not normally visible in the SharePoint user experience.</span></span>
| <span data-ttu-id="67941-119">**template**</span><span class="sxs-lookup"><span data-stu-id="67941-119">**template**</span></span>            | <span data-ttu-id="67941-120">String</span><span class="sxs-lookup"><span data-stu-id="67941-120">String</span></span>  | <span data-ttu-id="67941-121">Перечислимое значение, которое представляет базовый шаблон списка, используемый при создании списка.</span><span class="sxs-lookup"><span data-stu-id="67941-121">An enumerated value that represents the base list template used in creating the list.</span></span> <span data-ttu-id="67941-122">Возможные значения: `documentLibrary`, `genericList`, `task`, `survey`, `announcements`, `contacts` и другие.</span><span class="sxs-lookup"><span data-stu-id="67941-122">Possible values include `documentLibrary`, `genericList`, `task`, `survey`, `announcements`, `contacts`, and more.</span></span>

### <a name="remarks"></a><span data-ttu-id="67941-123">Примечания</span><span class="sxs-lookup"><span data-stu-id="67941-123">Remarks</span></span>

<span data-ttu-id="67941-124">Большинство списков, создаваемых пользователями, будут иметь одно из указанных выше значений, но можно также использовать и другие значения.</span><span class="sxs-lookup"><span data-stu-id="67941-124">While most lists created by users will have one of the values listed above, other values are possible as well.</span></span>
<span data-ttu-id="67941-125">Ваше приложение должно быть способно обрабатывать любые значения, которые не указаны здесь.</span><span class="sxs-lookup"><span data-stu-id="67941-125">Your app should be prepared to handle any values that are not listed here.</span></span>
<span data-ttu-id="67941-126">Для разработчиков, знакомых с API CSOM в SharePoint, значение `template` соответствует перечислению `SPListTemplateType`.</span><span class="sxs-lookup"><span data-stu-id="67941-126">For developers familiar with SharePoint's CSOM APIs, the `template` value corresponds to the `SPListTemplateType` enumeration.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
