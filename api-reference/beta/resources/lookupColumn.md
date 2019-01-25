---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: lookupColumn
localization_priority: Normal
ms.openlocfilehash: 2efb199fafbf7c60af0e13720ea1b9efd93dc05c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517521"
---
# <a name="lookupcolumn-resource-type"></a><span data-ttu-id="a18ef-102">Тип ресурса lookupColumn</span><span class="sxs-lookup"><span data-stu-id="a18ef-102">LookupColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a18ef-103">Ресурс **lookupColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца подставляются из другого источника на сайте.</span><span class="sxs-lookup"><span data-stu-id="a18ef-103">The **lookupColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are looked up from another source in the site.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a18ef-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a18ef-104">JSON representation</span></span>

<span data-ttu-id="a18ef-105">Ниже показано представление ресурса **lookupColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a18ef-105">Here is a JSON representation of a **lookupColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.lookupColumn" } -->

```json
{
  "allowMultipleValues": true,
  "allowUnlimitedLength": false,
  "columnName": "string",
  "listId": "string",
  "primaryLookupColumnId": "string"
}
```

## <a name="properties"></a><span data-ttu-id="a18ef-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a18ef-106">Properties</span></span>

| <span data-ttu-id="a18ef-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="a18ef-107">Property name</span></span>             | <span data-ttu-id="a18ef-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a18ef-108">Type</span></span>    | <span data-ttu-id="a18ef-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a18ef-109">Description</span></span>
|:--------------------------|:--------|:---------------------------------------
| <span data-ttu-id="a18ef-110">**allowMultipleValues**</span><span class="sxs-lookup"><span data-stu-id="a18ef-110">**allowMultipleValues**</span></span>   | <span data-ttu-id="a18ef-111">boolean</span><span class="sxs-lookup"><span data-stu-id="a18ef-111">boolean</span></span> | <span data-ttu-id="a18ef-112">Указывает, можно ли выбрать несколько значений в источнике.</span><span class="sxs-lookup"><span data-stu-id="a18ef-112">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="a18ef-113">**allowUnlimitedLength**</span><span class="sxs-lookup"><span data-stu-id="a18ef-113">**allowUnlimitedLength**</span></span>  | <span data-ttu-id="a18ef-114">boolean</span><span class="sxs-lookup"><span data-stu-id="a18ef-114">boolean</span></span> | <span data-ttu-id="a18ef-115">Указывает, может ли длина значений в столбце превышать стандартное ограничение в 255 символов.</span><span class="sxs-lookup"><span data-stu-id="a18ef-115">Indicates whether values in the column should be able to exceed the standard limit of 255 characters.</span></span>
| <span data-ttu-id="a18ef-116">**columnName**</span><span class="sxs-lookup"><span data-stu-id="a18ef-116">**columnName**</span></span>            | <span data-ttu-id="a18ef-117">string</span><span class="sxs-lookup"><span data-stu-id="a18ef-117">string</span></span>  | <span data-ttu-id="a18ef-118">Имя исходного столбца подстановки.</span><span class="sxs-lookup"><span data-stu-id="a18ef-118">The name of the lookup source column.</span></span>
| <span data-ttu-id="a18ef-119">**listId**</span><span class="sxs-lookup"><span data-stu-id="a18ef-119">**listId**</span></span>                | <span data-ttu-id="a18ef-120">string</span><span class="sxs-lookup"><span data-stu-id="a18ef-120">string</span></span>  | <span data-ttu-id="a18ef-121">Уникальный идентификатор исходного списка подстановки.</span><span class="sxs-lookup"><span data-stu-id="a18ef-121">The unique identifier of the lookup source list.</span></span>
| <span data-ttu-id="a18ef-122">**primaryLookupColumnId**</span><span class="sxs-lookup"><span data-stu-id="a18ef-122">**primaryLookupColumnId**</span></span> | <span data-ttu-id="a18ef-123">string</span><span class="sxs-lookup"><span data-stu-id="a18ef-123">string</span></span>  | <span data-ttu-id="a18ef-124">Если это свойство указано, то данный столбец представляет собой *вторичную подстановку*, для которой извлекается дополнительное поле из элемента списка, подставленного при *первичной подстановке*.</span><span class="sxs-lookup"><span data-stu-id="a18ef-124">If specified, this column is a *secondary lookup*, pulling an additional field from the list item looked up by the *primary lookup*.</span></span> <span data-ttu-id="a18ef-125">Используйте элемент списка, полученный в результате *первичной* подстановки, в качестве источника для указанного здесь столбца.</span><span class="sxs-lookup"><span data-stu-id="a18ef-125">Use the list item looked up by the *primary* as the source for the column named here.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/LookupColumn",
  "suppressions": [
    "Error: /api-reference/beta/resources/lookupColumn.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
