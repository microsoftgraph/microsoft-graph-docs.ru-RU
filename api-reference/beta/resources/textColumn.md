---
author: JeremyKelley
description: Ресурс textColumn в ресурсе columnDefinition указывает, что значения столбца представляют собой текст.
ms.date: 09/11/2017
title: TextColumn
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: ecfd6d72e0946519b570962577b03a9ffcbcdf10
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973549"
---
# <a name="textcolumn-resource-type"></a><span data-ttu-id="87505-103">Тип ресурса textColumn</span><span class="sxs-lookup"><span data-stu-id="87505-103">TextColumn resource type</span></span>

<span data-ttu-id="87505-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87505-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87505-105">Ресурс **textColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют собой текст.</span><span class="sxs-lookup"><span data-stu-id="87505-105">The **textColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are text.</span></span>

## <a name="json-representation"></a><span data-ttu-id="87505-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="87505-106">JSON representation</span></span>

<span data-ttu-id="87505-107">Ниже показано представление ресурса **textColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="87505-107">Here is a JSON representation of a **textColumn** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="87505-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="87505-108">Properties</span></span>

| <span data-ttu-id="87505-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="87505-109">Property name</span></span>                   | <span data-ttu-id="87505-110">Тип</span><span class="sxs-lookup"><span data-stu-id="87505-110">Type</span></span>   | <span data-ttu-id="87505-111">Описание</span><span class="sxs-lookup"><span data-stu-id="87505-111">Description</span></span>
|:--------------------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="87505-112">**allowMultipleLines**</span><span class="sxs-lookup"><span data-stu-id="87505-112">**allowMultipleLines**</span></span>          | <span data-ttu-id="87505-113">string</span><span class="sxs-lookup"><span data-stu-id="87505-113">string</span></span> | <span data-ttu-id="87505-114">Указывает, разрешено ли отображать несколько строк текста.</span><span class="sxs-lookup"><span data-stu-id="87505-114">Whether to allow multiple lines of text.</span></span>
| <span data-ttu-id="87505-115">**appendChangesToExistingText**</span><span class="sxs-lookup"><span data-stu-id="87505-115">**appendChangesToExistingText**</span></span> | <span data-ttu-id="87505-116">string</span><span class="sxs-lookup"><span data-stu-id="87505-116">string</span></span> | <span data-ttu-id="87505-117">Указывает, что должно происходить при обновлении данного столбца: новый текст должен заменять существующий либо дополнять его.</span><span class="sxs-lookup"><span data-stu-id="87505-117">Whether updates to this column should replace existing text, or append to it.</span></span>
| <span data-ttu-id="87505-118">**linesForEditing**</span><span class="sxs-lookup"><span data-stu-id="87505-118">**linesForEditing**</span></span>             | <span data-ttu-id="87505-119">int</span><span class="sxs-lookup"><span data-stu-id="87505-119">int</span></span>    | <span data-ttu-id="87505-120">Размер текстового поля.</span><span class="sxs-lookup"><span data-stu-id="87505-120">The size of the text box.</span></span>
| <span data-ttu-id="87505-121">**maxLength**</span><span class="sxs-lookup"><span data-stu-id="87505-121">**maxLength**</span></span>                   | <span data-ttu-id="87505-122">int</span><span class="sxs-lookup"><span data-stu-id="87505-122">int</span></span>    | <span data-ttu-id="87505-123">Максимальное количество символов для значения.</span><span class="sxs-lookup"><span data-stu-id="87505-123">The maximum number of characters for the value.</span></span>
| <span data-ttu-id="87505-124">**textType**</span><span class="sxs-lookup"><span data-stu-id="87505-124">**textType**</span></span>                    | <span data-ttu-id="87505-125">string</span><span class="sxs-lookup"><span data-stu-id="87505-125">string</span></span> | <span data-ttu-id="87505-126">Тип хранимого текста.</span><span class="sxs-lookup"><span data-stu-id="87505-126">The type of text being stored.</span></span> <span data-ttu-id="87505-127">Должно иметь тип `plain` или `richText`</span><span class="sxs-lookup"><span data-stu-id="87505-127">Must be one of `plain` or `richText`</span></span>

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


