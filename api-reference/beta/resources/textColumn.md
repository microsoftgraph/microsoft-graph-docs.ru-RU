---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: TextColumn
localization_priority: Normal
ms.openlocfilehash: b57caa76f8376bbd7f119546009f3aca97b78385
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339834"
---
# <a name="textcolumn-resource-type"></a><span data-ttu-id="4b93f-102">Тип ресурса textColumn</span><span class="sxs-lookup"><span data-stu-id="4b93f-102">TextColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b93f-103">Ресурс **textColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют собой текст.</span><span class="sxs-lookup"><span data-stu-id="4b93f-103">The **textColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are text.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4b93f-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4b93f-104">JSON representation</span></span>

<span data-ttu-id="4b93f-105">Ниже показано представление ресурса **textColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4b93f-105">Here is a JSON representation of a **textColumn** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="4b93f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="4b93f-106">Properties</span></span>

| <span data-ttu-id="4b93f-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="4b93f-107">Property name</span></span>                   | <span data-ttu-id="4b93f-108">Тип</span><span class="sxs-lookup"><span data-stu-id="4b93f-108">Type</span></span>   | <span data-ttu-id="4b93f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4b93f-109">Description</span></span>
|:--------------------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="4b93f-110">**allowMultipleLines**</span><span class="sxs-lookup"><span data-stu-id="4b93f-110">**allowMultipleLines**</span></span>          | <span data-ttu-id="4b93f-111">string</span><span class="sxs-lookup"><span data-stu-id="4b93f-111">string</span></span> | <span data-ttu-id="4b93f-112">Указывает, разрешено ли отображать несколько строк текста.</span><span class="sxs-lookup"><span data-stu-id="4b93f-112">Whether to allow multiple lines of text.</span></span>
| <span data-ttu-id="4b93f-113">**appendChangesToExistingText**</span><span class="sxs-lookup"><span data-stu-id="4b93f-113">**appendChangesToExistingText**</span></span> | <span data-ttu-id="4b93f-114">string</span><span class="sxs-lookup"><span data-stu-id="4b93f-114">string</span></span> | <span data-ttu-id="4b93f-115">Указывает, что должно происходить при обновлении данного столбца: новый текст должен заменять существующий либо дополнять его.</span><span class="sxs-lookup"><span data-stu-id="4b93f-115">Whether updates to this column should replace existing text, or append to it.</span></span>
| <span data-ttu-id="4b93f-116">**linesForEditing**</span><span class="sxs-lookup"><span data-stu-id="4b93f-116">**linesForEditing**</span></span>             | <span data-ttu-id="4b93f-117">int</span><span class="sxs-lookup"><span data-stu-id="4b93f-117">int</span></span>    | <span data-ttu-id="4b93f-118">Размер текстового поля.</span><span class="sxs-lookup"><span data-stu-id="4b93f-118">The size of the text box.</span></span>
| <span data-ttu-id="4b93f-119">**maxLength**</span><span class="sxs-lookup"><span data-stu-id="4b93f-119">**maxLength**</span></span>                   | <span data-ttu-id="4b93f-120">int</span><span class="sxs-lookup"><span data-stu-id="4b93f-120">int</span></span>    | <span data-ttu-id="4b93f-121">Максимальное количество символов для значения.</span><span class="sxs-lookup"><span data-stu-id="4b93f-121">The maximum number of characters for the value.</span></span>
| <span data-ttu-id="4b93f-122">**textType**</span><span class="sxs-lookup"><span data-stu-id="4b93f-122">**textType**</span></span>                    | <span data-ttu-id="4b93f-123">string</span><span class="sxs-lookup"><span data-stu-id="4b93f-123">string</span></span> | <span data-ttu-id="4b93f-124">Тип хранимого текста.</span><span class="sxs-lookup"><span data-stu-id="4b93f-124">The type of text being stored.</span></span> <span data-ttu-id="4b93f-125">Должно иметь тип `plain` или `richText`</span><span class="sxs-lookup"><span data-stu-id="4b93f-125">Must be one of `plain` or `richText`</span></span>

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
