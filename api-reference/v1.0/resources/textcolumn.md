---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: TextColumn
localization_priority: Normal
description: Ресурс textColumn в ресурсе columnDefinition указывает, что значения столбца представляют собой текст.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 37a5bbd985d163cf627f4bc0a16a756eaf00af66
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033658"
---
# <a name="textcolumn-resource-type"></a><span data-ttu-id="a4fbd-103">Тип ресурса textColumn</span><span class="sxs-lookup"><span data-stu-id="a4fbd-103">TextColumn resource type</span></span>

<span data-ttu-id="a4fbd-104">Ресурс **textColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют собой текст.</span><span class="sxs-lookup"><span data-stu-id="a4fbd-104">The **textColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are text.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a4fbd-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a4fbd-105">JSON representation</span></span>

<span data-ttu-id="a4fbd-106">Ниже показано представление ресурса **textColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a4fbd-106">Here is a JSON representation of a **textColumn** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="a4fbd-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a4fbd-107">Properties</span></span>

| <span data-ttu-id="a4fbd-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="a4fbd-108">Property name</span></span>                   | <span data-ttu-id="a4fbd-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a4fbd-109">Type</span></span>    | <span data-ttu-id="a4fbd-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a4fbd-110">Description</span></span>
|:--------------------------------|:--------|:---------------------------------
| <span data-ttu-id="a4fbd-111">**allowMultipleLines**</span><span class="sxs-lookup"><span data-stu-id="a4fbd-111">**allowMultipleLines**</span></span>          | <span data-ttu-id="a4fbd-112">boolean</span><span class="sxs-lookup"><span data-stu-id="a4fbd-112">boolean</span></span> | <span data-ttu-id="a4fbd-113">Указывает, разрешено ли отображать несколько строк текста.</span><span class="sxs-lookup"><span data-stu-id="a4fbd-113">Whether to allow multiple lines of text.</span></span>
| <span data-ttu-id="a4fbd-114">**appendChangesToExistingText**</span><span class="sxs-lookup"><span data-stu-id="a4fbd-114">**appendChangesToExistingText**</span></span> | <span data-ttu-id="a4fbd-115">boolean</span><span class="sxs-lookup"><span data-stu-id="a4fbd-115">boolean</span></span> | <span data-ttu-id="a4fbd-116">Указывает, что должно происходить при обновлении данного столбца: новый текст должен заменять существующий либо дополнять его.</span><span class="sxs-lookup"><span data-stu-id="a4fbd-116">Whether updates to this column should replace existing text, or append to it.</span></span>
| <span data-ttu-id="a4fbd-117">**linesForEditing**</span><span class="sxs-lookup"><span data-stu-id="a4fbd-117">**linesForEditing**</span></span>             | <span data-ttu-id="a4fbd-118">int32</span><span class="sxs-lookup"><span data-stu-id="a4fbd-118">int32</span></span>   | <span data-ttu-id="a4fbd-119">Размер текстового поля.</span><span class="sxs-lookup"><span data-stu-id="a4fbd-119">The size of the text box.</span></span>
| <span data-ttu-id="a4fbd-120">**maxLength**</span><span class="sxs-lookup"><span data-stu-id="a4fbd-120">**maxLength**</span></span>                   | <span data-ttu-id="a4fbd-121">int32</span><span class="sxs-lookup"><span data-stu-id="a4fbd-121">int32</span></span>   | <span data-ttu-id="a4fbd-122">Максимальное количество символов для значения.</span><span class="sxs-lookup"><span data-stu-id="a4fbd-122">The maximum number of characters for the value.</span></span>
| <span data-ttu-id="a4fbd-123">**textType**</span><span class="sxs-lookup"><span data-stu-id="a4fbd-123">**textType**</span></span>                    | <span data-ttu-id="a4fbd-124">string</span><span class="sxs-lookup"><span data-stu-id="a4fbd-124">string</span></span>  | <span data-ttu-id="a4fbd-125">Тип хранимого текста.</span><span class="sxs-lookup"><span data-stu-id="a4fbd-125">The type of text being stored.</span></span> <span data-ttu-id="a4fbd-126">Должно иметь тип `plain` или `richText`</span><span class="sxs-lookup"><span data-stu-id="a4fbd-126">Must be one of `plain` or `richText`</span></span>

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
