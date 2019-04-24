---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: choiceColumn
localization_priority: Normal
ms.openlocfilehash: 1dddbd4cfa4f26ecc0fd79a430c9d7f725bebbf9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32584999"
---
# <a name="choicecolumn-resource-type"></a><span data-ttu-id="04618-102">Тип ресурса choiceColumn</span><span class="sxs-lookup"><span data-stu-id="04618-102">ChoiceColumn resource type</span></span>

<span data-ttu-id="04618-103">Ресурс **choiceColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца можно выбрать из списка вариантов.</span><span class="sxs-lookup"><span data-stu-id="04618-103">The **choiceColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values can be selected from a list of choices.</span></span>

## <a name="json-representation"></a><span data-ttu-id="04618-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="04618-104">JSON representation</span></span>

<span data-ttu-id="04618-105">Ниже показано представление ресурса **choiceColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="04618-105">Here is a JSON representation of a **choiceColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.choiceColumn" } -->

```json
{
  "allowTextEntry": true,
  "choices": ["red", "blue", "green"],
  "displayAs": "checkBoxes | dropDownMenu | radioButtons"
}
```

## <a name="properties"></a><span data-ttu-id="04618-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="04618-106">Properties</span></span>

| <span data-ttu-id="04618-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="04618-107">Property name</span></span>      | <span data-ttu-id="04618-108">Тип</span><span class="sxs-lookup"><span data-stu-id="04618-108">Type</span></span>               | <span data-ttu-id="04618-109">Описание</span><span class="sxs-lookup"><span data-stu-id="04618-109">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="04618-110">**allowTextEntry**</span><span class="sxs-lookup"><span data-stu-id="04618-110">**allowTextEntry**</span></span> | <span data-ttu-id="04618-111">boolean</span><span class="sxs-lookup"><span data-stu-id="04618-111">boolean</span></span>            | <span data-ttu-id="04618-112">Если это свойство имеет значение true, то разрешено указывать значения, которых нет в списке заранее настроенных вариантов.</span><span class="sxs-lookup"><span data-stu-id="04618-112">If true, allows custom values that aren't in the configured choices.</span></span>
| <span data-ttu-id="04618-113">**choices**</span><span class="sxs-lookup"><span data-stu-id="04618-113">**choices**</span></span>        | <span data-ttu-id="04618-114">Коллекция (string)</span><span class="sxs-lookup"><span data-stu-id="04618-114">collection(string)</span></span> | <span data-ttu-id="04618-115">Список значений, доступных для данного столбца.</span><span class="sxs-lookup"><span data-stu-id="04618-115">The list of values available for this column.</span></span>
| <span data-ttu-id="04618-116">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="04618-116">**displayAs**</span></span>      | <span data-ttu-id="04618-117">string</span><span class="sxs-lookup"><span data-stu-id="04618-117">string</span></span>             | <span data-ttu-id="04618-118">Способ отображения вариантов в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="04618-118">How the choices are to be presented in the UX.</span></span> <span data-ttu-id="04618-119">Должно иметь один из типов `checkBoxes`, `dropDownMenu` или `radioButtons`.</span><span class="sxs-lookup"><span data-stu-id="04618-119">Must be one of `checkBoxes`, `dropDownMenu`, or `radioButtons`</span></span>


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
