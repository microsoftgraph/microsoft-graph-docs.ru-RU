---
title: Тип ресурса deviceEnrollmentConfiguration
description: Базовый класс конфигурации регистрации устройств
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bd21f5dea3bab467abf1b19754ada88a4fbb531a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523718"
---
# <a name="deviceenrollmentconfiguration-resource-type"></a><span data-ttu-id="a6886-103">Тип ресурса deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="a6886-103">deviceEnrollmentConfiguration resource type</span></span>

<span data-ttu-id="a6886-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a6886-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a6886-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6886-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a6886-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a6886-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6886-107">Базовый класс конфигурации регистрации устройств</span><span class="sxs-lookup"><span data-stu-id="a6886-107">The Base Class of Device Enrollment Configuration</span></span>

## <a name="methods"></a><span data-ttu-id="a6886-108">Методы</span><span class="sxs-lookup"><span data-stu-id="a6886-108">Methods</span></span>
|<span data-ttu-id="a6886-109">Метод</span><span class="sxs-lookup"><span data-stu-id="a6886-109">Method</span></span>|<span data-ttu-id="a6886-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a6886-110">Return Type</span></span>|<span data-ttu-id="a6886-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a6886-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a6886-112">Список объектов deviceEnrollmentConfigurations</span><span class="sxs-lookup"><span data-stu-id="a6886-112">List deviceEnrollmentConfigurations</span></span>](../api/intune-shared-deviceenrollmentconfiguration-list.md)|<span data-ttu-id="a6886-113">Коллекция [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6886-113">[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) collection</span></span>|<span data-ttu-id="a6886-114">Список свойств и связей объектов [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a6886-114">List properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="a6886-115">Получение объекта deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="a6886-115">Get deviceEnrollmentConfiguration</span></span>](../api/intune-shared-deviceenrollmentconfiguration-get.md)|[<span data-ttu-id="a6886-116">deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="a6886-116">deviceEnrollmentConfiguration</span></span>](../resources/intune-shared-deviceenrollmentconfiguration.md)|<span data-ttu-id="a6886-117">Чтение свойств и связей объекта [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a6886-117">Read properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) object.</span></span>|
|<span data-ttu-id="a6886-118">**Адаптация**</span><span class="sxs-lookup"><span data-stu-id="a6886-118">**Onboarding**</span></span>|
|[<span data-ttu-id="a6886-119">Действие setPriority</span><span class="sxs-lookup"><span data-stu-id="a6886-119">setPriority action</span></span>](../api/intune-shared-deviceenrollmentconfiguration-setpriority.md)|<span data-ttu-id="a6886-120">Нет</span><span class="sxs-lookup"><span data-stu-id="a6886-120">None</span></span>|<span data-ttu-id="a6886-121">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a6886-121">Not yet documented</span></span>|
|[<span data-ttu-id="a6886-122">Действие assign</span><span class="sxs-lookup"><span data-stu-id="a6886-122">assign action</span></span>](../api/intune-shared-deviceenrollmentconfiguration-assign.md)|<span data-ttu-id="a6886-123">Нет</span><span class="sxs-lookup"><span data-stu-id="a6886-123">None</span></span>|<span data-ttu-id="a6886-124">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a6886-124">Not yet documented</span></span>|
|<span data-ttu-id="a6886-125">**Набор политик**</span><span class="sxs-lookup"><span data-stu-id="a6886-125">**Policy Set**</span></span>|
|[<span data-ttu-id="a6886-126">действие Хаспайлоадлинкс</span><span class="sxs-lookup"><span data-stu-id="a6886-126">hasPayloadLinks action</span></span>](../api/intune-shared-deviceenrollmentconfiguration-haspayloadlinks.md)|<span data-ttu-id="a6886-127">Коллекция [хаспайлоадлинкресултитем](../resources/intune-policyset-haspayloadlinkresultitem.md)</span><span class="sxs-lookup"><span data-stu-id="a6886-127">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection</span></span>|<span data-ttu-id="a6886-128">Пока не задокументировано</span><span class="sxs-lookup"><span data-stu-id="a6886-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="a6886-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="a6886-129">Properties</span></span>
|<span data-ttu-id="a6886-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a6886-130">Property</span></span>|<span data-ttu-id="a6886-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a6886-131">Type</span></span>|<span data-ttu-id="a6886-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a6886-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6886-133">id</span><span class="sxs-lookup"><span data-stu-id="a6886-133">id</span></span>|<span data-ttu-id="a6886-134">String</span><span class="sxs-lookup"><span data-stu-id="a6886-134">String</span></span>|<span data-ttu-id="a6886-135">Уникальный идентификатор для учетной записи</span><span class="sxs-lookup"><span data-stu-id="a6886-135">Unique Identifier for the account</span></span>|
|<span data-ttu-id="a6886-136">displayName</span><span class="sxs-lookup"><span data-stu-id="a6886-136">displayName</span></span>|<span data-ttu-id="a6886-137">Строка</span><span class="sxs-lookup"><span data-stu-id="a6886-137">String</span></span>|<span data-ttu-id="a6886-138">Отображаемое имя конфигурации регистрации устройств</span><span class="sxs-lookup"><span data-stu-id="a6886-138">The display name of the device enrollment configuration</span></span>|
|<span data-ttu-id="a6886-139">description</span><span class="sxs-lookup"><span data-stu-id="a6886-139">description</span></span>|<span data-ttu-id="a6886-140">String</span><span class="sxs-lookup"><span data-stu-id="a6886-140">String</span></span>|<span data-ttu-id="a6886-141">Описание конфигурации регистрации устройств</span><span class="sxs-lookup"><span data-stu-id="a6886-141">The description of the device enrollment configuration</span></span>|
|<span data-ttu-id="a6886-142">priority</span><span class="sxs-lookup"><span data-stu-id="a6886-142">priority</span></span>|<span data-ttu-id="a6886-143">Int32</span><span class="sxs-lookup"><span data-stu-id="a6886-143">Int32</span></span>|<span data-ttu-id="a6886-144">Priority используется, когда пользователь существует в нескольких группах, которым назначена Настройка регистрации.</span><span class="sxs-lookup"><span data-stu-id="a6886-144">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="a6886-145">Пользователи подчиняются только конфигурации с наименьшим значением приоритета.</span><span class="sxs-lookup"><span data-stu-id="a6886-145">Users are subject only to the configuration with the lowest priority value.</span></span>|
|<span data-ttu-id="a6886-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a6886-146">createdDateTime</span></span>|<span data-ttu-id="a6886-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6886-147">DateTimeOffset</span></span>|<span data-ttu-id="a6886-148">Созданная Дата и время в формате UTC для конфигурации регистрации устройств</span><span class="sxs-lookup"><span data-stu-id="a6886-148">Created date time in UTC of the device enrollment configuration</span></span>|
|<span data-ttu-id="a6886-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a6886-149">lastModifiedDateTime</span></span>|<span data-ttu-id="a6886-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6886-150">DateTimeOffset</span></span>|<span data-ttu-id="a6886-151">Дата и время последнего изменения конфигурации регистрации устройств в формате UTC</span><span class="sxs-lookup"><span data-stu-id="a6886-151">Last modified date time in UTC of the device enrollment configuration</span></span>|
|<span data-ttu-id="a6886-152">version</span><span class="sxs-lookup"><span data-stu-id="a6886-152">version</span></span>|<span data-ttu-id="a6886-153">Int32</span><span class="sxs-lookup"><span data-stu-id="a6886-153">Int32</span></span>|<span data-ttu-id="a6886-154">Версия конфигурации регистрации устройств</span><span class="sxs-lookup"><span data-stu-id="a6886-154">The version of the device enrollment configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="a6886-155">Связи</span><span class="sxs-lookup"><span data-stu-id="a6886-155">Relationships</span></span>
|<span data-ttu-id="a6886-156">Связь</span><span class="sxs-lookup"><span data-stu-id="a6886-156">Relationship</span></span>|<span data-ttu-id="a6886-157">Тип</span><span class="sxs-lookup"><span data-stu-id="a6886-157">Type</span></span>|<span data-ttu-id="a6886-158">Описание</span><span class="sxs-lookup"><span data-stu-id="a6886-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6886-159">**Адаптация**</span><span class="sxs-lookup"><span data-stu-id="a6886-159">**Onboarding**</span></span>|
|<span data-ttu-id="a6886-160">assignments</span><span class="sxs-lookup"><span data-stu-id="a6886-160">assignments</span></span>|<span data-ttu-id="a6886-161">Коллекция [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="a6886-161">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) collection</span></span>|<span data-ttu-id="a6886-162">Список назначений групп для профиля конфигурации устройства</span><span class="sxs-lookup"><span data-stu-id="a6886-162">The list of group assignments for the device configuration profile</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a6886-163">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a6886-163">JSON Representation</span></span>
<span data-ttu-id="a6886-164">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a6886-164">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceEnrollmentConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentConfiguration",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "priority": 1024,
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": 1024
}
```



