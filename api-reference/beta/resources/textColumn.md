---
author: JeremyKelley
description: Ресурс textColumn в ресурсе columnDefinition указывает, что значения столбца представляют собой текст.
ms.date: 09/11/2017
title: TextColumn
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 6681875328695d2e67cc10508f47183fcedb0df4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964344"
---
# <a name="textcolumn-resource-type"></a><span data-ttu-id="0e9e7-103">Тип ресурса textColumn</span><span class="sxs-lookup"><span data-stu-id="0e9e7-103">TextColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e9e7-104">Ресурс **textColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют собой текст.</span><span class="sxs-lookup"><span data-stu-id="0e9e7-104">The **textColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are text.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0e9e7-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="0e9e7-105">JSON representation</span></span>

<span data-ttu-id="0e9e7-106">Ниже показано представление ресурса **textColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0e9e7-106">Here is a JSON representation of a **textColumn** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="0e9e7-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="0e9e7-107">Properties</span></span>

| <span data-ttu-id="0e9e7-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="0e9e7-108">Property name</span></span>                   | <span data-ttu-id="0e9e7-109">Тип</span><span class="sxs-lookup"><span data-stu-id="0e9e7-109">Type</span></span>   | <span data-ttu-id="0e9e7-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0e9e7-110">Description</span></span>
|:--------------------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="0e9e7-111">**allowMultipleLines**</span><span class="sxs-lookup"><span data-stu-id="0e9e7-111">**allowMultipleLines**</span></span>          | <span data-ttu-id="0e9e7-112">string</span><span class="sxs-lookup"><span data-stu-id="0e9e7-112">string</span></span> | <span data-ttu-id="0e9e7-113">Указывает, разрешено ли отображать несколько строк текста.</span><span class="sxs-lookup"><span data-stu-id="0e9e7-113">Whether to allow multiple lines of text.</span></span>
| <span data-ttu-id="0e9e7-114">**appendChangesToExistingText**</span><span class="sxs-lookup"><span data-stu-id="0e9e7-114">**appendChangesToExistingText**</span></span> | <span data-ttu-id="0e9e7-115">string</span><span class="sxs-lookup"><span data-stu-id="0e9e7-115">string</span></span> | <span data-ttu-id="0e9e7-116">Указывает, что должно происходить при обновлении данного столбца: новый текст должен заменять существующий либо дополнять его.</span><span class="sxs-lookup"><span data-stu-id="0e9e7-116">Whether updates to this column should replace existing text, or append to it.</span></span>
| <span data-ttu-id="0e9e7-117">**linesForEditing**</span><span class="sxs-lookup"><span data-stu-id="0e9e7-117">**linesForEditing**</span></span>             | <span data-ttu-id="0e9e7-118">int</span><span class="sxs-lookup"><span data-stu-id="0e9e7-118">int</span></span>    | <span data-ttu-id="0e9e7-119">Размер текстового поля.</span><span class="sxs-lookup"><span data-stu-id="0e9e7-119">The size of the text box.</span></span>
| <span data-ttu-id="0e9e7-120">**maxLength**</span><span class="sxs-lookup"><span data-stu-id="0e9e7-120">**maxLength**</span></span>                   | <span data-ttu-id="0e9e7-121">int</span><span class="sxs-lookup"><span data-stu-id="0e9e7-121">int</span></span>    | <span data-ttu-id="0e9e7-122">Максимальное количество символов для значения.</span><span class="sxs-lookup"><span data-stu-id="0e9e7-122">The maximum number of characters for the value.</span></span>
| <span data-ttu-id="0e9e7-123">**textType**</span><span class="sxs-lookup"><span data-stu-id="0e9e7-123">**textType**</span></span>                    | <span data-ttu-id="0e9e7-124">string</span><span class="sxs-lookup"><span data-stu-id="0e9e7-124">string</span></span> | <span data-ttu-id="0e9e7-125">Тип хранимого текста.</span><span class="sxs-lookup"><span data-stu-id="0e9e7-125">The type of text being stored.</span></span> <span data-ttu-id="0e9e7-126">Должно иметь тип `plain` или `richText`</span><span class="sxs-lookup"><span data-stu-id="0e9e7-126">Must be one of `plain` or `richText`</span></span>

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
