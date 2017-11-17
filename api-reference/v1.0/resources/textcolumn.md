---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: textColumn
ms.openlocfilehash: 80e41b379b9b4ce51a3ee6c910447a22f43356c3
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="textcolumn-resource-type"></a><span data-ttu-id="255c7-102">Тип ресурса textColumn</span><span class="sxs-lookup"><span data-stu-id="255c7-102">TextColumn resource type</span></span>

<span data-ttu-id="255c7-103">Ресурс **textColumn** в ресурсе [columnDefinition](columnDefinition.md) указывает, что значения столбца представляют собой текст.</span><span class="sxs-lookup"><span data-stu-id="255c7-103">The **textColumn** on a [columnDefinition](columnDefinition.md) resource indicates that the column's values are text.</span></span>

## <a name="json-representation"></a><span data-ttu-id="255c7-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="255c7-104">JSON representation</span></span>

<span data-ttu-id="255c7-105">Ниже показано представление ресурса **textColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="255c7-105">Here is a JSON representation of a **baseItem** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="255c7-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="255c7-106">Properties</span></span>

| <span data-ttu-id="255c7-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="255c7-107">Property name</span></span>                   | <span data-ttu-id="255c7-108">Тип</span><span class="sxs-lookup"><span data-stu-id="255c7-108">Type</span></span>   | <span data-ttu-id="255c7-109">Описание</span><span class="sxs-lookup"><span data-stu-id="255c7-109">Description</span></span>
|:--------------------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="255c7-110">**allowMultipleLines**</span><span class="sxs-lookup"><span data-stu-id="255c7-110">**allowMultipleLines**</span></span>          | <span data-ttu-id="255c7-111">строка</span><span class="sxs-lookup"><span data-stu-id="255c7-111">string</span></span> | <span data-ttu-id="255c7-112">Указывает, разрешено ли отображать несколько строк текста.</span><span class="sxs-lookup"><span data-stu-id="255c7-112">Whether to allow multiple lines of text.</span></span>
| <span data-ttu-id="255c7-113">**appendChangesToExistingText**</span><span class="sxs-lookup"><span data-stu-id="255c7-113">**appendChangesToExistingText**</span></span> | <span data-ttu-id="255c7-114">строка</span><span class="sxs-lookup"><span data-stu-id="255c7-114">string</span></span> | <span data-ttu-id="255c7-115">Указывает, что должно происходить при изменении столбца: новый текст должен заменять существующий либо дополнять его.</span><span class="sxs-lookup"><span data-stu-id="255c7-115">Whether updates to this column should replace existing text, or append to it.</span></span>
| <span data-ttu-id="255c7-116">**linesForEditing**</span><span class="sxs-lookup"><span data-stu-id="255c7-116">**linesForEditing**</span></span>             | <span data-ttu-id="255c7-117">int</span><span class="sxs-lookup"><span data-stu-id="255c7-117">int</span></span>    | <span data-ttu-id="255c7-118">Размер текстового поля.</span><span class="sxs-lookup"><span data-stu-id="255c7-118">Optional. The width of the text box in pixels.</span></span>
| <span data-ttu-id="255c7-119">**maxLength**</span><span class="sxs-lookup"><span data-stu-id="255c7-119">**maxLength**</span></span>                   | <span data-ttu-id="255c7-120">int</span><span class="sxs-lookup"><span data-stu-id="255c7-120">int</span></span>    | <span data-ttu-id="255c7-121">Максимальное количество символов для значения.</span><span class="sxs-lookup"><span data-stu-id="255c7-121">The maximum number of characters for the value.</span></span>
| <span data-ttu-id="255c7-122">**textType**</span><span class="sxs-lookup"><span data-stu-id="255c7-122">**textType**</span></span>                    | <span data-ttu-id="255c7-123">строка</span><span class="sxs-lookup"><span data-stu-id="255c7-123">string</span></span> | <span data-ttu-id="255c7-124">Тип хранимого текста.</span><span class="sxs-lookup"><span data-stu-id="255c7-124">The type of text being stored.</span></span> <span data-ttu-id="255c7-125">Должно иметь тип `plain` или `richText`</span><span class="sxs-lookup"><span data-stu-id="255c7-125">Must be one of `plain` or `richText`</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/TextColumn"
} -->
