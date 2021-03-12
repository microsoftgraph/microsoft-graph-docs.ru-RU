---
title: Тип ресурса onPremisesExtensionAttributes
description: Свойство **onPremisesExtensionAttributes** объекта пользователя содержит 15 пользовательских свойств атрибута расширения. Для **пользователя onPremisesSyncEnabled** этот набор свойств освоен в локальном Active Directory и синхронизирован с Azure AD и является только для чтения. Для облачного пользователя (где **onPremisesSyncEnabled** является ложным), эти свойства могут быть заданы во время создания или обновления.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: c8e44879b3248cab502ee2aeabdaa732a2b35e1f
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50718959"
---
# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="7ec69-105">Тип ресурса onPremisesExtensionAttributes</span><span class="sxs-lookup"><span data-stu-id="7ec69-105">onPremisesExtensionAttributes resource type</span></span>

<span data-ttu-id="7ec69-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ec69-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7ec69-107">Свойство **onPremisesExtensionAttributes** объекта пользователя содержит [15](user.md) пользовательских свойств атрибута расширения.</span><span class="sxs-lookup"><span data-stu-id="7ec69-107">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="7ec69-108">Для **пользователя onPremisesSyncEnabled** источником полномочий для этого набора свойств является локальное Active Directory, синхронизированное с Azure AD и только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7ec69-108">For an **onPremisesSyncEnabled** user, the source of authority for this set of properties is the on-premises Active Directory which is synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="7ec69-109">Для облачного пользователя (где **onPremisesSyncEnabled** является ложным), эти свойства могут быть заданы во время создания или обновления.</span><span class="sxs-lookup"><span data-stu-id="7ec69-109">For a cloud-only user (where **onPremisesSyncEnabled** is false), these properties may be set during creation or update.</span></span>

> <span data-ttu-id="7ec69-110">**Примечание:** Эти атрибуты расширения также известны как пользовательские атрибуты Exchange 1-15.</span><span class="sxs-lookup"><span data-stu-id="7ec69-110">**Note:** These extension attributes are also known as Exchange custom attributes 1-15.</span></span>

## <a name="properties"></a><span data-ttu-id="7ec69-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="7ec69-111">Properties</span></span>
| <span data-ttu-id="7ec69-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="7ec69-112">Property</span></span>     | <span data-ttu-id="7ec69-113">Тип</span><span class="sxs-lookup"><span data-stu-id="7ec69-113">Type</span></span>   |<span data-ttu-id="7ec69-114">Описание</span><span class="sxs-lookup"><span data-stu-id="7ec69-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7ec69-115">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="7ec69-115">extensionAttribute1</span></span>|<span data-ttu-id="7ec69-116">String</span><span class="sxs-lookup"><span data-stu-id="7ec69-116">String</span></span>| <span data-ttu-id="7ec69-117">Первый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="7ec69-117">First customizable extension attribute.</span></span> |
|<span data-ttu-id="7ec69-118">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="7ec69-118">extensionAttribute2</span></span>|<span data-ttu-id="7ec69-119">String</span><span class="sxs-lookup"><span data-stu-id="7ec69-119">String</span></span>| <span data-ttu-id="7ec69-120">Второй настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="7ec69-120">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="7ec69-121">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="7ec69-121">extensionAttribute3</span></span>|<span data-ttu-id="7ec69-122">String</span><span class="sxs-lookup"><span data-stu-id="7ec69-122">String</span></span>| <span data-ttu-id="7ec69-123">Третий настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="7ec69-123">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="7ec69-124">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="7ec69-124">extensionAttribute4</span></span>|<span data-ttu-id="7ec69-125">String</span><span class="sxs-lookup"><span data-stu-id="7ec69-125">String</span></span>| <span data-ttu-id="7ec69-126">Четвертый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="7ec69-126">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="7ec69-127">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="7ec69-127">extensionAttribute5</span></span>|<span data-ttu-id="7ec69-128">String</span><span class="sxs-lookup"><span data-stu-id="7ec69-128">String</span></span>| <span data-ttu-id="7ec69-129">Пятый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="7ec69-129">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="7ec69-130">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="7ec69-130">extensionAttribute6</span></span>|<span data-ttu-id="7ec69-131">String</span><span class="sxs-lookup"><span data-stu-id="7ec69-131">String</span></span>| <span data-ttu-id="7ec69-132">Шестой настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="7ec69-132">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="7ec69-133">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="7ec69-133">extensionAttribute7</span></span>|<span data-ttu-id="7ec69-134">String</span><span class="sxs-lookup"><span data-stu-id="7ec69-134">String</span></span>| <span data-ttu-id="7ec69-135">Седьмой настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="7ec69-135">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="7ec69-136">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="7ec69-136">extensionAttribute8</span></span>|<span data-ttu-id="7ec69-137">String</span><span class="sxs-lookup"><span data-stu-id="7ec69-137">String</span></span>| <span data-ttu-id="7ec69-138">Восьмой настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="7ec69-138">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="7ec69-139">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="7ec69-139">extensionAttribute9</span></span>|<span data-ttu-id="7ec69-140">String</span><span class="sxs-lookup"><span data-stu-id="7ec69-140">String</span></span>| <span data-ttu-id="7ec69-141">Девятый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="7ec69-141">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="7ec69-142">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="7ec69-142">extensionAttribute10</span></span>|<span data-ttu-id="7ec69-143">String</span><span class="sxs-lookup"><span data-stu-id="7ec69-143">String</span></span>| <span data-ttu-id="7ec69-144">Десятый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="7ec69-144">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="7ec69-145">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="7ec69-145">extensionAttribute11</span></span>|<span data-ttu-id="7ec69-146">String</span><span class="sxs-lookup"><span data-stu-id="7ec69-146">String</span></span>| <span data-ttu-id="7ec69-147">Одиннадцатый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="7ec69-147">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="7ec69-148">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="7ec69-148">extensionAttribute12</span></span>|<span data-ttu-id="7ec69-149">String</span><span class="sxs-lookup"><span data-stu-id="7ec69-149">String</span></span>| <span data-ttu-id="7ec69-150">Двенадцатый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="7ec69-150">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="7ec69-151">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="7ec69-151">extensionAttribute13</span></span>|<span data-ttu-id="7ec69-152">String</span><span class="sxs-lookup"><span data-stu-id="7ec69-152">String</span></span>| <span data-ttu-id="7ec69-153">Тринадцатый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="7ec69-153">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="7ec69-154">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="7ec69-154">extensionAttribute14</span></span>|<span data-ttu-id="7ec69-155">String</span><span class="sxs-lookup"><span data-stu-id="7ec69-155">String</span></span>| <span data-ttu-id="7ec69-156">Четырнадцатый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="7ec69-156">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="7ec69-157">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="7ec69-157">extensionAttribute15</span></span>|<span data-ttu-id="7ec69-158">String</span><span class="sxs-lookup"><span data-stu-id="7ec69-158">String</span></span>| <span data-ttu-id="7ec69-159">Пятнадцатый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="7ec69-159">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7ec69-160">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7ec69-160">JSON representation</span></span>

<span data-ttu-id="7ec69-161">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7ec69-161">Here is a JSON representation of the resource</span></span>

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

