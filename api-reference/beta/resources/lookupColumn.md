---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: LookupColumn
localization_priority: Normal
ms.openlocfilehash: 1a38cc3e08917b0d4aa2a8df4943ebc932c937d4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506231"
---
# <a name="lookupcolumn-resource-type"></a><span data-ttu-id="b09bd-102">Тип ресурса lookupColumn</span><span class="sxs-lookup"><span data-stu-id="b09bd-102">LookupColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b09bd-103">Ресурс **lookupColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца подставляются из другого источника на сайте.</span><span class="sxs-lookup"><span data-stu-id="b09bd-103">The **lookupColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are looked up from another source in the site.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b09bd-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b09bd-104">JSON representation</span></span>

<span data-ttu-id="b09bd-105">Ниже показано представление ресурса **lookupColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b09bd-105">Here is a JSON representation of a **lookupColumn** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="b09bd-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b09bd-106">Properties</span></span>

| <span data-ttu-id="b09bd-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="b09bd-107">Property name</span></span>             | <span data-ttu-id="b09bd-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b09bd-108">Type</span></span>    | <span data-ttu-id="b09bd-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b09bd-109">Description</span></span>
|:--------------------------|:--------|:---------------------------------------
| <span data-ttu-id="b09bd-110">**allowMultipleValues**</span><span class="sxs-lookup"><span data-stu-id="b09bd-110">**allowMultipleValues**</span></span>   | <span data-ttu-id="b09bd-111">логический</span><span class="sxs-lookup"><span data-stu-id="b09bd-111">boolean</span></span> | <span data-ttu-id="b09bd-112">Указывает, можно ли выбрать несколько значений в источнике.</span><span class="sxs-lookup"><span data-stu-id="b09bd-112">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="b09bd-113">**allowUnlimitedLength**</span><span class="sxs-lookup"><span data-stu-id="b09bd-113">**allowUnlimitedLength**</span></span>  | <span data-ttu-id="b09bd-114">boolean</span><span class="sxs-lookup"><span data-stu-id="b09bd-114">boolean</span></span> | <span data-ttu-id="b09bd-115">Указывает, может ли длина значений в столбце превышать стандартное ограничение в 255 символов.</span><span class="sxs-lookup"><span data-stu-id="b09bd-115">Indicates whether values in the column should be able to exceed the standard limit of 255 characters.</span></span>
| <span data-ttu-id="b09bd-116">**columnName**</span><span class="sxs-lookup"><span data-stu-id="b09bd-116">**columnName**</span></span>            | <span data-ttu-id="b09bd-117">строка</span><span class="sxs-lookup"><span data-stu-id="b09bd-117">string</span></span>  | <span data-ttu-id="b09bd-118">Имя исходного столбца подстановки.</span><span class="sxs-lookup"><span data-stu-id="b09bd-118">The name of the lookup source column.</span></span>
| <span data-ttu-id="b09bd-119">**listId**</span><span class="sxs-lookup"><span data-stu-id="b09bd-119">**listId**</span></span>                | <span data-ttu-id="b09bd-120">строка</span><span class="sxs-lookup"><span data-stu-id="b09bd-120">string</span></span>  | <span data-ttu-id="b09bd-121">Уникальный идентификатор исходного списка подстановки.</span><span class="sxs-lookup"><span data-stu-id="b09bd-121">The unique identifier of the lookup source list.</span></span>
| <span data-ttu-id="b09bd-122">**primaryLookupColumnId**</span><span class="sxs-lookup"><span data-stu-id="b09bd-122">**primaryLookupColumnId**</span></span> | <span data-ttu-id="b09bd-123">string</span><span class="sxs-lookup"><span data-stu-id="b09bd-123">string</span></span>  | <span data-ttu-id="b09bd-124">Если это свойство указано, то данный столбец представляет собой *вторичную подстановку*, для которой извлекается дополнительное поле из элемента списка, подставленного при *первичной подстановке*.</span><span class="sxs-lookup"><span data-stu-id="b09bd-124">If specified, this column is a *secondary lookup*, pulling an additional field from the list item looked up by the *primary lookup*.</span></span> <span data-ttu-id="b09bd-125">Используйте элемент списка, полученный в результате *первичной* подстановки, в качестве источника для указанного здесь столбца.</span><span class="sxs-lookup"><span data-stu-id="b09bd-125">Use the list item looked up by the *primary* as the source for the column named here.</span></span>

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
