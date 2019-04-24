---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: TextColumn
localization_priority: Normal
ms.openlocfilehash: 1e10997bd70f97fa91177aee48a6ffcecff40ab5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32456999"
---
# <a name="textcolumn-resource-type"></a><span data-ttu-id="d7eaf-102">Тип ресурса textColumn</span><span class="sxs-lookup"><span data-stu-id="d7eaf-102">TextColumn resource type</span></span>

<span data-ttu-id="d7eaf-103">Ресурс **textColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют собой текст.</span><span class="sxs-lookup"><span data-stu-id="d7eaf-103">The **textColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are text.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d7eaf-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d7eaf-104">JSON representation</span></span>

<span data-ttu-id="d7eaf-105">Ниже показано представление ресурса **textColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d7eaf-105">Here is a JSON representation of a **textColumn** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="d7eaf-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="d7eaf-106">Properties</span></span>

| <span data-ttu-id="d7eaf-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="d7eaf-107">Property name</span></span>                   | <span data-ttu-id="d7eaf-108">Тип</span><span class="sxs-lookup"><span data-stu-id="d7eaf-108">Type</span></span>    | <span data-ttu-id="d7eaf-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d7eaf-109">Description</span></span>
|:--------------------------------|:--------|:---------------------------------
| <span data-ttu-id="d7eaf-110">**allowMultipleLines**</span><span class="sxs-lookup"><span data-stu-id="d7eaf-110">**allowMultipleLines**</span></span>          | <span data-ttu-id="d7eaf-111">логический</span><span class="sxs-lookup"><span data-stu-id="d7eaf-111">boolean</span></span> | <span data-ttu-id="d7eaf-112">Указывает, разрешено ли отображать несколько строк текста.</span><span class="sxs-lookup"><span data-stu-id="d7eaf-112">Whether to allow multiple lines of text.</span></span>
| <span data-ttu-id="d7eaf-113">**appendChangesToExistingText**</span><span class="sxs-lookup"><span data-stu-id="d7eaf-113">**appendChangesToExistingText**</span></span> | <span data-ttu-id="d7eaf-114">логический</span><span class="sxs-lookup"><span data-stu-id="d7eaf-114">boolean</span></span> | <span data-ttu-id="d7eaf-115">Указывает, что должно происходить при обновлении данного столбца: новый текст должен заменять существующий либо дополнять его.</span><span class="sxs-lookup"><span data-stu-id="d7eaf-115">Whether updates to this column should replace existing text, or append to it.</span></span>
| <span data-ttu-id="d7eaf-116">**linesForEditing**</span><span class="sxs-lookup"><span data-stu-id="d7eaf-116">**linesForEditing**</span></span>             | <span data-ttu-id="d7eaf-117">Int32</span><span class="sxs-lookup"><span data-stu-id="d7eaf-117">int32</span></span>   | <span data-ttu-id="d7eaf-118">Размер текстового поля.</span><span class="sxs-lookup"><span data-stu-id="d7eaf-118">The size of the text box.</span></span>
| <span data-ttu-id="d7eaf-119">**maxLength**</span><span class="sxs-lookup"><span data-stu-id="d7eaf-119">**maxLength**</span></span>                   | <span data-ttu-id="d7eaf-120">Int32</span><span class="sxs-lookup"><span data-stu-id="d7eaf-120">int32</span></span>   | <span data-ttu-id="d7eaf-121">Максимальное количество символов для значения.</span><span class="sxs-lookup"><span data-stu-id="d7eaf-121">The maximum number of characters for the value.</span></span>
| <span data-ttu-id="d7eaf-122">**textType**</span><span class="sxs-lookup"><span data-stu-id="d7eaf-122">**textType**</span></span>                    | <span data-ttu-id="d7eaf-123">string</span><span class="sxs-lookup"><span data-stu-id="d7eaf-123">string</span></span>  | <span data-ttu-id="d7eaf-124">Тип хранимого текста.</span><span class="sxs-lookup"><span data-stu-id="d7eaf-124">The type of text being stored.</span></span> <span data-ttu-id="d7eaf-125">Должно иметь тип `plain` или `richText`</span><span class="sxs-lookup"><span data-stu-id="d7eaf-125">Must be one of `plain` or `richText`</span></span>

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
