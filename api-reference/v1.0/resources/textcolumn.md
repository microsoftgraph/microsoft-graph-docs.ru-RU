---
author: JeremyKelley
ms.date: 09/11/2017
title: TextColumn
localization_priority: Normal
description: Ресурс textColumn в ресурсе columnDefinition указывает, что значения столбца представляют собой текст.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 62711f2f44004e5b3d594eb472b7c018205d9e31
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239276"
---
# <a name="textcolumn-resource-type"></a><span data-ttu-id="95c6e-103">Тип ресурса textColumn</span><span class="sxs-lookup"><span data-stu-id="95c6e-103">TextColumn resource type</span></span>

<span data-ttu-id="95c6e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95c6e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="95c6e-105">Ресурс **textColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют собой текст.</span><span class="sxs-lookup"><span data-stu-id="95c6e-105">The **textColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are text.</span></span>

## <a name="json-representation"></a><span data-ttu-id="95c6e-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="95c6e-106">JSON representation</span></span>

<span data-ttu-id="95c6e-107">Ниже показано представление ресурса **textColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="95c6e-107">Here is a JSON representation of a **textColumn** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="95c6e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="95c6e-108">Properties</span></span>

| <span data-ttu-id="95c6e-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="95c6e-109">Property name</span></span>                   | <span data-ttu-id="95c6e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="95c6e-110">Type</span></span>    | <span data-ttu-id="95c6e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="95c6e-111">Description</span></span>
|:--------------------------------|:--------|:---------------------------------
| <span data-ttu-id="95c6e-112">**allowMultipleLines**</span><span class="sxs-lookup"><span data-stu-id="95c6e-112">**allowMultipleLines**</span></span>          | <span data-ttu-id="95c6e-113">boolean</span><span class="sxs-lookup"><span data-stu-id="95c6e-113">boolean</span></span> | <span data-ttu-id="95c6e-114">Указывает, разрешено ли отображать несколько строк текста.</span><span class="sxs-lookup"><span data-stu-id="95c6e-114">Whether to allow multiple lines of text.</span></span>
| <span data-ttu-id="95c6e-115">**appendChangesToExistingText**</span><span class="sxs-lookup"><span data-stu-id="95c6e-115">**appendChangesToExistingText**</span></span> | <span data-ttu-id="95c6e-116">boolean</span><span class="sxs-lookup"><span data-stu-id="95c6e-116">boolean</span></span> | <span data-ttu-id="95c6e-117">Указывает, что должно происходить при обновлении данного столбца: новый текст должен заменять существующий либо дополнять его.</span><span class="sxs-lookup"><span data-stu-id="95c6e-117">Whether updates to this column should replace existing text, or append to it.</span></span>
| <span data-ttu-id="95c6e-118">**linesForEditing**</span><span class="sxs-lookup"><span data-stu-id="95c6e-118">**linesForEditing**</span></span>             | <span data-ttu-id="95c6e-119">int32</span><span class="sxs-lookup"><span data-stu-id="95c6e-119">int32</span></span>   | <span data-ttu-id="95c6e-120">Размер текстового поля.</span><span class="sxs-lookup"><span data-stu-id="95c6e-120">The size of the text box.</span></span>
| <span data-ttu-id="95c6e-121">**maxLength**</span><span class="sxs-lookup"><span data-stu-id="95c6e-121">**maxLength**</span></span>                   | <span data-ttu-id="95c6e-122">int32</span><span class="sxs-lookup"><span data-stu-id="95c6e-122">int32</span></span>   | <span data-ttu-id="95c6e-123">Максимальное количество символов для значения.</span><span class="sxs-lookup"><span data-stu-id="95c6e-123">The maximum number of characters for the value.</span></span>
| <span data-ttu-id="95c6e-124">**textType**</span><span class="sxs-lookup"><span data-stu-id="95c6e-124">**textType**</span></span>                    | <span data-ttu-id="95c6e-125">string</span><span class="sxs-lookup"><span data-stu-id="95c6e-125">string</span></span>  | <span data-ttu-id="95c6e-126">Тип хранимого текста.</span><span class="sxs-lookup"><span data-stu-id="95c6e-126">The type of text being stored.</span></span> <span data-ttu-id="95c6e-127">Должно иметь тип `plain` или `richText`</span><span class="sxs-lookup"><span data-stu-id="95c6e-127">Must be one of `plain` or `richText`</span></span>

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

