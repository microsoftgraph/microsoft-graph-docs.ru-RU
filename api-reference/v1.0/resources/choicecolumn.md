---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: choiceColumn
localization_priority: Normal
description: Ресурс choiceColumn в ресурсе columnDefinition указывает, что значения столбца можно выбрать из списка вариантов.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a29a80bccd2afb76804b2e1a4d81b5a69d44adf1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533074"
---
# <a name="choicecolumn-resource-type"></a><span data-ttu-id="4a51b-103">Тип ресурса choiceColumn</span><span class="sxs-lookup"><span data-stu-id="4a51b-103">ChoiceColumn resource type</span></span>

<span data-ttu-id="4a51b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a51b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4a51b-105">Ресурс **choiceColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца можно выбрать из списка вариантов.</span><span class="sxs-lookup"><span data-stu-id="4a51b-105">The **choiceColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values can be selected from a list of choices.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4a51b-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4a51b-106">JSON representation</span></span>

<span data-ttu-id="4a51b-107">Ниже показано представление ресурса **choiceColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4a51b-107">Here is a JSON representation of a **choiceColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.choiceColumn" } -->

```json
{
  "allowTextEntry": true,
  "choices": ["red", "blue", "green"],
  "displayAs": "checkBoxes | dropDownMenu | radioButtons"
}
```

## <a name="properties"></a><span data-ttu-id="4a51b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="4a51b-108">Properties</span></span>

| <span data-ttu-id="4a51b-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="4a51b-109">Property name</span></span>      | <span data-ttu-id="4a51b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="4a51b-110">Type</span></span>               | <span data-ttu-id="4a51b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4a51b-111">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="4a51b-112">**allowTextEntry**</span><span class="sxs-lookup"><span data-stu-id="4a51b-112">**allowTextEntry**</span></span> | <span data-ttu-id="4a51b-113">boolean</span><span class="sxs-lookup"><span data-stu-id="4a51b-113">boolean</span></span>            | <span data-ttu-id="4a51b-114">Если это свойство имеет значение true, то разрешено указывать значения, которых нет в списке заранее настроенных вариантов.</span><span class="sxs-lookup"><span data-stu-id="4a51b-114">If true, allows custom values that aren't in the configured choices.</span></span>
| <span data-ttu-id="4a51b-115">**choices**</span><span class="sxs-lookup"><span data-stu-id="4a51b-115">**choices**</span></span>        | <span data-ttu-id="4a51b-116">Коллекция (string)</span><span class="sxs-lookup"><span data-stu-id="4a51b-116">collection(string)</span></span> | <span data-ttu-id="4a51b-117">Список значений, доступных для данного столбца.</span><span class="sxs-lookup"><span data-stu-id="4a51b-117">The list of values available for this column.</span></span>
| <span data-ttu-id="4a51b-118">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="4a51b-118">**displayAs**</span></span>      | <span data-ttu-id="4a51b-119">string</span><span class="sxs-lookup"><span data-stu-id="4a51b-119">string</span></span>             | <span data-ttu-id="4a51b-120">Способ отображения вариантов в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="4a51b-120">How the choices are to be presented in the UX.</span></span> <span data-ttu-id="4a51b-121">Должно иметь один из типов `checkBoxes`, `dropDownMenu` или `radioButtons`.</span><span class="sxs-lookup"><span data-stu-id="4a51b-121">Must be one of `checkBoxes`, `dropDownMenu`, or `radioButtons`</span></span>


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
