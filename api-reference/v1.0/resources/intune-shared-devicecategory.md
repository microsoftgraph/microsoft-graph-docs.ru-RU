---
title: Тип ресурса deviceCategory
description: Эти категории затем можно применить к устройству в консоли Azure Intune или выбрать во время регистрации устройства пользователем. На основе категорий устройств вы можете фильтровать отчеты и создавать динамические группы устройств Azure Active Directory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 067e7894cc5c5daa4cd73c5bb5ba88f66b283366
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732758"
---
# <a name="devicecategory-resource-type"></a><span data-ttu-id="d201b-104">Тип ресурса deviceCategory</span><span class="sxs-lookup"><span data-stu-id="d201b-104">deviceCategory resource type</span></span>

<span data-ttu-id="d201b-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d201b-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d201b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d201b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d201b-107">Категории устройств используются для упорядочивания устройств.</span><span class="sxs-lookup"><span data-stu-id="d201b-107">Device categories provides a way to organize your devices.</span></span> <span data-ttu-id="d201b-108">Используя категории устройств, администраторы могут определить собственные категории, применимые к их организации.</span><span class="sxs-lookup"><span data-stu-id="d201b-108">Using device categories, company administrators can define their own categories that make sense to their company.</span></span> <span data-ttu-id="d201b-109">Эти категории затем можно применить к устройству в консоли Azure Intune или выбрать во время регистрации устройства пользователем.</span><span class="sxs-lookup"><span data-stu-id="d201b-109">These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment.</span></span> <span data-ttu-id="d201b-110">На основе категорий устройств вы можете фильтровать отчеты и создавать динамические группы устройств Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d201b-110">You can filter reports and create dynamic Azure Active Directory device groups based on device categories.</span></span>

## <a name="methods"></a><span data-ttu-id="d201b-111">Методы</span><span class="sxs-lookup"><span data-stu-id="d201b-111">Methods</span></span>
|<span data-ttu-id="d201b-112">Метод</span><span class="sxs-lookup"><span data-stu-id="d201b-112">Method</span></span>|<span data-ttu-id="d201b-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d201b-113">Return Type</span></span>|<span data-ttu-id="d201b-114">Описание</span><span class="sxs-lookup"><span data-stu-id="d201b-114">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d201b-115">[Коллекция list deviceCategories](../api/intune-shared-devicecategory-list.md)</span><span class="sxs-lookup"><span data-stu-id="d201b-115">[List deviceCategories](../api/intune-shared-devicecategory-list.md) collection</span></span>|<span data-ttu-id="d201b-116">Список свойств и связей объектов [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="d201b-116">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>|
|[<span data-ttu-id="d201b-117">Получение объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="d201b-117">Get deviceCategory</span></span>](../api/intune-shared-devicecategory-get.md)|<span data-ttu-id="d201b-118">Чтение свойств и связей объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="d201b-118">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="d201b-119">Создание объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="d201b-119">Create deviceCategory</span></span>](../api/intune-shared-devicecategory-create.md)|<span data-ttu-id="d201b-120">Создание объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="d201b-120">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|<span data-ttu-id="d201b-121">[Удаление deviceCategory](../api/intune-shared-devicecategory-delete.md).</span><span class="sxs-lookup"><span data-stu-id="d201b-121">[Delete deviceCategory](../api/intune-shared-devicecategory-delete.md).</span></span>|
|[<span data-ttu-id="d201b-122">Обновление объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="d201b-122">Update deviceCategory</span></span>](../api/intune-shared-devicecategory-update.md)|<span data-ttu-id="d201b-123">Обновление свойств объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="d201b-123">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d201b-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="d201b-124">Properties</span></span>
|<span data-ttu-id="d201b-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="d201b-125">Property</span></span>|<span data-ttu-id="d201b-126">Тип</span><span class="sxs-lookup"><span data-stu-id="d201b-126">Type</span></span>|<span data-ttu-id="d201b-127">Описание</span><span class="sxs-lookup"><span data-stu-id="d201b-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d201b-128">id</span><span class="sxs-lookup"><span data-stu-id="d201b-128">id</span></span>|<span data-ttu-id="d201b-129">String</span><span class="sxs-lookup"><span data-stu-id="d201b-129">String</span></span>|<span data-ttu-id="d201b-130">Уникальный идентификатор категории устройства.</span><span class="sxs-lookup"><span data-stu-id="d201b-130">Unique identifier for the device category.</span></span> <span data-ttu-id="d201b-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d201b-131">Read-only.</span></span>|
|<span data-ttu-id="d201b-132">**Адаптация**</span><span class="sxs-lookup"><span data-stu-id="d201b-132">**Onboarding**</span></span>|
|<span data-ttu-id="d201b-133">displayName</span><span class="sxs-lookup"><span data-stu-id="d201b-133">displayName</span></span>|<span data-ttu-id="d201b-134">String</span><span class="sxs-lookup"><span data-stu-id="d201b-134">String</span></span>|<span data-ttu-id="d201b-135">Отображаемое имя категории устройств.</span><span class="sxs-lookup"><span data-stu-id="d201b-135">Display name for the device category.</span></span>|
|<span data-ttu-id="d201b-136">description</span><span class="sxs-lookup"><span data-stu-id="d201b-136">description</span></span>|<span data-ttu-id="d201b-137">String</span><span class="sxs-lookup"><span data-stu-id="d201b-137">String</span></span>|<span data-ttu-id="d201b-138">Необязательное описание категории устройств.</span><span class="sxs-lookup"><span data-stu-id="d201b-138">Optional description for the device category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d201b-139">Отношения</span><span class="sxs-lookup"><span data-stu-id="d201b-139">Relationships</span></span>
<span data-ttu-id="d201b-140">Нет</span><span class="sxs-lookup"><span data-stu-id="d201b-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d201b-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d201b-141">JSON Representation</span></span>
<span data-ttu-id="d201b-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d201b-142">Here is a JSON representation of the resource.</span></span>
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









