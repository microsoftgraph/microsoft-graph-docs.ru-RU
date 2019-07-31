---
author: JeremyKelley
description: Ресурс choiceColumn в ресурсе columnDefinition указывает, что значения столбца можно выбрать из списка вариантов.
ms.date: 09/11/2017
title: choiceColumn
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 72ef8adb96614fc32b9aee8141eb19248e963639
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973508"
---
# <a name="choicecolumn-resource-type"></a><span data-ttu-id="5d5c2-103">Тип ресурса choiceColumn</span><span class="sxs-lookup"><span data-stu-id="5d5c2-103">ChoiceColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d5c2-104">Ресурс **choiceColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца можно выбрать из списка вариантов.</span><span class="sxs-lookup"><span data-stu-id="5d5c2-104">The **choiceColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values can be selected from a list of choices.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5d5c2-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="5d5c2-105">JSON representation</span></span>

<span data-ttu-id="5d5c2-106">Ниже показано представление ресурса **choiceColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5d5c2-106">Here is a JSON representation of a **choiceColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.choiceColumn" } -->

```json
{
  "allowTextEntry": true,
  "choices": ["red", "blue", "green"],
  "displayAs": "checkBoxes | dropDownMenu | radioButtons"
}
```

## <a name="properties"></a><span data-ttu-id="5d5c2-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5d5c2-107">Properties</span></span>

| <span data-ttu-id="5d5c2-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="5d5c2-108">Property name</span></span>      | <span data-ttu-id="5d5c2-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5d5c2-109">Type</span></span>               | <span data-ttu-id="5d5c2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5d5c2-110">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="5d5c2-111">**allowTextEntry**</span><span class="sxs-lookup"><span data-stu-id="5d5c2-111">**allowTextEntry**</span></span> | <span data-ttu-id="5d5c2-112">boolean</span><span class="sxs-lookup"><span data-stu-id="5d5c2-112">boolean</span></span>            | <span data-ttu-id="5d5c2-113">Если это свойство имеет значение true, то разрешено указывать значения, которых нет в списке заранее настроенных вариантов.</span><span class="sxs-lookup"><span data-stu-id="5d5c2-113">If true, allows custom values that aren't in the configured choices.</span></span>
| <span data-ttu-id="5d5c2-114">**choices**</span><span class="sxs-lookup"><span data-stu-id="5d5c2-114">**choices**</span></span>        | <span data-ttu-id="5d5c2-115">Коллекция (string)</span><span class="sxs-lookup"><span data-stu-id="5d5c2-115">collection(string)</span></span> | <span data-ttu-id="5d5c2-116">Список значений, доступных для данного столбца.</span><span class="sxs-lookup"><span data-stu-id="5d5c2-116">The list of values available for this column.</span></span>
| <span data-ttu-id="5d5c2-117">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="5d5c2-117">**displayAs**</span></span>      | <span data-ttu-id="5d5c2-118">string</span><span class="sxs-lookup"><span data-stu-id="5d5c2-118">string</span></span>             | <span data-ttu-id="5d5c2-119">Способ отображения вариантов в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="5d5c2-119">How the choices are to be presented in the UX.</span></span> <span data-ttu-id="5d5c2-120">Должно иметь один из типов `checkBoxes`, `dropDownMenu` или `radioButtons`.</span><span class="sxs-lookup"><span data-stu-id="5d5c2-120">Must be one of `checkBoxes`, `dropDownMenu`, or `radioButtons`</span></span>


<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ChoiceColumn",
  "suppressions": []
}
-->
