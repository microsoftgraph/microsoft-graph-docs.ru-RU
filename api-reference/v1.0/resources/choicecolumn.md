---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: choiceColumn
localization_priority: Normal
description: Ресурс choiceColumn в ресурсе columnDefinition указывает, что значения столбца можно выбрать из списка вариантов.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a86cb783fb170c2b9528b47272fc214ea0010760
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029738"
---
# <a name="choicecolumn-resource-type"></a><span data-ttu-id="3a236-103">Тип ресурса choiceColumn</span><span class="sxs-lookup"><span data-stu-id="3a236-103">ChoiceColumn resource type</span></span>

<span data-ttu-id="3a236-104">Ресурс **choiceColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца можно выбрать из списка вариантов.</span><span class="sxs-lookup"><span data-stu-id="3a236-104">The **choiceColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values can be selected from a list of choices.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3a236-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="3a236-105">JSON representation</span></span>

<span data-ttu-id="3a236-106">Ниже показано представление ресурса **choiceColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3a236-106">Here is a JSON representation of a **choiceColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.choiceColumn" } -->

```json
{
  "allowTextEntry": true,
  "choices": ["red", "blue", "green"],
  "displayAs": "checkBoxes | dropDownMenu | radioButtons"
}
```

## <a name="properties"></a><span data-ttu-id="3a236-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="3a236-107">Properties</span></span>

| <span data-ttu-id="3a236-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="3a236-108">Property name</span></span>      | <span data-ttu-id="3a236-109">Тип</span><span class="sxs-lookup"><span data-stu-id="3a236-109">Type</span></span>               | <span data-ttu-id="3a236-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3a236-110">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="3a236-111">**allowTextEntry**</span><span class="sxs-lookup"><span data-stu-id="3a236-111">**allowTextEntry**</span></span> | <span data-ttu-id="3a236-112">boolean</span><span class="sxs-lookup"><span data-stu-id="3a236-112">boolean</span></span>            | <span data-ttu-id="3a236-113">Если это свойство имеет значение true, то разрешено указывать значения, которых нет в списке заранее настроенных вариантов.</span><span class="sxs-lookup"><span data-stu-id="3a236-113">If true, allows custom values that aren't in the configured choices.</span></span>
| <span data-ttu-id="3a236-114">**choices**</span><span class="sxs-lookup"><span data-stu-id="3a236-114">**choices**</span></span>        | <span data-ttu-id="3a236-115">Коллекция (string)</span><span class="sxs-lookup"><span data-stu-id="3a236-115">collection(string)</span></span> | <span data-ttu-id="3a236-116">Список значений, доступных для данного столбца.</span><span class="sxs-lookup"><span data-stu-id="3a236-116">The list of values available for this column.</span></span>
| <span data-ttu-id="3a236-117">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="3a236-117">**displayAs**</span></span>      | <span data-ttu-id="3a236-118">string</span><span class="sxs-lookup"><span data-stu-id="3a236-118">string</span></span>             | <span data-ttu-id="3a236-119">Способ отображения вариантов в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="3a236-119">How the choices are to be presented in the UX.</span></span> <span data-ttu-id="3a236-120">Должно иметь один из типов `checkBoxes`, `dropDownMenu` или `radioButtons`.</span><span class="sxs-lookup"><span data-stu-id="3a236-120">Must be one of `checkBoxes`, `dropDownMenu`, or `radioButtons`</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/choicecolumn.md:
      Found potential enums in resource example that weren't defined in a table:(checkBoxes,dropDownMenu,radioButtons) are in resource, but () are in table"
  ],
  "tocPath": "Resources/ChoiceColumn"
} -->
