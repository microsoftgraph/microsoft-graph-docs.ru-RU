---
title: Тип ресурса deviceEnrollmentConfiguration
description: Базовый класс конфигурации регистрации устройств
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 79941f498efae8167e6d9abcd9bcdf78b9557677
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37201235"
---
# <a name="deviceenrollmentconfiguration-resource-type"></a><span data-ttu-id="c6387-103">Тип ресурса deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="c6387-103">deviceEnrollmentConfiguration resource type</span></span>

> <span data-ttu-id="c6387-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6387-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c6387-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c6387-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c6387-106">Базовый класс конфигурации регистрации устройств</span><span class="sxs-lookup"><span data-stu-id="c6387-106">The Base Class of Device Enrollment Configuration</span></span>

## <a name="methods"></a><span data-ttu-id="c6387-107">Методы</span><span class="sxs-lookup"><span data-stu-id="c6387-107">Methods</span></span>
|<span data-ttu-id="c6387-108">Метод</span><span class="sxs-lookup"><span data-stu-id="c6387-108">Method</span></span>|<span data-ttu-id="c6387-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c6387-109">Return Type</span></span>|<span data-ttu-id="c6387-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c6387-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c6387-111">Список объектов deviceEnrollmentConfigurations</span><span class="sxs-lookup"><span data-stu-id="c6387-111">List deviceEnrollmentConfigurations</span></span>](../api/intune-shared-deviceenrollmentconfiguration-list.md)|<span data-ttu-id="c6387-112">Коллекция [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c6387-112">[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) collection</span></span>|<span data-ttu-id="c6387-113">Список свойств и связей объектов [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c6387-113">List properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="c6387-114">Получение объекта deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="c6387-114">Get deviceEnrollmentConfiguration</span></span>](../api/intune-shared-deviceenrollmentconfiguration-get.md)|[<span data-ttu-id="c6387-115">deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="c6387-115">deviceEnrollmentConfiguration</span></span>](../resources/intune-shared-deviceenrollmentconfiguration.md)|<span data-ttu-id="c6387-116">Чтение свойств и связей объекта [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c6387-116">Read properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) object.</span></span>|
|<span data-ttu-id="c6387-117">**Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="c6387-117">**Onboarding**</span></span>|
|[<span data-ttu-id="c6387-118">Действие setPriority</span><span class="sxs-lookup"><span data-stu-id="c6387-118">setPriority action</span></span>](../api/intune-shared-deviceenrollmentconfiguration-setpriority.md)|<span data-ttu-id="c6387-119">Нет</span><span class="sxs-lookup"><span data-stu-id="c6387-119">None</span></span>|<span data-ttu-id="c6387-120">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c6387-120">Not yet documented</span></span>|
|[<span data-ttu-id="c6387-121">Действие assign</span><span class="sxs-lookup"><span data-stu-id="c6387-121">assign action</span></span>](../api/intune-shared-deviceenrollmentconfiguration-assign.md)|<span data-ttu-id="c6387-122">Нет</span><span class="sxs-lookup"><span data-stu-id="c6387-122">None</span></span>|<span data-ttu-id="c6387-123">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c6387-123">Not yet documented</span></span>|
|<span data-ttu-id="c6387-124">**Набор политик**</span><span class="sxs-lookup"><span data-stu-id="c6387-124">**Policy Set**</span></span>|
|[<span data-ttu-id="c6387-125">действие Хаспайлоадлинкс</span><span class="sxs-lookup"><span data-stu-id="c6387-125">hasPayloadLinks action</span></span>](../api/intune-shared-deviceenrollmentconfiguration-haspayloadlinks.md)|<span data-ttu-id="c6387-126">Коллекция [хаспайлоадлинкресултитем](../resources/intune-policyset-haspayloadlinkresultitem.md)</span><span class="sxs-lookup"><span data-stu-id="c6387-126">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection</span></span>|<span data-ttu-id="c6387-127">Пока не задокументировано</span><span class="sxs-lookup"><span data-stu-id="c6387-127">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="c6387-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="c6387-128">Properties</span></span>
|<span data-ttu-id="c6387-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c6387-129">Property</span></span>|<span data-ttu-id="c6387-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c6387-130">Type</span></span>|<span data-ttu-id="c6387-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c6387-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6387-132">id</span><span class="sxs-lookup"><span data-stu-id="c6387-132">id</span></span>|<span data-ttu-id="c6387-133">String</span><span class="sxs-lookup"><span data-stu-id="c6387-133">String</span></span>|<span data-ttu-id="c6387-134">Уникальный идентификатор для учетной записи</span><span class="sxs-lookup"><span data-stu-id="c6387-134">Unique Identifier for the account</span></span>|
|<span data-ttu-id="c6387-135">displayName</span><span class="sxs-lookup"><span data-stu-id="c6387-135">displayName</span></span>|<span data-ttu-id="c6387-136">Строка</span><span class="sxs-lookup"><span data-stu-id="c6387-136">String</span></span>|<span data-ttu-id="c6387-137">Отображаемое имя конфигурации регистрации устройств</span><span class="sxs-lookup"><span data-stu-id="c6387-137">The display name of the device enrollment configuration</span></span>|
|<span data-ttu-id="c6387-138">description</span><span class="sxs-lookup"><span data-stu-id="c6387-138">description</span></span>|<span data-ttu-id="c6387-139">String</span><span class="sxs-lookup"><span data-stu-id="c6387-139">String</span></span>|<span data-ttu-id="c6387-140">Описание конфигурации регистрации устройств</span><span class="sxs-lookup"><span data-stu-id="c6387-140">The description of the device enrollment configuration</span></span>|
|<span data-ttu-id="c6387-141">priority</span><span class="sxs-lookup"><span data-stu-id="c6387-141">priority</span></span>|<span data-ttu-id="c6387-142">Int32</span><span class="sxs-lookup"><span data-stu-id="c6387-142">Int32</span></span>|<span data-ttu-id="c6387-143">Priority используется, когда пользователь существует в нескольких группах, которым назначена Настройка регистрации.</span><span class="sxs-lookup"><span data-stu-id="c6387-143">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="c6387-144">Пользователи подчиняются только конфигурации с наименьшим значением приоритета.</span><span class="sxs-lookup"><span data-stu-id="c6387-144">Users are subject only to the configuration with the lowest priority value.</span></span>|
|<span data-ttu-id="c6387-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c6387-145">createdDateTime</span></span>|<span data-ttu-id="c6387-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6387-146">DateTimeOffset</span></span>|<span data-ttu-id="c6387-147">Созданная Дата и время в формате UTC для конфигурации регистрации устройств</span><span class="sxs-lookup"><span data-stu-id="c6387-147">Created date time in UTC of the device enrollment configuration</span></span>|
|<span data-ttu-id="c6387-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c6387-148">lastModifiedDateTime</span></span>|<span data-ttu-id="c6387-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6387-149">DateTimeOffset</span></span>|<span data-ttu-id="c6387-150">Дата и время последнего изменения конфигурации регистрации устройств в формате UTC</span><span class="sxs-lookup"><span data-stu-id="c6387-150">Last modified date time in UTC of the device enrollment configuration</span></span>|
|<span data-ttu-id="c6387-151">version</span><span class="sxs-lookup"><span data-stu-id="c6387-151">version</span></span>|<span data-ttu-id="c6387-152">Int32</span><span class="sxs-lookup"><span data-stu-id="c6387-152">Int32</span></span>|<span data-ttu-id="c6387-153">Версия конфигурации регистрации устройств</span><span class="sxs-lookup"><span data-stu-id="c6387-153">The version of the device enrollment configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="c6387-154">Отношения</span><span class="sxs-lookup"><span data-stu-id="c6387-154">Relationships</span></span>
|<span data-ttu-id="c6387-155">Отношение</span><span class="sxs-lookup"><span data-stu-id="c6387-155">Relationship</span></span>|<span data-ttu-id="c6387-156">Тип</span><span class="sxs-lookup"><span data-stu-id="c6387-156">Type</span></span>|<span data-ttu-id="c6387-157">Описание</span><span class="sxs-lookup"><span data-stu-id="c6387-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6387-158">**Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="c6387-158">**Onboarding**</span></span>|
|<span data-ttu-id="c6387-159">assignments</span><span class="sxs-lookup"><span data-stu-id="c6387-159">assignments</span></span>|<span data-ttu-id="c6387-160">Коллекция [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c6387-160">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) collection</span></span>|<span data-ttu-id="c6387-161">Список назначений групп для профиля конфигурации устройства</span><span class="sxs-lookup"><span data-stu-id="c6387-161">The list of group assignments for the device configuration profile</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c6387-162">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c6387-162">JSON Representation</span></span>
<span data-ttu-id="c6387-163">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c6387-163">Here is a JSON representation of the resource.</span></span>
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



