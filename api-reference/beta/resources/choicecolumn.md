---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: ChoiceColumn
localization_priority: Normal
ms.openlocfilehash: 21405fe3aa28e0eef1233cd6f27e63568fb4b00e
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482219"
---
# <a name="choicecolumn-resource-type"></a><span data-ttu-id="dfd65-102">Тип ресурса choiceColumn</span><span class="sxs-lookup"><span data-stu-id="dfd65-102">ChoiceColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dfd65-103">Ресурс **choiceColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца можно выбрать из списка вариантов.</span><span class="sxs-lookup"><span data-stu-id="dfd65-103">The **choiceColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values can be selected from a list of choices.</span></span>

## <a name="json-representation"></a><span data-ttu-id="dfd65-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="dfd65-104">JSON representation</span></span>

<span data-ttu-id="dfd65-105">Ниже показано представление ресурса **choiceColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dfd65-105">Here is a JSON representation of a **choiceColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.choiceColumn" } -->

```json
{
  "allowTextEntry": true,
  "choices": ["red", "blue", "green"],
  "displayAs": "checkBoxes | dropDownMenu | radioButtons"
}
```

## <a name="properties"></a><span data-ttu-id="dfd65-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="dfd65-106">Properties</span></span>

| <span data-ttu-id="dfd65-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="dfd65-107">Property name</span></span>      | <span data-ttu-id="dfd65-108">Тип</span><span class="sxs-lookup"><span data-stu-id="dfd65-108">Type</span></span>               | <span data-ttu-id="dfd65-109">Описание</span><span class="sxs-lookup"><span data-stu-id="dfd65-109">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="dfd65-110">**allowTextEntry**</span><span class="sxs-lookup"><span data-stu-id="dfd65-110">**allowTextEntry**</span></span> | <span data-ttu-id="dfd65-111">boolean</span><span class="sxs-lookup"><span data-stu-id="dfd65-111">boolean</span></span>            | <span data-ttu-id="dfd65-112">Если это свойство имеет значение true, то разрешено указывать значения, которых нет в списке заранее настроенных вариантов.</span><span class="sxs-lookup"><span data-stu-id="dfd65-112">If true, allows custom values that aren't in the configured choices.</span></span>
| <span data-ttu-id="dfd65-113">**choices**</span><span class="sxs-lookup"><span data-stu-id="dfd65-113">**choices**</span></span>        | <span data-ttu-id="dfd65-114">Коллекция (string)</span><span class="sxs-lookup"><span data-stu-id="dfd65-114">collection(string)</span></span> | <span data-ttu-id="dfd65-115">Список значений, доступных для данного столбца.</span><span class="sxs-lookup"><span data-stu-id="dfd65-115">The list of values available for this column.</span></span>
| <span data-ttu-id="dfd65-116">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="dfd65-116">**displayAs**</span></span>      | <span data-ttu-id="dfd65-117">string</span><span class="sxs-lookup"><span data-stu-id="dfd65-117">string</span></span>             | <span data-ttu-id="dfd65-118">Способ отображения вариантов в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="dfd65-118">How the choices are to be presented in the UX.</span></span> <span data-ttu-id="dfd65-119">Должно иметь один из типов `checkBoxes`, `dropDownMenu` или `radioButtons`.</span><span class="sxs-lookup"><span data-stu-id="dfd65-119">Must be one of `checkBoxes`, `dropDownMenu`, or `radioButtons`</span></span>


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
