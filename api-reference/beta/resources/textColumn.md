---
author: JeremyKelley
description: Ресурс textColumn в ресурсе columnDefinition указывает, что значения столбца представляют собой текст.
ms.date: 09/11/2017
title: TextColumn
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: e6167a81c0898b2de1c5878926633f8dbd0baa2d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519794"
---
# <a name="textcolumn-resource-type"></a><span data-ttu-id="535fc-103">Тип ресурса textColumn</span><span class="sxs-lookup"><span data-stu-id="535fc-103">TextColumn resource type</span></span>

<span data-ttu-id="535fc-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="535fc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="535fc-105">Ресурс **textColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют собой текст.</span><span class="sxs-lookup"><span data-stu-id="535fc-105">The **textColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are text.</span></span>

## <a name="json-representation"></a><span data-ttu-id="535fc-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="535fc-106">JSON representation</span></span>

<span data-ttu-id="535fc-107">Ниже показано представление ресурса **textColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="535fc-107">Here is a JSON representation of a **textColumn** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="535fc-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="535fc-108">Properties</span></span>

| <span data-ttu-id="535fc-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="535fc-109">Property name</span></span>                   | <span data-ttu-id="535fc-110">Тип</span><span class="sxs-lookup"><span data-stu-id="535fc-110">Type</span></span>   | <span data-ttu-id="535fc-111">Описание</span><span class="sxs-lookup"><span data-stu-id="535fc-111">Description</span></span>
|:--------------------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="535fc-112">**allowMultipleLines**</span><span class="sxs-lookup"><span data-stu-id="535fc-112">**allowMultipleLines**</span></span>          | <span data-ttu-id="535fc-113">строка</span><span class="sxs-lookup"><span data-stu-id="535fc-113">string</span></span> | <span data-ttu-id="535fc-114">Указывает, разрешено ли отображать несколько строк текста.</span><span class="sxs-lookup"><span data-stu-id="535fc-114">Whether to allow multiple lines of text.</span></span>
| <span data-ttu-id="535fc-115">**appendChangesToExistingText**</span><span class="sxs-lookup"><span data-stu-id="535fc-115">**appendChangesToExistingText**</span></span> | <span data-ttu-id="535fc-116">строка</span><span class="sxs-lookup"><span data-stu-id="535fc-116">string</span></span> | <span data-ttu-id="535fc-117">Указывает, что должно происходить при обновлении данного столбца: новый текст должен заменять существующий либо дополнять его.</span><span class="sxs-lookup"><span data-stu-id="535fc-117">Whether updates to this column should replace existing text, or append to it.</span></span>
| <span data-ttu-id="535fc-118">**linesForEditing**</span><span class="sxs-lookup"><span data-stu-id="535fc-118">**linesForEditing**</span></span>             | <span data-ttu-id="535fc-119">int</span><span class="sxs-lookup"><span data-stu-id="535fc-119">int</span></span>    | <span data-ttu-id="535fc-120">Размер текстового поля.</span><span class="sxs-lookup"><span data-stu-id="535fc-120">The size of the text box.</span></span>
| <span data-ttu-id="535fc-121">**maxLength**</span><span class="sxs-lookup"><span data-stu-id="535fc-121">**maxLength**</span></span>                   | <span data-ttu-id="535fc-122">int</span><span class="sxs-lookup"><span data-stu-id="535fc-122">int</span></span>    | <span data-ttu-id="535fc-123">Максимальное количество символов для значения.</span><span class="sxs-lookup"><span data-stu-id="535fc-123">The maximum number of characters for the value.</span></span>
| <span data-ttu-id="535fc-124">**textType**</span><span class="sxs-lookup"><span data-stu-id="535fc-124">**textType**</span></span>                    | <span data-ttu-id="535fc-125">string</span><span class="sxs-lookup"><span data-stu-id="535fc-125">string</span></span> | <span data-ttu-id="535fc-126">Тип хранимого текста.</span><span class="sxs-lookup"><span data-stu-id="535fc-126">The type of text being stored.</span></span> <span data-ttu-id="535fc-127">Должно иметь тип `plain` или `richText`</span><span class="sxs-lookup"><span data-stu-id="535fc-127">Must be one of `plain` or `richText`</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/TextColumn",
  "suppressions": []
}
-->
