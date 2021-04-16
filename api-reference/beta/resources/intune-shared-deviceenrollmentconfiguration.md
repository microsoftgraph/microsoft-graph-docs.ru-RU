---
title: Тип ресурса deviceEnrollmentConfiguration
description: Базовый класс конфигурации регистрации устройств
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0d46e446aab9806ad856f71cb8ac57c2f75f1b55
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51865798"
---
# <a name="deviceenrollmentconfiguration-resource-type"></a><span data-ttu-id="4b148-103">Тип ресурса deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="4b148-103">deviceEnrollmentConfiguration resource type</span></span>

<span data-ttu-id="4b148-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b148-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4b148-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b148-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4b148-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4b148-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b148-107">Базовый класс конфигурации регистрации устройств</span><span class="sxs-lookup"><span data-stu-id="4b148-107">The Base Class of Device Enrollment Configuration</span></span>

## <a name="methods"></a><span data-ttu-id="4b148-108">Методы</span><span class="sxs-lookup"><span data-stu-id="4b148-108">Methods</span></span>
|<span data-ttu-id="4b148-109">Метод</span><span class="sxs-lookup"><span data-stu-id="4b148-109">Method</span></span>|<span data-ttu-id="4b148-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4b148-110">Return Type</span></span>|<span data-ttu-id="4b148-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4b148-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4b148-112">Список объектов deviceEnrollmentConfigurations</span><span class="sxs-lookup"><span data-stu-id="4b148-112">List deviceEnrollmentConfigurations</span></span>](../api/intune-shared-deviceenrollmentconfiguration-list.md)|<span data-ttu-id="4b148-113">Коллекция [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4b148-113">[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) collection</span></span>|<span data-ttu-id="4b148-114">Список свойств и связей объектов [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b148-114">List properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="4b148-115">Получение объекта deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="4b148-115">Get deviceEnrollmentConfiguration</span></span>](../api/intune-shared-deviceenrollmentconfiguration-get.md)|[<span data-ttu-id="4b148-116">deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="4b148-116">deviceEnrollmentConfiguration</span></span>](../resources/intune-shared-deviceenrollmentconfiguration.md)|<span data-ttu-id="4b148-117">Чтение свойств и связей объекта [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b148-117">Read properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) object.</span></span>|
|<span data-ttu-id="4b148-118">**Адаптация**</span><span class="sxs-lookup"><span data-stu-id="4b148-118">**Onboarding**</span></span>|
|[<span data-ttu-id="4b148-119">Действие setPriority</span><span class="sxs-lookup"><span data-stu-id="4b148-119">setPriority action</span></span>](../api/intune-shared-deviceenrollmentconfiguration-setpriority.md)|<span data-ttu-id="4b148-120">Нет</span><span class="sxs-lookup"><span data-stu-id="4b148-120">None</span></span>|<span data-ttu-id="4b148-121">Н/Д</span><span class="sxs-lookup"><span data-stu-id="4b148-121">Not yet documented</span></span>|
|[<span data-ttu-id="4b148-122">Действие assign</span><span class="sxs-lookup"><span data-stu-id="4b148-122">assign action</span></span>](../api/intune-shared-deviceenrollmentconfiguration-assign.md)|<span data-ttu-id="4b148-123">Нет</span><span class="sxs-lookup"><span data-stu-id="4b148-123">None</span></span>|<span data-ttu-id="4b148-124">Н/Д</span><span class="sxs-lookup"><span data-stu-id="4b148-124">Not yet documented</span></span>|
|<span data-ttu-id="4b148-125">**Набор политик**</span><span class="sxs-lookup"><span data-stu-id="4b148-125">**Policy Set**</span></span>|
|[<span data-ttu-id="4b148-126">действие hasPayloadLinks</span><span class="sxs-lookup"><span data-stu-id="4b148-126">hasPayloadLinks action</span></span>](../api/intune-shared-deviceenrollmentconfiguration-haspayloadlinks.md)|<span data-ttu-id="4b148-127">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection</span><span class="sxs-lookup"><span data-stu-id="4b148-127">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection</span></span>|<span data-ttu-id="4b148-128">Н/Д</span><span class="sxs-lookup"><span data-stu-id="4b148-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="4b148-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="4b148-129">Properties</span></span>
|<span data-ttu-id="4b148-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4b148-130">Property</span></span>|<span data-ttu-id="4b148-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4b148-131">Type</span></span>|<span data-ttu-id="4b148-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4b148-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b148-133">id</span><span class="sxs-lookup"><span data-stu-id="4b148-133">id</span></span>|<span data-ttu-id="4b148-134">String</span><span class="sxs-lookup"><span data-stu-id="4b148-134">String</span></span>|<span data-ttu-id="4b148-135">Уникальный идентификатор учетной записи</span><span class="sxs-lookup"><span data-stu-id="4b148-135">Unique Identifier for the account</span></span>|
|<span data-ttu-id="4b148-136">displayName</span><span class="sxs-lookup"><span data-stu-id="4b148-136">displayName</span></span>|<span data-ttu-id="4b148-137">String</span><span class="sxs-lookup"><span data-stu-id="4b148-137">String</span></span>|<span data-ttu-id="4b148-138">Отображающее имя конфигурации регистрации устройства</span><span class="sxs-lookup"><span data-stu-id="4b148-138">The display name of the device enrollment configuration</span></span>|
|<span data-ttu-id="4b148-139">description</span><span class="sxs-lookup"><span data-stu-id="4b148-139">description</span></span>|<span data-ttu-id="4b148-140">String</span><span class="sxs-lookup"><span data-stu-id="4b148-140">String</span></span>|<span data-ttu-id="4b148-141">Описание конфигурации регистрации устройства</span><span class="sxs-lookup"><span data-stu-id="4b148-141">The description of the device enrollment configuration</span></span>|
|<span data-ttu-id="4b148-142">priority</span><span class="sxs-lookup"><span data-stu-id="4b148-142">priority</span></span>|<span data-ttu-id="4b148-143">Int32</span><span class="sxs-lookup"><span data-stu-id="4b148-143">Int32</span></span>|<span data-ttu-id="4b148-144">Приоритет используется, когда пользователь существует в нескольких группах, которые назначены конфигурации регистрации.</span><span class="sxs-lookup"><span data-stu-id="4b148-144">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="4b148-145">Пользователи подчиняются только конфигурации с наименьшим значением приоритета.</span><span class="sxs-lookup"><span data-stu-id="4b148-145">Users are subject only to the configuration with the lowest priority value.</span></span>|
|<span data-ttu-id="4b148-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4b148-146">createdDateTime</span></span>|<span data-ttu-id="4b148-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b148-147">DateTimeOffset</span></span>|<span data-ttu-id="4b148-148">Создано время даты в UTC конфигурации регистрации устройства</span><span class="sxs-lookup"><span data-stu-id="4b148-148">Created date time in UTC of the device enrollment configuration</span></span>|
|<span data-ttu-id="4b148-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4b148-149">lastModifiedDateTime</span></span>|<span data-ttu-id="4b148-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b148-150">DateTimeOffset</span></span>|<span data-ttu-id="4b148-151">Последнее измененное время даты в UTC конфигурации регистрации устройства</span><span class="sxs-lookup"><span data-stu-id="4b148-151">Last modified date time in UTC of the device enrollment configuration</span></span>|
|<span data-ttu-id="4b148-152">version</span><span class="sxs-lookup"><span data-stu-id="4b148-152">version</span></span>|<span data-ttu-id="4b148-153">Int32</span><span class="sxs-lookup"><span data-stu-id="4b148-153">Int32</span></span>|<span data-ttu-id="4b148-154">Версия конфигурации регистрации устройства</span><span class="sxs-lookup"><span data-stu-id="4b148-154">The version of the device enrollment configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="4b148-155">Связи</span><span class="sxs-lookup"><span data-stu-id="4b148-155">Relationships</span></span>
|<span data-ttu-id="4b148-156">Связь</span><span class="sxs-lookup"><span data-stu-id="4b148-156">Relationship</span></span>|<span data-ttu-id="4b148-157">Тип</span><span class="sxs-lookup"><span data-stu-id="4b148-157">Type</span></span>|<span data-ttu-id="4b148-158">Описание</span><span class="sxs-lookup"><span data-stu-id="4b148-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b148-159">**Адаптация**</span><span class="sxs-lookup"><span data-stu-id="4b148-159">**Onboarding**</span></span>|
|<span data-ttu-id="4b148-160">assignments</span><span class="sxs-lookup"><span data-stu-id="4b148-160">assignments</span></span>|<span data-ttu-id="4b148-161">Коллекция [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="4b148-161">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) collection</span></span>|<span data-ttu-id="4b148-162">Список групповых назначений для профиля конфигурации устройства</span><span class="sxs-lookup"><span data-stu-id="4b148-162">The list of group assignments for the device configuration profile</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4b148-163">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4b148-163">JSON Representation</span></span>
<span data-ttu-id="4b148-164">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4b148-164">Here is a JSON representation of the resource.</span></span>
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




