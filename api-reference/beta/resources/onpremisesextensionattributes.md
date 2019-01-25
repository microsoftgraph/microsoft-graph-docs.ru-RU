---
title: Тип ресурса onPremisesExtensionAttributes
description: Свойство **onPremisesExtensionAttributes** удостоверение пользователя содержит пятнадцать свойства атрибут настраиваемого расширения. Для пользователя onPremisesSyncEnabled этот набор свойств управляется в локальной службе Active Directory, синхронизирован с Azure AD и доступен только для чтения. Для исключительно облачных пользователей (где значением для onPremisesSyncEnabled является false) эти свойства можно задать при создании или обновлении.
localization_priority: Normal
ms.openlocfilehash: f44f71fdcd86d2165289282568a2d7153ccc99b1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518242"
---
# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="f694f-105">Тип ресурса onPremisesExtensionAttributes</span><span class="sxs-lookup"><span data-stu-id="f694f-105">onPremisesExtensionAttributes resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f694f-106">Свойство **onPremisesExtensionAttributes** удостоверение [пользователя](user.md) содержит пятнадцать свойства атрибут настраиваемого расширения.</span><span class="sxs-lookup"><span data-stu-id="f694f-106">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="f694f-107">Для пользователя onPremisesSyncEnabled этот набор свойств управляется в локальной службе Active Directory, синхронизирован с Azure AD и доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f694f-107">For an **onPremisesSyncEnabled** user, this set of properties is mastered in on-premises Active Directory and synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="f694f-108">Для исключительно облачных пользователей (где значением для onPremisesSyncEnabled является false) эти свойства можно задать при создании или обновлении.</span><span class="sxs-lookup"><span data-stu-id="f694f-108">For a cloud-only user (where **onPremisesSyncEnabled** is false), these properties may be set during creation or update.</span></span>


## <a name="properties"></a><span data-ttu-id="f694f-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="f694f-109">Properties</span></span>
| <span data-ttu-id="f694f-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="f694f-110">Property</span></span>     | <span data-ttu-id="f694f-111">Тип</span><span class="sxs-lookup"><span data-stu-id="f694f-111">Type</span></span>   |<span data-ttu-id="f694f-112">Описание</span><span class="sxs-lookup"><span data-stu-id="f694f-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f694f-113">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="f694f-113">extensionAttribute1</span></span>|<span data-ttu-id="f694f-114">String</span><span class="sxs-lookup"><span data-stu-id="f694f-114">String</span></span>| <span data-ttu-id="f694f-115">Первый атрибут настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="f694f-115">First customizable extension attribute.</span></span> |
|<span data-ttu-id="f694f-116">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="f694f-116">extensionAttribute2</span></span>|<span data-ttu-id="f694f-117">String</span><span class="sxs-lookup"><span data-stu-id="f694f-117">String</span></span>| <span data-ttu-id="f694f-118">Второй атрибут настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="f694f-118">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="f694f-119">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="f694f-119">extensionAttribute3</span></span>|<span data-ttu-id="f694f-120">String</span><span class="sxs-lookup"><span data-stu-id="f694f-120">String</span></span>| <span data-ttu-id="f694f-121">Третий атрибут настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="f694f-121">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="f694f-122">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="f694f-122">extensionAttribute4</span></span>|<span data-ttu-id="f694f-123">String</span><span class="sxs-lookup"><span data-stu-id="f694f-123">String</span></span>| <span data-ttu-id="f694f-124">Четвертая атрибут настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="f694f-124">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="f694f-125">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="f694f-125">extensionAttribute5</span></span>|<span data-ttu-id="f694f-126">String</span><span class="sxs-lookup"><span data-stu-id="f694f-126">String</span></span>| <span data-ttu-id="f694f-127">Атрибут пятый настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="f694f-127">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="f694f-128">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="f694f-128">extensionAttribute6</span></span>|<span data-ttu-id="f694f-129">String</span><span class="sxs-lookup"><span data-stu-id="f694f-129">String</span></span>| <span data-ttu-id="f694f-130">Атрибут шестой настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="f694f-130">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="f694f-131">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="f694f-131">extensionAttribute7</span></span>|<span data-ttu-id="f694f-132">String</span><span class="sxs-lookup"><span data-stu-id="f694f-132">String</span></span>| <span data-ttu-id="f694f-133">Атрибут седьмой настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="f694f-133">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="f694f-134">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="f694f-134">extensionAttribute8</span></span>|<span data-ttu-id="f694f-135">String</span><span class="sxs-lookup"><span data-stu-id="f694f-135">String</span></span>| <span data-ttu-id="f694f-136">Атрибут восьмому настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="f694f-136">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="f694f-137">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="f694f-137">extensionAttribute9</span></span>|<span data-ttu-id="f694f-138">String</span><span class="sxs-lookup"><span data-stu-id="f694f-138">String</span></span>| <span data-ttu-id="f694f-139">Атрибут девятого настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="f694f-139">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="f694f-140">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="f694f-140">extensionAttribute10</span></span>|<span data-ttu-id="f694f-141">String</span><span class="sxs-lookup"><span data-stu-id="f694f-141">String</span></span>| <span data-ttu-id="f694f-142">Десятое атрибут настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="f694f-142">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="f694f-143">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="f694f-143">extensionAttribute11</span></span>|<span data-ttu-id="f694f-144">String</span><span class="sxs-lookup"><span data-stu-id="f694f-144">String</span></span>| <span data-ttu-id="f694f-145">Атрибут eleventh настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="f694f-145">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="f694f-146">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="f694f-146">extensionAttribute12</span></span>|<span data-ttu-id="f694f-147">String</span><span class="sxs-lookup"><span data-stu-id="f694f-147">String</span></span>| <span data-ttu-id="f694f-148">Атрибут twelfth настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="f694f-148">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="f694f-149">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="f694f-149">extensionAttribute13</span></span>|<span data-ttu-id="f694f-150">String</span><span class="sxs-lookup"><span data-stu-id="f694f-150">String</span></span>| <span data-ttu-id="f694f-151">Атрибут thirteenth настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="f694f-151">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="f694f-152">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="f694f-152">extensionAttribute14</span></span>|<span data-ttu-id="f694f-153">String</span><span class="sxs-lookup"><span data-stu-id="f694f-153">String</span></span>| <span data-ttu-id="f694f-154">Атрибут fourteenth настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="f694f-154">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="f694f-155">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="f694f-155">extensionAttribute15</span></span>|<span data-ttu-id="f694f-156">String</span><span class="sxs-lookup"><span data-stu-id="f694f-156">String</span></span>| <span data-ttu-id="f694f-157">Атрибут пятнадцатого настраиваемые расширения.</span><span class="sxs-lookup"><span data-stu-id="f694f-157">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f694f-158">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f694f-158">JSON representation</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/onpremisesextensionattributes.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
