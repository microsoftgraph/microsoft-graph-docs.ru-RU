---
title: Тип ресурса onPremisesExtensionAttributes
description: Свойство **onPremisesExtensionAttributes** объекта user содержит пятнадцать свойств настраиваемого атрибута расширения. Для пользователя **onPremisesSyncEnabled** этот набор свойств размещается в локальной службе Active Directory и синхронизируется с Azure AD и доступен только для чтения. Для пользователя, предназначенного только для облачного облака (где **onPremisesSyncEnabled** имеет значение false), эти свойства можно задать при создании или обновлении.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: japere
ms.openlocfilehash: 06f1fb9fea5338a93c92a2bce2e31098046528bc
ms.sourcegitcommit: ee41ba9ec6001716f1a9d575741bbeef577e2473
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/09/2020
ms.locfileid: "43200231"
---
# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="814aa-105">Тип ресурса onPremisesExtensionAttributes</span><span class="sxs-lookup"><span data-stu-id="814aa-105">onPremisesExtensionAttributes resource type</span></span>

<span data-ttu-id="814aa-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="814aa-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="814aa-107">Свойство **onPremisesExtensionAttributes** объекта [User](user.md) содержит пятнадцать свойств настраиваемого атрибута расширения.</span><span class="sxs-lookup"><span data-stu-id="814aa-107">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="814aa-108">Для пользователя **onPremisesSyncEnabled** этот набор свойств размещается в локальной службе Active Directory и синхронизируется с Azure AD и доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="814aa-108">For an **onPremisesSyncEnabled** user, this set of properties is mastered in on-premises Active Directory and synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="814aa-109">Для пользователя, предназначенного только для облачного облака (где **onPremisesSyncEnabled** имеет значение false), эти свойства можно задать при создании или обновлении.</span><span class="sxs-lookup"><span data-stu-id="814aa-109">For a cloud-only user (where **onPremisesSyncEnabled** is false), these properties may be set during creation or update.</span></span>


## <a name="properties"></a><span data-ttu-id="814aa-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="814aa-110">Properties</span></span>
| <span data-ttu-id="814aa-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="814aa-111">Property</span></span>     | <span data-ttu-id="814aa-112">Тип</span><span class="sxs-lookup"><span data-stu-id="814aa-112">Type</span></span>   |<span data-ttu-id="814aa-113">Описание</span><span class="sxs-lookup"><span data-stu-id="814aa-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="814aa-114">От extensionattribute1</span><span class="sxs-lookup"><span data-stu-id="814aa-114">extensionAttribute1</span></span>|<span data-ttu-id="814aa-115">String</span><span class="sxs-lookup"><span data-stu-id="814aa-115">String</span></span>| <span data-ttu-id="814aa-116">Первый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="814aa-116">First customizable extension attribute.</span></span> |
|<span data-ttu-id="814aa-117">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="814aa-117">extensionAttribute2</span></span>|<span data-ttu-id="814aa-118">String</span><span class="sxs-lookup"><span data-stu-id="814aa-118">String</span></span>| <span data-ttu-id="814aa-119">Второй настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="814aa-119">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="814aa-120">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="814aa-120">extensionAttribute3</span></span>|<span data-ttu-id="814aa-121">String</span><span class="sxs-lookup"><span data-stu-id="814aa-121">String</span></span>| <span data-ttu-id="814aa-122">Третий настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="814aa-122">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="814aa-123">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="814aa-123">extensionAttribute4</span></span>|<span data-ttu-id="814aa-124">String</span><span class="sxs-lookup"><span data-stu-id="814aa-124">String</span></span>| <span data-ttu-id="814aa-125">Четвертый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="814aa-125">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="814aa-126">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="814aa-126">extensionAttribute5</span></span>|<span data-ttu-id="814aa-127">String</span><span class="sxs-lookup"><span data-stu-id="814aa-127">String</span></span>| <span data-ttu-id="814aa-128">Пятый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="814aa-128">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="814aa-129">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="814aa-129">extensionAttribute6</span></span>|<span data-ttu-id="814aa-130">String</span><span class="sxs-lookup"><span data-stu-id="814aa-130">String</span></span>| <span data-ttu-id="814aa-131">Шестой настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="814aa-131">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="814aa-132">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="814aa-132">extensionAttribute7</span></span>|<span data-ttu-id="814aa-133">String</span><span class="sxs-lookup"><span data-stu-id="814aa-133">String</span></span>| <span data-ttu-id="814aa-134">Седьмой настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="814aa-134">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="814aa-135">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="814aa-135">extensionAttribute8</span></span>|<span data-ttu-id="814aa-136">String</span><span class="sxs-lookup"><span data-stu-id="814aa-136">String</span></span>| <span data-ttu-id="814aa-137">Восьмой настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="814aa-137">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="814aa-138">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="814aa-138">extensionAttribute9</span></span>|<span data-ttu-id="814aa-139">String</span><span class="sxs-lookup"><span data-stu-id="814aa-139">String</span></span>| <span data-ttu-id="814aa-140">Девятый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="814aa-140">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="814aa-141">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="814aa-141">extensionAttribute10</span></span>|<span data-ttu-id="814aa-142">String</span><span class="sxs-lookup"><span data-stu-id="814aa-142">String</span></span>| <span data-ttu-id="814aa-143">Десятый атрибут расширенной настройки.</span><span class="sxs-lookup"><span data-stu-id="814aa-143">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="814aa-144">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="814aa-144">extensionAttribute11</span></span>|<span data-ttu-id="814aa-145">String</span><span class="sxs-lookup"><span data-stu-id="814aa-145">String</span></span>| <span data-ttu-id="814aa-146">Одиннадцатый атрибут настраиваемого расширения.</span><span class="sxs-lookup"><span data-stu-id="814aa-146">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="814aa-147">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="814aa-147">extensionAttribute12</span></span>|<span data-ttu-id="814aa-148">String</span><span class="sxs-lookup"><span data-stu-id="814aa-148">String</span></span>| <span data-ttu-id="814aa-149">Двенадцатый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="814aa-149">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="814aa-150">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="814aa-150">extensionAttribute13</span></span>|<span data-ttu-id="814aa-151">String</span><span class="sxs-lookup"><span data-stu-id="814aa-151">String</span></span>| <span data-ttu-id="814aa-152">Настраиваемый атрибут расширения сиртинс.</span><span class="sxs-lookup"><span data-stu-id="814aa-152">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="814aa-153">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="814aa-153">extensionAttribute14</span></span>|<span data-ttu-id="814aa-154">String</span><span class="sxs-lookup"><span data-stu-id="814aa-154">String</span></span>| <span data-ttu-id="814aa-155">Настраиваемый атрибут расширения фауртинс.</span><span class="sxs-lookup"><span data-stu-id="814aa-155">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="814aa-156">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="814aa-156">extensionAttribute15</span></span>|<span data-ttu-id="814aa-157">String</span><span class="sxs-lookup"><span data-stu-id="814aa-157">String</span></span>| <span data-ttu-id="814aa-158">Пятнадцатый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="814aa-158">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="814aa-159">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="814aa-159">JSON representation</span></span>

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
