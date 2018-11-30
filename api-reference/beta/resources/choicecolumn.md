---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: choiceColumn
ms.openlocfilehash: 659ece2eab255fe7b55a258b0980eda4e7bde5b2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074826"
---
# <a name="choicecolumn-resource-type"></a><span data-ttu-id="e5000-102">Тип ресурса choiceColumn</span><span class="sxs-lookup"><span data-stu-id="e5000-102">ChoiceColumn resource type</span></span>

> <span data-ttu-id="e5000-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e5000-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e5000-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5000-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e5000-105">Ресурс **choiceColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца можно выбрать из списка вариантов.</span><span class="sxs-lookup"><span data-stu-id="e5000-105">The **choiceColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values can be selected from a list of choices.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e5000-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e5000-106">JSON representation</span></span>

<span data-ttu-id="e5000-107">Ниже показано представление ресурса **choiceColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e5000-107">Here is a JSON representation of a **choiceColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.choiceColumn" } -->

```json
{
  "allowTextEntry": true,
  "choices": ["red", "blue", "green"],
  "displayAs": "checkBoxes | dropDownMenu | radioButtons"
}
```

## <a name="properties"></a><span data-ttu-id="e5000-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e5000-108">Properties</span></span>

| <span data-ttu-id="e5000-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="e5000-109">Property name</span></span>      | <span data-ttu-id="e5000-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e5000-110">Type</span></span>               | <span data-ttu-id="e5000-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e5000-111">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="e5000-112">**allowTextEntry**</span><span class="sxs-lookup"><span data-stu-id="e5000-112">**allowTextEntry**</span></span> | <span data-ttu-id="e5000-113">логический</span><span class="sxs-lookup"><span data-stu-id="e5000-113">boolean</span></span>            | <span data-ttu-id="e5000-114">Если это свойство имеет значение true, то разрешено указывать значения, которых нет в списке заранее настроенных вариантов.</span><span class="sxs-lookup"><span data-stu-id="e5000-114">If true, allows custom values that aren't in the configured choices.</span></span>
| <span data-ttu-id="e5000-115">**choices**</span><span class="sxs-lookup"><span data-stu-id="e5000-115">**choices**</span></span>        | <span data-ttu-id="e5000-116">Коллекция (string)</span><span class="sxs-lookup"><span data-stu-id="e5000-116">collection(string)</span></span> | <span data-ttu-id="e5000-117">Список значений, доступных для данного столбца.</span><span class="sxs-lookup"><span data-stu-id="e5000-117">The list of values available for this column.</span></span>
| <span data-ttu-id="e5000-118">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="e5000-118">**displayAs**</span></span>      | <span data-ttu-id="e5000-119">строка</span><span class="sxs-lookup"><span data-stu-id="e5000-119">string</span></span>             | <span data-ttu-id="e5000-120">Способ отображения вариантов в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="e5000-120">How the choices are to be presented in the UX.</span></span> <span data-ttu-id="e5000-121">Должно иметь один из типов `checkBoxes`, `dropDownMenu` или `radioButtons`.</span><span class="sxs-lookup"><span data-stu-id="e5000-121">Must be one of `checkBoxes`, `dropDownMenu`, or `radioButtons`</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ChoiceColumn"
} -->
