---
title: Тип ресурса onPremisesExtensionAttributes
description: Свойство **onPremisesExtensionAttributes** удостоверение пользователя содержит пятнадцать свойства атрибут настраиваемого расширения. Для пользователя с **onPremisesSyncEnabled** , этот набор свойств, создаются в локальной службе Active Directory и синхронизируются с Azure AD и доступен только для чтения. Для пользователей только в облаке, (где **onPremisesSyncEnabled** имеет значение false) эти свойства могут быть установлены во время создания или обновления.
localization_priority: Normal
ms.openlocfilehash: c0cb765efe9e94c8254e45eaa9d55bc16382f6d2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824747"
---
# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="aae99-105">Тип ресурса onPremisesExtensionAttributes</span><span class="sxs-lookup"><span data-stu-id="aae99-105">onPremisesExtensionAttributes resource type</span></span>

<span data-ttu-id="aae99-106">Свойство **onPremisesExtensionAttributes** удостоверение [пользователя](user.md) содержит пятнадцать свойства атрибут настраиваемого расширения.</span><span class="sxs-lookup"><span data-stu-id="aae99-106">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="aae99-107">Для пользователя с **onPremisesSyncEnabled** , этот набор свойств, создаются в локальной службе Active Directory и синхронизируются с Azure AD и доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="aae99-107">For an **onPremisesSyncEnabled** user, this set of properties is mastered in on-premises Active Directory and synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="aae99-108">Для пользователей только в облаке, (где **onPremisesSyncEnabled** имеет значение false) эти свойства могут быть установлены во время создания или обновления.</span><span class="sxs-lookup"><span data-stu-id="aae99-108">For a cloud-only user (where **onPremisesSyncEnabled** is false), these properties may be set during creation or update.</span></span>


## <a name="properties"></a><span data-ttu-id="aae99-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="aae99-109">Properties</span></span>
| <span data-ttu-id="aae99-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="aae99-110">Property</span></span>     | <span data-ttu-id="aae99-111">Тип</span><span class="sxs-lookup"><span data-stu-id="aae99-111">Type</span></span>   |<span data-ttu-id="aae99-112">Описание</span><span class="sxs-lookup"><span data-stu-id="aae99-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aae99-113">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="aae99-113">extensionAttribute1</span></span>|<span data-ttu-id="aae99-114">Строка</span><span class="sxs-lookup"><span data-stu-id="aae99-114">String</span></span>| <span data-ttu-id="aae99-115">Первый атрибут настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="aae99-115">First customizable extension attribute.</span></span> |
|<span data-ttu-id="aae99-116">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="aae99-116">extensionAttribute2</span></span>|<span data-ttu-id="aae99-117">Строка</span><span class="sxs-lookup"><span data-stu-id="aae99-117">String</span></span>| <span data-ttu-id="aae99-118">Второй атрибут настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="aae99-118">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="aae99-119">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="aae99-119">extensionAttribute3</span></span>|<span data-ttu-id="aae99-120">Строка</span><span class="sxs-lookup"><span data-stu-id="aae99-120">String</span></span>| <span data-ttu-id="aae99-121">Третий атрибут настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="aae99-121">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="aae99-122">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="aae99-122">extensionAttribute4</span></span>|<span data-ttu-id="aae99-123">Строка</span><span class="sxs-lookup"><span data-stu-id="aae99-123">String</span></span>| <span data-ttu-id="aae99-124">Четвертая атрибут настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="aae99-124">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="aae99-125">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="aae99-125">extensionAttribute5</span></span>|<span data-ttu-id="aae99-126">Строка</span><span class="sxs-lookup"><span data-stu-id="aae99-126">String</span></span>| <span data-ttu-id="aae99-127">Атрибут пятый настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="aae99-127">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="aae99-128">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="aae99-128">extensionAttribute6</span></span>|<span data-ttu-id="aae99-129">Строка</span><span class="sxs-lookup"><span data-stu-id="aae99-129">String</span></span>| <span data-ttu-id="aae99-130">Атрибут шестой настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="aae99-130">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="aae99-131">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="aae99-131">extensionAttribute7</span></span>|<span data-ttu-id="aae99-132">Строка</span><span class="sxs-lookup"><span data-stu-id="aae99-132">String</span></span>| <span data-ttu-id="aae99-133">Атрибут седьмой настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="aae99-133">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="aae99-134">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="aae99-134">extensionAttribute8</span></span>|<span data-ttu-id="aae99-135">Строка</span><span class="sxs-lookup"><span data-stu-id="aae99-135">String</span></span>| <span data-ttu-id="aae99-136">Атрибут восьмому настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="aae99-136">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="aae99-137">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="aae99-137">extensionAttribute9</span></span>|<span data-ttu-id="aae99-138">Строка</span><span class="sxs-lookup"><span data-stu-id="aae99-138">String</span></span>| <span data-ttu-id="aae99-139">Атрибут девятого настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="aae99-139">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="aae99-140">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="aae99-140">extensionAttribute10</span></span>|<span data-ttu-id="aae99-141">Строка</span><span class="sxs-lookup"><span data-stu-id="aae99-141">String</span></span>| <span data-ttu-id="aae99-142">Десятое атрибут настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="aae99-142">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="aae99-143">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="aae99-143">extensionAttribute11</span></span>|<span data-ttu-id="aae99-144">Строка</span><span class="sxs-lookup"><span data-stu-id="aae99-144">String</span></span>| <span data-ttu-id="aae99-145">Атрибут eleventh настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="aae99-145">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="aae99-146">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="aae99-146">extensionAttribute12</span></span>|<span data-ttu-id="aae99-147">Строка</span><span class="sxs-lookup"><span data-stu-id="aae99-147">String</span></span>| <span data-ttu-id="aae99-148">Атрибут twelfth настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="aae99-148">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="aae99-149">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="aae99-149">extensionAttribute13</span></span>|<span data-ttu-id="aae99-150">Строка</span><span class="sxs-lookup"><span data-stu-id="aae99-150">String</span></span>| <span data-ttu-id="aae99-151">Атрибут thirteenth настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="aae99-151">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="aae99-152">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="aae99-152">extensionAttribute14</span></span>|<span data-ttu-id="aae99-153">Строка</span><span class="sxs-lookup"><span data-stu-id="aae99-153">String</span></span>| <span data-ttu-id="aae99-154">Атрибут fourteenth настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="aae99-154">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="aae99-155">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="aae99-155">extensionAttribute15</span></span>|<span data-ttu-id="aae99-156">Строка</span><span class="sxs-lookup"><span data-stu-id="aae99-156">String</span></span>| <span data-ttu-id="aae99-157">Атрибут пятнадцатого настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="aae99-157">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="aae99-158">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aae99-158">JSON representation</span></span>

<span data-ttu-id="aae99-159">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aae99-159">Here is a JSON representation of the resource</span></span>

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
