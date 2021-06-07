---
title: Тип ресурса deviceEnrollmentConfiguration
description: Базовый класс конфигурации регистрации устройств
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 03787eed949221af2b4cbee5ca08d107aa60c229
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752758"
---
# <a name="deviceenrollmentconfiguration-resource-type"></a><span data-ttu-id="4b290-103">Тип ресурса deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="4b290-103">deviceEnrollmentConfiguration resource type</span></span>

<span data-ttu-id="4b290-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b290-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4b290-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4b290-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b290-106">Базовый класс конфигурации регистрации устройств</span><span class="sxs-lookup"><span data-stu-id="4b290-106">The Base Class of Device Enrollment Configuration</span></span>

## <a name="methods"></a><span data-ttu-id="4b290-107">Методы</span><span class="sxs-lookup"><span data-stu-id="4b290-107">Methods</span></span>
|<span data-ttu-id="4b290-108">Метод</span><span class="sxs-lookup"><span data-stu-id="4b290-108">Method</span></span>|<span data-ttu-id="4b290-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4b290-109">Return Type</span></span>|<span data-ttu-id="4b290-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4b290-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4b290-111">Список объектов deviceEnrollmentConfigurations</span><span class="sxs-lookup"><span data-stu-id="4b290-111">List deviceEnrollmentConfigurations</span></span>](../api/intune-onboarding-deviceenrollmentconfiguration-list.md)|<span data-ttu-id="4b290-112">Коллекция [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4b290-112">[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) collection</span></span>|<span data-ttu-id="4b290-113">Список свойств и связей объектов [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b290-113">List properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="4b290-114">Получение объекта deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="4b290-114">Get deviceEnrollmentConfiguration</span></span>](../api/intune-onboarding-deviceenrollmentconfiguration-get.md)|[<span data-ttu-id="4b290-115">deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="4b290-115">deviceEnrollmentConfiguration</span></span>](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|<span data-ttu-id="4b290-116">Чтение свойств и связей объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b290-116">Read properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) object.</span></span>|
|[<span data-ttu-id="4b290-117">Действие setPriority</span><span class="sxs-lookup"><span data-stu-id="4b290-117">setPriority action</span></span>](../api/intune-onboarding-deviceenrollmentconfiguration-setpriority.md)|<span data-ttu-id="4b290-118">Нет</span><span class="sxs-lookup"><span data-stu-id="4b290-118">None</span></span>|<span data-ttu-id="4b290-119">Н/Д</span><span class="sxs-lookup"><span data-stu-id="4b290-119">Not yet documented</span></span>|
|[<span data-ttu-id="4b290-120">Действие assign</span><span class="sxs-lookup"><span data-stu-id="4b290-120">assign action</span></span>](../api/intune-onboarding-deviceenrollmentconfiguration-assign.md)|<span data-ttu-id="4b290-121">Нет</span><span class="sxs-lookup"><span data-stu-id="4b290-121">None</span></span>|<span data-ttu-id="4b290-122">Н/Д</span><span class="sxs-lookup"><span data-stu-id="4b290-122">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="4b290-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="4b290-123">Properties</span></span>
|<span data-ttu-id="4b290-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="4b290-124">Property</span></span>|<span data-ttu-id="4b290-125">Тип</span><span class="sxs-lookup"><span data-stu-id="4b290-125">Type</span></span>|<span data-ttu-id="4b290-126">Описание</span><span class="sxs-lookup"><span data-stu-id="4b290-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b290-127">id</span><span class="sxs-lookup"><span data-stu-id="4b290-127">id</span></span>|<span data-ttu-id="4b290-128">String</span><span class="sxs-lookup"><span data-stu-id="4b290-128">String</span></span>|<span data-ttu-id="4b290-129">Уникальный идентификатор учетной записи</span><span class="sxs-lookup"><span data-stu-id="4b290-129">Unique Identifier for the account</span></span>|
|<span data-ttu-id="4b290-130">displayName</span><span class="sxs-lookup"><span data-stu-id="4b290-130">displayName</span></span>|<span data-ttu-id="4b290-131">String</span><span class="sxs-lookup"><span data-stu-id="4b290-131">String</span></span>|<span data-ttu-id="4b290-132">Отображающее имя конфигурации регистрации устройства</span><span class="sxs-lookup"><span data-stu-id="4b290-132">The display name of the device enrollment configuration</span></span>|
|<span data-ttu-id="4b290-133">description</span><span class="sxs-lookup"><span data-stu-id="4b290-133">description</span></span>|<span data-ttu-id="4b290-134">String</span><span class="sxs-lookup"><span data-stu-id="4b290-134">String</span></span>|<span data-ttu-id="4b290-135">Описание конфигурации регистрации устройства</span><span class="sxs-lookup"><span data-stu-id="4b290-135">The description of the device enrollment configuration</span></span>|
|<span data-ttu-id="4b290-136">priority</span><span class="sxs-lookup"><span data-stu-id="4b290-136">priority</span></span>|<span data-ttu-id="4b290-137">Int32</span><span class="sxs-lookup"><span data-stu-id="4b290-137">Int32</span></span>|<span data-ttu-id="4b290-138">Приоритет используется, когда пользователь существует в нескольких группах, которые назначены конфигурации регистрации.</span><span class="sxs-lookup"><span data-stu-id="4b290-138">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="4b290-139">Пользователи подчиняются только конфигурации с наименьшим значением приоритета.</span><span class="sxs-lookup"><span data-stu-id="4b290-139">Users are subject only to the configuration with the lowest priority value.</span></span>|
|<span data-ttu-id="4b290-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4b290-140">createdDateTime</span></span>|<span data-ttu-id="4b290-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b290-141">DateTimeOffset</span></span>|<span data-ttu-id="4b290-142">Создано время даты в UTC конфигурации регистрации устройства</span><span class="sxs-lookup"><span data-stu-id="4b290-142">Created date time in UTC of the device enrollment configuration</span></span>|
|<span data-ttu-id="4b290-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4b290-143">lastModifiedDateTime</span></span>|<span data-ttu-id="4b290-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b290-144">DateTimeOffset</span></span>|<span data-ttu-id="4b290-145">Последнее измененное время даты в UTC конфигурации регистрации устройства</span><span class="sxs-lookup"><span data-stu-id="4b290-145">Last modified date time in UTC of the device enrollment configuration</span></span>|
|<span data-ttu-id="4b290-146">version</span><span class="sxs-lookup"><span data-stu-id="4b290-146">version</span></span>|<span data-ttu-id="4b290-147">Int32</span><span class="sxs-lookup"><span data-stu-id="4b290-147">Int32</span></span>|<span data-ttu-id="4b290-148">Версия конфигурации регистрации устройства</span><span class="sxs-lookup"><span data-stu-id="4b290-148">The version of the device enrollment configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="4b290-149">Отношения</span><span class="sxs-lookup"><span data-stu-id="4b290-149">Relationships</span></span>
|<span data-ttu-id="4b290-150">Связь</span><span class="sxs-lookup"><span data-stu-id="4b290-150">Relationship</span></span>|<span data-ttu-id="4b290-151">Тип</span><span class="sxs-lookup"><span data-stu-id="4b290-151">Type</span></span>|<span data-ttu-id="4b290-152">Описание</span><span class="sxs-lookup"><span data-stu-id="4b290-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b290-153">assignments</span><span class="sxs-lookup"><span data-stu-id="4b290-153">assignments</span></span>|<span data-ttu-id="4b290-154">Коллекция [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="4b290-154">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) collection</span></span>|<span data-ttu-id="4b290-155">Список групповых назначений для профиля конфигурации устройства</span><span class="sxs-lookup"><span data-stu-id="4b290-155">The list of group assignments for the device configuration profile</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4b290-156">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4b290-156">JSON Representation</span></span>
<span data-ttu-id="4b290-157">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4b290-157">Here is a JSON representation of the resource.</span></span>
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




