---
title: Тип ресурса onPremisesExtensionAttributes
description: Свойство **onPremisesExtensionAttributes** объекта пользователя содержит 15 пользовательских свойств атрибута расширения. Для **пользователя onPremisesSyncEnabled** этот набор свойств освоен в локальном Active Directory и синхронизирован с Azure AD и является только для чтения. Для пользователя с облачным доступом (если **onPremisesSyncEnabled** является ложным), эти свойства можно настроить в Exchange Online. Атрибуты читают только в Microsoft Graph.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: f21369156e1a1337d16d64be40bd6de210bd56d2
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766107"
---
# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="52736-106">Тип ресурса onPremisesExtensionAttributes</span><span class="sxs-lookup"><span data-stu-id="52736-106">onPremisesExtensionAttributes resource type</span></span>

<span data-ttu-id="52736-107">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52736-107">Namespace: microsoft.graph</span></span>

<span data-ttu-id="52736-108">Свойство **onPremisesExtensionAttributes** объекта пользователя содержит [15](user.md) пользовательских свойств атрибута расширения.</span><span class="sxs-lookup"><span data-stu-id="52736-108">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="52736-109">Для **пользователя onPremisesSyncEnabled** источником полномочий для этого набора свойств является локальное Active Directory, синхронизированное с Azure AD и только для чтения.</span><span class="sxs-lookup"><span data-stu-id="52736-109">For an **onPremisesSyncEnabled** user, the source of authority for this set of properties is the on-premises Active Directory which is synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="52736-110">Для пользователя с облачным доступом (если **onPremisesSyncEnabled** является ложным), эти свойства можно настроить в Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="52736-110">For a cloud-only user (where **onPremisesSyncEnabled** is false), these properties can be set over Exchange Online.</span></span> <span data-ttu-id="52736-111">Атрибуты читают только в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="52736-111">The attributes are read only in Microsoft Graph.</span></span>

> <span data-ttu-id="52736-112">**Примечание:** Эти атрибуты расширения также известны как пользовательские атрибуты Exchange 1-15.</span><span class="sxs-lookup"><span data-stu-id="52736-112">**Note:** These extension attributes are also known as Exchange custom attributes 1-15.</span></span>

## <a name="properties"></a><span data-ttu-id="52736-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="52736-113">Properties</span></span>
| <span data-ttu-id="52736-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="52736-114">Property</span></span>     | <span data-ttu-id="52736-115">Тип</span><span class="sxs-lookup"><span data-stu-id="52736-115">Type</span></span>   |<span data-ttu-id="52736-116">Описание</span><span class="sxs-lookup"><span data-stu-id="52736-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="52736-117">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="52736-117">extensionAttribute1</span></span>|<span data-ttu-id="52736-118">String</span><span class="sxs-lookup"><span data-stu-id="52736-118">String</span></span>| <span data-ttu-id="52736-119">Первый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="52736-119">First customizable extension attribute.</span></span> |
|<span data-ttu-id="52736-120">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="52736-120">extensionAttribute2</span></span>|<span data-ttu-id="52736-121">String</span><span class="sxs-lookup"><span data-stu-id="52736-121">String</span></span>| <span data-ttu-id="52736-122">Второй настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="52736-122">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="52736-123">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="52736-123">extensionAttribute3</span></span>|<span data-ttu-id="52736-124">String</span><span class="sxs-lookup"><span data-stu-id="52736-124">String</span></span>| <span data-ttu-id="52736-125">Третий настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="52736-125">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="52736-126">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="52736-126">extensionAttribute4</span></span>|<span data-ttu-id="52736-127">String</span><span class="sxs-lookup"><span data-stu-id="52736-127">String</span></span>| <span data-ttu-id="52736-128">Четвертый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="52736-128">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="52736-129">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="52736-129">extensionAttribute5</span></span>|<span data-ttu-id="52736-130">String</span><span class="sxs-lookup"><span data-stu-id="52736-130">String</span></span>| <span data-ttu-id="52736-131">Пятый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="52736-131">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="52736-132">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="52736-132">extensionAttribute6</span></span>|<span data-ttu-id="52736-133">String</span><span class="sxs-lookup"><span data-stu-id="52736-133">String</span></span>| <span data-ttu-id="52736-134">Шестой настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="52736-134">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="52736-135">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="52736-135">extensionAttribute7</span></span>|<span data-ttu-id="52736-136">String</span><span class="sxs-lookup"><span data-stu-id="52736-136">String</span></span>| <span data-ttu-id="52736-137">Седьмой настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="52736-137">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="52736-138">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="52736-138">extensionAttribute8</span></span>|<span data-ttu-id="52736-139">String</span><span class="sxs-lookup"><span data-stu-id="52736-139">String</span></span>| <span data-ttu-id="52736-140">Восьмой настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="52736-140">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="52736-141">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="52736-141">extensionAttribute9</span></span>|<span data-ttu-id="52736-142">String</span><span class="sxs-lookup"><span data-stu-id="52736-142">String</span></span>| <span data-ttu-id="52736-143">Девятый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="52736-143">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="52736-144">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="52736-144">extensionAttribute10</span></span>|<span data-ttu-id="52736-145">String</span><span class="sxs-lookup"><span data-stu-id="52736-145">String</span></span>| <span data-ttu-id="52736-146">Десятый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="52736-146">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="52736-147">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="52736-147">extensionAttribute11</span></span>|<span data-ttu-id="52736-148">String</span><span class="sxs-lookup"><span data-stu-id="52736-148">String</span></span>| <span data-ttu-id="52736-149">Одиннадцатый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="52736-149">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="52736-150">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="52736-150">extensionAttribute12</span></span>|<span data-ttu-id="52736-151">String</span><span class="sxs-lookup"><span data-stu-id="52736-151">String</span></span>| <span data-ttu-id="52736-152">Двенадцатый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="52736-152">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="52736-153">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="52736-153">extensionAttribute13</span></span>|<span data-ttu-id="52736-154">String</span><span class="sxs-lookup"><span data-stu-id="52736-154">String</span></span>| <span data-ttu-id="52736-155">Тринадцатый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="52736-155">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="52736-156">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="52736-156">extensionAttribute14</span></span>|<span data-ttu-id="52736-157">String</span><span class="sxs-lookup"><span data-stu-id="52736-157">String</span></span>| <span data-ttu-id="52736-158">Четырнадцатый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="52736-158">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="52736-159">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="52736-159">extensionAttribute15</span></span>|<span data-ttu-id="52736-160">String</span><span class="sxs-lookup"><span data-stu-id="52736-160">String</span></span>| <span data-ttu-id="52736-161">Пятнадцатый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="52736-161">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="52736-162">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="52736-162">JSON representation</span></span>

<span data-ttu-id="52736-163">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="52736-163">Here is a JSON representation of the resource</span></span>

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

