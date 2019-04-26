---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: choiceColumn
localization_priority: Normal
ms.openlocfilehash: d6c0db61fe3d919f780e14a950183619bb027801
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341480"
---
# <a name="choicecolumn-resource-type"></a><span data-ttu-id="26985-102">Тип ресурса choiceColumn</span><span class="sxs-lookup"><span data-stu-id="26985-102">ChoiceColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26985-103">Ресурс **choiceColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца можно выбрать из списка вариантов.</span><span class="sxs-lookup"><span data-stu-id="26985-103">The **choiceColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values can be selected from a list of choices.</span></span>

## <a name="json-representation"></a><span data-ttu-id="26985-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="26985-104">JSON representation</span></span>

<span data-ttu-id="26985-105">Ниже показано представление ресурса **choiceColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="26985-105">Here is a JSON representation of a **choiceColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.choiceColumn" } -->

```json
{
  "allowTextEntry": true,
  "choices": ["red", "blue", "green"],
  "displayAs": "checkBoxes | dropDownMenu | radioButtons"
}
```

## <a name="properties"></a><span data-ttu-id="26985-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="26985-106">Properties</span></span>

| <span data-ttu-id="26985-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="26985-107">Property name</span></span>      | <span data-ttu-id="26985-108">Тип</span><span class="sxs-lookup"><span data-stu-id="26985-108">Type</span></span>               | <span data-ttu-id="26985-109">Описание</span><span class="sxs-lookup"><span data-stu-id="26985-109">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="26985-110">**allowTextEntry**</span><span class="sxs-lookup"><span data-stu-id="26985-110">**allowTextEntry**</span></span> | <span data-ttu-id="26985-111">boolean</span><span class="sxs-lookup"><span data-stu-id="26985-111">boolean</span></span>            | <span data-ttu-id="26985-112">Если это свойство имеет значение true, то разрешено указывать значения, которых нет в списке заранее настроенных вариантов.</span><span class="sxs-lookup"><span data-stu-id="26985-112">If true, allows custom values that aren't in the configured choices.</span></span>
| <span data-ttu-id="26985-113">**choices**</span><span class="sxs-lookup"><span data-stu-id="26985-113">**choices**</span></span>        | <span data-ttu-id="26985-114">Коллекция (string)</span><span class="sxs-lookup"><span data-stu-id="26985-114">collection(string)</span></span> | <span data-ttu-id="26985-115">Список значений, доступных для данного столбца.</span><span class="sxs-lookup"><span data-stu-id="26985-115">The list of values available for this column.</span></span>
| <span data-ttu-id="26985-116">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="26985-116">**displayAs**</span></span>      | <span data-ttu-id="26985-117">string</span><span class="sxs-lookup"><span data-stu-id="26985-117">string</span></span>             | <span data-ttu-id="26985-118">Способ отображения вариантов в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="26985-118">How the choices are to be presented in the UX.</span></span> <span data-ttu-id="26985-119">Должно иметь один из типов `checkBoxes`, `dropDownMenu` или `radioButtons`.</span><span class="sxs-lookup"><span data-stu-id="26985-119">Must be one of `checkBoxes`, `dropDownMenu`, or `radioButtons`</span></span>


<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ChoiceColumn",
  "suppressions": []
}
-->
