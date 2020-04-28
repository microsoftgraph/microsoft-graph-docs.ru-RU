---
title: Тип ресурса Информатионпротектионлабел
description: Описывает метку Information Protection, которая подробно описывает, как правильно применять метку конфиденциальности к данным.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 183a5856aafd8aa2a5b8b1fe3b1eb48bddcc5358
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42496042"
---
# <a name="informationprotectionlabel-resource-type"></a><span data-ttu-id="47a79-103">Тип ресурса Информатионпротектионлабел</span><span class="sxs-lookup"><span data-stu-id="47a79-103">informationProtectionLabel resource type</span></span>

<span data-ttu-id="47a79-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47a79-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="47a79-105">Описывает метку Information Protection, которая подробно описывает, как правильно применять метку конфиденциальности к данным.</span><span class="sxs-lookup"><span data-stu-id="47a79-105">Describes the information protection label that details how to properly apply a sensitivity label to information.</span></span> <span data-ttu-id="47a79-106">Ресурс **информатионпротектионлабел** описывает конфигурацию меток конфиденциальности, которые применяются к пользователю или клиенту.</span><span class="sxs-lookup"><span data-stu-id="47a79-106">The **informationProtectionLabel** resource describes the configuration of sensitivity labels that apply to a user or tenant.</span></span>  

## <a name="methods"></a><span data-ttu-id="47a79-107">Методы</span><span class="sxs-lookup"><span data-stu-id="47a79-107">Methods</span></span>

| <span data-ttu-id="47a79-108">Метод</span><span class="sxs-lookup"><span data-stu-id="47a79-108">Method</span></span>                                                                                              | <span data-ttu-id="47a79-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="47a79-109">Return Type</span></span>                                                               | <span data-ttu-id="47a79-110">Описание</span><span class="sxs-lookup"><span data-stu-id="47a79-110">Description</span></span>                                                                                                                                                            |
| :-------------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------ | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [<span data-ttu-id="47a79-111">Список Информатионпротектионлабел</span><span class="sxs-lookup"><span data-stu-id="47a79-111">List informationProtectionLabel</span></span>](../api/informationprotectionpolicy-list-labels.md)                | <span data-ttu-id="47a79-112">Коллекция [информатионпротектионлабел](informationprotectionlabel.md)</span><span class="sxs-lookup"><span data-stu-id="47a79-112">[informationProtectionLabel](informationprotectionlabel.md) collection</span></span> | <span data-ttu-id="47a79-113">Перечисление всех настроенных меток защиты информации для пользователя или клиента.</span><span class="sxs-lookup"><span data-stu-id="47a79-113">List all configured information protection labels for a user or tenant.</span></span>                                                                                                |
| [<span data-ttu-id="47a79-114">Получение Информатионпротектионлабел</span><span class="sxs-lookup"><span data-stu-id="47a79-114">Get informationProtectionLabel</span></span>](../api/informationprotectionlabel-get.md)                          | [<span data-ttu-id="47a79-115">информатионпротектионлабел</span><span class="sxs-lookup"><span data-stu-id="47a79-115">informationProtectionLabel</span></span>](informationprotectionlabel.md)               | <span data-ttu-id="47a79-116">При наличии определенного идентификатора метки возвратите **информатионпротектионлабел**.</span><span class="sxs-lookup"><span data-stu-id="47a79-116">Given a specific label ID, return the **informationProtectionLabel**.</span></span>                                                                                                  |
| [<span data-ttu-id="47a79-117">евалуатеаппликатион</span><span class="sxs-lookup"><span data-stu-id="47a79-117">evaluateapplication</span></span>](../api/informationprotectionlabel-evaluateapplication.md)                     | <span data-ttu-id="47a79-118">Коллекция [информатионпротектионактион](informationprotectionaction.md)</span><span class="sxs-lookup"><span data-stu-id="47a79-118">[informationProtectionAction](informationprotectionaction.md) collection</span></span>  | <span data-ttu-id="47a79-119">При наличии входных данных для [контентинфо](contentinfo.md) и [лабелингоптионс](labelingoptions.md)расчет набора действий требует применения метки.</span><span class="sxs-lookup"><span data-stu-id="47a79-119">Given an input of [contentInfo](contentinfo.md) and [labelingOptions](labelingoptions.md), compute the set of actions require to apply the label.</span></span>                      |
| [<span data-ttu-id="47a79-120">евалуатеклассификатионресултс</span><span class="sxs-lookup"><span data-stu-id="47a79-120">evaluateClassificationResults</span></span>](../api/informationprotectionlabel-evaluateclassificationresults.md) | <span data-ttu-id="47a79-121">Коллекция [информатионпротектионактион](informationprotectionaction.md)</span><span class="sxs-lookup"><span data-stu-id="47a79-121">[informationProtectionAction](informationprotectionaction.md) collection</span></span>  | <span data-ttu-id="47a79-122">Имея входные данные о [контентинфо](contentinfo.md) и классификации, вычислите набор действий, необходимых для применения метки.</span><span class="sxs-lookup"><span data-stu-id="47a79-122">Given an input of [contentInfo](contentinfo.md) and classification results, compute the set of actions require to apply the label.</span></span>                                  |
| [<span data-ttu-id="47a79-123">евалуатеремовал</span><span class="sxs-lookup"><span data-stu-id="47a79-123">evaluateRemoval</span></span>](../api/informationprotectionlabel-evaluateremoval.md)                             | <span data-ttu-id="47a79-124">Коллекция [информатионпротектионактион](informationprotectionaction.md)</span><span class="sxs-lookup"><span data-stu-id="47a79-124">[informationProtectionAction](informationprotectionaction.md) collection</span></span>  | <span data-ttu-id="47a79-125">При наличии входных данных для [контентинфо](contentinfo.md) и [довнградежустификатион](downgradejustification.md)вычисляет действия, которые следует предпринять для удаления метки.</span><span class="sxs-lookup"><span data-stu-id="47a79-125">Given an input of [contentInfo](contentinfo.md) and [downgradeJustification](downgradejustification.md), compute the actions that should be taken to remove the label.</span></span> |
| [<span data-ttu-id="47a79-126">екстрактлабел</span><span class="sxs-lookup"><span data-stu-id="47a79-126">extractLabel</span></span>](../api/informationprotectionlabel-extractlabel.md)                                   | [<span data-ttu-id="47a79-127">информатионпротектионконтентлабел</span><span class="sxs-lookup"><span data-stu-id="47a79-127">informationProtectionContentLabel</span></span>](informationprotectioncontentlabel.md) | <span data-ttu-id="47a79-128">При наличии входных данных [контентинфо](contentinfo.md)возвращает сведения о [информатионпротектионлабел](informationprotectionlabel.md) , которые представляют метаданные.</span><span class="sxs-lookup"><span data-stu-id="47a79-128">Given an input of [contentInfo](contentinfo.md), return details on the [informationProtectionLabel](informationprotectionlabel.md) that the metadata represents.</span></span>       |

## <a name="properties"></a><span data-ttu-id="47a79-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="47a79-129">Properties</span></span>

| <span data-ttu-id="47a79-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="47a79-130">Property</span></span>    | <span data-ttu-id="47a79-131">Тип</span><span class="sxs-lookup"><span data-stu-id="47a79-131">Type</span></span>    | <span data-ttu-id="47a79-132">Описание</span><span class="sxs-lookup"><span data-stu-id="47a79-132">Description</span></span>                                                                                     |
| :---------- | :------ | :---------------------------------------------------------------------------------------------- |
| <span data-ttu-id="47a79-133">color</span><span class="sxs-lookup"><span data-stu-id="47a79-133">color</span></span>       | <span data-ttu-id="47a79-134">String</span><span class="sxs-lookup"><span data-stu-id="47a79-134">String</span></span>  | <span data-ttu-id="47a79-135">Цвет, который должен отображаться в пользовательском интерфейсе для метки, если она настроена.</span><span class="sxs-lookup"><span data-stu-id="47a79-135">The color that the UI should display for the label, if configured.</span></span>                              |
| <span data-ttu-id="47a79-136">description</span><span class="sxs-lookup"><span data-stu-id="47a79-136">description</span></span> | <span data-ttu-id="47a79-137">String</span><span class="sxs-lookup"><span data-stu-id="47a79-137">String</span></span>  | <span data-ttu-id="47a79-138">Заданное администратором описание метки.</span><span class="sxs-lookup"><span data-stu-id="47a79-138">The admin-defined description for the label.</span></span>                                                    |
| <span data-ttu-id="47a79-139">id</span><span class="sxs-lookup"><span data-stu-id="47a79-139">id</span></span>          | <span data-ttu-id="47a79-140">Строка</span><span class="sxs-lookup"><span data-stu-id="47a79-140">String</span></span>  | <span data-ttu-id="47a79-141">ИДЕНТИФИКАТОР метки является глобальным уникальным идентификатором (GUID)</span><span class="sxs-lookup"><span data-stu-id="47a79-141">The label ID is a globally unique identifier (GUID)</span></span>                                             |
| <span data-ttu-id="47a79-142">isActive</span><span class="sxs-lookup"><span data-stu-id="47a79-142">isActive</span></span>    | <span data-ttu-id="47a79-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="47a79-143">Boolean</span></span> | <span data-ttu-id="47a79-144">Указывает, активна ли метка.</span><span class="sxs-lookup"><span data-stu-id="47a79-144">Indicates whether the label is active or not.</span></span> <span data-ttu-id="47a79-145">Активные метки должны быть скрыты или отключены в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="47a79-145">Active labels should be hidden or disabled in UI.</span></span> |
| <span data-ttu-id="47a79-146">name</span><span class="sxs-lookup"><span data-stu-id="47a79-146">name</span></span>        | <span data-ttu-id="47a79-147">String</span><span class="sxs-lookup"><span data-stu-id="47a79-147">String</span></span>  | <span data-ttu-id="47a79-148">Имя в виде открытого текста метки.</span><span class="sxs-lookup"><span data-stu-id="47a79-148">The plaintext name of the label.</span></span>                                                                |
| <span data-ttu-id="47a79-149">sensitivity</span><span class="sxs-lookup"><span data-stu-id="47a79-149">sensitivity</span></span> | <span data-ttu-id="47a79-150">Int32</span><span class="sxs-lookup"><span data-stu-id="47a79-150">Int32</span></span>   | <span data-ttu-id="47a79-151">Значение чувствительности метки, где меньше конфиденциально.</span><span class="sxs-lookup"><span data-stu-id="47a79-151">The sensitivity value of the label, where lower is less sensitive.</span></span>                              |
| <span data-ttu-id="47a79-152">tooltip</span><span class="sxs-lookup"><span data-stu-id="47a79-152">tooltip</span></span>     | <span data-ttu-id="47a79-153">String</span><span class="sxs-lookup"><span data-stu-id="47a79-153">String</span></span>  | <span data-ttu-id="47a79-154">Всплывающая подсказка, отображаемая для метки в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="47a79-154">The tooltip that should be displayed for the label in a UI.</span></span>                                     |

## <a name="relationships"></a><span data-ttu-id="47a79-155">Связи</span><span class="sxs-lookup"><span data-stu-id="47a79-155">Relationships</span></span>

<span data-ttu-id="47a79-156">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="47a79-156">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="47a79-157">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="47a79-157">JSON representation</span></span>

<span data-ttu-id="47a79-158">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="47a79-158">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.informationProtectionLabel",
  "baseType": "",
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
