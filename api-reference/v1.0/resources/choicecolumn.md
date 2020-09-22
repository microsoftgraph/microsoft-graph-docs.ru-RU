---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: choiceColumn
localization_priority: Normal
description: Ресурс choiceColumn в ресурсе columnDefinition указывает, что значения столбца можно выбрать из списка вариантов.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 298eab65c77df57c6ec70715239dcc7f4e13d316
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48059161"
---
# <a name="choicecolumn-resource-type"></a><span data-ttu-id="54389-103">Тип ресурса choiceColumn</span><span class="sxs-lookup"><span data-stu-id="54389-103">ChoiceColumn resource type</span></span>

<span data-ttu-id="54389-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54389-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="54389-105">Ресурс **choiceColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца можно выбрать из списка вариантов.</span><span class="sxs-lookup"><span data-stu-id="54389-105">The **choiceColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values can be selected from a list of choices.</span></span>

## <a name="json-representation"></a><span data-ttu-id="54389-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="54389-106">JSON representation</span></span>

<span data-ttu-id="54389-107">Ниже показано представление ресурса **choiceColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="54389-107">Here is a JSON representation of a **choiceColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.choiceColumn" } -->

```json
{
  "allowTextEntry": true,
  "choices": ["red", "blue", "green"],
  "displayAs": "checkBoxes | dropDownMenu | radioButtons"
}
```

## <a name="properties"></a><span data-ttu-id="54389-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="54389-108">Properties</span></span>

| <span data-ttu-id="54389-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="54389-109">Property name</span></span>      | <span data-ttu-id="54389-110">Тип</span><span class="sxs-lookup"><span data-stu-id="54389-110">Type</span></span>               | <span data-ttu-id="54389-111">Описание</span><span class="sxs-lookup"><span data-stu-id="54389-111">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="54389-112">**allowTextEntry**</span><span class="sxs-lookup"><span data-stu-id="54389-112">**allowTextEntry**</span></span> | <span data-ttu-id="54389-113">boolean</span><span class="sxs-lookup"><span data-stu-id="54389-113">boolean</span></span>            | <span data-ttu-id="54389-114">Если это свойство имеет значение true, то разрешено указывать значения, которых нет в списке заранее настроенных вариантов.</span><span class="sxs-lookup"><span data-stu-id="54389-114">If true, allows custom values that aren't in the configured choices.</span></span>
| <span data-ttu-id="54389-115">**choices**</span><span class="sxs-lookup"><span data-stu-id="54389-115">**choices**</span></span>        | <span data-ttu-id="54389-116">Коллекция (string)</span><span class="sxs-lookup"><span data-stu-id="54389-116">collection(string)</span></span> | <span data-ttu-id="54389-117">Список значений, доступных для данного столбца.</span><span class="sxs-lookup"><span data-stu-id="54389-117">The list of values available for this column.</span></span>
| <span data-ttu-id="54389-118">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="54389-118">**displayAs**</span></span>      | <span data-ttu-id="54389-119">string</span><span class="sxs-lookup"><span data-stu-id="54389-119">string</span></span>             | <span data-ttu-id="54389-120">Способ отображения вариантов в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="54389-120">How the choices are to be presented in the UX.</span></span> <span data-ttu-id="54389-121">Должно иметь один из типов `checkBoxes`, `dropDownMenu` или `radioButtons`.</span><span class="sxs-lookup"><span data-stu-id="54389-121">Must be one of `checkBoxes`, `dropDownMenu`, or `radioButtons`</span></span>


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

