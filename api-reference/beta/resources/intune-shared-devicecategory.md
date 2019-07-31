---
title: Тип ресурса deviceCategory
description: Эти категории затем можно применить к устройству в консоли Azure Intune или выбрать во время регистрации устройства пользователем. На основе категорий устройств вы можете фильтровать отчеты и создавать динамические группы устройств Azure Active Directory.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 159b7e38db24a103989e22209baf9a6424b2c1b1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967478"
---
# <a name="devicecategory-resource-type"></a><span data-ttu-id="6910b-104">Тип ресурса deviceCategory</span><span class="sxs-lookup"><span data-stu-id="6910b-104">deviceCategory resource type</span></span>

> <span data-ttu-id="6910b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6910b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6910b-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6910b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6910b-107">Категории устройств обеспечивают способ организации устройств.</span><span class="sxs-lookup"><span data-stu-id="6910b-107">Device categories provide a way to organize your devices.</span></span> <span data-ttu-id="6910b-108">С помощью категорий устройств Администраторы компании могут определять уникальные категории, которые имеют смысл в своей компании.</span><span class="sxs-lookup"><span data-stu-id="6910b-108">Using device categories, company administrators can define unique categories that make sense to their company.</span></span><span data-ttu-id="6910b-109">Эти категории затем можно применить к устройству в консоли Azure Intune или выбрать во время регистрации устройства пользователем.</span><span class="sxs-lookup"><span data-stu-id="6910b-109"> These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment.</span></span> <span data-ttu-id="6910b-110">На основе категорий устройств вы можете фильтровать отчеты и создавать динамические группы устройств Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="6910b-110">You can filter reports and create dynamic Azure Active Directory device groups based on device categories.</span></span>

## <a name="methods"></a><span data-ttu-id="6910b-111">Методы</span><span class="sxs-lookup"><span data-stu-id="6910b-111">Methods</span></span>
|<span data-ttu-id="6910b-112">Метод</span><span class="sxs-lookup"><span data-stu-id="6910b-112">Method</span></span>|<span data-ttu-id="6910b-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6910b-113">Return Type</span></span>|<span data-ttu-id="6910b-114">Описание</span><span class="sxs-lookup"><span data-stu-id="6910b-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6910b-115">Перечисление объектов deviceCategory</span><span class="sxs-lookup"><span data-stu-id="6910b-115">List deviceCategories</span></span>](../api/intune-shared-devicecategory-list.md)|<span data-ttu-id="6910b-116">Коллекция объектов [deviceCategory](../resources/intune-shared-devicecategory.md)</span><span class="sxs-lookup"><span data-stu-id="6910b-116">[deviceCategory](../resources/intune-shared-devicecategory.md) collection</span></span>|<span data-ttu-id="6910b-117">Список свойств и связей объектов [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="6910b-117">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>|
|[<span data-ttu-id="6910b-118">Получение объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="6910b-118">Get deviceCategory</span></span>](../api/intune-shared-devicecategory-get.md)|<span data-ttu-id="6910b-119">[deviceCategory](../resources/intune-shared-devicecategory.md);</span><span class="sxs-lookup"><span data-stu-id="6910b-119">[deviceCategory](../resources/intune-shared-devicecategory.md)</span></span>|<span data-ttu-id="6910b-120">Чтение свойств и связей объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="6910b-120">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="6910b-121">Создание объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="6910b-121">Create deviceCategory</span></span>](../api/intune-shared-devicecategory-create.md)|[<span data-ttu-id="6910b-122">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="6910b-122">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="6910b-123">Создание объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="6910b-123">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="6910b-124">Удаление объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="6910b-124">Delete deviceCategory</span></span>](../api/intune-shared-devicecategory-delete.md)|<span data-ttu-id="6910b-125">Нет</span><span class="sxs-lookup"><span data-stu-id="6910b-125">None</span></span>|<span data-ttu-id="6910b-126">Удаление объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="6910b-126">Deletes a [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>|
|[<span data-ttu-id="6910b-127">Обновление объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="6910b-127">Update deviceCategory</span></span>](../api/intune-shared-devicecategory-update.md)|<span data-ttu-id="6910b-128">[deviceCategory](../resources/intune-shared-devicecategory.md);</span><span class="sxs-lookup"><span data-stu-id="6910b-128">[deviceCategory](../resources/intune-shared-devicecategory.md)</span></span>|<span data-ttu-id="6910b-129">Обновление свойств объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="6910b-129">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6910b-130">Свойства</span><span class="sxs-lookup"><span data-stu-id="6910b-130">Properties</span></span>
|<span data-ttu-id="6910b-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="6910b-131">Property</span></span>|<span data-ttu-id="6910b-132">Тип</span><span class="sxs-lookup"><span data-stu-id="6910b-132">Type</span></span>|<span data-ttu-id="6910b-133">Описание</span><span class="sxs-lookup"><span data-stu-id="6910b-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6910b-134">id</span><span class="sxs-lookup"><span data-stu-id="6910b-134">id</span></span>|<span data-ttu-id="6910b-135">String</span><span class="sxs-lookup"><span data-stu-id="6910b-135">String</span></span>|<span data-ttu-id="6910b-136">Уникальный идентификатор категории устройства.</span><span class="sxs-lookup"><span data-stu-id="6910b-136">Unique identifier for the device category.</span></span> <span data-ttu-id="6910b-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6910b-137">Read-only.</span></span>|
|<span data-ttu-id="6910b-138">**Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="6910b-138">**Onboarding**</span></span>|
|<span data-ttu-id="6910b-139">displayName</span><span class="sxs-lookup"><span data-stu-id="6910b-139">displayName</span></span>|<span data-ttu-id="6910b-140">Строка</span><span class="sxs-lookup"><span data-stu-id="6910b-140">String</span></span>|<span data-ttu-id="6910b-141">Отображаемое имя категории устройств.</span><span class="sxs-lookup"><span data-stu-id="6910b-141">Display name for the device category.</span></span>|
|<span data-ttu-id="6910b-142">description</span><span class="sxs-lookup"><span data-stu-id="6910b-142">description</span></span>|<span data-ttu-id="6910b-143">String</span><span class="sxs-lookup"><span data-stu-id="6910b-143">String</span></span>|<span data-ttu-id="6910b-144">Необязательное описание категории устройств.</span><span class="sxs-lookup"><span data-stu-id="6910b-144">Optional description for the device category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6910b-145">Отношения</span><span class="sxs-lookup"><span data-stu-id="6910b-145">Relationships</span></span>
<span data-ttu-id="6910b-146">Нет</span><span class="sxs-lookup"><span data-stu-id="6910b-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6910b-147">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6910b-147">JSON Representation</span></span>
<span data-ttu-id="6910b-148">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6910b-148">Here is a JSON representation of the resource.</span></span>
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



