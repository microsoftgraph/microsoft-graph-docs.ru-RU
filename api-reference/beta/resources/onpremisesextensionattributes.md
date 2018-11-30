---
title: Тип ресурса onPremisesExtensionAttributes
description: Свойство **onPremisesExtensionAttributes** удостоверение пользователя содержит пятнадцать свойства атрибут настраиваемого расширения. Для пользователя с **onPremisesSyncEnabled** , этот набор свойств, создаются в локальной службе Active Directory и синхронизируются с Azure AD и доступен только для чтения. Для пользователей только в облаке, (где **onPremisesSyncEnabled** имеет значение false) эти свойства могут быть установлены во время создания или обновления.
ms.openlocfilehash: 547fc8ac19059611f5983a8b5ee0bd905f130f79
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080303"
---
# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="ad205-105">Тип ресурса onPremisesExtensionAttributes</span><span class="sxs-lookup"><span data-stu-id="ad205-105">onPremisesExtensionAttributes resource type</span></span>

> <span data-ttu-id="ad205-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ad205-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ad205-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad205-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ad205-108">Свойство **onPremisesExtensionAttributes** удостоверение [пользователя](user.md) содержит пятнадцать свойства атрибут настраиваемого расширения.</span><span class="sxs-lookup"><span data-stu-id="ad205-108">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="ad205-109">Для пользователя с **onPremisesSyncEnabled** , этот набор свойств, создаются в локальной службе Active Directory и синхронизируются с Azure AD и доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ad205-109">For an **onPremisesSyncEnabled** user, this set of properties is mastered in on-premises Active Directory and synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="ad205-110">Для пользователей только в облаке, (где **onPremisesSyncEnabled** имеет значение false) эти свойства могут быть установлены во время создания или обновления.</span><span class="sxs-lookup"><span data-stu-id="ad205-110">For a cloud-only user (where **onPremisesSyncEnabled** is false), these properties may be set during creation or update.</span></span>


## <a name="properties"></a><span data-ttu-id="ad205-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="ad205-111">Properties</span></span>
| <span data-ttu-id="ad205-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="ad205-112">Property</span></span>     | <span data-ttu-id="ad205-113">Тип</span><span class="sxs-lookup"><span data-stu-id="ad205-113">Type</span></span>   |<span data-ttu-id="ad205-114">Description</span><span class="sxs-lookup"><span data-stu-id="ad205-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ad205-115">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="ad205-115">extensionAttribute1</span></span>|<span data-ttu-id="ad205-116">String</span><span class="sxs-lookup"><span data-stu-id="ad205-116">String</span></span>| <span data-ttu-id="ad205-117">Первый атрибут настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="ad205-117">First customizable extension attribute.</span></span> |
|<span data-ttu-id="ad205-118">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="ad205-118">extensionAttribute2</span></span>|<span data-ttu-id="ad205-119">String</span><span class="sxs-lookup"><span data-stu-id="ad205-119">String</span></span>| <span data-ttu-id="ad205-120">Второй атрибут настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="ad205-120">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="ad205-121">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="ad205-121">extensionAttribute3</span></span>|<span data-ttu-id="ad205-122">String</span><span class="sxs-lookup"><span data-stu-id="ad205-122">String</span></span>| <span data-ttu-id="ad205-123">Третий атрибут настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="ad205-123">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="ad205-124">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="ad205-124">extensionAttribute4</span></span>|<span data-ttu-id="ad205-125">String</span><span class="sxs-lookup"><span data-stu-id="ad205-125">String</span></span>| <span data-ttu-id="ad205-126">Четвертая атрибут настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="ad205-126">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="ad205-127">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="ad205-127">extensionAttribute5</span></span>|<span data-ttu-id="ad205-128">String</span><span class="sxs-lookup"><span data-stu-id="ad205-128">String</span></span>| <span data-ttu-id="ad205-129">Атрибут пятый настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="ad205-129">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="ad205-130">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="ad205-130">extensionAttribute6</span></span>|<span data-ttu-id="ad205-131">String</span><span class="sxs-lookup"><span data-stu-id="ad205-131">String</span></span>| <span data-ttu-id="ad205-132">Атрибут шестой настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="ad205-132">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="ad205-133">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="ad205-133">extensionAttribute7</span></span>|<span data-ttu-id="ad205-134">String</span><span class="sxs-lookup"><span data-stu-id="ad205-134">String</span></span>| <span data-ttu-id="ad205-135">Атрибут седьмой настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="ad205-135">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="ad205-136">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="ad205-136">extensionAttribute8</span></span>|<span data-ttu-id="ad205-137">String</span><span class="sxs-lookup"><span data-stu-id="ad205-137">String</span></span>| <span data-ttu-id="ad205-138">Атрибут восьмому настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="ad205-138">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="ad205-139">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="ad205-139">extensionAttribute9</span></span>|<span data-ttu-id="ad205-140">String</span><span class="sxs-lookup"><span data-stu-id="ad205-140">String</span></span>| <span data-ttu-id="ad205-141">Атрибут девятого настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="ad205-141">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="ad205-142">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="ad205-142">extensionAttribute10</span></span>|<span data-ttu-id="ad205-143">String</span><span class="sxs-lookup"><span data-stu-id="ad205-143">String</span></span>| <span data-ttu-id="ad205-144">Десятое атрибут настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="ad205-144">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="ad205-145">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="ad205-145">extensionAttribute11</span></span>|<span data-ttu-id="ad205-146">String</span><span class="sxs-lookup"><span data-stu-id="ad205-146">String</span></span>| <span data-ttu-id="ad205-147">Атрибут eleventh настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="ad205-147">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="ad205-148">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="ad205-148">extensionAttribute12</span></span>|<span data-ttu-id="ad205-149">String</span><span class="sxs-lookup"><span data-stu-id="ad205-149">String</span></span>| <span data-ttu-id="ad205-150">Атрибут twelfth настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="ad205-150">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="ad205-151">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="ad205-151">extensionAttribute13</span></span>|<span data-ttu-id="ad205-152">String</span><span class="sxs-lookup"><span data-stu-id="ad205-152">String</span></span>| <span data-ttu-id="ad205-153">Атрибут thirteenth настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="ad205-153">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="ad205-154">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="ad205-154">extensionAttribute14</span></span>|<span data-ttu-id="ad205-155">String</span><span class="sxs-lookup"><span data-stu-id="ad205-155">String</span></span>| <span data-ttu-id="ad205-156">Атрибут fourteenth настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="ad205-156">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="ad205-157">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="ad205-157">extensionAttribute15</span></span>|<span data-ttu-id="ad205-158">String</span><span class="sxs-lookup"><span data-stu-id="ad205-158">String</span></span>| <span data-ttu-id="ad205-159">Атрибут пятнадцатого настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="ad205-159">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ad205-160">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ad205-160">JSON representation</span></span>

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