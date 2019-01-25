---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: choiceColumn
localization_priority: Normal
ms.openlocfilehash: b0efefbbd6a47a547bc724274fd9bc26b2628442
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510759"
---
# <a name="choicecolumn-resource-type"></a><span data-ttu-id="1e543-102">Тип ресурса choiceColumn</span><span class="sxs-lookup"><span data-stu-id="1e543-102">ChoiceColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e543-103">Ресурс **choiceColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца можно выбрать из списка вариантов.</span><span class="sxs-lookup"><span data-stu-id="1e543-103">The **choiceColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values can be selected from a list of choices.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1e543-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="1e543-104">JSON representation</span></span>

<span data-ttu-id="1e543-105">Ниже показано представление ресурса **choiceColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1e543-105">Here is a JSON representation of a **choiceColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.choiceColumn" } -->

```json
{
  "allowTextEntry": true,
  "choices": ["red", "blue", "green"],
  "displayAs": "checkBoxes | dropDownMenu | radioButtons"
}
```

## <a name="properties"></a><span data-ttu-id="1e543-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="1e543-106">Properties</span></span>

| <span data-ttu-id="1e543-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="1e543-107">Property name</span></span>      | <span data-ttu-id="1e543-108">Тип</span><span class="sxs-lookup"><span data-stu-id="1e543-108">Type</span></span>               | <span data-ttu-id="1e543-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1e543-109">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="1e543-110">**allowTextEntry**</span><span class="sxs-lookup"><span data-stu-id="1e543-110">**allowTextEntry**</span></span> | <span data-ttu-id="1e543-111">boolean</span><span class="sxs-lookup"><span data-stu-id="1e543-111">boolean</span></span>            | <span data-ttu-id="1e543-112">Если это свойство имеет значение true, то разрешено указывать значения, которых нет в списке заранее настроенных вариантов.</span><span class="sxs-lookup"><span data-stu-id="1e543-112">If true, allows custom values that aren't in the configured choices.</span></span>
| <span data-ttu-id="1e543-113">**choices**</span><span class="sxs-lookup"><span data-stu-id="1e543-113">**choices**</span></span>        | <span data-ttu-id="1e543-114">Коллекция (string)</span><span class="sxs-lookup"><span data-stu-id="1e543-114">collection(string)</span></span> | <span data-ttu-id="1e543-115">Список значений, доступных для данного столбца.</span><span class="sxs-lookup"><span data-stu-id="1e543-115">The list of values available for this column.</span></span>
| <span data-ttu-id="1e543-116">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="1e543-116">**displayAs**</span></span>      | <span data-ttu-id="1e543-117">string</span><span class="sxs-lookup"><span data-stu-id="1e543-117">string</span></span>             | <span data-ttu-id="1e543-118">Способ отображения вариантов в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="1e543-118">How the choices are to be presented in the UX.</span></span> <span data-ttu-id="1e543-119">Должно иметь один из типов `checkBoxes`, `dropDownMenu` или `radioButtons`.</span><span class="sxs-lookup"><span data-stu-id="1e543-119">Must be one of `checkBoxes`, `dropDownMenu`, or `radioButtons`</span></span>


<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ChoiceColumn",
  "suppressions": [
    "Error: /api-reference/beta/resources/choicecolumn.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
