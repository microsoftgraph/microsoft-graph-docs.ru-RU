---
title: Тип ресурса deviceEnrollmentConfiguration
description: Базовый класс конфигурации регистрации устройств
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f7e15322dd41eaa15e4b00c83a59b361059bbedb
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49287664"
---
# <a name="deviceenrollmentconfiguration-resource-type"></a><span data-ttu-id="cb20c-103">Тип ресурса deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="cb20c-103">deviceEnrollmentConfiguration resource type</span></span>

<span data-ttu-id="cb20c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb20c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cb20c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb20c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cb20c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cb20c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb20c-107">Базовый класс конфигурации регистрации устройств</span><span class="sxs-lookup"><span data-stu-id="cb20c-107">The Base Class of Device Enrollment Configuration</span></span>

## <a name="methods"></a><span data-ttu-id="cb20c-108">Методы</span><span class="sxs-lookup"><span data-stu-id="cb20c-108">Methods</span></span>
|<span data-ttu-id="cb20c-109">Метод</span><span class="sxs-lookup"><span data-stu-id="cb20c-109">Method</span></span>|<span data-ttu-id="cb20c-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="cb20c-110">Return Type</span></span>|<span data-ttu-id="cb20c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="cb20c-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cb20c-112">Список объектов deviceEnrollmentConfigurations</span><span class="sxs-lookup"><span data-stu-id="cb20c-112">List deviceEnrollmentConfigurations</span></span>](../api/intune-shared-deviceenrollmentconfiguration-list.md)|<span data-ttu-id="cb20c-113">Коллекция [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cb20c-113">[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) collection</span></span>|<span data-ttu-id="cb20c-114">Список свойств и связей объектов [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cb20c-114">List properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="cb20c-115">Получение объекта deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="cb20c-115">Get deviceEnrollmentConfiguration</span></span>](../api/intune-shared-deviceenrollmentconfiguration-get.md)|[<span data-ttu-id="cb20c-116">deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="cb20c-116">deviceEnrollmentConfiguration</span></span>](../resources/intune-shared-deviceenrollmentconfiguration.md)|<span data-ttu-id="cb20c-117">Чтение свойств и связей объекта [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cb20c-117">Read properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) object.</span></span>|
|<span data-ttu-id="cb20c-118">**Адаптация**</span><span class="sxs-lookup"><span data-stu-id="cb20c-118">**Onboarding**</span></span>|
|[<span data-ttu-id="cb20c-119">Действие setPriority</span><span class="sxs-lookup"><span data-stu-id="cb20c-119">setPriority action</span></span>](../api/intune-shared-deviceenrollmentconfiguration-setpriority.md)|<span data-ttu-id="cb20c-120">Нет</span><span class="sxs-lookup"><span data-stu-id="cb20c-120">None</span></span>|<span data-ttu-id="cb20c-121">Н/Д</span><span class="sxs-lookup"><span data-stu-id="cb20c-121">Not yet documented</span></span>|
|[<span data-ttu-id="cb20c-122">Действие assign</span><span class="sxs-lookup"><span data-stu-id="cb20c-122">assign action</span></span>](../api/intune-shared-deviceenrollmentconfiguration-assign.md)|<span data-ttu-id="cb20c-123">Нет</span><span class="sxs-lookup"><span data-stu-id="cb20c-123">None</span></span>|<span data-ttu-id="cb20c-124">Н/Д</span><span class="sxs-lookup"><span data-stu-id="cb20c-124">Not yet documented</span></span>|
|<span data-ttu-id="cb20c-125">**Набор политик**</span><span class="sxs-lookup"><span data-stu-id="cb20c-125">**Policy Set**</span></span>|
|[<span data-ttu-id="cb20c-126">действие Хаспайлоадлинкс</span><span class="sxs-lookup"><span data-stu-id="cb20c-126">hasPayloadLinks action</span></span>](../api/intune-shared-deviceenrollmentconfiguration-haspayloadlinks.md)|<span data-ttu-id="cb20c-127">Коллекция [хаспайлоадлинкресултитем](../resources/intune-policyset-haspayloadlinkresultitem.md)</span><span class="sxs-lookup"><span data-stu-id="cb20c-127">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection</span></span>|<span data-ttu-id="cb20c-128">Н/Д</span><span class="sxs-lookup"><span data-stu-id="cb20c-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="cb20c-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="cb20c-129">Properties</span></span>
|<span data-ttu-id="cb20c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="cb20c-130">Property</span></span>|<span data-ttu-id="cb20c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="cb20c-131">Type</span></span>|<span data-ttu-id="cb20c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="cb20c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb20c-133">id</span><span class="sxs-lookup"><span data-stu-id="cb20c-133">id</span></span>|<span data-ttu-id="cb20c-134">String</span><span class="sxs-lookup"><span data-stu-id="cb20c-134">String</span></span>|<span data-ttu-id="cb20c-135">Уникальный идентификатор для учетной записи</span><span class="sxs-lookup"><span data-stu-id="cb20c-135">Unique Identifier for the account</span></span>|
|<span data-ttu-id="cb20c-136">displayName</span><span class="sxs-lookup"><span data-stu-id="cb20c-136">displayName</span></span>|<span data-ttu-id="cb20c-137">String</span><span class="sxs-lookup"><span data-stu-id="cb20c-137">String</span></span>|<span data-ttu-id="cb20c-138">Отображаемое имя конфигурации регистрации устройств</span><span class="sxs-lookup"><span data-stu-id="cb20c-138">The display name of the device enrollment configuration</span></span>|
|<span data-ttu-id="cb20c-139">description</span><span class="sxs-lookup"><span data-stu-id="cb20c-139">description</span></span>|<span data-ttu-id="cb20c-140">String</span><span class="sxs-lookup"><span data-stu-id="cb20c-140">String</span></span>|<span data-ttu-id="cb20c-141">Описание конфигурации регистрации устройств</span><span class="sxs-lookup"><span data-stu-id="cb20c-141">The description of the device enrollment configuration</span></span>|
|<span data-ttu-id="cb20c-142">priority</span><span class="sxs-lookup"><span data-stu-id="cb20c-142">priority</span></span>|<span data-ttu-id="cb20c-143">Int32</span><span class="sxs-lookup"><span data-stu-id="cb20c-143">Int32</span></span>|<span data-ttu-id="cb20c-144">Priority используется, когда пользователь существует в нескольких группах, которым назначена Настройка регистрации.</span><span class="sxs-lookup"><span data-stu-id="cb20c-144">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="cb20c-145">Пользователи подчиняются только конфигурации с наименьшим значением приоритета.</span><span class="sxs-lookup"><span data-stu-id="cb20c-145">Users are subject only to the configuration with the lowest priority value.</span></span>|
|<span data-ttu-id="cb20c-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cb20c-146">createdDateTime</span></span>|<span data-ttu-id="cb20c-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb20c-147">DateTimeOffset</span></span>|<span data-ttu-id="cb20c-148">Созданная Дата и время в формате UTC для конфигурации регистрации устройств</span><span class="sxs-lookup"><span data-stu-id="cb20c-148">Created date time in UTC of the device enrollment configuration</span></span>|
|<span data-ttu-id="cb20c-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cb20c-149">lastModifiedDateTime</span></span>|<span data-ttu-id="cb20c-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb20c-150">DateTimeOffset</span></span>|<span data-ttu-id="cb20c-151">Дата и время последнего изменения конфигурации регистрации устройств в формате UTC</span><span class="sxs-lookup"><span data-stu-id="cb20c-151">Last modified date time in UTC of the device enrollment configuration</span></span>|
|<span data-ttu-id="cb20c-152">version</span><span class="sxs-lookup"><span data-stu-id="cb20c-152">version</span></span>|<span data-ttu-id="cb20c-153">Int32</span><span class="sxs-lookup"><span data-stu-id="cb20c-153">Int32</span></span>|<span data-ttu-id="cb20c-154">Версия конфигурации регистрации устройств</span><span class="sxs-lookup"><span data-stu-id="cb20c-154">The version of the device enrollment configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="cb20c-155">Связи</span><span class="sxs-lookup"><span data-stu-id="cb20c-155">Relationships</span></span>
|<span data-ttu-id="cb20c-156">Связь</span><span class="sxs-lookup"><span data-stu-id="cb20c-156">Relationship</span></span>|<span data-ttu-id="cb20c-157">Тип</span><span class="sxs-lookup"><span data-stu-id="cb20c-157">Type</span></span>|<span data-ttu-id="cb20c-158">Описание</span><span class="sxs-lookup"><span data-stu-id="cb20c-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb20c-159">**Адаптация**</span><span class="sxs-lookup"><span data-stu-id="cb20c-159">**Onboarding**</span></span>|
|<span data-ttu-id="cb20c-160">assignments</span><span class="sxs-lookup"><span data-stu-id="cb20c-160">assignments</span></span>|<span data-ttu-id="cb20c-161">Коллекция [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="cb20c-161">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) collection</span></span>|<span data-ttu-id="cb20c-162">Список назначений групп для профиля конфигурации устройства</span><span class="sxs-lookup"><span data-stu-id="cb20c-162">The list of group assignments for the device configuration profile</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cb20c-163">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cb20c-163">JSON Representation</span></span>
<span data-ttu-id="cb20c-164">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cb20c-164">Here is a JSON representation of the resource.</span></span>
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




