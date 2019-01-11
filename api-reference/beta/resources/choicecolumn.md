---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: choiceColumn
localization_priority: Normal
ms.openlocfilehash: 2e0798f558ace72f59a6acccc0cc8ce3eb6e2291
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842548"
---
# <a name="choicecolumn-resource-type"></a><span data-ttu-id="579d7-102">Тип ресурса choiceColumn</span><span class="sxs-lookup"><span data-stu-id="579d7-102">ChoiceColumn resource type</span></span>

> <span data-ttu-id="579d7-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="579d7-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="579d7-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="579d7-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="579d7-105">Ресурс **choiceColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца можно выбрать из списка вариантов.</span><span class="sxs-lookup"><span data-stu-id="579d7-105">The **choiceColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values can be selected from a list of choices.</span></span>

## <a name="json-representation"></a><span data-ttu-id="579d7-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="579d7-106">JSON representation</span></span>

<span data-ttu-id="579d7-107">Ниже показано представление ресурса **choiceColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="579d7-107">Here is a JSON representation of a **choiceColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.choiceColumn" } -->

```json
{
  "allowTextEntry": true,
  "choices": ["red", "blue", "green"],
  "displayAs": "checkBoxes | dropDownMenu | radioButtons"
}
```

## <a name="properties"></a><span data-ttu-id="579d7-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="579d7-108">Properties</span></span>

| <span data-ttu-id="579d7-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="579d7-109">Property name</span></span>      | <span data-ttu-id="579d7-110">Тип</span><span class="sxs-lookup"><span data-stu-id="579d7-110">Type</span></span>               | <span data-ttu-id="579d7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="579d7-111">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="579d7-112">**allowTextEntry**</span><span class="sxs-lookup"><span data-stu-id="579d7-112">**allowTextEntry**</span></span> | <span data-ttu-id="579d7-113">логический</span><span class="sxs-lookup"><span data-stu-id="579d7-113">boolean</span></span>            | <span data-ttu-id="579d7-114">Если это свойство имеет значение true, то разрешено указывать значения, которых нет в списке заранее настроенных вариантов.</span><span class="sxs-lookup"><span data-stu-id="579d7-114">If true, allows custom values that aren't in the configured choices.</span></span>
| <span data-ttu-id="579d7-115">**choices**</span><span class="sxs-lookup"><span data-stu-id="579d7-115">**choices**</span></span>        | <span data-ttu-id="579d7-116">Коллекция (string)</span><span class="sxs-lookup"><span data-stu-id="579d7-116">collection(string)</span></span> | <span data-ttu-id="579d7-117">Список значений, доступных для данного столбца.</span><span class="sxs-lookup"><span data-stu-id="579d7-117">The list of values available for this column.</span></span>
| <span data-ttu-id="579d7-118">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="579d7-118">**displayAs**</span></span>      | <span data-ttu-id="579d7-119">строка</span><span class="sxs-lookup"><span data-stu-id="579d7-119">string</span></span>             | <span data-ttu-id="579d7-120">Способ отображения вариантов в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="579d7-120">How the choices are to be presented in the UX.</span></span> <span data-ttu-id="579d7-121">Должно иметь один из типов `checkBoxes`, `dropDownMenu` или `radioButtons`.</span><span class="sxs-lookup"><span data-stu-id="579d7-121">Must be one of `checkBoxes`, `dropDownMenu`, or `radioButtons`</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ChoiceColumn"
} -->
