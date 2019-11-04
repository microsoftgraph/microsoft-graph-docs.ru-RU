---
title: Тип ресурса Информатионпротектионлабел
description: Описывает метку Information Protection, которая подробно описывает, как правильно применять метку конфиденциальности к данным.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 528238d904ac9807027dd51a8c59ed03570c7bc3
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938746"
---
# <a name="informationprotectionlabel-resource-type"></a><span data-ttu-id="e3e35-103">Тип ресурса Информатионпротектионлабел</span><span class="sxs-lookup"><span data-stu-id="e3e35-103">informationProtectionLabel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3e35-104">Описывает метку Information Protection, которая подробно описывает, как правильно применять метку конфиденциальности к данным.</span><span class="sxs-lookup"><span data-stu-id="e3e35-104">Describes the information protection label that details how to properly apply a sensitivity label to information.</span></span> <span data-ttu-id="e3e35-105">Ресурс **информатионпротектионлабел** описывает конфигурацию меток конфиденциальности, которые применяются к пользователю или клиенту.</span><span class="sxs-lookup"><span data-stu-id="e3e35-105">The **informationProtectionLabel** resource describes the configuration of sensitivity labels that apply to a user or tenant.</span></span>  

## <a name="methods"></a><span data-ttu-id="e3e35-106">Методы</span><span class="sxs-lookup"><span data-stu-id="e3e35-106">Methods</span></span>

| <span data-ttu-id="e3e35-107">Метод</span><span class="sxs-lookup"><span data-stu-id="e3e35-107">Method</span></span>                                                                                              | <span data-ttu-id="e3e35-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e3e35-108">Return Type</span></span>                                                               | <span data-ttu-id="e3e35-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e3e35-109">Description</span></span>                                                                                                                                                            |
| :-------------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------ | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [<span data-ttu-id="e3e35-110">Список Информатионпротектионлабел</span><span class="sxs-lookup"><span data-stu-id="e3e35-110">List informationProtectionLabel</span></span>](../api/informationprotectionpolicy-list-labels.md)                | <span data-ttu-id="e3e35-111">Коллекция [информатионпротектионлабел](informationprotectionlabel.md)</span><span class="sxs-lookup"><span data-stu-id="e3e35-111">[informationProtectionLabel](informationprotectionlabel.md) collection</span></span> | <span data-ttu-id="e3e35-112">Перечисление всех настроенных меток защиты информации для пользователя или клиента.</span><span class="sxs-lookup"><span data-stu-id="e3e35-112">List all configured information protection labels for a user or tenant.</span></span>                                                                                                |
| [<span data-ttu-id="e3e35-113">Получение Информатионпротектионлабел</span><span class="sxs-lookup"><span data-stu-id="e3e35-113">Get informationProtectionLabel</span></span>](../api/informationprotectionlabel-get.md)                          | [<span data-ttu-id="e3e35-114">информатионпротектионлабел</span><span class="sxs-lookup"><span data-stu-id="e3e35-114">informationProtectionLabel</span></span>](informationprotectionlabel.md)               | <span data-ttu-id="e3e35-115">При наличии определенного идентификатора метки возвратите **информатионпротектионлабел**.</span><span class="sxs-lookup"><span data-stu-id="e3e35-115">Given a specific label ID, return the **informationProtectionLabel**.</span></span>                                                                                                  |
| [<span data-ttu-id="e3e35-116">евалуатеаппликатион</span><span class="sxs-lookup"><span data-stu-id="e3e35-116">evaluateapplication</span></span>](../api/informationprotectionlabel-evaluateapplication.md)                     | <span data-ttu-id="e3e35-117">Коллекция [информатионпротектионактион](informationprotectionaction.md)</span><span class="sxs-lookup"><span data-stu-id="e3e35-117">[informationProtectionAction](informationprotectionaction.md) collection</span></span>  | <span data-ttu-id="e3e35-118">При наличии входных данных для [контентинфо](contentinfo.md) и [лабелингоптионс](labelingoptions.md)расчет набора действий требует применения метки.</span><span class="sxs-lookup"><span data-stu-id="e3e35-118">Given an input of [contentInfo](contentinfo.md) and [labelingOptions](labelingoptions.md), compute the set of actions require to apply the label.</span></span>                      |
| [<span data-ttu-id="e3e35-119">евалуатеклассификатионресултс</span><span class="sxs-lookup"><span data-stu-id="e3e35-119">evaluateClassificationResults</span></span>](../api/informationprotectionlabel-evaluateclassificationresults.md) | <span data-ttu-id="e3e35-120">Коллекция [информатионпротектионактион](informationprotectionaction.md)</span><span class="sxs-lookup"><span data-stu-id="e3e35-120">[informationProtectionAction](informationprotectionaction.md) collection</span></span>  | <span data-ttu-id="e3e35-121">Имея входные данные о [контентинфо](contentinfo.md) и классификации, вычислите набор действий, необходимых для применения метки.</span><span class="sxs-lookup"><span data-stu-id="e3e35-121">Given an input of [contentInfo](contentinfo.md) and classification results, compute the set of actions require to apply the label.</span></span>                                  |
| [<span data-ttu-id="e3e35-122">евалуатеремовал</span><span class="sxs-lookup"><span data-stu-id="e3e35-122">evaluateRemoval</span></span>](../api/informationprotectionlabel-evaluateremoval.md)                             | <span data-ttu-id="e3e35-123">Коллекция [информатионпротектионактион](informationprotectionaction.md)</span><span class="sxs-lookup"><span data-stu-id="e3e35-123">[informationProtectionAction](informationprotectionaction.md) collection</span></span>  | <span data-ttu-id="e3e35-124">При наличии входных данных для [контентинфо](contentinfo.md) и [довнградежустификатион](downgradejustification.md)вычисляет действия, которые следует предпринять для удаления метки.</span><span class="sxs-lookup"><span data-stu-id="e3e35-124">Given an input of [contentInfo](contentinfo.md) and [downgradeJustification](downgradejustification.md), compute the actions that should be taken to remove the label.</span></span> |
| [<span data-ttu-id="e3e35-125">екстрактлабел</span><span class="sxs-lookup"><span data-stu-id="e3e35-125">extractLabel</span></span>](../api/informationprotectionlabel-extractlabel.md)                                   | [<span data-ttu-id="e3e35-126">информатионпротектионконтентлабел</span><span class="sxs-lookup"><span data-stu-id="e3e35-126">informationProtectionContentLabel</span></span>](informationprotectioncontentlabel.md) | <span data-ttu-id="e3e35-127">При наличии входных данных [контентинфо](contentinfo.md)возвращает сведения о [информатионпротектионлабел](informationprotectionlabel.md) , которые представляют метаданные.</span><span class="sxs-lookup"><span data-stu-id="e3e35-127">Given an input of [contentInfo](contentinfo.md), return details on the [informationProtectionLabel](informationprotectionlabel.md) that the metadata represents.</span></span>       |

## <a name="properties"></a><span data-ttu-id="e3e35-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="e3e35-128">Properties</span></span>

| <span data-ttu-id="e3e35-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e3e35-129">Property</span></span>    | <span data-ttu-id="e3e35-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e3e35-130">Type</span></span>    | <span data-ttu-id="e3e35-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e3e35-131">Description</span></span>                                                                                     |
| :---------- | :------ | :---------------------------------------------------------------------------------------------- |
| <span data-ttu-id="e3e35-132">color</span><span class="sxs-lookup"><span data-stu-id="e3e35-132">color</span></span>       | <span data-ttu-id="e3e35-133">String</span><span class="sxs-lookup"><span data-stu-id="e3e35-133">String</span></span>  | <span data-ttu-id="e3e35-134">Цвет, который должен отображаться в пользовательском интерфейсе для метки, если она настроена.</span><span class="sxs-lookup"><span data-stu-id="e3e35-134">The color that the UI should display for the label, if configured.</span></span>                              |
| <span data-ttu-id="e3e35-135">description</span><span class="sxs-lookup"><span data-stu-id="e3e35-135">description</span></span> | <span data-ttu-id="e3e35-136">Строка</span><span class="sxs-lookup"><span data-stu-id="e3e35-136">String</span></span>  | <span data-ttu-id="e3e35-137">Заданное администратором описание метки.</span><span class="sxs-lookup"><span data-stu-id="e3e35-137">The admin-defined description for the label.</span></span>                                                    |
| <span data-ttu-id="e3e35-138">id</span><span class="sxs-lookup"><span data-stu-id="e3e35-138">id</span></span>          | <span data-ttu-id="e3e35-139">Строка</span><span class="sxs-lookup"><span data-stu-id="e3e35-139">String</span></span>  | <span data-ttu-id="e3e35-140">ИДЕНТИФИКАТОР метки является глобальным уникальным идентификатором (GUID)</span><span class="sxs-lookup"><span data-stu-id="e3e35-140">The label ID is a globally unique identifier (GUID)</span></span>                                             |
| <span data-ttu-id="e3e35-141">isActive</span><span class="sxs-lookup"><span data-stu-id="e3e35-141">isActive</span></span>    | <span data-ttu-id="e3e35-142">Логический</span><span class="sxs-lookup"><span data-stu-id="e3e35-142">Boolean</span></span> | <span data-ttu-id="e3e35-143">Указывает, активна ли метка.</span><span class="sxs-lookup"><span data-stu-id="e3e35-143">Indicates whether the label is active or not.</span></span> <span data-ttu-id="e3e35-144">Активные метки должны быть скрыты или отключены в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="e3e35-144">Active labels should be hidden or disabled in UI.</span></span> |
| <span data-ttu-id="e3e35-145">name</span><span class="sxs-lookup"><span data-stu-id="e3e35-145">name</span></span>        | <span data-ttu-id="e3e35-146">String</span><span class="sxs-lookup"><span data-stu-id="e3e35-146">String</span></span>  | <span data-ttu-id="e3e35-147">Имя в виде открытого текста метки.</span><span class="sxs-lookup"><span data-stu-id="e3e35-147">The plaintext name of the label.</span></span>                                                                |
| <span data-ttu-id="e3e35-148">sensitivity</span><span class="sxs-lookup"><span data-stu-id="e3e35-148">sensitivity</span></span> | <span data-ttu-id="e3e35-149">Int32</span><span class="sxs-lookup"><span data-stu-id="e3e35-149">Int32</span></span>   | <span data-ttu-id="e3e35-150">Значение чувствительности метки, где меньше конфиденциально.</span><span class="sxs-lookup"><span data-stu-id="e3e35-150">The sensitivity value of the label, where lower is less sensitive.</span></span>                              |
| <span data-ttu-id="e3e35-151">tooltip</span><span class="sxs-lookup"><span data-stu-id="e3e35-151">tooltip</span></span>     | <span data-ttu-id="e3e35-152">Строка</span><span class="sxs-lookup"><span data-stu-id="e3e35-152">String</span></span>  | <span data-ttu-id="e3e35-153">Всплывающая подсказка, отображаемая для метки в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="e3e35-153">The tooltip that should be displayed for the label in a UI.</span></span>                                     |

## <a name="relationships"></a><span data-ttu-id="e3e35-154">Связи</span><span class="sxs-lookup"><span data-stu-id="e3e35-154">Relationships</span></span>

<span data-ttu-id="e3e35-155">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e3e35-155">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e3e35-156">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e3e35-156">JSON representation</span></span>

<span data-ttu-id="e3e35-157">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e3e35-157">The following is a JSON representation of the resource.</span></span>

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
