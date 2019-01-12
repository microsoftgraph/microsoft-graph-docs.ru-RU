---
title: Тип ресурса deviceCategory
description: Эти категории затем можно применить к устройству в консоли Azure Intune или выбрать во время регистрации устройства пользователем. На основе категорий устройств вы можете фильтровать отчеты и создавать динамические группы устройств Azure Active Directory.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 885609c4bbbd01a9bf295e7c49a2790ce51b2941
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922216"
---
# <a name="devicecategory-resource-type"></a><span data-ttu-id="18763-104">Тип ресурса deviceCategory</span><span class="sxs-lookup"><span data-stu-id="18763-104">deviceCategory resource type</span></span>

> <span data-ttu-id="18763-105">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="18763-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="18763-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18763-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="18763-107">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="18763-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="18763-108">Категории устройств предоставляют способ организации устройство.</span><span class="sxs-lookup"><span data-stu-id="18763-108">Device categories provide a way to organize your devices.</span></span> <span data-ttu-id="18763-109">С помощью категории устройств, компании администраторы могут определить уникальный категорий, относящиеся к своей компании.</span><span class="sxs-lookup"><span data-stu-id="18763-109">Using device categories, company administrators can define unique categories that make sense to their company.</span></span><span data-ttu-id="18763-110">Эти категории затем можно применить к устройству в консоли Azure Intune или выбрать во время регистрации устройства пользователем.</span><span class="sxs-lookup"><span data-stu-id="18763-110"> These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment.</span></span> <span data-ttu-id="18763-111">На основе категорий устройств вы можете фильтровать отчеты и создавать динамические группы устройств Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="18763-111">You can filter reports and create dynamic Azure Active Directory device groups based on device categories.</span></span>

## <a name="methods"></a><span data-ttu-id="18763-112">Методы</span><span class="sxs-lookup"><span data-stu-id="18763-112">Methods</span></span>
|<span data-ttu-id="18763-113">Метод</span><span class="sxs-lookup"><span data-stu-id="18763-113">Method</span></span>|<span data-ttu-id="18763-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="18763-114">Return Type</span></span>|<span data-ttu-id="18763-115">Описание</span><span class="sxs-lookup"><span data-stu-id="18763-115">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="18763-116">Перечисление объектов deviceCategory</span><span class="sxs-lookup"><span data-stu-id="18763-116">List deviceCategories</span></span>](../api/intune-shared-devicecategory-list.md)|<span data-ttu-id="18763-117">Коллекция объектов [deviceCategory](../resources/intune-shared-devicecategory.md)</span><span class="sxs-lookup"><span data-stu-id="18763-117">[deviceCategory](../resources/intune-shared-devicecategory.md) collection</span></span>|<span data-ttu-id="18763-118">Список свойств и связей объектов [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="18763-118">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>|
|[<span data-ttu-id="18763-119">Получение объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="18763-119">Get deviceCategory</span></span>](../api/intune-shared-devicecategory-get.md)|[<span data-ttu-id="18763-120">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="18763-120">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="18763-121">Чтение свойств и связей объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="18763-121">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="18763-122">Создание объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="18763-122">Create deviceCategory</span></span>](../api/intune-shared-devicecategory-create.md)|[<span data-ttu-id="18763-123">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="18763-123">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="18763-124">Создание объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="18763-124">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="18763-125">Удаление объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="18763-125">Delete deviceCategory</span></span>](../api/intune-shared-devicecategory-delete.md)|<span data-ttu-id="18763-126">Нет</span><span class="sxs-lookup"><span data-stu-id="18763-126">None</span></span>|<span data-ttu-id="18763-127">Удаление объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="18763-127">Deletes a [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>|
|[<span data-ttu-id="18763-128">Обновление объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="18763-128">Update deviceCategory</span></span>](../api/intune-shared-devicecategory-update.md)|[<span data-ttu-id="18763-129">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="18763-129">deviceCategory</span></span>](../resources/intune-shared-devicecategory.md)|<span data-ttu-id="18763-130">Обновление свойств объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="18763-130">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="18763-131">Свойства</span><span class="sxs-lookup"><span data-stu-id="18763-131">Properties</span></span>
|<span data-ttu-id="18763-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="18763-132">Property</span></span>|<span data-ttu-id="18763-133">Тип</span><span class="sxs-lookup"><span data-stu-id="18763-133">Type</span></span>|<span data-ttu-id="18763-134">Описание</span><span class="sxs-lookup"><span data-stu-id="18763-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18763-135">id</span><span class="sxs-lookup"><span data-stu-id="18763-135">id</span></span>|<span data-ttu-id="18763-136">String</span><span class="sxs-lookup"><span data-stu-id="18763-136">String</span></span>|<span data-ttu-id="18763-137">Уникальный идентификатор категории устройства.</span><span class="sxs-lookup"><span data-stu-id="18763-137">Unique identifier for the device category.</span></span> <span data-ttu-id="18763-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="18763-138">Read-only.</span></span>|
|<span data-ttu-id="18763-139">**Адаптация новых сотрудников**</span><span class="sxs-lookup"><span data-stu-id="18763-139">**Onboarding**</span></span>|
|<span data-ttu-id="18763-140">displayName</span><span class="sxs-lookup"><span data-stu-id="18763-140">displayName</span></span>|<span data-ttu-id="18763-141">String</span><span class="sxs-lookup"><span data-stu-id="18763-141">String</span></span>|<span data-ttu-id="18763-142">Отображаемое имя категории устройств.</span><span class="sxs-lookup"><span data-stu-id="18763-142">Display name for the device category.</span></span>|
|<span data-ttu-id="18763-143">описание</span><span class="sxs-lookup"><span data-stu-id="18763-143">description</span></span>|<span data-ttu-id="18763-144">String</span><span class="sxs-lookup"><span data-stu-id="18763-144">String</span></span>|<span data-ttu-id="18763-145">Необязательное описание категории устройств.</span><span class="sxs-lookup"><span data-stu-id="18763-145">Optional description for the device category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="18763-146">Связи</span><span class="sxs-lookup"><span data-stu-id="18763-146">Relationships</span></span>
<span data-ttu-id="18763-147">Нет</span><span class="sxs-lookup"><span data-stu-id="18763-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="18763-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="18763-148">JSON Representation</span></span>
<span data-ttu-id="18763-149">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="18763-149">Here is a JSON representation of the resource.</span></span>
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



