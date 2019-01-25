---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: listInfo
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 1f94bf51169a6b056e010386f88d859aeaf41b9b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512376"
---
# <a name="listinfo-resource"></a><span data-ttu-id="88822-102">Ресурс listInfo</span><span class="sxs-lookup"><span data-stu-id="88822-102">ListInfo resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88822-103">Сложный тип **listInfo** используется для хранения дополнительных сведений о [списке][].</span><span class="sxs-lookup"><span data-stu-id="88822-103">The **listInfo** complex type provides additional information about a [list][].</span></span>

[списке]: list.md
[list]: list.md

## <a name="json-representation"></a><span data-ttu-id="88822-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="88822-105">JSON representation</span></span>

<span data-ttu-id="88822-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="88822-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="88822-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="88822-107">Properties</span></span>

| <span data-ttu-id="88822-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="88822-108">Property name</span></span>           | <span data-ttu-id="88822-109">Тип</span><span class="sxs-lookup"><span data-stu-id="88822-109">Type</span></span>    | <span data-ttu-id="88822-110">Описание</span><span class="sxs-lookup"><span data-stu-id="88822-110">Description</span></span>
|:------------------------|:--------|:------------------------------------------------
| <span data-ttu-id="88822-111">**contentTypesEnabled**</span><span class="sxs-lookup"><span data-stu-id="88822-111">**contentTypesEnabled**</span></span> | <span data-ttu-id="88822-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="88822-112">Boolean</span></span> | <span data-ttu-id="88822-113">Если свойство имеет значение `true`, это указывает на то, что для этого списка разрешено использовать типы контента.</span><span class="sxs-lookup"><span data-stu-id="88822-113">If `true`, indicates that content types are enabled for this list.</span></span>
| <span data-ttu-id="88822-114">**hidden**</span><span class="sxs-lookup"><span data-stu-id="88822-114">**hidden**</span></span>              | <span data-ttu-id="88822-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="88822-115">Boolean</span></span> | <span data-ttu-id="88822-116">Если это свойство имеет значение `true`, это указывает на то, что список обычно не отображается в пользовательском интерфейсе SharePoint.</span><span class="sxs-lookup"><span data-stu-id="88822-116">If `true`, indicates that the list is not normally visible in the SharePoint user experience.</span></span>
| <span data-ttu-id="88822-117">**template**</span><span class="sxs-lookup"><span data-stu-id="88822-117">**template**</span></span>            | <span data-ttu-id="88822-118">String</span><span class="sxs-lookup"><span data-stu-id="88822-118">String</span></span>  | <span data-ttu-id="88822-119">Перечислимое значение, которое представляет базовый шаблон списка, используемый при создании списка.</span><span class="sxs-lookup"><span data-stu-id="88822-119">An enumerated value that represents the base list template used in creating the list.</span></span> <span data-ttu-id="88822-120">Возможные значения: `documentLibrary`, `genericList`, `task`, `survey`, `announcements`, `contacts` и другие.</span><span class="sxs-lookup"><span data-stu-id="88822-120">Possible values include `documentLibrary`, `genericList`, `task`, `survey`, `announcements`, `contacts`, and more.</span></span>

### <a name="remarks"></a><span data-ttu-id="88822-121">Замечания</span><span class="sxs-lookup"><span data-stu-id="88822-121">Remarks</span></span>

<span data-ttu-id="88822-122">Большинство списков, создаваемых пользователями, будут иметь одно из указанных выше значений, но можно также использовать и другие значения.</span><span class="sxs-lookup"><span data-stu-id="88822-122">While most lists created by users will have one of the values listed above, other values are possible as well.</span></span>
<span data-ttu-id="88822-123">Ваше приложение должно быть способно обрабатывать любые значения, которые не указаны здесь.</span><span class="sxs-lookup"><span data-stu-id="88822-123">Your app should be prepared to handle any values that are not listed here.</span></span>
<span data-ttu-id="88822-124">Для разработчиков, знакомых с API CSOM в SharePoint, значение `template` соответствует перечислению `SPListTemplateType`.</span><span class="sxs-lookup"><span data-stu-id="88822-124">For developers familiar with SharePoint's CSOM APIs, the `template` value corresponds to the `SPListTemplateType` enumeration.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/listinfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
