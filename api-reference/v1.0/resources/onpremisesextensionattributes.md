---
title: Тип ресурса onPremisesExtensionAttributes
description: Свойство **onPremisesExtensionAttributes** объекта user содержит пятнадцать свойств настраиваемого атрибута расширения. Для пользователя **onPremisesSyncEnabled** этот набор свойств размещается в локальной службе Active Directory и синхронизируется с Azure AD и доступен только для чтения. Для пользователя, предназначенного только для облачного облака (где **onPremisesSyncEnabled** имеет значение false), эти свойства можно задать при создании или обновлении.
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 84929229c18b905ff66b4a1bbbbf765771180a06
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2020
ms.locfileid: "44864093"
---
# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="482de-105">Тип ресурса onPremisesExtensionAttributes</span><span class="sxs-lookup"><span data-stu-id="482de-105">onPremisesExtensionAttributes resource type</span></span>

<span data-ttu-id="482de-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="482de-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="482de-107">Свойство **onPremisesExtensionAttributes** объекта [User](user.md) содержит пятнадцать свойств настраиваемого атрибута расширения.</span><span class="sxs-lookup"><span data-stu-id="482de-107">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="482de-108">Для пользователя **onPremisesSyncEnabled** источником полномочий для этого набора свойств является локальный каталог Active Directory, который синхронизируется с Azure AD и доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="482de-108">For an **onPremisesSyncEnabled** user, the source of authority for this set of properties is the on-premises Active Directory which is synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="482de-109">Для пользователя, предназначенного только для облачного облака (где **onPremisesSyncEnabled** имеет значение false), эти свойства можно задать при создании или обновлении.</span><span class="sxs-lookup"><span data-stu-id="482de-109">For a cloud-only user (where **onPremisesSyncEnabled** is false), these properties may be set during creation or update.</span></span>

> <span data-ttu-id="482de-110">**Примечание:** Эти атрибуты расширения также называются пользовательскими атрибутами Exchange 1-15.</span><span class="sxs-lookup"><span data-stu-id="482de-110">**Note:** These extension attributes are also known as Exchange custom attributes 1-15.</span></span>

## <a name="properties"></a><span data-ttu-id="482de-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="482de-111">Properties</span></span>
| <span data-ttu-id="482de-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="482de-112">Property</span></span>     | <span data-ttu-id="482de-113">Тип</span><span class="sxs-lookup"><span data-stu-id="482de-113">Type</span></span>   |<span data-ttu-id="482de-114">Описание</span><span class="sxs-lookup"><span data-stu-id="482de-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="482de-115">От extensionattribute1</span><span class="sxs-lookup"><span data-stu-id="482de-115">extensionAttribute1</span></span>|<span data-ttu-id="482de-116">String</span><span class="sxs-lookup"><span data-stu-id="482de-116">String</span></span>| <span data-ttu-id="482de-117">Первый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="482de-117">First customizable extension attribute.</span></span> |
|<span data-ttu-id="482de-118">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="482de-118">extensionAttribute2</span></span>|<span data-ttu-id="482de-119">String</span><span class="sxs-lookup"><span data-stu-id="482de-119">String</span></span>| <span data-ttu-id="482de-120">Второй настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="482de-120">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="482de-121">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="482de-121">extensionAttribute3</span></span>|<span data-ttu-id="482de-122">String</span><span class="sxs-lookup"><span data-stu-id="482de-122">String</span></span>| <span data-ttu-id="482de-123">Третий настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="482de-123">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="482de-124">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="482de-124">extensionAttribute4</span></span>|<span data-ttu-id="482de-125">String</span><span class="sxs-lookup"><span data-stu-id="482de-125">String</span></span>| <span data-ttu-id="482de-126">Четвертый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="482de-126">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="482de-127">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="482de-127">extensionAttribute5</span></span>|<span data-ttu-id="482de-128">String</span><span class="sxs-lookup"><span data-stu-id="482de-128">String</span></span>| <span data-ttu-id="482de-129">Пятый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="482de-129">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="482de-130">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="482de-130">extensionAttribute6</span></span>|<span data-ttu-id="482de-131">String</span><span class="sxs-lookup"><span data-stu-id="482de-131">String</span></span>| <span data-ttu-id="482de-132">Шестой настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="482de-132">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="482de-133">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="482de-133">extensionAttribute7</span></span>|<span data-ttu-id="482de-134">String</span><span class="sxs-lookup"><span data-stu-id="482de-134">String</span></span>| <span data-ttu-id="482de-135">Седьмой настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="482de-135">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="482de-136">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="482de-136">extensionAttribute8</span></span>|<span data-ttu-id="482de-137">String</span><span class="sxs-lookup"><span data-stu-id="482de-137">String</span></span>| <span data-ttu-id="482de-138">Восьмой настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="482de-138">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="482de-139">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="482de-139">extensionAttribute9</span></span>|<span data-ttu-id="482de-140">String</span><span class="sxs-lookup"><span data-stu-id="482de-140">String</span></span>| <span data-ttu-id="482de-141">Девятый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="482de-141">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="482de-142">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="482de-142">extensionAttribute10</span></span>|<span data-ttu-id="482de-143">String</span><span class="sxs-lookup"><span data-stu-id="482de-143">String</span></span>| <span data-ttu-id="482de-144">Десятый атрибут расширенной настройки.</span><span class="sxs-lookup"><span data-stu-id="482de-144">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="482de-145">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="482de-145">extensionAttribute11</span></span>|<span data-ttu-id="482de-146">String</span><span class="sxs-lookup"><span data-stu-id="482de-146">String</span></span>| <span data-ttu-id="482de-147">Одиннадцатый атрибут настраиваемого расширения.</span><span class="sxs-lookup"><span data-stu-id="482de-147">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="482de-148">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="482de-148">extensionAttribute12</span></span>|<span data-ttu-id="482de-149">String</span><span class="sxs-lookup"><span data-stu-id="482de-149">String</span></span>| <span data-ttu-id="482de-150">Двенадцатый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="482de-150">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="482de-151">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="482de-151">extensionAttribute13</span></span>|<span data-ttu-id="482de-152">String</span><span class="sxs-lookup"><span data-stu-id="482de-152">String</span></span>| <span data-ttu-id="482de-153">Настраиваемый атрибут расширения сиртинс.</span><span class="sxs-lookup"><span data-stu-id="482de-153">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="482de-154">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="482de-154">extensionAttribute14</span></span>|<span data-ttu-id="482de-155">String</span><span class="sxs-lookup"><span data-stu-id="482de-155">String</span></span>| <span data-ttu-id="482de-156">Настраиваемый атрибут расширения фауртинс.</span><span class="sxs-lookup"><span data-stu-id="482de-156">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="482de-157">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="482de-157">extensionAttribute15</span></span>|<span data-ttu-id="482de-158">String</span><span class="sxs-lookup"><span data-stu-id="482de-158">String</span></span>| <span data-ttu-id="482de-159">Пятнадцатый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="482de-159">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="482de-160">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="482de-160">JSON representation</span></span>

<span data-ttu-id="482de-161">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="482de-161">Here is a JSON representation of the resource</span></span>

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
