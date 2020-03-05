---
author: JeremyKelley
description: Ресурс choiceColumn в ресурсе columnDefinition указывает, что значения столбца можно выбрать из списка вариантов.
ms.date: 09/11/2017
title: choiceColumn
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 8b9b6db64bb1215a4be3fde10bce1a40bb5ffce3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507686"
---
# <a name="choicecolumn-resource-type"></a><span data-ttu-id="aff3f-103">Тип ресурса choiceColumn</span><span class="sxs-lookup"><span data-stu-id="aff3f-103">ChoiceColumn resource type</span></span>

<span data-ttu-id="aff3f-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="aff3f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aff3f-105">Ресурс **choiceColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца можно выбрать из списка вариантов.</span><span class="sxs-lookup"><span data-stu-id="aff3f-105">The **choiceColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values can be selected from a list of choices.</span></span>

## <a name="json-representation"></a><span data-ttu-id="aff3f-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="aff3f-106">JSON representation</span></span>

<span data-ttu-id="aff3f-107">Ниже показано представление ресурса **choiceColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aff3f-107">Here is a JSON representation of a **choiceColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.choiceColumn" } -->

```json
{
  "allowTextEntry": true,
  "choices": ["red", "blue", "green"],
  "displayAs": "checkBoxes | dropDownMenu | radioButtons"
}
```

## <a name="properties"></a><span data-ttu-id="aff3f-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="aff3f-108">Properties</span></span>

| <span data-ttu-id="aff3f-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="aff3f-109">Property name</span></span>      | <span data-ttu-id="aff3f-110">Тип</span><span class="sxs-lookup"><span data-stu-id="aff3f-110">Type</span></span>               | <span data-ttu-id="aff3f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="aff3f-111">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="aff3f-112">**allowTextEntry**</span><span class="sxs-lookup"><span data-stu-id="aff3f-112">**allowTextEntry**</span></span> | <span data-ttu-id="aff3f-113">boolean</span><span class="sxs-lookup"><span data-stu-id="aff3f-113">boolean</span></span>            | <span data-ttu-id="aff3f-114">Если это свойство имеет значение true, то разрешено указывать значения, которых нет в списке заранее настроенных вариантов.</span><span class="sxs-lookup"><span data-stu-id="aff3f-114">If true, allows custom values that aren't in the configured choices.</span></span>
| <span data-ttu-id="aff3f-115">**choices**</span><span class="sxs-lookup"><span data-stu-id="aff3f-115">**choices**</span></span>        | <span data-ttu-id="aff3f-116">Коллекция (string)</span><span class="sxs-lookup"><span data-stu-id="aff3f-116">collection(string)</span></span> | <span data-ttu-id="aff3f-117">Список значений, доступных для данного столбца.</span><span class="sxs-lookup"><span data-stu-id="aff3f-117">The list of values available for this column.</span></span>
| <span data-ttu-id="aff3f-118">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="aff3f-118">**displayAs**</span></span>      | <span data-ttu-id="aff3f-119">string</span><span class="sxs-lookup"><span data-stu-id="aff3f-119">string</span></span>             | <span data-ttu-id="aff3f-120">Способ отображения вариантов в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="aff3f-120">How the choices are to be presented in the UX.</span></span> <span data-ttu-id="aff3f-121">Должно иметь один из типов `checkBoxes`, `dropDownMenu` или `radioButtons`.</span><span class="sxs-lookup"><span data-stu-id="aff3f-121">Must be one of `checkBoxes`, `dropDownMenu`, or `radioButtons`</span></span>


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
