---
title: тип ресурса userAttributeValuesItem
description: Представляет значения атрибута потока пользователей в потоке пользователей.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 367f5d835f3790c589a8d7d28b7994484fd9613c
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882450"
---
# <a name="userattributevaluesitem-resource-type"></a><span data-ttu-id="2f2f6-103">тип ресурса userAttributeValuesItem</span><span class="sxs-lookup"><span data-stu-id="2f2f6-103">userAttributeValuesItem resource type</span></span>

<span data-ttu-id="2f2f6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f2f6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2f2f6-105">Представляет значения атрибута потока пользователей в потоке пользователей, если необходимо выбрать несколько выборов.</span><span class="sxs-lookup"><span data-stu-id="2f2f6-105">Represents user flow attribute values within a user flow when there are multiple selections to choose from.</span></span>  <span data-ttu-id="2f2f6-106">UserAttributeValuesItem применим к userInputTypes , и для `radioSingleSelect` `dropdownSingleSelect` `checkboxMultiSelect` [identityUserFlowAttributeAssignment](..\resources\identityuserflowattributeassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2f2f6-106">The userAttributeValuesItem is applicable to the userInputTypes of `radioSingleSelect`, `dropdownSingleSelect`, and `checkboxMultiSelect` for an [identityUserFlowAttributeAssignment](..\resources\identityuserflowattributeassignment.md).</span></span>

## <a name="properties"></a><span data-ttu-id="2f2f6-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2f2f6-107">Properties</span></span>

|<span data-ttu-id="2f2f6-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="2f2f6-108">Property</span></span>|<span data-ttu-id="2f2f6-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2f2f6-109">Type</span></span>|<span data-ttu-id="2f2f6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2f2f6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f2f6-111">isDefault</span><span class="sxs-lookup"><span data-stu-id="2f2f6-111">isDefault</span></span>|<span data-ttu-id="2f2f6-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f2f6-112">Boolean</span></span>|<span data-ttu-id="2f2f6-113">Определяет, установлено ли значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="2f2f6-113">Determines whether the value is set as the default.</span></span>|
|<span data-ttu-id="2f2f6-114">name</span><span class="sxs-lookup"><span data-stu-id="2f2f6-114">name</span></span>|<span data-ttu-id="2f2f6-115">String</span><span class="sxs-lookup"><span data-stu-id="2f2f6-115">String</span></span>|<span data-ttu-id="2f2f6-116">Отображает имя свойства, отображаемого пользователю в потоке пользователей.</span><span class="sxs-lookup"><span data-stu-id="2f2f6-116">The display name of the property displayed to the user in the user flow.</span></span>|
|<span data-ttu-id="2f2f6-117">value</span><span class="sxs-lookup"><span data-stu-id="2f2f6-117">value</span></span>|<span data-ttu-id="2f2f6-118">String</span><span class="sxs-lookup"><span data-stu-id="2f2f6-118">String</span></span>|<span data-ttu-id="2f2f6-119">Значение, заданной при выборе этого элемента.</span><span class="sxs-lookup"><span data-stu-id="2f2f6-119">The value that is set when this item is selected.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2f2f6-120">Связи</span><span class="sxs-lookup"><span data-stu-id="2f2f6-120">Relationships</span></span>

<span data-ttu-id="2f2f6-121">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="2f2f6-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2f2f6-122">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="2f2f6-122">JSON representation</span></span>

<span data-ttu-id="2f2f6-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2f2f6-123">The following is a JSON representation of the resource.</span></span>
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
