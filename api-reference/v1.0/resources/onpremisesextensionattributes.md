---
title: Тип ресурса onPremisesExtensionAttributes
description: Свойство **onPremisesExtensionAttributes** объекта user содержит пятнадцать свойств настраиваемого атрибута расширения. Для пользователя **onPremisesSyncEnabled** этот набор свойств размещается в локальной службе Active Directory и синхронизируется с Azure AD и доступен только для чтения. Для пользователя, предназначенного только для облачного облака (где **onPremisesSyncEnabled** имеет значение false), эти свойства можно задать при создании или обновлении.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f6c80e5ee55409545f744556390a515125aee394
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447299"
---
# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="5196a-105">Тип ресурса onPremisesExtensionAttributes</span><span class="sxs-lookup"><span data-stu-id="5196a-105">onPremisesExtensionAttributes resource type</span></span>

<span data-ttu-id="5196a-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5196a-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5196a-107">Свойство **onPremisesExtensionAttributes** объекта [User](user.md) содержит пятнадцать свойств настраиваемого атрибута расширения.</span><span class="sxs-lookup"><span data-stu-id="5196a-107">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="5196a-108">Для пользователя **onPremisesSyncEnabled** этот набор свойств размещается в локальной службе Active Directory и синхронизируется с Azure AD и доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5196a-108">For an **onPremisesSyncEnabled** user, this set of properties is mastered in on-premises Active Directory and synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="5196a-109">Для пользователя, предназначенного только для облачного облака (где **onPremisesSyncEnabled** имеет значение false), эти свойства можно задать при создании или обновлении.</span><span class="sxs-lookup"><span data-stu-id="5196a-109">For a cloud-only user (where **onPremisesSyncEnabled** is false), these properties may be set during creation or update.</span></span>


## <a name="properties"></a><span data-ttu-id="5196a-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="5196a-110">Properties</span></span>
| <span data-ttu-id="5196a-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="5196a-111">Property</span></span>     | <span data-ttu-id="5196a-112">Тип</span><span class="sxs-lookup"><span data-stu-id="5196a-112">Type</span></span>   |<span data-ttu-id="5196a-113">Описание</span><span class="sxs-lookup"><span data-stu-id="5196a-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5196a-114">От extensionattribute1</span><span class="sxs-lookup"><span data-stu-id="5196a-114">extensionAttribute1</span></span>|<span data-ttu-id="5196a-115">String</span><span class="sxs-lookup"><span data-stu-id="5196a-115">String</span></span>| <span data-ttu-id="5196a-116">Первый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="5196a-116">First customizable extension attribute.</span></span> |
|<span data-ttu-id="5196a-117">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="5196a-117">extensionAttribute2</span></span>|<span data-ttu-id="5196a-118">String</span><span class="sxs-lookup"><span data-stu-id="5196a-118">String</span></span>| <span data-ttu-id="5196a-119">Второй настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="5196a-119">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="5196a-120">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="5196a-120">extensionAttribute3</span></span>|<span data-ttu-id="5196a-121">String</span><span class="sxs-lookup"><span data-stu-id="5196a-121">String</span></span>| <span data-ttu-id="5196a-122">Третий настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="5196a-122">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="5196a-123">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="5196a-123">extensionAttribute4</span></span>|<span data-ttu-id="5196a-124">String</span><span class="sxs-lookup"><span data-stu-id="5196a-124">String</span></span>| <span data-ttu-id="5196a-125">Четвертый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="5196a-125">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="5196a-126">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="5196a-126">extensionAttribute5</span></span>|<span data-ttu-id="5196a-127">String</span><span class="sxs-lookup"><span data-stu-id="5196a-127">String</span></span>| <span data-ttu-id="5196a-128">Пятый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="5196a-128">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="5196a-129">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="5196a-129">extensionAttribute6</span></span>|<span data-ttu-id="5196a-130">String</span><span class="sxs-lookup"><span data-stu-id="5196a-130">String</span></span>| <span data-ttu-id="5196a-131">Шестой настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="5196a-131">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="5196a-132">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="5196a-132">extensionAttribute7</span></span>|<span data-ttu-id="5196a-133">String</span><span class="sxs-lookup"><span data-stu-id="5196a-133">String</span></span>| <span data-ttu-id="5196a-134">Седьмой настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="5196a-134">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="5196a-135">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="5196a-135">extensionAttribute8</span></span>|<span data-ttu-id="5196a-136">String</span><span class="sxs-lookup"><span data-stu-id="5196a-136">String</span></span>| <span data-ttu-id="5196a-137">Восьмой настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="5196a-137">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="5196a-138">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="5196a-138">extensionAttribute9</span></span>|<span data-ttu-id="5196a-139">String</span><span class="sxs-lookup"><span data-stu-id="5196a-139">String</span></span>| <span data-ttu-id="5196a-140">Девятый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="5196a-140">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="5196a-141">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="5196a-141">extensionAttribute10</span></span>|<span data-ttu-id="5196a-142">String</span><span class="sxs-lookup"><span data-stu-id="5196a-142">String</span></span>| <span data-ttu-id="5196a-143">Десятый атрибут расширенной настройки.</span><span class="sxs-lookup"><span data-stu-id="5196a-143">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="5196a-144">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="5196a-144">extensionAttribute11</span></span>|<span data-ttu-id="5196a-145">String</span><span class="sxs-lookup"><span data-stu-id="5196a-145">String</span></span>| <span data-ttu-id="5196a-146">Одиннадцатый атрибут настраиваемого расширения.</span><span class="sxs-lookup"><span data-stu-id="5196a-146">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="5196a-147">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="5196a-147">extensionAttribute12</span></span>|<span data-ttu-id="5196a-148">String</span><span class="sxs-lookup"><span data-stu-id="5196a-148">String</span></span>| <span data-ttu-id="5196a-149">Двенадцатый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="5196a-149">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="5196a-150">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="5196a-150">extensionAttribute13</span></span>|<span data-ttu-id="5196a-151">String</span><span class="sxs-lookup"><span data-stu-id="5196a-151">String</span></span>| <span data-ttu-id="5196a-152">Настраиваемый атрибут расширения сиртинс.</span><span class="sxs-lookup"><span data-stu-id="5196a-152">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="5196a-153">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="5196a-153">extensionAttribute14</span></span>|<span data-ttu-id="5196a-154">String</span><span class="sxs-lookup"><span data-stu-id="5196a-154">String</span></span>| <span data-ttu-id="5196a-155">Настраиваемый атрибут расширения фауртинс.</span><span class="sxs-lookup"><span data-stu-id="5196a-155">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="5196a-156">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="5196a-156">extensionAttribute15</span></span>|<span data-ttu-id="5196a-157">String</span><span class="sxs-lookup"><span data-stu-id="5196a-157">String</span></span>| <span data-ttu-id="5196a-158">Пятнадцатый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="5196a-158">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5196a-159">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5196a-159">JSON representation</span></span>

<span data-ttu-id="5196a-160">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5196a-160">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesExtensionAttributes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
