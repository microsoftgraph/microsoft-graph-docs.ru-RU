---
title: Тип ресурса onPremisesExtensionAttributes
description: Свойство **onPremisesExtensionAttributes** объекта пользователя содержит 15 пользовательских свойств атрибута расширения.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: users
author: jpettere
ms.openlocfilehash: 902ebfa8efe11613d6622d93ec0d39becc9e9bae
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912105"
---
# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="53522-103">Тип ресурса onPremisesExtensionAttributes</span><span class="sxs-lookup"><span data-stu-id="53522-103">onPremisesExtensionAttributes resource type</span></span>

<span data-ttu-id="53522-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53522-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53522-105">Свойство **onPremisesExtensionAttributes** объекта пользователя содержит [15](user.md) пользовательских свойств атрибута расширения.</span><span class="sxs-lookup"><span data-stu-id="53522-105">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="53522-106">Для **пользователя onPremisesSyncEnabled** источником полномочий для этого набора свойств является локальное Active Directory, синхронизированное с Azure AD и только для чтения.</span><span class="sxs-lookup"><span data-stu-id="53522-106">For an **onPremisesSyncEnabled** user, the source of authority for this set of properties is the on-premises Active Directory which is synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="53522-107">Для облачного пользователя (где **находится onPremisesSyncEnabled)** эти свойства можно задать при создании `false` или [обновлении.](../api/user-update.md) [](../api/user-post-users.md)</span><span class="sxs-lookup"><span data-stu-id="53522-107">For a cloud-only user (where **onPremisesSyncEnabled** is `false`), these properties may be set during [creation](../api/user-post-users.md) or [update](../api/user-update.md).</span></span>

> <span data-ttu-id="53522-108">**Примечание:** Эти атрибуты расширения также известны как Exchange пользовательские атрибуты 1-15.</span><span class="sxs-lookup"><span data-stu-id="53522-108">**Note:** These extension attributes are also known as Exchange custom attributes 1-15.</span></span>


## <a name="properties"></a><span data-ttu-id="53522-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="53522-109">Properties</span></span>
| <span data-ttu-id="53522-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="53522-110">Property</span></span>     | <span data-ttu-id="53522-111">Тип</span><span class="sxs-lookup"><span data-stu-id="53522-111">Type</span></span>   |<span data-ttu-id="53522-112">Описание</span><span class="sxs-lookup"><span data-stu-id="53522-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="53522-113">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="53522-113">extensionAttribute1</span></span>|<span data-ttu-id="53522-114">String</span><span class="sxs-lookup"><span data-stu-id="53522-114">String</span></span>| <span data-ttu-id="53522-115">Первый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="53522-115">First customizable extension attribute.</span></span> |
|<span data-ttu-id="53522-116">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="53522-116">extensionAttribute2</span></span>|<span data-ttu-id="53522-117">String</span><span class="sxs-lookup"><span data-stu-id="53522-117">String</span></span>| <span data-ttu-id="53522-118">Второй настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="53522-118">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="53522-119">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="53522-119">extensionAttribute3</span></span>|<span data-ttu-id="53522-120">String</span><span class="sxs-lookup"><span data-stu-id="53522-120">String</span></span>| <span data-ttu-id="53522-121">Третий настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="53522-121">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="53522-122">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="53522-122">extensionAttribute4</span></span>|<span data-ttu-id="53522-123">String</span><span class="sxs-lookup"><span data-stu-id="53522-123">String</span></span>| <span data-ttu-id="53522-124">Четвертый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="53522-124">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="53522-125">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="53522-125">extensionAttribute5</span></span>|<span data-ttu-id="53522-126">String</span><span class="sxs-lookup"><span data-stu-id="53522-126">String</span></span>| <span data-ttu-id="53522-127">Пятый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="53522-127">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="53522-128">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="53522-128">extensionAttribute6</span></span>|<span data-ttu-id="53522-129">String</span><span class="sxs-lookup"><span data-stu-id="53522-129">String</span></span>| <span data-ttu-id="53522-130">Шестой настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="53522-130">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="53522-131">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="53522-131">extensionAttribute7</span></span>|<span data-ttu-id="53522-132">String</span><span class="sxs-lookup"><span data-stu-id="53522-132">String</span></span>| <span data-ttu-id="53522-133">Седьмой настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="53522-133">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="53522-134">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="53522-134">extensionAttribute8</span></span>|<span data-ttu-id="53522-135">String</span><span class="sxs-lookup"><span data-stu-id="53522-135">String</span></span>| <span data-ttu-id="53522-136">Восьмой настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="53522-136">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="53522-137">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="53522-137">extensionAttribute9</span></span>|<span data-ttu-id="53522-138">String</span><span class="sxs-lookup"><span data-stu-id="53522-138">String</span></span>| <span data-ttu-id="53522-139">Девятый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="53522-139">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="53522-140">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="53522-140">extensionAttribute10</span></span>|<span data-ttu-id="53522-141">String</span><span class="sxs-lookup"><span data-stu-id="53522-141">String</span></span>| <span data-ttu-id="53522-142">Десятый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="53522-142">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="53522-143">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="53522-143">extensionAttribute11</span></span>|<span data-ttu-id="53522-144">String</span><span class="sxs-lookup"><span data-stu-id="53522-144">String</span></span>| <span data-ttu-id="53522-145">Одиннадцатый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="53522-145">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="53522-146">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="53522-146">extensionAttribute12</span></span>|<span data-ttu-id="53522-147">String</span><span class="sxs-lookup"><span data-stu-id="53522-147">String</span></span>| <span data-ttu-id="53522-148">Двенадцатый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="53522-148">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="53522-149">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="53522-149">extensionAttribute13</span></span>|<span data-ttu-id="53522-150">String</span><span class="sxs-lookup"><span data-stu-id="53522-150">String</span></span>| <span data-ttu-id="53522-151">Тринадцатый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="53522-151">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="53522-152">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="53522-152">extensionAttribute14</span></span>|<span data-ttu-id="53522-153">String</span><span class="sxs-lookup"><span data-stu-id="53522-153">String</span></span>| <span data-ttu-id="53522-154">Четырнадцатый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="53522-154">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="53522-155">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="53522-155">extensionAttribute15</span></span>|<span data-ttu-id="53522-156">String</span><span class="sxs-lookup"><span data-stu-id="53522-156">String</span></span>| <span data-ttu-id="53522-157">Пятнадцатый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="53522-157">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="53522-158">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="53522-158">JSON representation</span></span>

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


