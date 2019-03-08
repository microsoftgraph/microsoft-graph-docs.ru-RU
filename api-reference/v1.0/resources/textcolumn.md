---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: TextColumn
localization_priority: Normal
ms.openlocfilehash: 1e10997bd70f97fa91177aee48a6ffcecff40ab5
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480840"
---
# <a name="textcolumn-resource-type"></a><span data-ttu-id="e2825-102">Тип ресурса textColumn</span><span class="sxs-lookup"><span data-stu-id="e2825-102">TextColumn resource type</span></span>

<span data-ttu-id="e2825-103">Ресурс **textColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют собой текст.</span><span class="sxs-lookup"><span data-stu-id="e2825-103">The **textColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are text.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e2825-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e2825-104">JSON representation</span></span>

<span data-ttu-id="e2825-105">Ниже показано представление ресурса **textColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e2825-105">Here is a JSON representation of a **textColumn** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="e2825-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e2825-106">Properties</span></span>

| <span data-ttu-id="e2825-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="e2825-107">Property name</span></span>                   | <span data-ttu-id="e2825-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e2825-108">Type</span></span>    | <span data-ttu-id="e2825-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e2825-109">Description</span></span>
|:--------------------------------|:--------|:---------------------------------
| <span data-ttu-id="e2825-110">**allowMultipleLines**</span><span class="sxs-lookup"><span data-stu-id="e2825-110">**allowMultipleLines**</span></span>          | <span data-ttu-id="e2825-111">логический</span><span class="sxs-lookup"><span data-stu-id="e2825-111">boolean</span></span> | <span data-ttu-id="e2825-112">Указывает, разрешено ли отображать несколько строк текста.</span><span class="sxs-lookup"><span data-stu-id="e2825-112">Whether to allow multiple lines of text.</span></span>
| <span data-ttu-id="e2825-113">**appendChangesToExistingText**</span><span class="sxs-lookup"><span data-stu-id="e2825-113">**appendChangesToExistingText**</span></span> | <span data-ttu-id="e2825-114">логический</span><span class="sxs-lookup"><span data-stu-id="e2825-114">boolean</span></span> | <span data-ttu-id="e2825-115">Указывает, что должно происходить при обновлении данного столбца: новый текст должен заменять существующий либо дополнять его.</span><span class="sxs-lookup"><span data-stu-id="e2825-115">Whether updates to this column should replace existing text, or append to it.</span></span>
| <span data-ttu-id="e2825-116">**linesForEditing**</span><span class="sxs-lookup"><span data-stu-id="e2825-116">**linesForEditing**</span></span>             | <span data-ttu-id="e2825-117">Int32</span><span class="sxs-lookup"><span data-stu-id="e2825-117">int32</span></span>   | <span data-ttu-id="e2825-118">Размер текстового поля.</span><span class="sxs-lookup"><span data-stu-id="e2825-118">The size of the text box.</span></span>
| <span data-ttu-id="e2825-119">**maxLength**</span><span class="sxs-lookup"><span data-stu-id="e2825-119">**maxLength**</span></span>                   | <span data-ttu-id="e2825-120">Int32</span><span class="sxs-lookup"><span data-stu-id="e2825-120">int32</span></span>   | <span data-ttu-id="e2825-121">Максимальное количество символов для значения.</span><span class="sxs-lookup"><span data-stu-id="e2825-121">The maximum number of characters for the value.</span></span>
| <span data-ttu-id="e2825-122">**textType**</span><span class="sxs-lookup"><span data-stu-id="e2825-122">**textType**</span></span>                    | <span data-ttu-id="e2825-123">string</span><span class="sxs-lookup"><span data-stu-id="e2825-123">string</span></span>  | <span data-ttu-id="e2825-124">Тип хранимого текста.</span><span class="sxs-lookup"><span data-stu-id="e2825-124">The type of text being stored.</span></span> <span data-ttu-id="e2825-125">Должно иметь тип `plain` или `richText`</span><span class="sxs-lookup"><span data-stu-id="e2825-125">Must be one of `plain` or `richText`</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/textcolumn.md:
      Found potential enums in resource example that weren't defined in a table:(plain,richText) are in resource, but () are in table"
  ],
  "tocPath": "Resources/TextColumn"
} -->
