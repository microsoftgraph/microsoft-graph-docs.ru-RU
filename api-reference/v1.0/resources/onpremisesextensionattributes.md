---
title: Тип ресурса onPremisesExtensionAttributes
description: Свойство **onPremisesExtensionAttributes** объекта пользователя содержит 15 пользовательских свойств атрибута расширения. Для **пользователя onPremisesSyncEnabled** этот набор свойств освоен в локальном Active Directory и синхронизирован с Azure AD и является только для чтения. Для облачного пользователя (где **onPremisesSyncEnabled** является ложным), эти свойства можно Exchange Online. Атрибуты читают только в Microsoft Graph.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 3081b377a30bbf09131650517dcee61597dea597
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912049"
---
# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="b80f6-106">Тип ресурса onPremisesExtensionAttributes</span><span class="sxs-lookup"><span data-stu-id="b80f6-106">onPremisesExtensionAttributes resource type</span></span>

<span data-ttu-id="b80f6-107">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b80f6-107">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b80f6-108">Свойство **onPremisesExtensionAttributes** объекта пользователя содержит [15](user.md) пользовательских свойств атрибута расширения.</span><span class="sxs-lookup"><span data-stu-id="b80f6-108">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="b80f6-109">Для **пользователя onPremisesSyncEnabled** источником полномочий для этого набора свойств является локальное Active Directory, синхронизированное с Azure AD и только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b80f6-109">For an **onPremisesSyncEnabled** user, the source of authority for this set of properties is the on-premises Active Directory which is synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="b80f6-110">Для облачного пользователя (где **находится onPremisesSyncEnabled)** эти свойства можно задать при создании `false` или [обновлении.](../api/user-update.md) [](../api/user-post-users.md)</span><span class="sxs-lookup"><span data-stu-id="b80f6-110">For a cloud-only user (where **onPremisesSyncEnabled** is `false`), these properties may be set during [creation](../api/user-post-users.md) or [update](../api/user-update.md).</span></span>

> <span data-ttu-id="b80f6-111">**Примечание:** Эти атрибуты расширения также известны как Exchange пользовательские атрибуты 1-15.</span><span class="sxs-lookup"><span data-stu-id="b80f6-111">**Note:** These extension attributes are also known as Exchange custom attributes 1-15.</span></span>

## <a name="properties"></a><span data-ttu-id="b80f6-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="b80f6-112">Properties</span></span>
| <span data-ttu-id="b80f6-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="b80f6-113">Property</span></span>     | <span data-ttu-id="b80f6-114">Тип</span><span class="sxs-lookup"><span data-stu-id="b80f6-114">Type</span></span>   |<span data-ttu-id="b80f6-115">Описание</span><span class="sxs-lookup"><span data-stu-id="b80f6-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b80f6-116">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="b80f6-116">extensionAttribute1</span></span>|<span data-ttu-id="b80f6-117">String</span><span class="sxs-lookup"><span data-stu-id="b80f6-117">String</span></span>| <span data-ttu-id="b80f6-118">Первый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="b80f6-118">First customizable extension attribute.</span></span> |
|<span data-ttu-id="b80f6-119">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="b80f6-119">extensionAttribute2</span></span>|<span data-ttu-id="b80f6-120">String</span><span class="sxs-lookup"><span data-stu-id="b80f6-120">String</span></span>| <span data-ttu-id="b80f6-121">Второй настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="b80f6-121">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="b80f6-122">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="b80f6-122">extensionAttribute3</span></span>|<span data-ttu-id="b80f6-123">String</span><span class="sxs-lookup"><span data-stu-id="b80f6-123">String</span></span>| <span data-ttu-id="b80f6-124">Третий настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="b80f6-124">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="b80f6-125">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="b80f6-125">extensionAttribute4</span></span>|<span data-ttu-id="b80f6-126">String</span><span class="sxs-lookup"><span data-stu-id="b80f6-126">String</span></span>| <span data-ttu-id="b80f6-127">Четвертый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="b80f6-127">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="b80f6-128">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="b80f6-128">extensionAttribute5</span></span>|<span data-ttu-id="b80f6-129">String</span><span class="sxs-lookup"><span data-stu-id="b80f6-129">String</span></span>| <span data-ttu-id="b80f6-130">Пятый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="b80f6-130">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="b80f6-131">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="b80f6-131">extensionAttribute6</span></span>|<span data-ttu-id="b80f6-132">String</span><span class="sxs-lookup"><span data-stu-id="b80f6-132">String</span></span>| <span data-ttu-id="b80f6-133">Шестой настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="b80f6-133">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="b80f6-134">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="b80f6-134">extensionAttribute7</span></span>|<span data-ttu-id="b80f6-135">String</span><span class="sxs-lookup"><span data-stu-id="b80f6-135">String</span></span>| <span data-ttu-id="b80f6-136">Седьмой настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="b80f6-136">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="b80f6-137">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="b80f6-137">extensionAttribute8</span></span>|<span data-ttu-id="b80f6-138">String</span><span class="sxs-lookup"><span data-stu-id="b80f6-138">String</span></span>| <span data-ttu-id="b80f6-139">Восьмой настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="b80f6-139">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="b80f6-140">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="b80f6-140">extensionAttribute9</span></span>|<span data-ttu-id="b80f6-141">String</span><span class="sxs-lookup"><span data-stu-id="b80f6-141">String</span></span>| <span data-ttu-id="b80f6-142">Девятый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="b80f6-142">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="b80f6-143">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="b80f6-143">extensionAttribute10</span></span>|<span data-ttu-id="b80f6-144">String</span><span class="sxs-lookup"><span data-stu-id="b80f6-144">String</span></span>| <span data-ttu-id="b80f6-145">Десятый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="b80f6-145">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="b80f6-146">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="b80f6-146">extensionAttribute11</span></span>|<span data-ttu-id="b80f6-147">String</span><span class="sxs-lookup"><span data-stu-id="b80f6-147">String</span></span>| <span data-ttu-id="b80f6-148">Одиннадцатый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="b80f6-148">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="b80f6-149">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="b80f6-149">extensionAttribute12</span></span>|<span data-ttu-id="b80f6-150">String</span><span class="sxs-lookup"><span data-stu-id="b80f6-150">String</span></span>| <span data-ttu-id="b80f6-151">Двенадцатый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="b80f6-151">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="b80f6-152">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="b80f6-152">extensionAttribute13</span></span>|<span data-ttu-id="b80f6-153">String</span><span class="sxs-lookup"><span data-stu-id="b80f6-153">String</span></span>| <span data-ttu-id="b80f6-154">Тринадцатый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="b80f6-154">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="b80f6-155">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="b80f6-155">extensionAttribute14</span></span>|<span data-ttu-id="b80f6-156">String</span><span class="sxs-lookup"><span data-stu-id="b80f6-156">String</span></span>| <span data-ttu-id="b80f6-157">Четырнадцатый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="b80f6-157">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="b80f6-158">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="b80f6-158">extensionAttribute15</span></span>|<span data-ttu-id="b80f6-159">String</span><span class="sxs-lookup"><span data-stu-id="b80f6-159">String</span></span>| <span data-ttu-id="b80f6-160">Пятнадцатый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="b80f6-160">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b80f6-161">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b80f6-161">JSON representation</span></span>

<span data-ttu-id="b80f6-162">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b80f6-162">Here is a JSON representation of the resource</span></span>

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

