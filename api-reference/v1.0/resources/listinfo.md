---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: ListInfo
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9be9d0dc133c9b62a89504a79ce9da4836337cfe
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32519880"
---
# <a name="listinfo-resource"></a><span data-ttu-id="39ae4-102">Ресурс listInfo</span><span class="sxs-lookup"><span data-stu-id="39ae4-102">ListInfo resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39ae4-103">Сложный тип **listInfo** используется для хранения дополнительных сведений о [списке][].</span><span class="sxs-lookup"><span data-stu-id="39ae4-103">The **listInfo** complex type provides additional information about a [list][].</span></span>

[списке]: list.md
[list]: list.md

## <a name="json-representation"></a><span data-ttu-id="39ae4-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="39ae4-105">JSON representation</span></span>

<span data-ttu-id="39ae4-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="39ae4-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="39ae4-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="39ae4-107">Properties</span></span>

| <span data-ttu-id="39ae4-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="39ae4-108">Property name</span></span>           | <span data-ttu-id="39ae4-109">Тип</span><span class="sxs-lookup"><span data-stu-id="39ae4-109">Type</span></span>    | <span data-ttu-id="39ae4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="39ae4-110">Description</span></span>
|:------------------------|:--------|:------------------------------------------------
| <span data-ttu-id="39ae4-111">**contentTypesEnabled**</span><span class="sxs-lookup"><span data-stu-id="39ae4-111">**contentTypesEnabled**</span></span> | <span data-ttu-id="39ae4-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="39ae4-112">Boolean</span></span> | <span data-ttu-id="39ae4-113">Если свойство имеет значение `true`, это указывает на то, что для этого списка разрешено использовать типы контента.</span><span class="sxs-lookup"><span data-stu-id="39ae4-113">If `true`, indicates that content types are enabled for this list.</span></span>
| <span data-ttu-id="39ae4-114">**hidden**</span><span class="sxs-lookup"><span data-stu-id="39ae4-114">**hidden**</span></span>              | <span data-ttu-id="39ae4-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="39ae4-115">Boolean</span></span> | <span data-ttu-id="39ae4-116">Если это свойство имеет значение `true`, это указывает на то, что список обычно не отображается в пользовательском интерфейсе SharePoint.</span><span class="sxs-lookup"><span data-stu-id="39ae4-116">If `true`, indicates that the list is not normally visible in the SharePoint user experience.</span></span>
| <span data-ttu-id="39ae4-117">**template**</span><span class="sxs-lookup"><span data-stu-id="39ae4-117">**template**</span></span>            | <span data-ttu-id="39ae4-118">String</span><span class="sxs-lookup"><span data-stu-id="39ae4-118">String</span></span>  | <span data-ttu-id="39ae4-119">Перечислимое значение, которое представляет базовый шаблон списка, используемый при создании списка.</span><span class="sxs-lookup"><span data-stu-id="39ae4-119">An enumerated value that represents the base list template used in creating the list.</span></span> <span data-ttu-id="39ae4-120">Возможные значения: `documentLibrary`, `genericList`, `task`, `survey`, `announcements`, `contacts` и другие.</span><span class="sxs-lookup"><span data-stu-id="39ae4-120">Possible values include `documentLibrary`, `genericList`, `task`, `survey`, `announcements`, `contacts`, and more.</span></span>

### <a name="remarks"></a><span data-ttu-id="39ae4-121">Замечания</span><span class="sxs-lookup"><span data-stu-id="39ae4-121">Remarks</span></span>

<span data-ttu-id="39ae4-122">Большинство списков, создаваемых пользователями, будут иметь одно из указанных выше значений, но можно также использовать и другие значения.</span><span class="sxs-lookup"><span data-stu-id="39ae4-122">While most lists created by users will have one of the values listed above, other values are possible as well.</span></span>
<span data-ttu-id="39ae4-123">Ваше приложение должно быть способно обрабатывать любые значения, которые не указаны здесь.</span><span class="sxs-lookup"><span data-stu-id="39ae4-123">Your app should be prepared to handle any values that are not listed here.</span></span>
<span data-ttu-id="39ae4-124">Для разработчиков, знакомых с API CSOM в SharePoint, значение `template` соответствует перечислению `SPListTemplateType`.</span><span class="sxs-lookup"><span data-stu-id="39ae4-124">For developers familiar with SharePoint's CSOM APIs, the `template` value corresponds to the `SPListTemplateType` enumeration.</span></span>

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
