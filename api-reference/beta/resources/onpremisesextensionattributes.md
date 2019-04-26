---
title: Тип ресурса onPremisesExtensionAttributes
description: Свойство **onPremisesExtensionAttributes** объекта user содержит пятнадцать свойств настраиваемого атрибута расширения. Для пользователя **onPremisesSyncEnabled** этот набор свойств размещается в локальной службе Active Directory и синхронизируется с Azure AD и доступен только для чтения. Для пользователя, предназначенного только для облачного облака (где **onPremisesSyncEnabled** имеет значение false), эти свойства можно задать при создании или обновлении.
localization_priority: Normal
ms.openlocfilehash: 14e6d8530e67f40704d1052ef5e66cf9046b883f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341811"
---
# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="fb883-105">Тип ресурса onPremisesExtensionAttributes</span><span class="sxs-lookup"><span data-stu-id="fb883-105">onPremisesExtensionAttributes resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb883-106">Свойство **onPremisesExtensionAttributes** объекта [User](user.md) содержит пятнадцать свойств настраиваемого атрибута расширения.</span><span class="sxs-lookup"><span data-stu-id="fb883-106">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="fb883-107">Для пользователя **onPremisesSyncEnabled** этот набор свойств размещается в локальной службе Active Directory и синхронизируется с Azure AD и доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fb883-107">For an **onPremisesSyncEnabled** user, this set of properties is mastered in on-premises Active Directory and synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="fb883-108">Для пользователя, предназначенного только для облачного облака (где **onPremisesSyncEnabled** имеет значение false), эти свойства можно задать при создании или обновлении.</span><span class="sxs-lookup"><span data-stu-id="fb883-108">For a cloud-only user (where **onPremisesSyncEnabled** is false), these properties may be set during creation or update.</span></span>


## <a name="properties"></a><span data-ttu-id="fb883-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="fb883-109">Properties</span></span>
| <span data-ttu-id="fb883-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="fb883-110">Property</span></span>     | <span data-ttu-id="fb883-111">Тип</span><span class="sxs-lookup"><span data-stu-id="fb883-111">Type</span></span>   |<span data-ttu-id="fb883-112">Описание</span><span class="sxs-lookup"><span data-stu-id="fb883-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fb883-113">От extensionattribute1</span><span class="sxs-lookup"><span data-stu-id="fb883-113">extensionAttribute1</span></span>|<span data-ttu-id="fb883-114">String</span><span class="sxs-lookup"><span data-stu-id="fb883-114">String</span></span>| <span data-ttu-id="fb883-115">Первый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="fb883-115">First customizable extension attribute.</span></span> |
|<span data-ttu-id="fb883-116">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="fb883-116">extensionAttribute2</span></span>|<span data-ttu-id="fb883-117">String</span><span class="sxs-lookup"><span data-stu-id="fb883-117">String</span></span>| <span data-ttu-id="fb883-118">Второй настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="fb883-118">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="fb883-119">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="fb883-119">extensionAttribute3</span></span>|<span data-ttu-id="fb883-120">String</span><span class="sxs-lookup"><span data-stu-id="fb883-120">String</span></span>| <span data-ttu-id="fb883-121">Третий настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="fb883-121">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="fb883-122">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="fb883-122">extensionAttribute4</span></span>|<span data-ttu-id="fb883-123">String</span><span class="sxs-lookup"><span data-stu-id="fb883-123">String</span></span>| <span data-ttu-id="fb883-124">Четвертый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="fb883-124">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="fb883-125">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="fb883-125">extensionAttribute5</span></span>|<span data-ttu-id="fb883-126">String</span><span class="sxs-lookup"><span data-stu-id="fb883-126">String</span></span>| <span data-ttu-id="fb883-127">Пятый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="fb883-127">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="fb883-128">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="fb883-128">extensionAttribute6</span></span>|<span data-ttu-id="fb883-129">String</span><span class="sxs-lookup"><span data-stu-id="fb883-129">String</span></span>| <span data-ttu-id="fb883-130">Шестой настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="fb883-130">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="fb883-131">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="fb883-131">extensionAttribute7</span></span>|<span data-ttu-id="fb883-132">String</span><span class="sxs-lookup"><span data-stu-id="fb883-132">String</span></span>| <span data-ttu-id="fb883-133">Седьмой настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="fb883-133">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="fb883-134">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="fb883-134">extensionAttribute8</span></span>|<span data-ttu-id="fb883-135">String</span><span class="sxs-lookup"><span data-stu-id="fb883-135">String</span></span>| <span data-ttu-id="fb883-136">Восьмой настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="fb883-136">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="fb883-137">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="fb883-137">extensionAttribute9</span></span>|<span data-ttu-id="fb883-138">String</span><span class="sxs-lookup"><span data-stu-id="fb883-138">String</span></span>| <span data-ttu-id="fb883-139">Девятый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="fb883-139">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="fb883-140">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="fb883-140">extensionAttribute10</span></span>|<span data-ttu-id="fb883-141">String</span><span class="sxs-lookup"><span data-stu-id="fb883-141">String</span></span>| <span data-ttu-id="fb883-142">Десятый атрибут расширенной настройки.</span><span class="sxs-lookup"><span data-stu-id="fb883-142">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="fb883-143">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="fb883-143">extensionAttribute11</span></span>|<span data-ttu-id="fb883-144">String</span><span class="sxs-lookup"><span data-stu-id="fb883-144">String</span></span>| <span data-ttu-id="fb883-145">Одиннадцатый атрибут настраиваемого расширения.</span><span class="sxs-lookup"><span data-stu-id="fb883-145">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="fb883-146">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="fb883-146">extensionAttribute12</span></span>|<span data-ttu-id="fb883-147">String</span><span class="sxs-lookup"><span data-stu-id="fb883-147">String</span></span>| <span data-ttu-id="fb883-148">Двенадцатый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="fb883-148">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="fb883-149">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="fb883-149">extensionAttribute13</span></span>|<span data-ttu-id="fb883-150">String</span><span class="sxs-lookup"><span data-stu-id="fb883-150">String</span></span>| <span data-ttu-id="fb883-151">Настраиваемый атрибут расширения Сиртинс.</span><span class="sxs-lookup"><span data-stu-id="fb883-151">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="fb883-152">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="fb883-152">extensionAttribute14</span></span>|<span data-ttu-id="fb883-153">String</span><span class="sxs-lookup"><span data-stu-id="fb883-153">String</span></span>| <span data-ttu-id="fb883-154">Настраиваемый атрибут расширения Фауртинс.</span><span class="sxs-lookup"><span data-stu-id="fb883-154">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="fb883-155">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="fb883-155">extensionAttribute15</span></span>|<span data-ttu-id="fb883-156">String</span><span class="sxs-lookup"><span data-stu-id="fb883-156">String</span></span>| <span data-ttu-id="fb883-157">Пятнадцатый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="fb883-157">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fb883-158">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fb883-158">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesExtensionAttributes"
}-->


```json
{
      "extensionAttribute1": "string",
      "extensionAttribute2": "string",
      "extensionAttribute3": "string",
      "extensionAttribute4": "string",
      "extensionAttribute5": "string",
      "extensionAttribute6": "string",
      "extensionAttribute7": "string",
      "extensionAttribute8": "string",
      "extensionAttribute9": "string",
      "extensionAttribute10": "string",
      "extensionAttribute11": "string",
      "extensionAttribute12": "string",
      "extensionAttribute13": "string",
      "extensionAttribute14": "string",
      "extensionAttribute15": "string"
  }

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onPremisesExtensionAttributes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
