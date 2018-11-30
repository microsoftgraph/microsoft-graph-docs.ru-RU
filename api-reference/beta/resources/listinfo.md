---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: listInfo
ms.openlocfilehash: fb955a89c8dfb7b399d15f00666f21899abdc33d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077148"
---
# <a name="listinfo-resource"></a><span data-ttu-id="8cb51-102">Ресурс listInfo</span><span class="sxs-lookup"><span data-stu-id="8cb51-102">ListInfo resource</span></span>

> <span data-ttu-id="8cb51-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8cb51-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8cb51-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8cb51-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8cb51-105">Сложный тип **listInfo** используется для хранения дополнительных сведений о [списке][].</span><span class="sxs-lookup"><span data-stu-id="8cb51-105">The **listInfo** complex type provides additional information about a [list][].</span></span>

[list]: list.md

## <a name="json-representation"></a><span data-ttu-id="8cb51-107">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="8cb51-107">JSON representation</span></span>

<span data-ttu-id="8cb51-108">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8cb51-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="8cb51-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="8cb51-109">Properties</span></span>

| <span data-ttu-id="8cb51-110">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="8cb51-110">Property name</span></span>           | <span data-ttu-id="8cb51-111">Тип</span><span class="sxs-lookup"><span data-stu-id="8cb51-111">Type</span></span>    | <span data-ttu-id="8cb51-112">Описание</span><span class="sxs-lookup"><span data-stu-id="8cb51-112">Description</span></span>
|:------------------------|:--------|:------------------------------------------------
| <span data-ttu-id="8cb51-113">**contentTypesEnabled**</span><span class="sxs-lookup"><span data-stu-id="8cb51-113">**contentTypesEnabled**</span></span> | <span data-ttu-id="8cb51-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="8cb51-114">Boolean</span></span> | <span data-ttu-id="8cb51-115">Если свойство имеет значение `true`, это указывает на то, что для этого списка разрешено использовать типы контента.</span><span class="sxs-lookup"><span data-stu-id="8cb51-115">If `true`, indicates that content types are enabled for this list.</span></span>
| <span data-ttu-id="8cb51-116">**hidden**</span><span class="sxs-lookup"><span data-stu-id="8cb51-116">**hidden**</span></span>              | <span data-ttu-id="8cb51-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="8cb51-117">Boolean</span></span> | <span data-ttu-id="8cb51-118">Если это свойство имеет значение `true`, это указывает на то, что список обычно не отображается в пользовательском интерфейсе SharePoint.</span><span class="sxs-lookup"><span data-stu-id="8cb51-118">If `true`, indicates that the list is not normally visible in the SharePoint user experience.</span></span>
| <span data-ttu-id="8cb51-119">**template**</span><span class="sxs-lookup"><span data-stu-id="8cb51-119">**template**</span></span>            | <span data-ttu-id="8cb51-120">String</span><span class="sxs-lookup"><span data-stu-id="8cb51-120">String</span></span>  | <span data-ttu-id="8cb51-121">Перечислимое значение, которое представляет базовый шаблон списка, используемый при создании списка.</span><span class="sxs-lookup"><span data-stu-id="8cb51-121">An enumerated value that represents the base list template used in creating the list.</span></span> <span data-ttu-id="8cb51-122">Возможные значения: `documentLibrary`, `genericList`, `task`, `survey`, `announcements`, `contacts` и другие.</span><span class="sxs-lookup"><span data-stu-id="8cb51-122">Possible values include `documentLibrary`, `genericList`, `task`, `survey`, `announcements`, `contacts`, and more.</span></span>

### <a name="remarks"></a><span data-ttu-id="8cb51-123">Примечания</span><span class="sxs-lookup"><span data-stu-id="8cb51-123">Remarks</span></span>

<span data-ttu-id="8cb51-124">Большинство списков, создаваемых пользователями, будут иметь одно из указанных выше значений, но можно также использовать и другие значения.</span><span class="sxs-lookup"><span data-stu-id="8cb51-124">While most lists created by users will have one of the values listed above, other values are possible as well.</span></span>
<span data-ttu-id="8cb51-125">Ваше приложение должно быть способно обрабатывать любые значения, которые не указаны здесь.</span><span class="sxs-lookup"><span data-stu-id="8cb51-125">Your app should be prepared to handle any values that are not listed here.</span></span>
<span data-ttu-id="8cb51-126">Для разработчиков, знакомых с API CSOM в SharePoint, значение `template` соответствует перечислению `SPListTemplateType`.</span><span class="sxs-lookup"><span data-stu-id="8cb51-126">For developers familiar with SharePoint's CSOM APIs, the `template` value corresponds to the `SPListTemplateType` enumeration.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
