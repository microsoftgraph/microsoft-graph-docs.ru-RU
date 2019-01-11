---
title: Тип ресурса onPremisesExtensionAttributes
description: Свойство **onPremisesExtensionAttributes** удостоверение пользователя содержит пятнадцать свойства атрибут настраиваемого расширения. Для пользователя с **onPremisesSyncEnabled** , этот набор свойств, создаются в локальной службе Active Directory и синхронизируются с Azure AD и доступен только для чтения. Для пользователей только в облаке, (где **onPremisesSyncEnabled** имеет значение false) эти свойства могут быть установлены во время создания или обновления.
localization_priority: Normal
ms.openlocfilehash: 44589338e25e01cb483df6bfa3c1e078e352f5ed
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868161"
---
# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="d490d-105">Тип ресурса onPremisesExtensionAttributes</span><span class="sxs-lookup"><span data-stu-id="d490d-105">onPremisesExtensionAttributes resource type</span></span>

> <span data-ttu-id="d490d-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d490d-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d490d-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d490d-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d490d-108">Свойство **onPremisesExtensionAttributes** удостоверение [пользователя](user.md) содержит пятнадцать свойства атрибут настраиваемого расширения.</span><span class="sxs-lookup"><span data-stu-id="d490d-108">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="d490d-109">Для пользователя с **onPremisesSyncEnabled** , этот набор свойств, создаются в локальной службе Active Directory и синхронизируются с Azure AD и доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d490d-109">For an **onPremisesSyncEnabled** user, this set of properties is mastered in on-premises Active Directory and synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="d490d-110">Для пользователей только в облаке, (где **onPremisesSyncEnabled** имеет значение false) эти свойства могут быть установлены во время создания или обновления.</span><span class="sxs-lookup"><span data-stu-id="d490d-110">For a cloud-only user (where **onPremisesSyncEnabled** is false), these properties may be set during creation or update.</span></span>


## <a name="properties"></a><span data-ttu-id="d490d-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="d490d-111">Properties</span></span>
| <span data-ttu-id="d490d-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="d490d-112">Property</span></span>     | <span data-ttu-id="d490d-113">Тип</span><span class="sxs-lookup"><span data-stu-id="d490d-113">Type</span></span>   |<span data-ttu-id="d490d-114">Описание</span><span class="sxs-lookup"><span data-stu-id="d490d-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d490d-115">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="d490d-115">extensionAttribute1</span></span>|<span data-ttu-id="d490d-116">Строка</span><span class="sxs-lookup"><span data-stu-id="d490d-116">String</span></span>| <span data-ttu-id="d490d-117">Первый атрибут настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="d490d-117">First customizable extension attribute.</span></span> |
|<span data-ttu-id="d490d-118">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="d490d-118">extensionAttribute2</span></span>|<span data-ttu-id="d490d-119">Строка</span><span class="sxs-lookup"><span data-stu-id="d490d-119">String</span></span>| <span data-ttu-id="d490d-120">Второй атрибут настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="d490d-120">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="d490d-121">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="d490d-121">extensionAttribute3</span></span>|<span data-ttu-id="d490d-122">Строка</span><span class="sxs-lookup"><span data-stu-id="d490d-122">String</span></span>| <span data-ttu-id="d490d-123">Третий атрибут настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="d490d-123">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="d490d-124">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="d490d-124">extensionAttribute4</span></span>|<span data-ttu-id="d490d-125">Строка</span><span class="sxs-lookup"><span data-stu-id="d490d-125">String</span></span>| <span data-ttu-id="d490d-126">Четвертая атрибут настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="d490d-126">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="d490d-127">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="d490d-127">extensionAttribute5</span></span>|<span data-ttu-id="d490d-128">Строка</span><span class="sxs-lookup"><span data-stu-id="d490d-128">String</span></span>| <span data-ttu-id="d490d-129">Атрибут пятый настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="d490d-129">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="d490d-130">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="d490d-130">extensionAttribute6</span></span>|<span data-ttu-id="d490d-131">Строка</span><span class="sxs-lookup"><span data-stu-id="d490d-131">String</span></span>| <span data-ttu-id="d490d-132">Атрибут шестой настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="d490d-132">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="d490d-133">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="d490d-133">extensionAttribute7</span></span>|<span data-ttu-id="d490d-134">Строка</span><span class="sxs-lookup"><span data-stu-id="d490d-134">String</span></span>| <span data-ttu-id="d490d-135">Атрибут седьмой настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="d490d-135">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="d490d-136">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="d490d-136">extensionAttribute8</span></span>|<span data-ttu-id="d490d-137">Строка</span><span class="sxs-lookup"><span data-stu-id="d490d-137">String</span></span>| <span data-ttu-id="d490d-138">Атрибут восьмому настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="d490d-138">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="d490d-139">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="d490d-139">extensionAttribute9</span></span>|<span data-ttu-id="d490d-140">Строка</span><span class="sxs-lookup"><span data-stu-id="d490d-140">String</span></span>| <span data-ttu-id="d490d-141">Атрибут девятого настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="d490d-141">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="d490d-142">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="d490d-142">extensionAttribute10</span></span>|<span data-ttu-id="d490d-143">Строка</span><span class="sxs-lookup"><span data-stu-id="d490d-143">String</span></span>| <span data-ttu-id="d490d-144">Десятое атрибут настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="d490d-144">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="d490d-145">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="d490d-145">extensionAttribute11</span></span>|<span data-ttu-id="d490d-146">Строка</span><span class="sxs-lookup"><span data-stu-id="d490d-146">String</span></span>| <span data-ttu-id="d490d-147">Атрибут eleventh настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="d490d-147">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="d490d-148">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="d490d-148">extensionAttribute12</span></span>|<span data-ttu-id="d490d-149">Строка</span><span class="sxs-lookup"><span data-stu-id="d490d-149">String</span></span>| <span data-ttu-id="d490d-150">Атрибут twelfth настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="d490d-150">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="d490d-151">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="d490d-151">extensionAttribute13</span></span>|<span data-ttu-id="d490d-152">Строка</span><span class="sxs-lookup"><span data-stu-id="d490d-152">String</span></span>| <span data-ttu-id="d490d-153">Атрибут thirteenth настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="d490d-153">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="d490d-154">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="d490d-154">extensionAttribute14</span></span>|<span data-ttu-id="d490d-155">Строка</span><span class="sxs-lookup"><span data-stu-id="d490d-155">String</span></span>| <span data-ttu-id="d490d-156">Атрибут fourteenth настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="d490d-156">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="d490d-157">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="d490d-157">extensionAttribute15</span></span>|<span data-ttu-id="d490d-158">Строка</span><span class="sxs-lookup"><span data-stu-id="d490d-158">String</span></span>| <span data-ttu-id="d490d-159">Атрибут пятнадцатого настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="d490d-159">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d490d-160">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d490d-160">JSON representation</span></span>

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
