---
title: Тип ресурса deviceCategory
description: Эти категории затем можно применить к устройству в консоли Azure Intune или выбрать во время регистрации устройства пользователем. На основе категорий устройств вы можете фильтровать отчеты и создавать динамические группы устройств Azure Active Directory.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a0bb1e994bcf42ba91a55fdfc75946204d1f9b06
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254900"
---
# <a name="devicecategory-resource-type"></a><span data-ttu-id="7ac43-104">Тип ресурса deviceCategory</span><span class="sxs-lookup"><span data-stu-id="7ac43-104">deviceCategory resource type</span></span>

> <span data-ttu-id="7ac43-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7ac43-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ac43-106">Категории устройств используются для упорядочивания устройств.</span><span class="sxs-lookup"><span data-stu-id="7ac43-106">Device categories provides a way to organize your devices.</span></span> <span data-ttu-id="7ac43-107">Используя категории устройств, администраторы могут определить собственные категории, применимые к их организации.</span><span class="sxs-lookup"><span data-stu-id="7ac43-107">Using device categories, company administrators can define their own categories that make sense to their company.</span></span><span data-ttu-id="7ac43-108">Эти категории затем можно применить к устройству в консоли Azure Intune или выбрать во время регистрации устройства пользователем.</span><span class="sxs-lookup"><span data-stu-id="7ac43-108"> These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment.</span></span> <span data-ttu-id="7ac43-109">На основе категорий устройств вы можете фильтровать отчеты и создавать динамические группы устройств Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="7ac43-109">You can filter reports and create dynamic Azure Active Directory device groups based on device categories.</span></span>

## <a name="methods"></a><span data-ttu-id="7ac43-110">Методы</span><span class="sxs-lookup"><span data-stu-id="7ac43-110">Methods</span></span>
|<span data-ttu-id="7ac43-111">Метод</span><span class="sxs-lookup"><span data-stu-id="7ac43-111">Method</span></span>|<span data-ttu-id="7ac43-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7ac43-112">Return Type</span></span>|<span data-ttu-id="7ac43-113">Описание</span><span class="sxs-lookup"><span data-stu-id="7ac43-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ac43-114">Коллекция [перечисление devicecategory списка](../api/intune-shared-devicecategory-list.md)</span><span class="sxs-lookup"><span data-stu-id="7ac43-114">[List deviceCategories](../api/intune-shared-devicecategory-list.md) collection</span></span>|<span data-ttu-id="7ac43-115">Список свойств и связей объектов [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="7ac43-115">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>|
|[<span data-ttu-id="7ac43-116">Получение объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="7ac43-116">Get deviceCategory</span></span>](../api/intune-shared-devicecategory-get.md)|<span data-ttu-id="7ac43-117">Чтение свойств и связей объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="7ac43-117">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="7ac43-118">Создание объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="7ac43-118">Create deviceCategory</span></span>](../api/intune-shared-devicecategory-create.md)|<span data-ttu-id="7ac43-119">Создание объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="7ac43-119">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|<span data-ttu-id="7ac43-120">[Удаление deviceCategory](../api/intune-shared-devicecategory-delete.md).</span><span class="sxs-lookup"><span data-stu-id="7ac43-120">[Delete deviceCategory](../api/intune-shared-devicecategory-delete.md).</span></span>|
|[<span data-ttu-id="7ac43-121">Обновление объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="7ac43-121">Update deviceCategory</span></span>](../api/intune-shared-devicecategory-update.md)|<span data-ttu-id="7ac43-122">Обновление свойств объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="7ac43-122">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7ac43-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="7ac43-123">Properties</span></span>
|<span data-ttu-id="7ac43-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="7ac43-124">Property</span></span>|<span data-ttu-id="7ac43-125">Тип</span><span class="sxs-lookup"><span data-stu-id="7ac43-125">Type</span></span>|<span data-ttu-id="7ac43-126">Описание</span><span class="sxs-lookup"><span data-stu-id="7ac43-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ac43-127">id</span><span class="sxs-lookup"><span data-stu-id="7ac43-127">id</span></span>|<span data-ttu-id="7ac43-128">String</span><span class="sxs-lookup"><span data-stu-id="7ac43-128">String</span></span>|<span data-ttu-id="7ac43-129">Уникальный идентификатор категории устройства.</span><span class="sxs-lookup"><span data-stu-id="7ac43-129">Unique identifier for the device category.</span></span> <span data-ttu-id="7ac43-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7ac43-130">Read-only.</span></span>|
|<span data-ttu-id="7ac43-131">**Подключение**</span><span class="sxs-lookup"><span data-stu-id="7ac43-131">**Onboarding**</span></span>|
|<span data-ttu-id="7ac43-132">displayName</span><span class="sxs-lookup"><span data-stu-id="7ac43-132">displayName</span></span>|<span data-ttu-id="7ac43-133">String</span><span class="sxs-lookup"><span data-stu-id="7ac43-133">String</span></span>|<span data-ttu-id="7ac43-134">Отображаемое имя категории устройств.</span><span class="sxs-lookup"><span data-stu-id="7ac43-134">Display name for the device category.</span></span>|
|<span data-ttu-id="7ac43-135">description</span><span class="sxs-lookup"><span data-stu-id="7ac43-135">description</span></span>|<span data-ttu-id="7ac43-136">String</span><span class="sxs-lookup"><span data-stu-id="7ac43-136">String</span></span>|<span data-ttu-id="7ac43-137">Необязательное описание категории устройств.</span><span class="sxs-lookup"><span data-stu-id="7ac43-137">Optional description for the device category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7ac43-138">Связи</span><span class="sxs-lookup"><span data-stu-id="7ac43-138">Relationships</span></span>
<span data-ttu-id="7ac43-139">Нет</span><span class="sxs-lookup"><span data-stu-id="7ac43-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7ac43-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7ac43-140">JSON Representation</span></span>
<span data-ttu-id="7ac43-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7ac43-141">Here is a JSON representation of the resource.</span></span>
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



