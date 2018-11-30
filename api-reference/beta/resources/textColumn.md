---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: textColumn
ms.openlocfilehash: 5ff280b6c969d9832e2f81f77dc32237f9905aad
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078304"
---
# <a name="textcolumn-resource-type"></a><span data-ttu-id="2c540-102">Тип ресурса textColumn</span><span class="sxs-lookup"><span data-stu-id="2c540-102">TextColumn resource type</span></span>

> <span data-ttu-id="2c540-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2c540-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2c540-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c540-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2c540-105">Ресурс **textColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют собой текст.</span><span class="sxs-lookup"><span data-stu-id="2c540-105">The **textColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are text.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2c540-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="2c540-106">JSON representation</span></span>

<span data-ttu-id="2c540-107">Ниже показано представление ресурса **textColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2c540-107">Here is a JSON representation of a **textColumn** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="2c540-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="2c540-108">Properties</span></span>

| <span data-ttu-id="2c540-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="2c540-109">Property name</span></span>                   | <span data-ttu-id="2c540-110">Тип</span><span class="sxs-lookup"><span data-stu-id="2c540-110">Type</span></span>   | <span data-ttu-id="2c540-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2c540-111">Description</span></span>
|:--------------------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="2c540-112">**allowMultipleLines**</span><span class="sxs-lookup"><span data-stu-id="2c540-112">**allowMultipleLines**</span></span>          | <span data-ttu-id="2c540-113">строка</span><span class="sxs-lookup"><span data-stu-id="2c540-113">string</span></span> | <span data-ttu-id="2c540-114">Указывает, разрешено ли отображать несколько строк текста.</span><span class="sxs-lookup"><span data-stu-id="2c540-114">Whether to allow multiple lines of text.</span></span>
| <span data-ttu-id="2c540-115">**appendChangesToExistingText**</span><span class="sxs-lookup"><span data-stu-id="2c540-115">**appendChangesToExistingText**</span></span> | <span data-ttu-id="2c540-116">строка</span><span class="sxs-lookup"><span data-stu-id="2c540-116">string</span></span> | <span data-ttu-id="2c540-117">Указывает, что должно происходить при обновлении данного столбца: новый текст должен заменять существующий либо дополнять его.</span><span class="sxs-lookup"><span data-stu-id="2c540-117">Whether updates to this column should replace existing text, or append to it.</span></span>
| <span data-ttu-id="2c540-118">**linesForEditing**</span><span class="sxs-lookup"><span data-stu-id="2c540-118">**linesForEditing**</span></span>             | <span data-ttu-id="2c540-119">целое</span><span class="sxs-lookup"><span data-stu-id="2c540-119">int</span></span>    | <span data-ttu-id="2c540-120">Размер текстового поля.</span><span class="sxs-lookup"><span data-stu-id="2c540-120">The size of the text box.</span></span>
| <span data-ttu-id="2c540-121">**maxLength**</span><span class="sxs-lookup"><span data-stu-id="2c540-121">**maxLength**</span></span>                   | <span data-ttu-id="2c540-122">целое</span><span class="sxs-lookup"><span data-stu-id="2c540-122">int</span></span>    | <span data-ttu-id="2c540-123">Максимальное количество символов для значения.</span><span class="sxs-lookup"><span data-stu-id="2c540-123">The maximum number of characters for the value.</span></span>
| <span data-ttu-id="2c540-124">**textType**</span><span class="sxs-lookup"><span data-stu-id="2c540-124">**textType**</span></span>                    | <span data-ttu-id="2c540-125">строка</span><span class="sxs-lookup"><span data-stu-id="2c540-125">string</span></span> | <span data-ttu-id="2c540-126">Тип хранимого текста.</span><span class="sxs-lookup"><span data-stu-id="2c540-126">The type of text being stored.</span></span> <span data-ttu-id="2c540-127">Должно иметь тип `plain` или `richText`</span><span class="sxs-lookup"><span data-stu-id="2c540-127">Must be one of `plain` or `richText`</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/TextColumn"
} -->
