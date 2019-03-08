---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: TextColumn
localization_priority: Normal
ms.openlocfilehash: c69dc7c30bff0f43327ec256af6071e34de6b898
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481498"
---
# <a name="textcolumn-resource-type"></a><span data-ttu-id="45d50-102">Тип ресурса textColumn</span><span class="sxs-lookup"><span data-stu-id="45d50-102">TextColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45d50-103">Ресурс **textColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют собой текст.</span><span class="sxs-lookup"><span data-stu-id="45d50-103">The **textColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are text.</span></span>

## <a name="json-representation"></a><span data-ttu-id="45d50-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="45d50-104">JSON representation</span></span>

<span data-ttu-id="45d50-105">Ниже показано представление ресурса **textColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="45d50-105">Here is a JSON representation of a **textColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.textColumn" } -->

```json
{
  "allowMultipleLines": true,
  "appendChangesToExistingText": false,
  "linesForEditing": 6,
  "maxLength": 300,
  "textType": "plain | richText"
}
```

## <a name="properties"></a><span data-ttu-id="45d50-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="45d50-106">Properties</span></span>

| <span data-ttu-id="45d50-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="45d50-107">Property name</span></span>                   | <span data-ttu-id="45d50-108">Тип</span><span class="sxs-lookup"><span data-stu-id="45d50-108">Type</span></span>   | <span data-ttu-id="45d50-109">Описание</span><span class="sxs-lookup"><span data-stu-id="45d50-109">Description</span></span>
|:--------------------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="45d50-110">**allowMultipleLines**</span><span class="sxs-lookup"><span data-stu-id="45d50-110">**allowMultipleLines**</span></span>          | <span data-ttu-id="45d50-111">string</span><span class="sxs-lookup"><span data-stu-id="45d50-111">string</span></span> | <span data-ttu-id="45d50-112">Указывает, разрешено ли отображать несколько строк текста.</span><span class="sxs-lookup"><span data-stu-id="45d50-112">Whether to allow multiple lines of text.</span></span>
| <span data-ttu-id="45d50-113">**appendChangesToExistingText**</span><span class="sxs-lookup"><span data-stu-id="45d50-113">**appendChangesToExistingText**</span></span> | <span data-ttu-id="45d50-114">string</span><span class="sxs-lookup"><span data-stu-id="45d50-114">string</span></span> | <span data-ttu-id="45d50-115">Указывает, что должно происходить при обновлении данного столбца: новый текст должен заменять существующий либо дополнять его.</span><span class="sxs-lookup"><span data-stu-id="45d50-115">Whether updates to this column should replace existing text, or append to it.</span></span>
| <span data-ttu-id="45d50-116">**linesForEditing**</span><span class="sxs-lookup"><span data-stu-id="45d50-116">**linesForEditing**</span></span>             | <span data-ttu-id="45d50-117">int</span><span class="sxs-lookup"><span data-stu-id="45d50-117">int</span></span>    | <span data-ttu-id="45d50-118">Размер текстового поля.</span><span class="sxs-lookup"><span data-stu-id="45d50-118">The size of the text box.</span></span>
| <span data-ttu-id="45d50-119">**maxLength**</span><span class="sxs-lookup"><span data-stu-id="45d50-119">**maxLength**</span></span>                   | <span data-ttu-id="45d50-120">int</span><span class="sxs-lookup"><span data-stu-id="45d50-120">int</span></span>    | <span data-ttu-id="45d50-121">Максимальное количество символов для значения.</span><span class="sxs-lookup"><span data-stu-id="45d50-121">The maximum number of characters for the value.</span></span>
| <span data-ttu-id="45d50-122">**textType**</span><span class="sxs-lookup"><span data-stu-id="45d50-122">**textType**</span></span>                    | <span data-ttu-id="45d50-123">string</span><span class="sxs-lookup"><span data-stu-id="45d50-123">string</span></span> | <span data-ttu-id="45d50-124">Тип хранимого текста.</span><span class="sxs-lookup"><span data-stu-id="45d50-124">The type of text being stored.</span></span> <span data-ttu-id="45d50-125">Должно иметь тип `plain` или `richText`</span><span class="sxs-lookup"><span data-stu-id="45d50-125">Must be one of `plain` or `richText`</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/TextColumn",
  "suppressions": [
    "Error: /api-reference/beta/resources/textColumn.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
