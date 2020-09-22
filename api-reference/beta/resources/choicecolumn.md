---
author: JeremyKelley
description: Ресурс choiceColumn в ресурсе columnDefinition указывает, что значения столбца можно выбрать из списка вариантов.
ms.date: 09/11/2017
title: choiceColumn
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: a5e6efa944756077eb29467be6e75013d4bf28aa
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021989"
---
# <a name="choicecolumn-resource-type"></a><span data-ttu-id="2d085-103">Тип ресурса choiceColumn</span><span class="sxs-lookup"><span data-stu-id="2d085-103">ChoiceColumn resource type</span></span>

<span data-ttu-id="2d085-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d085-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d085-105">Ресурс **choiceColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца можно выбрать из списка вариантов.</span><span class="sxs-lookup"><span data-stu-id="2d085-105">The **choiceColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values can be selected from a list of choices.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2d085-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="2d085-106">JSON representation</span></span>

<span data-ttu-id="2d085-107">Ниже показано представление ресурса **choiceColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2d085-107">Here is a JSON representation of a **choiceColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.choiceColumn" } -->

```json
{
  "allowTextEntry": true,
  "choices": ["red", "blue", "green"],
  "displayAs": "checkBoxes | dropDownMenu | radioButtons"
}
```

## <a name="properties"></a><span data-ttu-id="2d085-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="2d085-108">Properties</span></span>

| <span data-ttu-id="2d085-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="2d085-109">Property name</span></span>      | <span data-ttu-id="2d085-110">Тип</span><span class="sxs-lookup"><span data-stu-id="2d085-110">Type</span></span>               | <span data-ttu-id="2d085-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2d085-111">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="2d085-112">**allowTextEntry**</span><span class="sxs-lookup"><span data-stu-id="2d085-112">**allowTextEntry**</span></span> | <span data-ttu-id="2d085-113">boolean</span><span class="sxs-lookup"><span data-stu-id="2d085-113">boolean</span></span>            | <span data-ttu-id="2d085-114">Если это свойство имеет значение true, то разрешено указывать значения, которых нет в списке заранее настроенных вариантов.</span><span class="sxs-lookup"><span data-stu-id="2d085-114">If true, allows custom values that aren't in the configured choices.</span></span>
| <span data-ttu-id="2d085-115">**choices**</span><span class="sxs-lookup"><span data-stu-id="2d085-115">**choices**</span></span>        | <span data-ttu-id="2d085-116">Коллекция (string)</span><span class="sxs-lookup"><span data-stu-id="2d085-116">collection(string)</span></span> | <span data-ttu-id="2d085-117">Список значений, доступных для данного столбца.</span><span class="sxs-lookup"><span data-stu-id="2d085-117">The list of values available for this column.</span></span>
| <span data-ttu-id="2d085-118">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="2d085-118">**displayAs**</span></span>      | <span data-ttu-id="2d085-119">string</span><span class="sxs-lookup"><span data-stu-id="2d085-119">string</span></span>             | <span data-ttu-id="2d085-120">Способ отображения вариантов в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="2d085-120">How the choices are to be presented in the UX.</span></span> <span data-ttu-id="2d085-121">Должно иметь один из типов `checkBoxes`, `dropDownMenu` или `radioButtons`.</span><span class="sxs-lookup"><span data-stu-id="2d085-121">Must be one of `checkBoxes`, `dropDownMenu`, or `radioButtons`</span></span>


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


