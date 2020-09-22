---
title: Тип ресурса deviceEnrollmentConfiguration
description: Базовый класс конфигурации регистрации устройств
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d7e5c2a1eef152ba613be8909ca80f6040305720
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055331"
---
# <a name="deviceenrollmentconfiguration-resource-type"></a><span data-ttu-id="d0355-103">Тип ресурса deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="d0355-103">deviceEnrollmentConfiguration resource type</span></span>

<span data-ttu-id="d0355-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0355-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d0355-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0355-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d0355-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d0355-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0355-107">Базовый класс конфигурации регистрации устройств</span><span class="sxs-lookup"><span data-stu-id="d0355-107">The Base Class of Device Enrollment Configuration</span></span>

## <a name="methods"></a><span data-ttu-id="d0355-108">Методы</span><span class="sxs-lookup"><span data-stu-id="d0355-108">Methods</span></span>
|<span data-ttu-id="d0355-109">Метод</span><span class="sxs-lookup"><span data-stu-id="d0355-109">Method</span></span>|<span data-ttu-id="d0355-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d0355-110">Return Type</span></span>|<span data-ttu-id="d0355-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d0355-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d0355-112">Список объектов deviceEnrollmentConfigurations</span><span class="sxs-lookup"><span data-stu-id="d0355-112">List deviceEnrollmentConfigurations</span></span>](../api/intune-shared-deviceenrollmentconfiguration-list.md)|<span data-ttu-id="d0355-113">Коллекция [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d0355-113">[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) collection</span></span>|<span data-ttu-id="d0355-114">Список свойств и связей объектов [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0355-114">List properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="d0355-115">Получение объекта deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="d0355-115">Get deviceEnrollmentConfiguration</span></span>](../api/intune-shared-deviceenrollmentconfiguration-get.md)|[<span data-ttu-id="d0355-116">deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="d0355-116">deviceEnrollmentConfiguration</span></span>](../resources/intune-shared-deviceenrollmentconfiguration.md)|<span data-ttu-id="d0355-117">Чтение свойств и связей объекта [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0355-117">Read properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) object.</span></span>|
|<span data-ttu-id="d0355-118">**Адаптация**</span><span class="sxs-lookup"><span data-stu-id="d0355-118">**Onboarding**</span></span>|
|[<span data-ttu-id="d0355-119">Действие setPriority</span><span class="sxs-lookup"><span data-stu-id="d0355-119">setPriority action</span></span>](../api/intune-shared-deviceenrollmentconfiguration-setpriority.md)|<span data-ttu-id="d0355-120">Нет</span><span class="sxs-lookup"><span data-stu-id="d0355-120">None</span></span>|<span data-ttu-id="d0355-121">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d0355-121">Not yet documented</span></span>|
|[<span data-ttu-id="d0355-122">Действие assign</span><span class="sxs-lookup"><span data-stu-id="d0355-122">assign action</span></span>](../api/intune-shared-deviceenrollmentconfiguration-assign.md)|<span data-ttu-id="d0355-123">Нет</span><span class="sxs-lookup"><span data-stu-id="d0355-123">None</span></span>|<span data-ttu-id="d0355-124">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d0355-124">Not yet documented</span></span>|
|<span data-ttu-id="d0355-125">**Набор политик**</span><span class="sxs-lookup"><span data-stu-id="d0355-125">**Policy Set**</span></span>|
|[<span data-ttu-id="d0355-126">действие Хаспайлоадлинкс</span><span class="sxs-lookup"><span data-stu-id="d0355-126">hasPayloadLinks action</span></span>](../api/intune-shared-deviceenrollmentconfiguration-haspayloadlinks.md)|<span data-ttu-id="d0355-127">Коллекция [хаспайлоадлинкресултитем](../resources/intune-policyset-haspayloadlinkresultitem.md)</span><span class="sxs-lookup"><span data-stu-id="d0355-127">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection</span></span>|<span data-ttu-id="d0355-128">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d0355-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="d0355-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="d0355-129">Properties</span></span>
|<span data-ttu-id="d0355-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d0355-130">Property</span></span>|<span data-ttu-id="d0355-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d0355-131">Type</span></span>|<span data-ttu-id="d0355-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d0355-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0355-133">id</span><span class="sxs-lookup"><span data-stu-id="d0355-133">id</span></span>|<span data-ttu-id="d0355-134">String</span><span class="sxs-lookup"><span data-stu-id="d0355-134">String</span></span>|<span data-ttu-id="d0355-135">Уникальный идентификатор для учетной записи</span><span class="sxs-lookup"><span data-stu-id="d0355-135">Unique Identifier for the account</span></span>|
|<span data-ttu-id="d0355-136">displayName</span><span class="sxs-lookup"><span data-stu-id="d0355-136">displayName</span></span>|<span data-ttu-id="d0355-137">String</span><span class="sxs-lookup"><span data-stu-id="d0355-137">String</span></span>|<span data-ttu-id="d0355-138">Отображаемое имя конфигурации регистрации устройств</span><span class="sxs-lookup"><span data-stu-id="d0355-138">The display name of the device enrollment configuration</span></span>|
|<span data-ttu-id="d0355-139">description</span><span class="sxs-lookup"><span data-stu-id="d0355-139">description</span></span>|<span data-ttu-id="d0355-140">String</span><span class="sxs-lookup"><span data-stu-id="d0355-140">String</span></span>|<span data-ttu-id="d0355-141">Описание конфигурации регистрации устройств</span><span class="sxs-lookup"><span data-stu-id="d0355-141">The description of the device enrollment configuration</span></span>|
|<span data-ttu-id="d0355-142">priority</span><span class="sxs-lookup"><span data-stu-id="d0355-142">priority</span></span>|<span data-ttu-id="d0355-143">Int32</span><span class="sxs-lookup"><span data-stu-id="d0355-143">Int32</span></span>|<span data-ttu-id="d0355-144">Priority используется, когда пользователь существует в нескольких группах, которым назначена Настройка регистрации.</span><span class="sxs-lookup"><span data-stu-id="d0355-144">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="d0355-145">Пользователи подчиняются только конфигурации с наименьшим значением приоритета.</span><span class="sxs-lookup"><span data-stu-id="d0355-145">Users are subject only to the configuration with the lowest priority value.</span></span>|
|<span data-ttu-id="d0355-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d0355-146">createdDateTime</span></span>|<span data-ttu-id="d0355-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0355-147">DateTimeOffset</span></span>|<span data-ttu-id="d0355-148">Созданная Дата и время в формате UTC для конфигурации регистрации устройств</span><span class="sxs-lookup"><span data-stu-id="d0355-148">Created date time in UTC of the device enrollment configuration</span></span>|
|<span data-ttu-id="d0355-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d0355-149">lastModifiedDateTime</span></span>|<span data-ttu-id="d0355-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0355-150">DateTimeOffset</span></span>|<span data-ttu-id="d0355-151">Дата и время последнего изменения конфигурации регистрации устройств в формате UTC</span><span class="sxs-lookup"><span data-stu-id="d0355-151">Last modified date time in UTC of the device enrollment configuration</span></span>|
|<span data-ttu-id="d0355-152">version</span><span class="sxs-lookup"><span data-stu-id="d0355-152">version</span></span>|<span data-ttu-id="d0355-153">Int32</span><span class="sxs-lookup"><span data-stu-id="d0355-153">Int32</span></span>|<span data-ttu-id="d0355-154">Версия конфигурации регистрации устройств</span><span class="sxs-lookup"><span data-stu-id="d0355-154">The version of the device enrollment configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="d0355-155">Связи</span><span class="sxs-lookup"><span data-stu-id="d0355-155">Relationships</span></span>
|<span data-ttu-id="d0355-156">Связь</span><span class="sxs-lookup"><span data-stu-id="d0355-156">Relationship</span></span>|<span data-ttu-id="d0355-157">Тип</span><span class="sxs-lookup"><span data-stu-id="d0355-157">Type</span></span>|<span data-ttu-id="d0355-158">Описание</span><span class="sxs-lookup"><span data-stu-id="d0355-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0355-159">**Адаптация**</span><span class="sxs-lookup"><span data-stu-id="d0355-159">**Onboarding**</span></span>|
|<span data-ttu-id="d0355-160">assignments</span><span class="sxs-lookup"><span data-stu-id="d0355-160">assignments</span></span>|<span data-ttu-id="d0355-161">Коллекция [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="d0355-161">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) collection</span></span>|<span data-ttu-id="d0355-162">Список назначений групп для профиля конфигурации устройства</span><span class="sxs-lookup"><span data-stu-id="d0355-162">The list of group assignments for the device configuration profile</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d0355-163">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d0355-163">JSON Representation</span></span>
<span data-ttu-id="d0355-164">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d0355-164">Here is a JSON representation of the resource.</span></span>
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






