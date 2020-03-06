---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: TextColumn
localization_priority: Normal
description: Ресурс textColumn в ресурсе columnDefinition указывает, что значения столбца представляют собой текст.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 67e6b1f24155a8cfcecb2fb2443f3b1536ba48bd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533472"
---
# <a name="textcolumn-resource-type"></a><span data-ttu-id="f3bd2-103">Тип ресурса textColumn</span><span class="sxs-lookup"><span data-stu-id="f3bd2-103">TextColumn resource type</span></span>

<span data-ttu-id="f3bd2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3bd2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f3bd2-105">Ресурс **textColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют собой текст.</span><span class="sxs-lookup"><span data-stu-id="f3bd2-105">The **textColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are text.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f3bd2-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f3bd2-106">JSON representation</span></span>

<span data-ttu-id="f3bd2-107">Ниже показано представление ресурса **textColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f3bd2-107">Here is a JSON representation of a **textColumn** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="f3bd2-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f3bd2-108">Properties</span></span>

| <span data-ttu-id="f3bd2-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="f3bd2-109">Property name</span></span>                   | <span data-ttu-id="f3bd2-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f3bd2-110">Type</span></span>    | <span data-ttu-id="f3bd2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f3bd2-111">Description</span></span>
|:--------------------------------|:--------|:---------------------------------
| <span data-ttu-id="f3bd2-112">**allowMultipleLines**</span><span class="sxs-lookup"><span data-stu-id="f3bd2-112">**allowMultipleLines**</span></span>          | <span data-ttu-id="f3bd2-113">boolean</span><span class="sxs-lookup"><span data-stu-id="f3bd2-113">boolean</span></span> | <span data-ttu-id="f3bd2-114">Указывает, разрешено ли отображать несколько строк текста.</span><span class="sxs-lookup"><span data-stu-id="f3bd2-114">Whether to allow multiple lines of text.</span></span>
| <span data-ttu-id="f3bd2-115">**appendChangesToExistingText**</span><span class="sxs-lookup"><span data-stu-id="f3bd2-115">**appendChangesToExistingText**</span></span> | <span data-ttu-id="f3bd2-116">boolean</span><span class="sxs-lookup"><span data-stu-id="f3bd2-116">boolean</span></span> | <span data-ttu-id="f3bd2-117">Указывает, что должно происходить при обновлении данного столбца: новый текст должен заменять существующий либо дополнять его.</span><span class="sxs-lookup"><span data-stu-id="f3bd2-117">Whether updates to this column should replace existing text, or append to it.</span></span>
| <span data-ttu-id="f3bd2-118">**linesForEditing**</span><span class="sxs-lookup"><span data-stu-id="f3bd2-118">**linesForEditing**</span></span>             | <span data-ttu-id="f3bd2-119">int32</span><span class="sxs-lookup"><span data-stu-id="f3bd2-119">int32</span></span>   | <span data-ttu-id="f3bd2-120">Размер текстового поля.</span><span class="sxs-lookup"><span data-stu-id="f3bd2-120">The size of the text box.</span></span>
| <span data-ttu-id="f3bd2-121">**maxLength**</span><span class="sxs-lookup"><span data-stu-id="f3bd2-121">**maxLength**</span></span>                   | <span data-ttu-id="f3bd2-122">int32</span><span class="sxs-lookup"><span data-stu-id="f3bd2-122">int32</span></span>   | <span data-ttu-id="f3bd2-123">Максимальное количество символов для значения.</span><span class="sxs-lookup"><span data-stu-id="f3bd2-123">The maximum number of characters for the value.</span></span>
| <span data-ttu-id="f3bd2-124">**textType**</span><span class="sxs-lookup"><span data-stu-id="f3bd2-124">**textType**</span></span>                    | <span data-ttu-id="f3bd2-125">string</span><span class="sxs-lookup"><span data-stu-id="f3bd2-125">string</span></span>  | <span data-ttu-id="f3bd2-126">Тип хранимого текста.</span><span class="sxs-lookup"><span data-stu-id="f3bd2-126">The type of text being stored.</span></span> <span data-ttu-id="f3bd2-127">Должно иметь тип `plain` или `richText`</span><span class="sxs-lookup"><span data-stu-id="f3bd2-127">Must be one of `plain` or `richText`</span></span>

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
