---
title: Обновление объекта deviceEnrollmentPlatformRestrictionsConfiguration
description: Обновление свойств объекта deviceEnrollmentPlatformRestrictionsConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a6c1826c790888f76d21999c4313faf9337b8eea
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42802981"
---
# <a name="update-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="8b3d5-103">Обновление объекта deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="8b3d5-103">Update deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="8b3d5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b3d5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8b3d5-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8b3d5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b3d5-106">Обновление свойств объекта [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8b3d5-106">Update the properties of a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8b3d5-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8b3d5-107">Prerequisites</span></span>
<span data-ttu-id="8b3d5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b3d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b3d5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8b3d5-110">Permission type</span></span>|<span data-ttu-id="8b3d5-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8b3d5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8b3d5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8b3d5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8b3d5-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b3d5-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8b3d5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8b3d5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8b3d5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b3d5-115">Not supported.</span></span>|
|<span data-ttu-id="8b3d5-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="8b3d5-116">Application</span></span>|<span data-ttu-id="8b3d5-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b3d5-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8b3d5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8b3d5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="8b3d5-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8b3d5-119">Request headers</span></span>
|<span data-ttu-id="8b3d5-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8b3d5-120">Header</span></span>|<span data-ttu-id="8b3d5-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8b3d5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8b3d5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b3d5-122">Authorization</span></span>|<span data-ttu-id="8b3d5-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8b3d5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8b3d5-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8b3d5-124">Accept</span></span>|<span data-ttu-id="8b3d5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8b3d5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8b3d5-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8b3d5-126">Request body</span></span>
<span data-ttu-id="8b3d5-127">В теле запроса добавьте представление объекта [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8b3d5-127">In the request body, supply a JSON representation for the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

<span data-ttu-id="8b3d5-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8b3d5-128">The following table shows the properties that are required when you create the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span></span>

|<span data-ttu-id="8b3d5-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="8b3d5-129">Property</span></span>|<span data-ttu-id="8b3d5-130">Тип</span><span class="sxs-lookup"><span data-stu-id="8b3d5-130">Type</span></span>|<span data-ttu-id="8b3d5-131">Описание</span><span class="sxs-lookup"><span data-stu-id="8b3d5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b3d5-132">id</span><span class="sxs-lookup"><span data-stu-id="8b3d5-132">id</span></span>|<span data-ttu-id="8b3d5-133">String</span><span class="sxs-lookup"><span data-stu-id="8b3d5-133">String</span></span>|<span data-ttu-id="8b3d5-134">Уникальный идентификатор для учетной записи, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8b3d5-134">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="8b3d5-135">displayName</span><span class="sxs-lookup"><span data-stu-id="8b3d5-135">displayName</span></span>|<span data-ttu-id="8b3d5-136">Строка</span><span class="sxs-lookup"><span data-stu-id="8b3d5-136">String</span></span>|<span data-ttu-id="8b3d5-137">Отображаемое имя конфигурации регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8b3d5-137">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="8b3d5-138">description</span><span class="sxs-lookup"><span data-stu-id="8b3d5-138">description</span></span>|<span data-ttu-id="8b3d5-139">String</span><span class="sxs-lookup"><span data-stu-id="8b3d5-139">String</span></span>|<span data-ttu-id="8b3d5-140">Описание конфигурации регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8b3d5-140">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="8b3d5-141">priority</span><span class="sxs-lookup"><span data-stu-id="8b3d5-141">priority</span></span>|<span data-ttu-id="8b3d5-142">Int32</span><span class="sxs-lookup"><span data-stu-id="8b3d5-142">Int32</span></span>|<span data-ttu-id="8b3d5-143">Priority используется, когда пользователь существует в нескольких группах, которым назначена Настройка регистрации.</span><span class="sxs-lookup"><span data-stu-id="8b3d5-143">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="8b3d5-144">Пользователи подчиняются только конфигурации с наименьшим значением приоритета.</span><span class="sxs-lookup"><span data-stu-id="8b3d5-144">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="8b3d5-145">Наследуется от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8b3d5-145">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="8b3d5-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8b3d5-146">createdDateTime</span></span>|<span data-ttu-id="8b3d5-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8b3d5-147">DateTimeOffset</span></span>|<span data-ttu-id="8b3d5-148">Созданная Дата и время в формате UTC для настройки регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8b3d5-148">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="8b3d5-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8b3d5-149">lastModifiedDateTime</span></span>|<span data-ttu-id="8b3d5-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8b3d5-150">DateTimeOffset</span></span>|<span data-ttu-id="8b3d5-151">Дата и время последнего изменения конфигурации регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8b3d5-151">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="8b3d5-152">version</span><span class="sxs-lookup"><span data-stu-id="8b3d5-152">version</span></span>|<span data-ttu-id="8b3d5-153">Int32</span><span class="sxs-lookup"><span data-stu-id="8b3d5-153">Int32</span></span>|<span data-ttu-id="8b3d5-154">Версия конфигурации регистрации устройств, унаследованная от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8b3d5-154">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="8b3d5-155">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="8b3d5-155">iosRestriction</span></span>|[<span data-ttu-id="8b3d5-156">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="8b3d5-156">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="8b3d5-157">Ограничения iOS на основе платформы, версии операционной системы платформы и владельца устройств</span><span class="sxs-lookup"><span data-stu-id="8b3d5-157">Ios restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="8b3d5-158">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="8b3d5-158">windowsRestriction</span></span>|[<span data-ttu-id="8b3d5-159">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="8b3d5-159">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="8b3d5-160">Ограничения Windows на основе платформы, версии операционной системы платформы и владельца устройств</span><span class="sxs-lookup"><span data-stu-id="8b3d5-160">Windows restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="8b3d5-161">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="8b3d5-161">windowsMobileRestriction</span></span>|[<span data-ttu-id="8b3d5-162">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="8b3d5-162">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="8b3d5-163">Ограничения для Windows Mobile на основе платформы, версии операционной системы платформы и владельца устройств</span><span class="sxs-lookup"><span data-stu-id="8b3d5-163">Windows mobile restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="8b3d5-164">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="8b3d5-164">androidRestriction</span></span>|[<span data-ttu-id="8b3d5-165">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="8b3d5-165">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="8b3d5-166">Ограничения для Android на основе платформы, версии операционной системы платформы и владельца устройств</span><span class="sxs-lookup"><span data-stu-id="8b3d5-166">Android restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="8b3d5-167">андроидфорворкрестриктион</span><span class="sxs-lookup"><span data-stu-id="8b3d5-167">androidForWorkRestriction</span></span>|[<span data-ttu-id="8b3d5-168">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="8b3d5-168">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="8b3d5-169">Ограничения для Android для работы на основе платформы, версии операционной системы платформы и владельца устройств</span><span class="sxs-lookup"><span data-stu-id="8b3d5-169">Android for work restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="8b3d5-170">макрестриктион</span><span class="sxs-lookup"><span data-stu-id="8b3d5-170">macRestriction</span></span>|[<span data-ttu-id="8b3d5-171">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="8b3d5-171">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="8b3d5-172">Ограничения для MAC-адресов на основе платформы, версии операционной системы платформы и владельца устройств</span><span class="sxs-lookup"><span data-stu-id="8b3d5-172">Mac restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="8b3d5-173">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="8b3d5-173">macOSRestriction</span></span>|[<span data-ttu-id="8b3d5-174">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="8b3d5-174">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="8b3d5-175">Ограничения для MAC-адресов на основе платформы, версии операционной системы платформы и владельца устройств</span><span class="sxs-lookup"><span data-stu-id="8b3d5-175">Mac restrictions based on platform, platform operating system version, and device ownership</span></span>|



## <a name="response"></a><span data-ttu-id="8b3d5-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b3d5-176">Response</span></span>
<span data-ttu-id="8b3d5-177">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8b3d5-177">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b3d5-178">Пример</span><span class="sxs-lookup"><span data-stu-id="8b3d5-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="8b3d5-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="8b3d5-179">Request</span></span>
<span data-ttu-id="8b3d5-180">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8b3d5-180">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 2763

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestrictionsConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "version": 7,
  "iosRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "blockedManufacturers": [
      "Blocked Manufacturers value"
    ]
  },
  "windowsRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "blockedManufacturers": [
      "Blocked Manufacturers value"
    ]
  },
  "windowsMobileRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "blockedManufacturers": [
      "Blocked Manufacturers value"
    ]
  },
  "androidRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "blockedManufacturers": [
      "Blocked Manufacturers value"
    ]
  },
  "androidForWorkRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "blockedManufacturers": [
      "Blocked Manufacturers value"
    ]
  },
  "macRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "blockedManufacturers": [
      "Blocked Manufacturers value"
    ]
  },
  "macOSRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "blockedManufacturers": [
      "Blocked Manufacturers value"
    ]
  }
}
```

### <a name="response"></a><span data-ttu-id="8b3d5-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b3d5-181">Response</span></span>
<span data-ttu-id="8b3d5-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8b3d5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2935

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestrictionsConfiguration",
  "id": "3acb2d75-2d75-3acb-752d-cb3a752dcb3a",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "iosRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "blockedManufacturers": [
      "Blocked Manufacturers value"
    ]
  },
  "windowsRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "blockedManufacturers": [
      "Blocked Manufacturers value"
    ]
  },
  "windowsMobileRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "blockedManufacturers": [
      "Blocked Manufacturers value"
    ]
  },
  "androidRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "blockedManufacturers": [
      "Blocked Manufacturers value"
    ]
  },
  "androidForWorkRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "blockedManufacturers": [
      "Blocked Manufacturers value"
    ]
  },
  "macRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "blockedManufacturers": [
      "Blocked Manufacturers value"
    ]
  },
  "macOSRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "blockedManufacturers": [
      "Blocked Manufacturers value"
    ]
  }
}
```




