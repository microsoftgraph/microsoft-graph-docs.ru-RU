---
title: Тип ресурса deviceCategory
description: Эти категории затем можно применить к устройству в консоли Azure Intune или выбрать во время регистрации устройства пользователем. На основе категорий устройств вы можете фильтровать отчеты и создавать динамические группы устройств Azure Active Directory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 20e630e9e15e98744b349edb3c2986ff1b36a01a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48684395"
---
# <a name="devicecategory-resource-type"></a><span data-ttu-id="8ce6b-104">Тип ресурса deviceCategory</span><span class="sxs-lookup"><span data-stu-id="8ce6b-104">deviceCategory resource type</span></span>

<span data-ttu-id="8ce6b-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ce6b-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8ce6b-106">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ce6b-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8ce6b-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8ce6b-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ce6b-108">Категории устройств обеспечивают способ организации устройств.</span><span class="sxs-lookup"><span data-stu-id="8ce6b-108">Device categories provide a way to organize your devices.</span></span> <span data-ttu-id="8ce6b-109">С помощью категорий устройств Администраторы компании могут определять уникальные категории, которые имеют смысл в своей компании.</span><span class="sxs-lookup"><span data-stu-id="8ce6b-109">Using device categories, company administrators can define unique categories that make sense to their company.</span></span> <span data-ttu-id="8ce6b-110">Эти категории затем можно применить к устройству в консоли Azure Intune или выбрать во время регистрации устройства пользователем.</span><span class="sxs-lookup"><span data-stu-id="8ce6b-110">These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment.</span></span> <span data-ttu-id="8ce6b-111">На основе категорий устройств вы можете фильтровать отчеты и создавать динамические группы устройств Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="8ce6b-111">You can filter reports and create dynamic Azure Active Directory device groups based on device categories.</span></span>

## <a name="methods"></a><span data-ttu-id="8ce6b-112">Методы</span><span class="sxs-lookup"><span data-stu-id="8ce6b-112">Methods</span></span>
|<span data-ttu-id="8ce6b-113">Метод</span><span class="sxs-lookup"><span data-stu-id="8ce6b-113">Method</span></span>|<span data-ttu-id="8ce6b-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8ce6b-114">Return Type</span></span>|<span data-ttu-id="8ce6b-115">Описание</span><span class="sxs-lookup"><span data-stu-id="8ce6b-115">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8ce6b-116">Перечисление объектов deviceCategory</span><span class="sxs-lookup"><span data-stu-id="8ce6b-116">List deviceCategories</span></span>](../api/intune-shared-devicecategory-list.md)|<span data-ttu-id="8ce6b-117">Коллекция объектов [deviceCategory](../resources/intune-shared-devicecategory.md)</span><span class="sxs-lookup"><span data-stu-id="8ce6b-117">[deviceCategory](../resources/intune-shared-devicecategory.md) collection</span></span>|<span data-ttu-id="8ce6b-118">Список свойств и связей объектов [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="8ce6b-118">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>|
|[<span data-ttu-id="8ce6b-119">Получение объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="8ce6b-119">Get deviceCategory</span></span>](../api/intune-shared-devicecategory-get.md)|[<span data-ttu-id="8ce6b-120">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="8ce6b-120">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="8ce6b-121">Чтение свойств и связей объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="8ce6b-121">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="8ce6b-122">Создание объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="8ce6b-122">Create deviceCategory</span></span>](../api/intune-shared-devicecategory-create.md)|[<span data-ttu-id="8ce6b-123">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="8ce6b-123">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="8ce6b-124">Создание объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="8ce6b-124">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="8ce6b-125">Удаление объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="8ce6b-125">Delete deviceCategory</span></span>](../api/intune-shared-devicecategory-delete.md)|<span data-ttu-id="8ce6b-126">Нет</span><span class="sxs-lookup"><span data-stu-id="8ce6b-126">None</span></span>|<span data-ttu-id="8ce6b-127">Удаление объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="8ce6b-127">Deletes a [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>|
|[<span data-ttu-id="8ce6b-128">Обновление объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="8ce6b-128">Update deviceCategory</span></span>](../api/intune-shared-devicecategory-update.md)|[<span data-ttu-id="8ce6b-129">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="8ce6b-129">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="8ce6b-130">Обновление свойств объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="8ce6b-130">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8ce6b-131">Свойства</span><span class="sxs-lookup"><span data-stu-id="8ce6b-131">Properties</span></span>
|<span data-ttu-id="8ce6b-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="8ce6b-132">Property</span></span>|<span data-ttu-id="8ce6b-133">Тип</span><span class="sxs-lookup"><span data-stu-id="8ce6b-133">Type</span></span>|<span data-ttu-id="8ce6b-134">Описание</span><span class="sxs-lookup"><span data-stu-id="8ce6b-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ce6b-135">id</span><span class="sxs-lookup"><span data-stu-id="8ce6b-135">id</span></span>|<span data-ttu-id="8ce6b-136">Строка</span><span class="sxs-lookup"><span data-stu-id="8ce6b-136">String</span></span>|<span data-ttu-id="8ce6b-137">Уникальный идентификатор категории устройства.</span><span class="sxs-lookup"><span data-stu-id="8ce6b-137">Unique identifier for the device category.</span></span> <span data-ttu-id="8ce6b-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8ce6b-138">Read-only.</span></span>|
|<span data-ttu-id="8ce6b-139">**Адаптация**</span><span class="sxs-lookup"><span data-stu-id="8ce6b-139">**Onboarding**</span></span>|
|<span data-ttu-id="8ce6b-140">displayName</span><span class="sxs-lookup"><span data-stu-id="8ce6b-140">displayName</span></span>|<span data-ttu-id="8ce6b-141">Строка</span><span class="sxs-lookup"><span data-stu-id="8ce6b-141">String</span></span>|<span data-ttu-id="8ce6b-142">Отображаемое имя категории устройств.</span><span class="sxs-lookup"><span data-stu-id="8ce6b-142">Display name for the device category.</span></span>|
|<span data-ttu-id="8ce6b-143">description</span><span class="sxs-lookup"><span data-stu-id="8ce6b-143">description</span></span>|<span data-ttu-id="8ce6b-144">Строка</span><span class="sxs-lookup"><span data-stu-id="8ce6b-144">String</span></span>|<span data-ttu-id="8ce6b-145">Необязательное описание категории устройств.</span><span class="sxs-lookup"><span data-stu-id="8ce6b-145">Optional description for the device category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8ce6b-146">Связи</span><span class="sxs-lookup"><span data-stu-id="8ce6b-146">Relationships</span></span>
<span data-ttu-id="8ce6b-147">Нет</span><span class="sxs-lookup"><span data-stu-id="8ce6b-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8ce6b-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8ce6b-148">JSON Representation</span></span>
<span data-ttu-id="8ce6b-149">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8ce6b-149">Here is a JSON representation of the resource.</span></span>
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





