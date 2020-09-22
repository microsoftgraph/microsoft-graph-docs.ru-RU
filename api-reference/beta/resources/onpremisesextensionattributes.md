---
title: Тип ресурса onPremisesExtensionAttributes
description: Свойство **onPremisesExtensionAttributes** объекта user содержит пятнадцать свойств настраиваемого атрибута расширения.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: users
author: krbain
ms.openlocfilehash: 2729d6d624f1bde304425229ccf4ae7df8ddf781
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48052600"
---
# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="29c6c-103">Тип ресурса onPremisesExtensionAttributes</span><span class="sxs-lookup"><span data-stu-id="29c6c-103">onPremisesExtensionAttributes resource type</span></span>

<span data-ttu-id="29c6c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29c6c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29c6c-105">Свойство **onPremisesExtensionAttributes** объекта [User](user.md) содержит пятнадцать свойств настраиваемого атрибута расширения.</span><span class="sxs-lookup"><span data-stu-id="29c6c-105">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="29c6c-106">Для пользователя **onPremisesSyncEnabled** источником полномочий для этого набора свойств является локальный каталог Active Directory, который синхронизируется с Azure AD и доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="29c6c-106">For an **onPremisesSyncEnabled** user, the source of authority for this set of properties is the on-premises Active Directory which is synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="29c6c-107">Для пользователя, предназначенного только для облачного облака (где **onPremisesSyncEnabled** имеет значение false), эти свойства можно задать при создании или обновлении.</span><span class="sxs-lookup"><span data-stu-id="29c6c-107">For a cloud-only user (where **onPremisesSyncEnabled** is false), these properties may be set during creation or update.</span></span>

> <span data-ttu-id="29c6c-108">**Примечание:** Эти атрибуты расширения также называются пользовательскими атрибутами Exchange 1-15.</span><span class="sxs-lookup"><span data-stu-id="29c6c-108">**Note:** These extension attributes are also known as Exchange custom attributes 1-15.</span></span>


## <a name="properties"></a><span data-ttu-id="29c6c-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="29c6c-109">Properties</span></span>
| <span data-ttu-id="29c6c-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="29c6c-110">Property</span></span>     | <span data-ttu-id="29c6c-111">Тип</span><span class="sxs-lookup"><span data-stu-id="29c6c-111">Type</span></span>   |<span data-ttu-id="29c6c-112">Описание</span><span class="sxs-lookup"><span data-stu-id="29c6c-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="29c6c-113">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="29c6c-113">extensionAttribute1</span></span>|<span data-ttu-id="29c6c-114">String</span><span class="sxs-lookup"><span data-stu-id="29c6c-114">String</span></span>| <span data-ttu-id="29c6c-115">Первый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="29c6c-115">First customizable extension attribute.</span></span> |
|<span data-ttu-id="29c6c-116">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="29c6c-116">extensionAttribute2</span></span>|<span data-ttu-id="29c6c-117">String</span><span class="sxs-lookup"><span data-stu-id="29c6c-117">String</span></span>| <span data-ttu-id="29c6c-118">Второй настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="29c6c-118">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="29c6c-119">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="29c6c-119">extensionAttribute3</span></span>|<span data-ttu-id="29c6c-120">String</span><span class="sxs-lookup"><span data-stu-id="29c6c-120">String</span></span>| <span data-ttu-id="29c6c-121">Третий настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="29c6c-121">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="29c6c-122">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="29c6c-122">extensionAttribute4</span></span>|<span data-ttu-id="29c6c-123">String</span><span class="sxs-lookup"><span data-stu-id="29c6c-123">String</span></span>| <span data-ttu-id="29c6c-124">Четвертый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="29c6c-124">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="29c6c-125">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="29c6c-125">extensionAttribute5</span></span>|<span data-ttu-id="29c6c-126">String</span><span class="sxs-lookup"><span data-stu-id="29c6c-126">String</span></span>| <span data-ttu-id="29c6c-127">Пятый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="29c6c-127">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="29c6c-128">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="29c6c-128">extensionAttribute6</span></span>|<span data-ttu-id="29c6c-129">String</span><span class="sxs-lookup"><span data-stu-id="29c6c-129">String</span></span>| <span data-ttu-id="29c6c-130">Шестой настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="29c6c-130">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="29c6c-131">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="29c6c-131">extensionAttribute7</span></span>|<span data-ttu-id="29c6c-132">String</span><span class="sxs-lookup"><span data-stu-id="29c6c-132">String</span></span>| <span data-ttu-id="29c6c-133">Седьмой настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="29c6c-133">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="29c6c-134">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="29c6c-134">extensionAttribute8</span></span>|<span data-ttu-id="29c6c-135">String</span><span class="sxs-lookup"><span data-stu-id="29c6c-135">String</span></span>| <span data-ttu-id="29c6c-136">Восьмой настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="29c6c-136">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="29c6c-137">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="29c6c-137">extensionAttribute9</span></span>|<span data-ttu-id="29c6c-138">String</span><span class="sxs-lookup"><span data-stu-id="29c6c-138">String</span></span>| <span data-ttu-id="29c6c-139">Девятый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="29c6c-139">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="29c6c-140">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="29c6c-140">extensionAttribute10</span></span>|<span data-ttu-id="29c6c-141">String</span><span class="sxs-lookup"><span data-stu-id="29c6c-141">String</span></span>| <span data-ttu-id="29c6c-142">Десятый атрибут расширенной настройки.</span><span class="sxs-lookup"><span data-stu-id="29c6c-142">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="29c6c-143">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="29c6c-143">extensionAttribute11</span></span>|<span data-ttu-id="29c6c-144">String</span><span class="sxs-lookup"><span data-stu-id="29c6c-144">String</span></span>| <span data-ttu-id="29c6c-145">Одиннадцатый атрибут настраиваемого расширения.</span><span class="sxs-lookup"><span data-stu-id="29c6c-145">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="29c6c-146">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="29c6c-146">extensionAttribute12</span></span>|<span data-ttu-id="29c6c-147">String</span><span class="sxs-lookup"><span data-stu-id="29c6c-147">String</span></span>| <span data-ttu-id="29c6c-148">Двенадцатый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="29c6c-148">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="29c6c-149">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="29c6c-149">extensionAttribute13</span></span>|<span data-ttu-id="29c6c-150">String</span><span class="sxs-lookup"><span data-stu-id="29c6c-150">String</span></span>| <span data-ttu-id="29c6c-151">Настраиваемый атрибут расширения сиртинс.</span><span class="sxs-lookup"><span data-stu-id="29c6c-151">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="29c6c-152">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="29c6c-152">extensionAttribute14</span></span>|<span data-ttu-id="29c6c-153">String</span><span class="sxs-lookup"><span data-stu-id="29c6c-153">String</span></span>| <span data-ttu-id="29c6c-154">Настраиваемый атрибут расширения фауртинс.</span><span class="sxs-lookup"><span data-stu-id="29c6c-154">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="29c6c-155">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="29c6c-155">extensionAttribute15</span></span>|<span data-ttu-id="29c6c-156">String</span><span class="sxs-lookup"><span data-stu-id="29c6c-156">String</span></span>| <span data-ttu-id="29c6c-157">Пятнадцатый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="29c6c-157">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="29c6c-158">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="29c6c-158">JSON representation</span></span>

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


