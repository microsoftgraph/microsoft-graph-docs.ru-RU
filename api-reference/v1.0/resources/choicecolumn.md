---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: choiceColumn
ms.openlocfilehash: 9feb49fc9c581a4518f63a0367087d54de32cff4
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2018
ms.locfileid: "23264072"
---
# <a name="choicecolumn-resource-type"></a><span data-ttu-id="3ea27-102">Тип ресурса choiceColumn</span><span class="sxs-lookup"><span data-stu-id="3ea27-102">ChoiceColumn resource type</span></span>

<span data-ttu-id="3ea27-103">Ресурс **choiceColumn** в ресурсе [columnDefinition](columnDefinition.md) указывает, что значения столбца можно выбрать из списка вариантов.</span><span class="sxs-lookup"><span data-stu-id="3ea27-103">The **choiceColumn** on a [columnDefinition](columnDefinition.md) resource indicates that the column's values can be selected from a list of choices.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3ea27-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="3ea27-104">JSON representation</span></span>

<span data-ttu-id="3ea27-105">Ниже показано представление ресурса **choiceColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3ea27-105">Here is a JSON representation of a **choiceColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.choiceColumn" } -->

```json
{
  "allowTextEntry": true,
  "choices": ["red", "blue", "green"],
  "displayAs": "checkBoxes | dropDownMenu | radioButtons"
}
```

## <a name="properties"></a><span data-ttu-id="3ea27-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="3ea27-106">Properties</span></span>

| <span data-ttu-id="3ea27-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="3ea27-107">Property name</span></span>      | <span data-ttu-id="3ea27-108">Тип</span><span class="sxs-lookup"><span data-stu-id="3ea27-108">Type</span></span>               | <span data-ttu-id="3ea27-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3ea27-109">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="3ea27-110">**allowTextEntry**</span><span class="sxs-lookup"><span data-stu-id="3ea27-110">**allowTextEntry**</span></span> | <span data-ttu-id="3ea27-111">логический</span><span class="sxs-lookup"><span data-stu-id="3ea27-111">boolean</span></span>            | <span data-ttu-id="3ea27-112">Если это свойство имеет значение true, то разрешено указывать значения, которых нет в списке заранее настроенных вариантов.</span><span class="sxs-lookup"><span data-stu-id="3ea27-112">If true, allows custom values that aren't in the configured choices.</span></span>
| <span data-ttu-id="3ea27-113">**choices**</span><span class="sxs-lookup"><span data-stu-id="3ea27-113">**choices**</span></span>        | <span data-ttu-id="3ea27-114">Коллекция (string)</span><span class="sxs-lookup"><span data-stu-id="3ea27-114">collection(string)</span></span> | <span data-ttu-id="3ea27-115">Список значений, доступных для данного столбца.</span><span class="sxs-lookup"><span data-stu-id="3ea27-115">The list of values available for this column.</span></span>
| <span data-ttu-id="3ea27-116">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="3ea27-116">**displayAs**</span></span>      | <span data-ttu-id="3ea27-117">строка</span><span class="sxs-lookup"><span data-stu-id="3ea27-117">string</span></span>             | <span data-ttu-id="3ea27-118">Способ отображения вариантов в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="3ea27-118">How the choices are to be presented in the UX.</span></span> <span data-ttu-id="3ea27-119">Должно иметь один из типов `checkBoxes`, `dropDownMenu` или `radioButtons`.</span><span class="sxs-lookup"><span data-stu-id="3ea27-119">Must be one of `checkBoxes`, `dropDownMenu`, or `radioButtons`</span></span>


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
