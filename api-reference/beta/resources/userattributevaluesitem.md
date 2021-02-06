---
title: Тип ресурса userAttributeValuesItem
description: Используется для заполнения значений атрибута пользовательского потока в пользовательском потоке при выборе нескольких вариантов.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 64b2416cd6fd0e8c92d9a00ff2d599226e3cd02c
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133023"
---
# <a name="userattributevaluesitem-resource-type"></a><span data-ttu-id="aa4c2-103">Тип ресурса userAttributeValuesItem</span><span class="sxs-lookup"><span data-stu-id="aa4c2-103">userAttributeValuesItem resource type</span></span>

<span data-ttu-id="aa4c2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa4c2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="aa4c2-105">Используется для заполнения значений атрибута пользовательского потока в пользовательском потоке при выборе нескольких вариантов.</span><span class="sxs-lookup"><span data-stu-id="aa4c2-105">Used to populate the values for a user flow attribute within a user flow when there are multiple selections to choose from.</span></span> <span data-ttu-id="aa4c2-106">userAttributeValuesItem применимо к userInputTypes , и `radioSingleSelect` `dropdownSingleSelect` для `checkboxMultiSelect` [identityUserFlowAttributeAssignment](..\resources\identityuserflowattributeassignment.md).</span><span class="sxs-lookup"><span data-stu-id="aa4c2-106">userAttributeValuesItem is applicable to the userInputTypes `radioSingleSelect`, `dropdownSingleSelect`, and `checkboxMultiSelect` for an [identityUserFlowAttributeAssignment](..\resources\identityuserflowattributeassignment.md).</span></span>

## <a name="properties"></a><span data-ttu-id="aa4c2-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="aa4c2-107">Properties</span></span>

|<span data-ttu-id="aa4c2-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="aa4c2-108">Property</span></span>|<span data-ttu-id="aa4c2-109">Тип</span><span class="sxs-lookup"><span data-stu-id="aa4c2-109">Type</span></span>|<span data-ttu-id="aa4c2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="aa4c2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa4c2-111">isDefault</span><span class="sxs-lookup"><span data-stu-id="aa4c2-111">isDefault</span></span>|<span data-ttu-id="aa4c2-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="aa4c2-112">Boolean</span></span>|<span data-ttu-id="aa4c2-113">Используется для настройки значения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="aa4c2-113">Used to set the value as the default.</span></span>|
|<span data-ttu-id="aa4c2-114">name</span><span class="sxs-lookup"><span data-stu-id="aa4c2-114">name</span></span>|<span data-ttu-id="aa4c2-115">String</span><span class="sxs-lookup"><span data-stu-id="aa4c2-115">String</span></span>|<span data-ttu-id="aa4c2-116">Отображаемого имени свойства, отображаемого для конечного пользователя в пользовательском потоке.</span><span class="sxs-lookup"><span data-stu-id="aa4c2-116">The display name of the property displayed to the end user in the user flow.</span></span>|
|<span data-ttu-id="aa4c2-117">value</span><span class="sxs-lookup"><span data-stu-id="aa4c2-117">value</span></span>|<span data-ttu-id="aa4c2-118">String</span><span class="sxs-lookup"><span data-stu-id="aa4c2-118">String</span></span>|<span data-ttu-id="aa4c2-119">Значение, заданной при выборе этого элемента.</span><span class="sxs-lookup"><span data-stu-id="aa4c2-119">The value that is set when this item is selected.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aa4c2-120">Связи</span><span class="sxs-lookup"><span data-stu-id="aa4c2-120">Relationships</span></span>

<span data-ttu-id="aa4c2-121">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="aa4c2-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="aa4c2-122">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="aa4c2-122">JSON representation</span></span>

<span data-ttu-id="aa4c2-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aa4c2-123">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userAttributeValuesItem"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.userAttributeValuesItem",
  "name": "String",
  "value": "String",
  "isDefault": "Boolean"
}
```
