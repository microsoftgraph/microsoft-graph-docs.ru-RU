---
title: Тип ресурса deviceEnrollmentConfiguration
description: Базовый класс конфигурации регистрации устройств
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ad0543a521d66ed6e515afe806b583e247a75a07
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42771182"
---
# <a name="deviceenrollmentconfiguration-resource-type"></a><span data-ttu-id="be5ed-103">Тип ресурса deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="be5ed-103">deviceEnrollmentConfiguration resource type</span></span>

> <span data-ttu-id="be5ed-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be5ed-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="be5ed-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="be5ed-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be5ed-106">Базовый класс конфигурации регистрации устройств</span><span class="sxs-lookup"><span data-stu-id="be5ed-106">The Base Class of Device Enrollment Configuration</span></span>

## <a name="methods"></a><span data-ttu-id="be5ed-107">Методы</span><span class="sxs-lookup"><span data-stu-id="be5ed-107">Methods</span></span>
|<span data-ttu-id="be5ed-108">Метод</span><span class="sxs-lookup"><span data-stu-id="be5ed-108">Method</span></span>|<span data-ttu-id="be5ed-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="be5ed-109">Return Type</span></span>|<span data-ttu-id="be5ed-110">Описание</span><span class="sxs-lookup"><span data-stu-id="be5ed-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="be5ed-111">Список объектов deviceEnrollmentConfigurations</span><span class="sxs-lookup"><span data-stu-id="be5ed-111">List deviceEnrollmentConfigurations</span></span>](../api/intune-shared-deviceenrollmentconfiguration-list.md)|<span data-ttu-id="be5ed-112">Коллекция [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="be5ed-112">[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) collection</span></span>|<span data-ttu-id="be5ed-113">Список свойств и связей объектов [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="be5ed-113">List properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="be5ed-114">Получение объекта deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="be5ed-114">Get deviceEnrollmentConfiguration</span></span>](../api/intune-shared-deviceenrollmentconfiguration-get.md)|[<span data-ttu-id="be5ed-115">deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="be5ed-115">deviceEnrollmentConfiguration</span></span>](../resources/intune-shared-deviceenrollmentconfiguration.md)|<span data-ttu-id="be5ed-116">Чтение свойств и связей объекта [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="be5ed-116">Read properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) object.</span></span>|
|<span data-ttu-id="be5ed-117">**Адаптация**</span><span class="sxs-lookup"><span data-stu-id="be5ed-117">**Onboarding**</span></span>|
|[<span data-ttu-id="be5ed-118">Действие setPriority</span><span class="sxs-lookup"><span data-stu-id="be5ed-118">setPriority action</span></span>](../api/intune-shared-deviceenrollmentconfiguration-setpriority.md)|<span data-ttu-id="be5ed-119">Нет</span><span class="sxs-lookup"><span data-stu-id="be5ed-119">None</span></span>|<span data-ttu-id="be5ed-120">Н/Д</span><span class="sxs-lookup"><span data-stu-id="be5ed-120">Not yet documented</span></span>|
|[<span data-ttu-id="be5ed-121">Действие assign</span><span class="sxs-lookup"><span data-stu-id="be5ed-121">assign action</span></span>](../api/intune-shared-deviceenrollmentconfiguration-assign.md)|<span data-ttu-id="be5ed-122">Нет</span><span class="sxs-lookup"><span data-stu-id="be5ed-122">None</span></span>|<span data-ttu-id="be5ed-123">Н/Д</span><span class="sxs-lookup"><span data-stu-id="be5ed-123">Not yet documented</span></span>|
|<span data-ttu-id="be5ed-124">**Набор политик**</span><span class="sxs-lookup"><span data-stu-id="be5ed-124">**Policy Set**</span></span>|
|[<span data-ttu-id="be5ed-125">действие Хаспайлоадлинкс</span><span class="sxs-lookup"><span data-stu-id="be5ed-125">hasPayloadLinks action</span></span>](../api/intune-shared-deviceenrollmentconfiguration-haspayloadlinks.md)|<span data-ttu-id="be5ed-126">Коллекция [хаспайлоадлинкресултитем](../resources/intune-policyset-haspayloadlinkresultitem.md)</span><span class="sxs-lookup"><span data-stu-id="be5ed-126">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection</span></span>|<span data-ttu-id="be5ed-127">Пока не задокументировано</span><span class="sxs-lookup"><span data-stu-id="be5ed-127">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="be5ed-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="be5ed-128">Properties</span></span>
|<span data-ttu-id="be5ed-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="be5ed-129">Property</span></span>|<span data-ttu-id="be5ed-130">Тип</span><span class="sxs-lookup"><span data-stu-id="be5ed-130">Type</span></span>|<span data-ttu-id="be5ed-131">Описание</span><span class="sxs-lookup"><span data-stu-id="be5ed-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be5ed-132">id</span><span class="sxs-lookup"><span data-stu-id="be5ed-132">id</span></span>|<span data-ttu-id="be5ed-133">String</span><span class="sxs-lookup"><span data-stu-id="be5ed-133">String</span></span>|<span data-ttu-id="be5ed-134">Уникальный идентификатор для учетной записи</span><span class="sxs-lookup"><span data-stu-id="be5ed-134">Unique Identifier for the account</span></span>|
|<span data-ttu-id="be5ed-135">displayName</span><span class="sxs-lookup"><span data-stu-id="be5ed-135">displayName</span></span>|<span data-ttu-id="be5ed-136">Строка</span><span class="sxs-lookup"><span data-stu-id="be5ed-136">String</span></span>|<span data-ttu-id="be5ed-137">Отображаемое имя конфигурации регистрации устройств</span><span class="sxs-lookup"><span data-stu-id="be5ed-137">The display name of the device enrollment configuration</span></span>|
|<span data-ttu-id="be5ed-138">description</span><span class="sxs-lookup"><span data-stu-id="be5ed-138">description</span></span>|<span data-ttu-id="be5ed-139">String</span><span class="sxs-lookup"><span data-stu-id="be5ed-139">String</span></span>|<span data-ttu-id="be5ed-140">Описание конфигурации регистрации устройств</span><span class="sxs-lookup"><span data-stu-id="be5ed-140">The description of the device enrollment configuration</span></span>|
|<span data-ttu-id="be5ed-141">priority</span><span class="sxs-lookup"><span data-stu-id="be5ed-141">priority</span></span>|<span data-ttu-id="be5ed-142">Int32</span><span class="sxs-lookup"><span data-stu-id="be5ed-142">Int32</span></span>|<span data-ttu-id="be5ed-143">Priority используется, когда пользователь существует в нескольких группах, которым назначена Настройка регистрации.</span><span class="sxs-lookup"><span data-stu-id="be5ed-143">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="be5ed-144">Пользователи подчиняются только конфигурации с наименьшим значением приоритета.</span><span class="sxs-lookup"><span data-stu-id="be5ed-144">Users are subject only to the configuration with the lowest priority value.</span></span>|
|<span data-ttu-id="be5ed-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="be5ed-145">createdDateTime</span></span>|<span data-ttu-id="be5ed-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be5ed-146">DateTimeOffset</span></span>|<span data-ttu-id="be5ed-147">Созданная Дата и время в формате UTC для конфигурации регистрации устройств</span><span class="sxs-lookup"><span data-stu-id="be5ed-147">Created date time in UTC of the device enrollment configuration</span></span>|
|<span data-ttu-id="be5ed-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="be5ed-148">lastModifiedDateTime</span></span>|<span data-ttu-id="be5ed-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be5ed-149">DateTimeOffset</span></span>|<span data-ttu-id="be5ed-150">Дата и время последнего изменения конфигурации регистрации устройств в формате UTC</span><span class="sxs-lookup"><span data-stu-id="be5ed-150">Last modified date time in UTC of the device enrollment configuration</span></span>|
|<span data-ttu-id="be5ed-151">version</span><span class="sxs-lookup"><span data-stu-id="be5ed-151">version</span></span>|<span data-ttu-id="be5ed-152">Int32</span><span class="sxs-lookup"><span data-stu-id="be5ed-152">Int32</span></span>|<span data-ttu-id="be5ed-153">Версия конфигурации регистрации устройств</span><span class="sxs-lookup"><span data-stu-id="be5ed-153">The version of the device enrollment configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="be5ed-154">Связи</span><span class="sxs-lookup"><span data-stu-id="be5ed-154">Relationships</span></span>
|<span data-ttu-id="be5ed-155">Связь</span><span class="sxs-lookup"><span data-stu-id="be5ed-155">Relationship</span></span>|<span data-ttu-id="be5ed-156">Тип</span><span class="sxs-lookup"><span data-stu-id="be5ed-156">Type</span></span>|<span data-ttu-id="be5ed-157">Описание</span><span class="sxs-lookup"><span data-stu-id="be5ed-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be5ed-158">**Адаптация**</span><span class="sxs-lookup"><span data-stu-id="be5ed-158">**Onboarding**</span></span>|
|<span data-ttu-id="be5ed-159">assignments</span><span class="sxs-lookup"><span data-stu-id="be5ed-159">assignments</span></span>|<span data-ttu-id="be5ed-160">Коллекция [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="be5ed-160">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) collection</span></span>|<span data-ttu-id="be5ed-161">Список назначений групп для профиля конфигурации устройства</span><span class="sxs-lookup"><span data-stu-id="be5ed-161">The list of group assignments for the device configuration profile</span></span>|

## <a name="json-representation"></a><span data-ttu-id="be5ed-162">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="be5ed-162">JSON Representation</span></span>
<span data-ttu-id="be5ed-163">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="be5ed-163">Here is a JSON representation of the resource.</span></span>
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



