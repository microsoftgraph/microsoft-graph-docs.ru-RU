---
title: Тип ресурса onPremisesExtensionAttributes
description: Свойство **onPremisesExtensionAttributes** удостоверение пользователя содержит пятнадцать свойства атрибут настраиваемого расширения. Для пользователя с **onPremisesSyncEnabled** , этот набор свойств, создаются в локальной службе Active Directory и синхронизируются с Azure AD и доступен только для чтения. Для пользователей только в облаке, (где **onPremisesSyncEnabled** имеет значение false) эти свойства могут быть установлены во время создания или обновления.
ms.openlocfilehash: e5a56b5a846cf48cfc819b6d884689be10d6992e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026640"
---
# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="981d0-105">Тип ресурса onPremisesExtensionAttributes</span><span class="sxs-lookup"><span data-stu-id="981d0-105">onPremisesExtensionAttributes resource type</span></span>

<span data-ttu-id="981d0-106">Свойство **onPremisesExtensionAttributes** удостоверение [пользователя](user.md) содержит пятнадцать свойства атрибут настраиваемого расширения.</span><span class="sxs-lookup"><span data-stu-id="981d0-106">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="981d0-107">Для пользователя с **onPremisesSyncEnabled** , этот набор свойств, создаются в локальной службе Active Directory и синхронизируются с Azure AD и доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="981d0-107">For an **onPremisesSyncEnabled** user, this set of properties is mastered in on-premises Active Directory and synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="981d0-108">Для пользователей только в облаке, (где **onPremisesSyncEnabled** имеет значение false) эти свойства могут быть установлены во время создания или обновления.</span><span class="sxs-lookup"><span data-stu-id="981d0-108">For a cloud-only user (where **onPremisesSyncEnabled** is false), these properties may be set during creation or update.</span></span>


## <a name="properties"></a><span data-ttu-id="981d0-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="981d0-109">Properties</span></span>
| <span data-ttu-id="981d0-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="981d0-110">Property</span></span>     | <span data-ttu-id="981d0-111">Тип</span><span class="sxs-lookup"><span data-stu-id="981d0-111">Type</span></span>   |<span data-ttu-id="981d0-112">Description</span><span class="sxs-lookup"><span data-stu-id="981d0-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="981d0-113">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="981d0-113">extensionAttribute1</span></span>|<span data-ttu-id="981d0-114">String</span><span class="sxs-lookup"><span data-stu-id="981d0-114">String</span></span>| <span data-ttu-id="981d0-115">Первый атрибут настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="981d0-115">First customizable extension attribute.</span></span> |
|<span data-ttu-id="981d0-116">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="981d0-116">extensionAttribute2</span></span>|<span data-ttu-id="981d0-117">String</span><span class="sxs-lookup"><span data-stu-id="981d0-117">String</span></span>| <span data-ttu-id="981d0-118">Второй атрибут настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="981d0-118">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="981d0-119">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="981d0-119">extensionAttribute3</span></span>|<span data-ttu-id="981d0-120">String</span><span class="sxs-lookup"><span data-stu-id="981d0-120">String</span></span>| <span data-ttu-id="981d0-121">Третий атрибут настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="981d0-121">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="981d0-122">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="981d0-122">extensionAttribute4</span></span>|<span data-ttu-id="981d0-123">String</span><span class="sxs-lookup"><span data-stu-id="981d0-123">String</span></span>| <span data-ttu-id="981d0-124">Четвертая атрибут настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="981d0-124">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="981d0-125">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="981d0-125">extensionAttribute5</span></span>|<span data-ttu-id="981d0-126">String</span><span class="sxs-lookup"><span data-stu-id="981d0-126">String</span></span>| <span data-ttu-id="981d0-127">Атрибут пятый настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="981d0-127">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="981d0-128">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="981d0-128">extensionAttribute6</span></span>|<span data-ttu-id="981d0-129">String</span><span class="sxs-lookup"><span data-stu-id="981d0-129">String</span></span>| <span data-ttu-id="981d0-130">Атрибут шестой настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="981d0-130">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="981d0-131">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="981d0-131">extensionAttribute7</span></span>|<span data-ttu-id="981d0-132">String</span><span class="sxs-lookup"><span data-stu-id="981d0-132">String</span></span>| <span data-ttu-id="981d0-133">Атрибут седьмой настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="981d0-133">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="981d0-134">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="981d0-134">extensionAttribute8</span></span>|<span data-ttu-id="981d0-135">String</span><span class="sxs-lookup"><span data-stu-id="981d0-135">String</span></span>| <span data-ttu-id="981d0-136">Атрибут восьмому настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="981d0-136">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="981d0-137">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="981d0-137">extensionAttribute9</span></span>|<span data-ttu-id="981d0-138">String</span><span class="sxs-lookup"><span data-stu-id="981d0-138">String</span></span>| <span data-ttu-id="981d0-139">Атрибут девятого настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="981d0-139">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="981d0-140">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="981d0-140">extensionAttribute10</span></span>|<span data-ttu-id="981d0-141">String</span><span class="sxs-lookup"><span data-stu-id="981d0-141">String</span></span>| <span data-ttu-id="981d0-142">Десятое атрибут настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="981d0-142">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="981d0-143">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="981d0-143">extensionAttribute11</span></span>|<span data-ttu-id="981d0-144">String</span><span class="sxs-lookup"><span data-stu-id="981d0-144">String</span></span>| <span data-ttu-id="981d0-145">Атрибут eleventh настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="981d0-145">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="981d0-146">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="981d0-146">extensionAttribute12</span></span>|<span data-ttu-id="981d0-147">String</span><span class="sxs-lookup"><span data-stu-id="981d0-147">String</span></span>| <span data-ttu-id="981d0-148">Атрибут twelfth настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="981d0-148">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="981d0-149">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="981d0-149">extensionAttribute13</span></span>|<span data-ttu-id="981d0-150">String</span><span class="sxs-lookup"><span data-stu-id="981d0-150">String</span></span>| <span data-ttu-id="981d0-151">Атрибут thirteenth настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="981d0-151">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="981d0-152">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="981d0-152">extensionAttribute14</span></span>|<span data-ttu-id="981d0-153">String</span><span class="sxs-lookup"><span data-stu-id="981d0-153">String</span></span>| <span data-ttu-id="981d0-154">Атрибут fourteenth настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="981d0-154">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="981d0-155">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="981d0-155">extensionAttribute15</span></span>|<span data-ttu-id="981d0-156">String</span><span class="sxs-lookup"><span data-stu-id="981d0-156">String</span></span>| <span data-ttu-id="981d0-157">Атрибут пятнадцатого настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="981d0-157">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="981d0-158">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="981d0-158">JSON representation</span></span>

<span data-ttu-id="981d0-159">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="981d0-159">Here is a JSON representation of the resource</span></span>

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