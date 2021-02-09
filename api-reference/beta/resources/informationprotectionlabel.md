---
title: Тип ресурса informationProtectionLabel
description: Описание метки защиты информации, которая описывает, как правильно применить метку конфиденциальности к информации.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 694015f819d1c1afc9fe9feb23c67c92c05eed70
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153636"
---
# <a name="informationprotectionlabel-resource-type"></a><span data-ttu-id="66ee5-103">Тип ресурса informationProtectionLabel</span><span class="sxs-lookup"><span data-stu-id="66ee5-103">informationProtectionLabel resource type</span></span>

<span data-ttu-id="66ee5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66ee5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66ee5-105">Описание метки защиты информации, которая описывает, как правильно применить метку конфиденциальности к информации.</span><span class="sxs-lookup"><span data-stu-id="66ee5-105">Describes the information protection label that details how to properly apply a sensitivity label to information.</span></span> <span data-ttu-id="66ee5-106">Ресурс **informationProtectionLabel** описывает конфигурацию меток конфиденциальности, которые применяются к пользователю или арендатору.</span><span class="sxs-lookup"><span data-stu-id="66ee5-106">The **informationProtectionLabel** resource describes the configuration of sensitivity labels that apply to a user or tenant.</span></span>  

## <a name="methods"></a><span data-ttu-id="66ee5-107">Методы</span><span class="sxs-lookup"><span data-stu-id="66ee5-107">Methods</span></span>

| <span data-ttu-id="66ee5-108">Метод</span><span class="sxs-lookup"><span data-stu-id="66ee5-108">Method</span></span>                                                                                              | <span data-ttu-id="66ee5-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="66ee5-109">Return Type</span></span>                                                               | <span data-ttu-id="66ee5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="66ee5-110">Description</span></span>                                                                                                                                                            |
| :-------------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------ | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [<span data-ttu-id="66ee5-111">Список informationProtectionLabel</span><span class="sxs-lookup"><span data-stu-id="66ee5-111">List informationProtectionLabel</span></span>](../api/informationprotectionpolicy-list-labels.md)                | <span data-ttu-id="66ee5-112">[Коллекция informationProtectionLabel](informationprotectionlabel.md)</span><span class="sxs-lookup"><span data-stu-id="66ee5-112">[informationProtectionLabel](informationprotectionlabel.md) collection</span></span> | <span data-ttu-id="66ee5-113">Список всех настроенных меток защиты информации для пользователя или клиента.</span><span class="sxs-lookup"><span data-stu-id="66ee5-113">List all configured information protection labels for a user or tenant.</span></span>                                                                                                |
| [<span data-ttu-id="66ee5-114">Get informationProtectionLabel</span><span class="sxs-lookup"><span data-stu-id="66ee5-114">Get informationProtectionLabel</span></span>](../api/informationprotectionlabel-get.md)                          | [<span data-ttu-id="66ee5-115">informationProtectionLabel</span><span class="sxs-lookup"><span data-stu-id="66ee5-115">informationProtectionLabel</span></span>](informationprotectionlabel.md)               | <span data-ttu-id="66ee5-116">С учетом определенного ИД метки **вернете informationProtectionLabel.**</span><span class="sxs-lookup"><span data-stu-id="66ee5-116">Given a specific label ID, return the **informationProtectionLabel**.</span></span>                                                                                                  |
| [<span data-ttu-id="66ee5-117">evaluateapplication</span><span class="sxs-lookup"><span data-stu-id="66ee5-117">evaluateapplication</span></span>](../api/informationprotectionlabel-evaluateapplication.md)                     | <span data-ttu-id="66ee5-118">[Коллекция informationProtectionAction](informationprotectionaction.md)</span><span class="sxs-lookup"><span data-stu-id="66ee5-118">[informationProtectionAction](informationprotectionaction.md) collection</span></span>  | <span data-ttu-id="66ee5-119">Учитывая входные данные [contentInfo](contentinfo.md) и [labelingOptions,](labelingoptions.md)вычислите набор действий, необходимых для применения метки.</span><span class="sxs-lookup"><span data-stu-id="66ee5-119">Given an input of [contentInfo](contentinfo.md) and [labelingOptions](labelingoptions.md), compute the set of actions require to apply the label.</span></span>                      |
| [<span data-ttu-id="66ee5-120">evaluateClassificationResults</span><span class="sxs-lookup"><span data-stu-id="66ee5-120">evaluateClassificationResults</span></span>](../api/informationprotectionlabel-evaluateclassificationresults.md) | <span data-ttu-id="66ee5-121">[Коллекция informationProtectionAction](informationprotectionaction.md)</span><span class="sxs-lookup"><span data-stu-id="66ee5-121">[informationProtectionAction](informationprotectionaction.md) collection</span></span>  | <span data-ttu-id="66ee5-122">С учетом [входных данных contentInfo](contentinfo.md) и результатов классификации вычислить набор действий, необходимых для применения метки.</span><span class="sxs-lookup"><span data-stu-id="66ee5-122">Given an input of [contentInfo](contentinfo.md) and classification results, compute the set of actions require to apply the label.</span></span>                                  |
| [<span data-ttu-id="66ee5-123">evaluateRemoval</span><span class="sxs-lookup"><span data-stu-id="66ee5-123">evaluateRemoval</span></span>](../api/informationprotectionlabel-evaluateremoval.md)                             | <span data-ttu-id="66ee5-124">[Коллекция informationProtectionAction](informationprotectionaction.md)</span><span class="sxs-lookup"><span data-stu-id="66ee5-124">[informationProtectionAction](informationprotectionaction.md) collection</span></span>  | <span data-ttu-id="66ee5-125">Учитывая входные данные [contentInfo](contentinfo.md) и [downgradeJustification,](downgradejustification.md)вычислите действия, которые необходимо принять для удаления метки.</span><span class="sxs-lookup"><span data-stu-id="66ee5-125">Given an input of [contentInfo](contentinfo.md) and [downgradeJustification](downgradejustification.md), compute the actions that should be taken to remove the label.</span></span> |
| [<span data-ttu-id="66ee5-126">extractLabel</span><span class="sxs-lookup"><span data-stu-id="66ee5-126">extractLabel</span></span>](../api/informationprotectionlabel-extractlabel.md)                                   | [<span data-ttu-id="66ee5-127">informationProtectionContentLabel</span><span class="sxs-lookup"><span data-stu-id="66ee5-127">informationProtectionContentLabel</span></span>](informationprotectioncontentlabel.md) | <span data-ttu-id="66ee5-128">При вводе [contentInfo](contentinfo.md)возвращает сведения о [метке informationProtectionLabel,](informationprotectionlabel.md) которую представляют метаданные.</span><span class="sxs-lookup"><span data-stu-id="66ee5-128">Given an input of [contentInfo](contentinfo.md), return details on the [informationProtectionLabel](informationprotectionlabel.md) that the metadata represents.</span></span>       |

## <a name="properties"></a><span data-ttu-id="66ee5-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="66ee5-129">Properties</span></span>

| <span data-ttu-id="66ee5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="66ee5-130">Property</span></span>    | <span data-ttu-id="66ee5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="66ee5-131">Type</span></span>    | <span data-ttu-id="66ee5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="66ee5-132">Description</span></span>                                                                                     |
| :---------- | :------ | :---------------------------------------------------------------------------------------------- |
| <span data-ttu-id="66ee5-133">color</span><span class="sxs-lookup"><span data-stu-id="66ee5-133">color</span></span>       | <span data-ttu-id="66ee5-134">String</span><span class="sxs-lookup"><span data-stu-id="66ee5-134">String</span></span>  | <span data-ttu-id="66ee5-135">Цвет, который должен отображаться в пользовательском интерфейсе для метки, если он настроен.</span><span class="sxs-lookup"><span data-stu-id="66ee5-135">The color that the UI should display for the label, if configured.</span></span>                              |
| <span data-ttu-id="66ee5-136">description</span><span class="sxs-lookup"><span data-stu-id="66ee5-136">description</span></span> | <span data-ttu-id="66ee5-137">String</span><span class="sxs-lookup"><span data-stu-id="66ee5-137">String</span></span>  | <span data-ttu-id="66ee5-138">Описание метки, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="66ee5-138">The admin-defined description for the label.</span></span>                                                    |
| <span data-ttu-id="66ee5-139">id</span><span class="sxs-lookup"><span data-stu-id="66ee5-139">id</span></span>          | <span data-ttu-id="66ee5-140">String</span><span class="sxs-lookup"><span data-stu-id="66ee5-140">String</span></span>  | <span data-ttu-id="66ee5-141">Идентификатор метки — это глобальный уникальный идентификатор (GUID)</span><span class="sxs-lookup"><span data-stu-id="66ee5-141">The label ID is a globally unique identifier (GUID)</span></span>                                             |
| <span data-ttu-id="66ee5-142">isActive</span><span class="sxs-lookup"><span data-stu-id="66ee5-142">isActive</span></span>    | <span data-ttu-id="66ee5-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="66ee5-143">Boolean</span></span> | <span data-ttu-id="66ee5-144">Указывает, активна ли метка.</span><span class="sxs-lookup"><span data-stu-id="66ee5-144">Indicates whether the label is active or not.</span></span> <span data-ttu-id="66ee5-145">Активные метки должны быть скрыты или отключены в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="66ee5-145">Active labels should be hidden or disabled in UI.</span></span> |
| <span data-ttu-id="66ee5-146">name</span><span class="sxs-lookup"><span data-stu-id="66ee5-146">name</span></span>        | <span data-ttu-id="66ee5-147">String</span><span class="sxs-lookup"><span data-stu-id="66ee5-147">String</span></span>  | <span data-ttu-id="66ee5-148">Обычное имя метки.</span><span class="sxs-lookup"><span data-stu-id="66ee5-148">The plaintext name of the label.</span></span>                                                                |
| <span data-ttu-id="66ee5-149">sensitivity</span><span class="sxs-lookup"><span data-stu-id="66ee5-149">sensitivity</span></span> | <span data-ttu-id="66ee5-150">Int32</span><span class="sxs-lookup"><span data-stu-id="66ee5-150">Int32</span></span>   | <span data-ttu-id="66ee5-151">Значение конфиденциальности метки, где меньшее значение менее конфиденциально.</span><span class="sxs-lookup"><span data-stu-id="66ee5-151">The sensitivity value of the label, where lower is less sensitive.</span></span>                              |
| <span data-ttu-id="66ee5-152">tooltip</span><span class="sxs-lookup"><span data-stu-id="66ee5-152">tooltip</span></span>     | <span data-ttu-id="66ee5-153">String</span><span class="sxs-lookup"><span data-stu-id="66ee5-153">String</span></span>  | <span data-ttu-id="66ee5-154">The tooltip that should be displayed for the label in a UI.</span><span class="sxs-lookup"><span data-stu-id="66ee5-154">The tooltip that should be displayed for the label in a UI.</span></span>                                     |

## <a name="relationships"></a><span data-ttu-id="66ee5-155">Связи</span><span class="sxs-lookup"><span data-stu-id="66ee5-155">Relationships</span></span>

<span data-ttu-id="66ee5-156">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="66ee5-156">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="66ee5-157">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="66ee5-157">JSON representation</span></span>

<span data-ttu-id="66ee5-158">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="66ee5-158">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.informationProtectionLabel",
  "keyProperty": "id"
}-->

```json
{
  "color": "String",
  "description": "String",
  "id": "String (identifier)",
  "isActive": true,
  "name": "String",
  "sensitivity": 1024,
  "tooltip": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "informationProtectionLabel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


