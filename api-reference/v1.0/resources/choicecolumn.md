---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: choiceColumn
ms.openlocfilehash: c266550e8918603c3ee6104818c0aa721f1281d9
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="choicecolumn-resource-type"></a><span data-ttu-id="1a84e-102">Тип ресурса choiceColumn</span><span class="sxs-lookup"><span data-stu-id="1a84e-102">ChoiceColumn resource type</span></span>

<span data-ttu-id="1a84e-103">Ресурс **choiceColumn** в ресурсе [columnDefinition](columnDefinition.md) указывает, что значения столбца можно выбрать из списка вариантов.</span><span class="sxs-lookup"><span data-stu-id="1a84e-103">The **choiceColumn** on a [columnDefinition](columnDefinition.md) resource indicates that the column's values can be selected from a list of choices.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1a84e-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="1a84e-104">JSON representation</span></span>

<span data-ttu-id="1a84e-105">Ниже показано представление ресурса **choiceColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1a84e-105">Here is a JSON representation of a **drive** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.choiceColumn" } -->

```json
{
  "allowTextEntry": true,
  "choices": ["red", "blue", "green"],
  "displayAs": "checkBoxes | dropDownMenu | radioButtons"
}
```

## <a name="properties"></a><span data-ttu-id="1a84e-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="1a84e-106">Properties</span></span>

| <span data-ttu-id="1a84e-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="1a84e-107">Property name</span></span>      | <span data-ttu-id="1a84e-108">Тип</span><span class="sxs-lookup"><span data-stu-id="1a84e-108">Type</span></span>               | <span data-ttu-id="1a84e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1a84e-109">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="1a84e-110">**allowTextEntry**</span><span class="sxs-lookup"><span data-stu-id="1a84e-110">**allowTextEntry**</span></span> | <span data-ttu-id="1a84e-111">логический</span><span class="sxs-lookup"><span data-stu-id="1a84e-111">boolean</span></span>            | <span data-ttu-id="1a84e-112">Если это свойство имеет значение true, то разрешено указывать значения, которых нет в списке заранее настроенных вариантов.</span><span class="sxs-lookup"><span data-stu-id="1a84e-112">If true, allows custom values that aren't in the configured choices.</span></span>
| <span data-ttu-id="1a84e-113">**choices**</span><span class="sxs-lookup"><span data-stu-id="1a84e-113">**CHOICES**</span></span>        | <span data-ttu-id="1a84e-114">collection(string)</span><span class="sxs-lookup"><span data-stu-id="1a84e-114">Collection(String)</span></span> | <span data-ttu-id="1a84e-115">Список значений, доступных для данного столбца.</span><span class="sxs-lookup"><span data-stu-id="1a84e-115">The list of values available for this column.</span></span>
| <span data-ttu-id="1a84e-116">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="1a84e-116">**displayAs**</span></span>      | <span data-ttu-id="1a84e-117">строка</span><span class="sxs-lookup"><span data-stu-id="1a84e-117">string</span></span>             | <span data-ttu-id="1a84e-118">Способ отображения вариантов в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="1a84e-118">How the choices are to be presented in the UX.</span></span> <span data-ttu-id="1a84e-119">Должно иметь один из типов `checkBoxes`, `dropDownMenu` или `radioButtons`.</span><span class="sxs-lookup"><span data-stu-id="1a84e-119">Must be one of `checkBoxes`, `dropDownMenu`, or `radioButtons`</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ChoiceColumn"
} -->
