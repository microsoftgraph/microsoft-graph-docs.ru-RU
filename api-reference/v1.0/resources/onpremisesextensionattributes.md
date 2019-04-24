---
title: Тип ресурса onPremisesExtensionAttributes
description: Свойство **onPremisesExtensionAttributes** объекта user содержит пятнадцать свойств настраиваемого атрибута расширения. Для пользователя **onPremisesSyncEnabled** этот набор свойств размещается в локальной службе Active Directory и синхронизируется с Azure AD и доступен только для чтения. Для пользователя, предназначенного только для облачного облака (где **onPremisesSyncEnabled** имеет значение false), эти свойства можно задать при создании или обновлении.
localization_priority: Normal
ms.openlocfilehash: c0cb765efe9e94c8254e45eaa9d55bc16382f6d2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462629"
---
# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="233e9-105">Тип ресурса onPremisesExtensionAttributes</span><span class="sxs-lookup"><span data-stu-id="233e9-105">onPremisesExtensionAttributes resource type</span></span>

<span data-ttu-id="233e9-106">Свойство **onPremisesExtensionAttributes** объекта [User](user.md) содержит пятнадцать свойств настраиваемого атрибута расширения.</span><span class="sxs-lookup"><span data-stu-id="233e9-106">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="233e9-107">Для пользователя **onPremisesSyncEnabled** этот набор свойств размещается в локальной службе Active Directory и синхронизируется с Azure AD и доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="233e9-107">For an **onPremisesSyncEnabled** user, this set of properties is mastered in on-premises Active Directory and synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="233e9-108">Для пользователя, предназначенного только для облачного облака (где **onPremisesSyncEnabled** имеет значение false), эти свойства можно задать при создании или обновлении.</span><span class="sxs-lookup"><span data-stu-id="233e9-108">For a cloud-only user (where **onPremisesSyncEnabled** is false), these properties may be set during creation or update.</span></span>


## <a name="properties"></a><span data-ttu-id="233e9-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="233e9-109">Properties</span></span>
| <span data-ttu-id="233e9-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="233e9-110">Property</span></span>     | <span data-ttu-id="233e9-111">Тип</span><span class="sxs-lookup"><span data-stu-id="233e9-111">Type</span></span>   |<span data-ttu-id="233e9-112">Описание</span><span class="sxs-lookup"><span data-stu-id="233e9-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="233e9-113">От extensionattribute1</span><span class="sxs-lookup"><span data-stu-id="233e9-113">extensionAttribute1</span></span>|<span data-ttu-id="233e9-114">String</span><span class="sxs-lookup"><span data-stu-id="233e9-114">String</span></span>| <span data-ttu-id="233e9-115">Первый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="233e9-115">First customizable extension attribute.</span></span> |
|<span data-ttu-id="233e9-116">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="233e9-116">extensionAttribute2</span></span>|<span data-ttu-id="233e9-117">String</span><span class="sxs-lookup"><span data-stu-id="233e9-117">String</span></span>| <span data-ttu-id="233e9-118">Второй настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="233e9-118">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="233e9-119">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="233e9-119">extensionAttribute3</span></span>|<span data-ttu-id="233e9-120">String</span><span class="sxs-lookup"><span data-stu-id="233e9-120">String</span></span>| <span data-ttu-id="233e9-121">Третий настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="233e9-121">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="233e9-122">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="233e9-122">extensionAttribute4</span></span>|<span data-ttu-id="233e9-123">String</span><span class="sxs-lookup"><span data-stu-id="233e9-123">String</span></span>| <span data-ttu-id="233e9-124">Четвертый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="233e9-124">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="233e9-125">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="233e9-125">extensionAttribute5</span></span>|<span data-ttu-id="233e9-126">String</span><span class="sxs-lookup"><span data-stu-id="233e9-126">String</span></span>| <span data-ttu-id="233e9-127">Пятый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="233e9-127">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="233e9-128">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="233e9-128">extensionAttribute6</span></span>|<span data-ttu-id="233e9-129">String</span><span class="sxs-lookup"><span data-stu-id="233e9-129">String</span></span>| <span data-ttu-id="233e9-130">Шестой настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="233e9-130">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="233e9-131">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="233e9-131">extensionAttribute7</span></span>|<span data-ttu-id="233e9-132">String</span><span class="sxs-lookup"><span data-stu-id="233e9-132">String</span></span>| <span data-ttu-id="233e9-133">Седьмой настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="233e9-133">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="233e9-134">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="233e9-134">extensionAttribute8</span></span>|<span data-ttu-id="233e9-135">String</span><span class="sxs-lookup"><span data-stu-id="233e9-135">String</span></span>| <span data-ttu-id="233e9-136">Восьмой настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="233e9-136">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="233e9-137">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="233e9-137">extensionAttribute9</span></span>|<span data-ttu-id="233e9-138">String</span><span class="sxs-lookup"><span data-stu-id="233e9-138">String</span></span>| <span data-ttu-id="233e9-139">Девятый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="233e9-139">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="233e9-140">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="233e9-140">extensionAttribute10</span></span>|<span data-ttu-id="233e9-141">String</span><span class="sxs-lookup"><span data-stu-id="233e9-141">String</span></span>| <span data-ttu-id="233e9-142">Десятый атрибут расширенной настройки.</span><span class="sxs-lookup"><span data-stu-id="233e9-142">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="233e9-143">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="233e9-143">extensionAttribute11</span></span>|<span data-ttu-id="233e9-144">String</span><span class="sxs-lookup"><span data-stu-id="233e9-144">String</span></span>| <span data-ttu-id="233e9-145">Одиннадцатый атрибут настраиваемого расширения.</span><span class="sxs-lookup"><span data-stu-id="233e9-145">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="233e9-146">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="233e9-146">extensionAttribute12</span></span>|<span data-ttu-id="233e9-147">String</span><span class="sxs-lookup"><span data-stu-id="233e9-147">String</span></span>| <span data-ttu-id="233e9-148">Двенадцатый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="233e9-148">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="233e9-149">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="233e9-149">extensionAttribute13</span></span>|<span data-ttu-id="233e9-150">String</span><span class="sxs-lookup"><span data-stu-id="233e9-150">String</span></span>| <span data-ttu-id="233e9-151">Настраиваемый атрибут расширения Сиртинс.</span><span class="sxs-lookup"><span data-stu-id="233e9-151">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="233e9-152">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="233e9-152">extensionAttribute14</span></span>|<span data-ttu-id="233e9-153">String</span><span class="sxs-lookup"><span data-stu-id="233e9-153">String</span></span>| <span data-ttu-id="233e9-154">Настраиваемый атрибут расширения Фауртинс.</span><span class="sxs-lookup"><span data-stu-id="233e9-154">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="233e9-155">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="233e9-155">extensionAttribute15</span></span>|<span data-ttu-id="233e9-156">String</span><span class="sxs-lookup"><span data-stu-id="233e9-156">String</span></span>| <span data-ttu-id="233e9-157">Пятнадцатый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="233e9-157">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="233e9-158">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="233e9-158">JSON representation</span></span>

<span data-ttu-id="233e9-159">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="233e9-159">Here is a JSON representation of the resource</span></span>

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
