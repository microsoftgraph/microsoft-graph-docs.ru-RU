---
title: тип ресурса informationProtectionLabel
description: Описывает метку защиты информации, которая описывает, как правильно применять метку конфиденциальности к сведениям.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: ee8865b4fa898a91ca79cfba29c928ed00e21ae2
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579671"
---
# <a name="informationprotectionlabel-resource-type"></a><span data-ttu-id="8a6d3-103">тип ресурса informationProtectionLabel</span><span class="sxs-lookup"><span data-stu-id="8a6d3-103">informationProtectionLabel resource type</span></span>

<span data-ttu-id="8a6d3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a6d3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a6d3-105">Описывает метку защиты информации, которая описывает, как правильно применять метку конфиденциальности к сведениям.</span><span class="sxs-lookup"><span data-stu-id="8a6d3-105">Describes the information protection label that details how to properly apply a sensitivity label to information.</span></span> <span data-ttu-id="8a6d3-106">Ресурс **informationProtectionLabel** описывает конфигурацию меток конфиденциальности, которые применяются к пользователю или клиенту.</span><span class="sxs-lookup"><span data-stu-id="8a6d3-106">The **informationProtectionLabel** resource describes the configuration of sensitivity labels that apply to a user or tenant.</span></span>  

## <a name="methods"></a><span data-ttu-id="8a6d3-107">Методы</span><span class="sxs-lookup"><span data-stu-id="8a6d3-107">Methods</span></span>

| <span data-ttu-id="8a6d3-108">Метод</span><span class="sxs-lookup"><span data-stu-id="8a6d3-108">Method</span></span>                                                                                              | <span data-ttu-id="8a6d3-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8a6d3-109">Return Type</span></span>                                                               | <span data-ttu-id="8a6d3-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8a6d3-110">Description</span></span>                                                                                                                                                            |
| :-------------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------ | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [<span data-ttu-id="8a6d3-111">List informationProtectionLabel</span><span class="sxs-lookup"><span data-stu-id="8a6d3-111">List informationProtectionLabel</span></span>](../api/informationprotectionpolicy-list-labels.md)                | <span data-ttu-id="8a6d3-112">[коллекция informationProtectionLabel](informationprotectionlabel.md)</span><span class="sxs-lookup"><span data-stu-id="8a6d3-112">[informationProtectionLabel](informationprotectionlabel.md) collection</span></span> | <span data-ttu-id="8a6d3-113">Список всех настроенных меток защиты информации для пользователя или клиента.</span><span class="sxs-lookup"><span data-stu-id="8a6d3-113">List all configured information protection labels for a user or tenant.</span></span>                                                                                                |
| [<span data-ttu-id="8a6d3-114">Получить informationProtectionLabel</span><span class="sxs-lookup"><span data-stu-id="8a6d3-114">Get informationProtectionLabel</span></span>](../api/informationprotectionlabel-get.md)                          | [<span data-ttu-id="8a6d3-115">informationProtectionLabel</span><span class="sxs-lookup"><span data-stu-id="8a6d3-115">informationProtectionLabel</span></span>](informationprotectionlabel.md)               | <span data-ttu-id="8a6d3-116">Учитывая определенный ID метки, **верните informationProtectionLabel**.</span><span class="sxs-lookup"><span data-stu-id="8a6d3-116">Given a specific label ID, return the **informationProtectionLabel**.</span></span>                                                                                                  |
| [<span data-ttu-id="8a6d3-117">evaluateapplication</span><span class="sxs-lookup"><span data-stu-id="8a6d3-117">evaluateapplication</span></span>](../api/informationprotectionlabel-evaluateapplication.md)                     | <span data-ttu-id="8a6d3-118">[коллекция informationProtectionAction](informationprotectionaction.md)</span><span class="sxs-lookup"><span data-stu-id="8a6d3-118">[informationProtectionAction](informationprotectionaction.md) collection</span></span>  | <span data-ttu-id="8a6d3-119">Учитывая вход [контентаInfo](contentinfo.md) и [labelingOptions,](labelingoptions.md)вычислить набор действий, необходимых для применения метки.</span><span class="sxs-lookup"><span data-stu-id="8a6d3-119">Given an input of [contentInfo](contentinfo.md) and [labelingOptions](labelingoptions.md), compute the set of actions require to apply the label.</span></span>                      |
| [<span data-ttu-id="8a6d3-120">evaluateClassificationResults</span><span class="sxs-lookup"><span data-stu-id="8a6d3-120">evaluateClassificationResults</span></span>](../api/informationprotectionlabel-evaluateclassificationresults.md) | <span data-ttu-id="8a6d3-121">[коллекция informationProtectionAction](informationprotectionaction.md)</span><span class="sxs-lookup"><span data-stu-id="8a6d3-121">[informationProtectionAction](informationprotectionaction.md) collection</span></span>  | <span data-ttu-id="8a6d3-122">Учитывая ввод [контентаInfo и](contentinfo.md) результаты классификации, вычислить набор действий, необходимых для применения метки.</span><span class="sxs-lookup"><span data-stu-id="8a6d3-122">Given an input of [contentInfo](contentinfo.md) and classification results, compute the set of actions require to apply the label.</span></span>                                  |
| [<span data-ttu-id="8a6d3-123">evaluateRemoval</span><span class="sxs-lookup"><span data-stu-id="8a6d3-123">evaluateRemoval</span></span>](../api/informationprotectionlabel-evaluateremoval.md)                             | <span data-ttu-id="8a6d3-124">[коллекция informationProtectionAction](informationprotectionaction.md)</span><span class="sxs-lookup"><span data-stu-id="8a6d3-124">[informationProtectionAction](informationprotectionaction.md) collection</span></span>  | <span data-ttu-id="8a6d3-125">Учитывая вход [контентаInfo](contentinfo.md) и [downgradeJustification,](downgradejustification.md)вычислять действия, которые необходимо принять для удаления метки.</span><span class="sxs-lookup"><span data-stu-id="8a6d3-125">Given an input of [contentInfo](contentinfo.md) and [downgradeJustification](downgradejustification.md), compute the actions that should be taken to remove the label.</span></span> |
| [<span data-ttu-id="8a6d3-126">extractLabel</span><span class="sxs-lookup"><span data-stu-id="8a6d3-126">extractLabel</span></span>](../api/informationprotectionlabel-extractlabel.md)                                   | [<span data-ttu-id="8a6d3-127">informationProtectionContentLabel</span><span class="sxs-lookup"><span data-stu-id="8a6d3-127">informationProtectionContentLabel</span></span>](informationprotectioncontentlabel.md) | <span data-ttu-id="8a6d3-128">Учитывая вход [контентаInfo,](contentinfo.md)возвращайте сведения о [informationProtectionLabel,](informationprotectionlabel.md) который представляют метаданные.</span><span class="sxs-lookup"><span data-stu-id="8a6d3-128">Given an input of [contentInfo](contentinfo.md), return details on the [informationProtectionLabel](informationprotectionlabel.md) that the metadata represents.</span></span>       |

## <a name="properties"></a><span data-ttu-id="8a6d3-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="8a6d3-129">Properties</span></span>

| <span data-ttu-id="8a6d3-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8a6d3-130">Property</span></span>    | <span data-ttu-id="8a6d3-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8a6d3-131">Type</span></span>    | <span data-ttu-id="8a6d3-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8a6d3-132">Description</span></span>                                                                                     |
| :---------- | :------ | :---------------------------------------------------------------------------------------------- |
| <span data-ttu-id="8a6d3-133">color</span><span class="sxs-lookup"><span data-stu-id="8a6d3-133">color</span></span>       | <span data-ttu-id="8a6d3-134">String</span><span class="sxs-lookup"><span data-stu-id="8a6d3-134">String</span></span>  | <span data-ttu-id="8a6d3-135">Цвет, который должен отображаться пользовательским интерфейсом для метки, если настроен.</span><span class="sxs-lookup"><span data-stu-id="8a6d3-135">The color that the UI should display for the label, if configured.</span></span>                              |
| <span data-ttu-id="8a6d3-136">description</span><span class="sxs-lookup"><span data-stu-id="8a6d3-136">description</span></span> | <span data-ttu-id="8a6d3-137">Строка</span><span class="sxs-lookup"><span data-stu-id="8a6d3-137">String</span></span>  | <span data-ttu-id="8a6d3-138">Описание метки, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="8a6d3-138">The admin-defined description for the label.</span></span>                                                    |
| <span data-ttu-id="8a6d3-139">id</span><span class="sxs-lookup"><span data-stu-id="8a6d3-139">id</span></span>          | <span data-ttu-id="8a6d3-140">Строка</span><span class="sxs-lookup"><span data-stu-id="8a6d3-140">String</span></span>  | <span data-ttu-id="8a6d3-141">Идентификатор метки — это уникальный идентификатор глобального масштаба (GUID)</span><span class="sxs-lookup"><span data-stu-id="8a6d3-141">The label ID is a globally unique identifier (GUID)</span></span>                                             |
| <span data-ttu-id="8a6d3-142">isActive</span><span class="sxs-lookup"><span data-stu-id="8a6d3-142">isActive</span></span>    | <span data-ttu-id="8a6d3-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a6d3-143">Boolean</span></span> | <span data-ttu-id="8a6d3-144">Указывает, активна метка или нет.</span><span class="sxs-lookup"><span data-stu-id="8a6d3-144">Indicates whether the label is active or not.</span></span> <span data-ttu-id="8a6d3-145">Активные метки должны быть скрыты или отключены в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="8a6d3-145">Active labels should be hidden or disabled in UI.</span></span> |
| <span data-ttu-id="8a6d3-146">name</span><span class="sxs-lookup"><span data-stu-id="8a6d3-146">name</span></span>        | <span data-ttu-id="8a6d3-147">String</span><span class="sxs-lookup"><span data-stu-id="8a6d3-147">String</span></span>  | <span data-ttu-id="8a6d3-148">Простое имя метки.</span><span class="sxs-lookup"><span data-stu-id="8a6d3-148">The plaintext name of the label.</span></span>                                                                |
| <span data-ttu-id="8a6d3-149">sensitivity</span><span class="sxs-lookup"><span data-stu-id="8a6d3-149">sensitivity</span></span> | <span data-ttu-id="8a6d3-150">Int32</span><span class="sxs-lookup"><span data-stu-id="8a6d3-150">Int32</span></span>   | <span data-ttu-id="8a6d3-151">Значение чувствительности метки, где более низкий уровень менее чувствителен.</span><span class="sxs-lookup"><span data-stu-id="8a6d3-151">The sensitivity value of the label, where lower is less sensitive.</span></span>                              |
| <span data-ttu-id="8a6d3-152">tooltip</span><span class="sxs-lookup"><span data-stu-id="8a6d3-152">tooltip</span></span>     | <span data-ttu-id="8a6d3-153">Строка</span><span class="sxs-lookup"><span data-stu-id="8a6d3-153">String</span></span>  | <span data-ttu-id="8a6d3-154">Инструмент, который должен отображаться для метки в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="8a6d3-154">The tooltip that should be displayed for the label in a UI.</span></span>                                     |
| <span data-ttu-id="8a6d3-155">родитель</span><span class="sxs-lookup"><span data-stu-id="8a6d3-155">parent</span></span>      | <span data-ttu-id="8a6d3-156">labelDetails</span><span class="sxs-lookup"><span data-stu-id="8a6d3-156">labelDetails</span></span>   | <span data-ttu-id="8a6d3-157">Родительская метка, связанная с детской меткой.</span><span class="sxs-lookup"><span data-stu-id="8a6d3-157">The parent label associated with a child label.</span></span> <span data-ttu-id="8a6d3-158">Null, если метка не имеет родительского знака.</span><span class="sxs-lookup"><span data-stu-id="8a6d3-158">Null if label has no parent.</span></span>

## <a name="relationships"></a><span data-ttu-id="8a6d3-159">Отношения</span><span class="sxs-lookup"><span data-stu-id="8a6d3-159">Relationships</span></span>

<span data-ttu-id="8a6d3-160">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="8a6d3-160">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8a6d3-161">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="8a6d3-161">JSON representation</span></span>

<span data-ttu-id="8a6d3-162">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8a6d3-162">The following is a JSON representation of the resource.</span></span>

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
  "tooltip": "String",
  "parent": {"@odata.type": "microsoft.graph.labelDetails" }
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


