---
title: Тип ресурса Усераттрибутевалуеситем
description: Используется для заполнения значений атрибута Flow Flow в пользовательском цикле, если выбрано несколько вариантов.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6fd0d582ef4dcdd83dba6947536c5acdbc14a8cb
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581419"
---
# <a name="userattributevaluesitem-resource-type"></a><span data-ttu-id="9e342-103">Тип ресурса Усераттрибутевалуеситем</span><span class="sxs-lookup"><span data-stu-id="9e342-103">userAttributeValuesItem resource type</span></span>

<span data-ttu-id="9e342-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e342-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9e342-105">Используется для заполнения значений атрибута Flow Flow в пользовательском цикле, если выбрано несколько вариантов.</span><span class="sxs-lookup"><span data-stu-id="9e342-105">Used to populate the values for a user flow attribute within a user flow when there are multiple selections to choose from.</span></span> <span data-ttu-id="9e342-106">Усераттрибутевалуеситем применяется к Усеринпуттипес `radioSingleSelect` , `dropdownSingleSelect` и `checkboxMultiSelect` для [идентитюсерфловаттрибутеассигнмент](..\resources\identityuserflowattributeassignment.md).</span><span class="sxs-lookup"><span data-stu-id="9e342-106">userAttributeValuesItem is applicable to the userInputTypes `radioSingleSelect`, `dropdownSingleSelect`, and `checkboxMultiSelect` for an [identityUserFlowAttributeAssignment](..\resources\identityuserflowattributeassignment.md).</span></span>

## <a name="properties"></a><span data-ttu-id="9e342-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="9e342-107">Properties</span></span>

|<span data-ttu-id="9e342-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="9e342-108">Property</span></span>|<span data-ttu-id="9e342-109">Тип</span><span class="sxs-lookup"><span data-stu-id="9e342-109">Type</span></span>|<span data-ttu-id="9e342-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9e342-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e342-111">isDefault</span><span class="sxs-lookup"><span data-stu-id="9e342-111">isDefault</span></span>|<span data-ttu-id="9e342-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e342-112">Boolean</span></span>|<span data-ttu-id="9e342-113">Используется, чтобы задать значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="9e342-113">Used to set the value as the default.</span></span>|
|<span data-ttu-id="9e342-114">name</span><span class="sxs-lookup"><span data-stu-id="9e342-114">name</span></span>|<span data-ttu-id="9e342-115">String</span><span class="sxs-lookup"><span data-stu-id="9e342-115">String</span></span>|<span data-ttu-id="9e342-116">Отображаемое имя свойства, отображаемого для конечного пользователя в пользовательском движении.</span><span class="sxs-lookup"><span data-stu-id="9e342-116">The display name of the property displayed to the end user in the user flow.</span></span>|
|<span data-ttu-id="9e342-117">value</span><span class="sxs-lookup"><span data-stu-id="9e342-117">value</span></span>|<span data-ttu-id="9e342-118">String</span><span class="sxs-lookup"><span data-stu-id="9e342-118">String</span></span>|<span data-ttu-id="9e342-119">Значение, заданное при выборе этого элемента.</span><span class="sxs-lookup"><span data-stu-id="9e342-119">The value that is set when this item is selected.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9e342-120">Связи</span><span class="sxs-lookup"><span data-stu-id="9e342-120">Relationships</span></span>

<span data-ttu-id="9e342-121">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9e342-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9e342-122">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="9e342-122">JSON representation</span></span>

<span data-ttu-id="9e342-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9e342-123">The following is a JSON representation of the resource.</span></span>
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
