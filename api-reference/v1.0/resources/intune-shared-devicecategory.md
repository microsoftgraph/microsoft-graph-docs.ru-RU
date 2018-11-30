---
title: Тип ресурса deviceCategory
description: Эти категории затем можно применить к устройству в консоли Azure Intune или выбрать во время регистрации устройства пользователем. На основе категорий устройств вы можете фильтровать отчеты и создавать динамические группы устройств Azure Active Directory.
ms.openlocfilehash: c970cd7d7a95d7a888194a15b37873f5c6a44052
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027685"
---
# <a name="devicecategory-resource-type"></a><span data-ttu-id="103c7-104">Тип ресурса deviceCategory</span><span class="sxs-lookup"><span data-stu-id="103c7-104">deviceCategory resource type</span></span>

> <span data-ttu-id="103c7-105">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="103c7-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="103c7-106">Категории устройств используются для упорядочивания устройств.</span><span class="sxs-lookup"><span data-stu-id="103c7-106">Device categories provides a way to organize your devices.</span></span> <span data-ttu-id="103c7-107">Используя категории устройств, администраторы могут определить собственные категории, применимые к их организации.</span><span class="sxs-lookup"><span data-stu-id="103c7-107">Using device categories, company administrators can define their own categories that make sense to their company.</span></span><span data-ttu-id="103c7-108">Эти категории затем можно применить к устройству в консоли Azure Intune или выбрать во время регистрации устройства пользователем.</span><span class="sxs-lookup"><span data-stu-id="103c7-108"> These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment.</span></span> <span data-ttu-id="103c7-109">На основе категорий устройств вы можете фильтровать отчеты и создавать динамические группы устройств Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="103c7-109">You can filter reports and create dynamic Azure Active Directory device groups based on device categories.</span></span>

## <a name="methods"></a><span data-ttu-id="103c7-110">Методы</span><span class="sxs-lookup"><span data-stu-id="103c7-110">Methods</span></span>
|<span data-ttu-id="103c7-111">Метод</span><span class="sxs-lookup"><span data-stu-id="103c7-111">Method</span></span>|<span data-ttu-id="103c7-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="103c7-112">Return Type</span></span>|<span data-ttu-id="103c7-113">Описание</span><span class="sxs-lookup"><span data-stu-id="103c7-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="103c7-114">[Список deviceCategories](../api/intune-shared-devicecategory-list.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="103c7-114">[List deviceCategories](../api/intune-shared-devicecategory-list.md) collection</span></span>|<span data-ttu-id="103c7-115">Список свойств и связей объектов [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="103c7-115">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>|
|[<span data-ttu-id="103c7-116">Получение объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="103c7-116">Get deviceCategory</span></span>](../api/intune-shared-devicecategory-get.md)|<span data-ttu-id="103c7-117">Чтение свойств и связей объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="103c7-117">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="103c7-118">Создание объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="103c7-118">Create deviceCategory</span></span>](../api/intune-shared-devicecategory-create.md)|<span data-ttu-id="103c7-119">Создание объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="103c7-119">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|<span data-ttu-id="103c7-120">[Удаление deviceCategory](../api/intune-shared-devicecategory-delete.md).</span><span class="sxs-lookup"><span data-stu-id="103c7-120">[Delete deviceCategory](../api/intune-shared-devicecategory-delete.md).</span></span>|
|[<span data-ttu-id="103c7-121">Обновление объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="103c7-121">Update deviceCategory</span></span>](../api/intune-shared-devicecategory-update.md)|<span data-ttu-id="103c7-122">Обновление свойств объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="103c7-122">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="103c7-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="103c7-123">Properties</span></span>
|<span data-ttu-id="103c7-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="103c7-124">Property</span></span>|<span data-ttu-id="103c7-125">Тип</span><span class="sxs-lookup"><span data-stu-id="103c7-125">Type</span></span>|<span data-ttu-id="103c7-126">Описание</span><span class="sxs-lookup"><span data-stu-id="103c7-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="103c7-127">id</span><span class="sxs-lookup"><span data-stu-id="103c7-127">id</span></span>|<span data-ttu-id="103c7-128">String</span><span class="sxs-lookup"><span data-stu-id="103c7-128">String</span></span>|<span data-ttu-id="103c7-129">Уникальный идентификатор категории устройства.</span><span class="sxs-lookup"><span data-stu-id="103c7-129">Unique identifier for the device category.</span></span> <span data-ttu-id="103c7-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="103c7-130">Read-only.</span></span>|
|<span data-ttu-id="103c7-131">**Адаптация новых сотрудников**</span><span class="sxs-lookup"><span data-stu-id="103c7-131">**Onboarding**</span></span>|
|<span data-ttu-id="103c7-132">displayName</span><span class="sxs-lookup"><span data-stu-id="103c7-132">displayName</span></span>|<span data-ttu-id="103c7-133">String</span><span class="sxs-lookup"><span data-stu-id="103c7-133">String</span></span>|<span data-ttu-id="103c7-134">Отображаемое имя категории устройств.</span><span class="sxs-lookup"><span data-stu-id="103c7-134">Display name for the device category.</span></span>|
|<span data-ttu-id="103c7-135">описание</span><span class="sxs-lookup"><span data-stu-id="103c7-135">description</span></span>|<span data-ttu-id="103c7-136">String</span><span class="sxs-lookup"><span data-stu-id="103c7-136">String</span></span>|<span data-ttu-id="103c7-137">Необязательное описание категории устройств.</span><span class="sxs-lookup"><span data-stu-id="103c7-137">Optional description for the device category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="103c7-138">Связи</span><span class="sxs-lookup"><span data-stu-id="103c7-138">Relationships</span></span>
<span data-ttu-id="103c7-139">Нет</span><span class="sxs-lookup"><span data-stu-id="103c7-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="103c7-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="103c7-140">JSON Representation</span></span>
<span data-ttu-id="103c7-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="103c7-141">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.deviceCategory"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```



