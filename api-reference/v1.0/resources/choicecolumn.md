---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: choiceColumn
ms.openlocfilehash: 6841f453cdfd423ead3edeea5895242a28b998f3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025023"
---
# <a name="choicecolumn-resource-type"></a><span data-ttu-id="5d488-102">Тип ресурса choiceColumn</span><span class="sxs-lookup"><span data-stu-id="5d488-102">ChoiceColumn resource type</span></span>

<span data-ttu-id="5d488-103">Ресурс **choiceColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца можно выбрать из списка вариантов.</span><span class="sxs-lookup"><span data-stu-id="5d488-103">The **choiceColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values can be selected from a list of choices.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5d488-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="5d488-104">JSON representation</span></span>

<span data-ttu-id="5d488-105">Ниже показано представление ресурса **choiceColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5d488-105">Here is a JSON representation of a **choiceColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.choiceColumn" } -->

```json
{
  "allowTextEntry": true,
  "choices": ["red", "blue", "green"],
  "displayAs": "checkBoxes | dropDownMenu | radioButtons"
}
```

## <a name="properties"></a><span data-ttu-id="5d488-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="5d488-106">Properties</span></span>

| <span data-ttu-id="5d488-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="5d488-107">Property name</span></span>      | <span data-ttu-id="5d488-108">Тип</span><span class="sxs-lookup"><span data-stu-id="5d488-108">Type</span></span>               | <span data-ttu-id="5d488-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5d488-109">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="5d488-110">**allowTextEntry**</span><span class="sxs-lookup"><span data-stu-id="5d488-110">**allowTextEntry**</span></span> | <span data-ttu-id="5d488-111">boolean</span><span class="sxs-lookup"><span data-stu-id="5d488-111">boolean</span></span>            | <span data-ttu-id="5d488-112">Если это свойство имеет значение true, то разрешено указывать значения, которых нет в списке заранее настроенных вариантов.</span><span class="sxs-lookup"><span data-stu-id="5d488-112">If true, allows custom values that aren't in the configured choices.</span></span>
| <span data-ttu-id="5d488-113">**choices**</span><span class="sxs-lookup"><span data-stu-id="5d488-113">**choices**</span></span>        | <span data-ttu-id="5d488-114">Коллекция (string)</span><span class="sxs-lookup"><span data-stu-id="5d488-114">collection(string)</span></span> | <span data-ttu-id="5d488-115">Список значений, доступных для данного столбца.</span><span class="sxs-lookup"><span data-stu-id="5d488-115">The list of values available for this column.</span></span>
| <span data-ttu-id="5d488-116">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="5d488-116">**displayAs**</span></span>      | <span data-ttu-id="5d488-117">string</span><span class="sxs-lookup"><span data-stu-id="5d488-117">string</span></span>             | <span data-ttu-id="5d488-118">Способ отображения вариантов в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="5d488-118">How the choices are to be presented in the UX.</span></span> <span data-ttu-id="5d488-119">Должно иметь один из типов `checkBoxes`, `dropDownMenu` или `radioButtons`.</span><span class="sxs-lookup"><span data-stu-id="5d488-119">Must be one of `checkBoxes`, `dropDownMenu`, or `radioButtons`</span></span>


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
