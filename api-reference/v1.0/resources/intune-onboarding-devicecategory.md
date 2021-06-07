---
title: Тип ресурса deviceCategory
description: Категории устройств используются для упорядочивания устройств. Используя категории устройств, администраторы могут определить собственные категории, применимые к их организации. Эти категории затем можно применить к устройству в консоли Azure Intune или выбрать во время регистрации устройства пользователем. На основе категорий устройств вы можете фильтровать отчеты и создавать динамические группы устройств Azure Active Directory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5def5ee6c6a97e91c9255a9808db7fc6b2fa07fc
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752048"
---
# <a name="devicecategory-resource-type"></a><span data-ttu-id="b976b-106">Тип ресурса deviceCategory</span><span class="sxs-lookup"><span data-stu-id="b976b-106">deviceCategory resource type</span></span>

<span data-ttu-id="b976b-107">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b976b-107">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b976b-108">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b976b-108">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b976b-109">Категории устройств используются для упорядочивания устройств.</span><span class="sxs-lookup"><span data-stu-id="b976b-109">Device categories provides a way to organize your devices.</span></span> <span data-ttu-id="b976b-110">Используя категории устройств, администраторы могут определить собственные категории, применимые к их организации.</span><span class="sxs-lookup"><span data-stu-id="b976b-110">Using device categories, company administrators can define their own categories that make sense to their company.</span></span> <span data-ttu-id="b976b-111">Эти категории затем можно применить к устройству в консоли Azure Intune или выбрать во время регистрации устройства пользователем.</span><span class="sxs-lookup"><span data-stu-id="b976b-111">These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment.</span></span> <span data-ttu-id="b976b-112">На основе категорий устройств вы можете фильтровать отчеты и создавать динамические группы устройств Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b976b-112">You can filter reports and create dynamic Azure Active Directory device groups based on device categories.</span></span>

## <a name="methods"></a><span data-ttu-id="b976b-113">Методы</span><span class="sxs-lookup"><span data-stu-id="b976b-113">Methods</span></span>
|<span data-ttu-id="b976b-114">Метод</span><span class="sxs-lookup"><span data-stu-id="b976b-114">Method</span></span>|<span data-ttu-id="b976b-115">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b976b-115">Return Type</span></span>|<span data-ttu-id="b976b-116">Описание</span><span class="sxs-lookup"><span data-stu-id="b976b-116">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b976b-117">Перечисление объектов deviceCategory</span><span class="sxs-lookup"><span data-stu-id="b976b-117">List deviceCategories</span></span>](../api/intune-onboarding-devicecategory-list.md)|<span data-ttu-id="b976b-118">Коллекция объектов [deviceCategory](../resources/intune-onboarding-devicecategory.md)</span><span class="sxs-lookup"><span data-stu-id="b976b-118">[deviceCategory](../resources/intune-onboarding-devicecategory.md) collection</span></span>|<span data-ttu-id="b976b-119">Список свойств и связей объектов [deviceCategory](../resources/intune-onboarding-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="b976b-119">List properties and relationships of the [deviceCategory](../resources/intune-onboarding-devicecategory.md) objects.</span></span>|
|[<span data-ttu-id="b976b-120">Получение объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="b976b-120">Get deviceCategory</span></span>](../api/intune-onboarding-devicecategory-get.md)|[<span data-ttu-id="b976b-121">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="b976b-121">deviceCategory</span></span>](../resources/intune-onboarding-devicecategory.md)|<span data-ttu-id="b976b-122">Чтение свойств и связей объекта [deviceCategory](../resources/intune-onboarding-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="b976b-122">Read properties and relationships of the [deviceCategory](../resources/intune-onboarding-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="b976b-123">Создание объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="b976b-123">Create deviceCategory</span></span>](../api/intune-onboarding-devicecategory-create.md)|[<span data-ttu-id="b976b-124">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="b976b-124">deviceCategory</span></span>](../resources/intune-onboarding-devicecategory.md)|<span data-ttu-id="b976b-125">Создание объекта [deviceCategory](../resources/intune-onboarding-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="b976b-125">Create a new [deviceCategory](../resources/intune-onboarding-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="b976b-126">Удаление объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="b976b-126">Delete deviceCategory</span></span>](../api/intune-onboarding-devicecategory-delete.md)|<span data-ttu-id="b976b-127">Нет</span><span class="sxs-lookup"><span data-stu-id="b976b-127">None</span></span>|<span data-ttu-id="b976b-128">Удаление объекта [deviceCategory](../resources/intune-onboarding-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="b976b-128">Deletes a [deviceCategory](../resources/intune-onboarding-devicecategory.md).</span></span>|
|[<span data-ttu-id="b976b-129">Обновление объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="b976b-129">Update deviceCategory</span></span>](../api/intune-onboarding-devicecategory-update.md)|[<span data-ttu-id="b976b-130">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="b976b-130">deviceCategory</span></span>](../resources/intune-onboarding-devicecategory.md)|<span data-ttu-id="b976b-131">Обновление свойств объекта [deviceCategory](../resources/intune-onboarding-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="b976b-131">Update the properties of a [deviceCategory](../resources/intune-onboarding-devicecategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b976b-132">Свойства</span><span class="sxs-lookup"><span data-stu-id="b976b-132">Properties</span></span>
|<span data-ttu-id="b976b-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="b976b-133">Property</span></span>|<span data-ttu-id="b976b-134">Тип</span><span class="sxs-lookup"><span data-stu-id="b976b-134">Type</span></span>|<span data-ttu-id="b976b-135">Описание</span><span class="sxs-lookup"><span data-stu-id="b976b-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b976b-136">id</span><span class="sxs-lookup"><span data-stu-id="b976b-136">id</span></span>|<span data-ttu-id="b976b-137">String</span><span class="sxs-lookup"><span data-stu-id="b976b-137">String</span></span>|<span data-ttu-id="b976b-138">Уникальный идентификатор категории устройства.</span><span class="sxs-lookup"><span data-stu-id="b976b-138">Unique identifier for the device category.</span></span> <span data-ttu-id="b976b-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b976b-139">Read-only.</span></span>|
|<span data-ttu-id="b976b-140">displayName</span><span class="sxs-lookup"><span data-stu-id="b976b-140">displayName</span></span>|<span data-ttu-id="b976b-141">String</span><span class="sxs-lookup"><span data-stu-id="b976b-141">String</span></span>|<span data-ttu-id="b976b-142">Отображаемое имя категории устройств.</span><span class="sxs-lookup"><span data-stu-id="b976b-142">Display name for the device category.</span></span>|
|<span data-ttu-id="b976b-143">description</span><span class="sxs-lookup"><span data-stu-id="b976b-143">description</span></span>|<span data-ttu-id="b976b-144">String</span><span class="sxs-lookup"><span data-stu-id="b976b-144">String</span></span>|<span data-ttu-id="b976b-145">Необязательное описание категории устройств.</span><span class="sxs-lookup"><span data-stu-id="b976b-145">Optional description for the device category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b976b-146">Связи</span><span class="sxs-lookup"><span data-stu-id="b976b-146">Relationships</span></span>
<span data-ttu-id="b976b-147">Нет</span><span class="sxs-lookup"><span data-stu-id="b976b-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b976b-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b976b-148">JSON Representation</span></span>
<span data-ttu-id="b976b-149">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b976b-149">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```




