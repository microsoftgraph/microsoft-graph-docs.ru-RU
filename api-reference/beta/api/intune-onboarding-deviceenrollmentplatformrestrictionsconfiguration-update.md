---
title: Обновление объекта deviceEnrollmentPlatformRestrictionsConfiguration
description: Обновление свойств объекта deviceEnrollmentPlatformRestrictionsConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6c4a54138be21f022e17d823d685706430525686
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42462420"
---
# <a name="update-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="885db-103">Обновление объекта deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="885db-103">Update deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

<span data-ttu-id="885db-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="885db-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="885db-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="885db-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="885db-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="885db-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="885db-107">Обновление свойств объекта [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="885db-107">Update the properties of a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="885db-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="885db-108">Prerequisites</span></span>
<span data-ttu-id="885db-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="885db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="885db-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="885db-111">Permission type</span></span>|<span data-ttu-id="885db-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="885db-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="885db-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="885db-113">Delegated (work or school account)</span></span>|<span data-ttu-id="885db-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="885db-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="885db-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="885db-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="885db-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="885db-116">Not supported.</span></span>|
|<span data-ttu-id="885db-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="885db-117">Application</span></span>|<span data-ttu-id="885db-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="885db-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="885db-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="885db-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="885db-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="885db-120">Request headers</span></span>
|<span data-ttu-id="885db-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="885db-121">Header</span></span>|<span data-ttu-id="885db-122">Значение</span><span class="sxs-lookup"><span data-stu-id="885db-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="885db-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="885db-123">Authorization</span></span>|<span data-ttu-id="885db-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="885db-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="885db-125">Accept</span><span class="sxs-lookup"><span data-stu-id="885db-125">Accept</span></span>|<span data-ttu-id="885db-126">application/json</span><span class="sxs-lookup"><span data-stu-id="885db-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="885db-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="885db-127">Request body</span></span>
<span data-ttu-id="885db-128">В теле запроса добавьте представление объекта [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="885db-128">In the request body, supply a JSON representation for the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

<span data-ttu-id="885db-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="885db-129">The following table shows the properties that are required when you create the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span></span>

|<span data-ttu-id="885db-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="885db-130">Property</span></span>|<span data-ttu-id="885db-131">Тип</span><span class="sxs-lookup"><span data-stu-id="885db-131">Type</span></span>|<span data-ttu-id="885db-132">Описание</span><span class="sxs-lookup"><span data-stu-id="885db-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="885db-133">id</span><span class="sxs-lookup"><span data-stu-id="885db-133">id</span></span>|<span data-ttu-id="885db-134">String</span><span class="sxs-lookup"><span data-stu-id="885db-134">String</span></span>|<span data-ttu-id="885db-135">Уникальный идентификатор для учетной записи, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="885db-135">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="885db-136">displayName</span><span class="sxs-lookup"><span data-stu-id="885db-136">displayName</span></span>|<span data-ttu-id="885db-137">Строка</span><span class="sxs-lookup"><span data-stu-id="885db-137">String</span></span>|<span data-ttu-id="885db-138">Отображаемое имя конфигурации регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="885db-138">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="885db-139">description</span><span class="sxs-lookup"><span data-stu-id="885db-139">description</span></span>|<span data-ttu-id="885db-140">String</span><span class="sxs-lookup"><span data-stu-id="885db-140">String</span></span>|<span data-ttu-id="885db-141">Описание конфигурации регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="885db-141">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="885db-142">priority</span><span class="sxs-lookup"><span data-stu-id="885db-142">priority</span></span>|<span data-ttu-id="885db-143">Int32</span><span class="sxs-lookup"><span data-stu-id="885db-143">Int32</span></span>|<span data-ttu-id="885db-144">Priority используется, когда пользователь существует в нескольких группах, которым назначена Настройка регистрации.</span><span class="sxs-lookup"><span data-stu-id="885db-144">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="885db-145">Пользователи подчиняются только конфигурации с наименьшим значением приоритета.</span><span class="sxs-lookup"><span data-stu-id="885db-145">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="885db-146">Наследуется от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="885db-146">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="885db-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="885db-147">createdDateTime</span></span>|<span data-ttu-id="885db-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="885db-148">DateTimeOffset</span></span>|<span data-ttu-id="885db-149">Созданная Дата и время в формате UTC для настройки регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="885db-149">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="885db-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="885db-150">lastModifiedDateTime</span></span>|<span data-ttu-id="885db-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="885db-151">DateTimeOffset</span></span>|<span data-ttu-id="885db-152">Дата и время последнего изменения конфигурации регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="885db-152">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="885db-153">version</span><span class="sxs-lookup"><span data-stu-id="885db-153">version</span></span>|<span data-ttu-id="885db-154">Int32</span><span class="sxs-lookup"><span data-stu-id="885db-154">Int32</span></span>|<span data-ttu-id="885db-155">Версия конфигурации регистрации устройств, унаследованная от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="885db-155">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="885db-156">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="885db-156">iosRestriction</span></span>|[<span data-ttu-id="885db-157">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="885db-157">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="885db-158">Ограничения iOS на основе платформы, версии операционной системы платформы и владельца устройств</span><span class="sxs-lookup"><span data-stu-id="885db-158">Ios restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="885db-159">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="885db-159">windowsRestriction</span></span>|[<span data-ttu-id="885db-160">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="885db-160">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="885db-161">Ограничения Windows на основе платформы, версии операционной системы платформы и владельца устройств</span><span class="sxs-lookup"><span data-stu-id="885db-161">Windows restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="885db-162">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="885db-162">windowsMobileRestriction</span></span>|[<span data-ttu-id="885db-163">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="885db-163">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="885db-164">Ограничения для Windows Mobile на основе платформы, версии операционной системы платформы и владельца устройств</span><span class="sxs-lookup"><span data-stu-id="885db-164">Windows mobile restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="885db-165">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="885db-165">androidRestriction</span></span>|[<span data-ttu-id="885db-166">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="885db-166">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="885db-167">Ограничения для Android на основе платформы, версии операционной системы платформы и владельца устройств</span><span class="sxs-lookup"><span data-stu-id="885db-167">Android restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="885db-168">андроидфорворкрестриктион</span><span class="sxs-lookup"><span data-stu-id="885db-168">androidForWorkRestriction</span></span>|[<span data-ttu-id="885db-169">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="885db-169">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="885db-170">Ограничения для Android для работы на основе платформы, версии операционной системы платформы и владельца устройств</span><span class="sxs-lookup"><span data-stu-id="885db-170">Android for work restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="885db-171">макрестриктион</span><span class="sxs-lookup"><span data-stu-id="885db-171">macRestriction</span></span>|[<span data-ttu-id="885db-172">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="885db-172">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="885db-173">Ограничения для MAC-адресов на основе платформы, версии операционной системы платформы и владельца устройств</span><span class="sxs-lookup"><span data-stu-id="885db-173">Mac restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="885db-174">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="885db-174">macOSRestriction</span></span>|[<span data-ttu-id="885db-175">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="885db-175">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="885db-176">Ограничения для MAC-адресов на основе платформы, версии операционной системы платформы и владельца устройств</span><span class="sxs-lookup"><span data-stu-id="885db-176">Mac restrictions based on platform, platform operating system version, and device ownership</span></span>|



## <a name="response"></a><span data-ttu-id="885db-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="885db-177">Response</span></span>
<span data-ttu-id="885db-178">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="885db-178">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="885db-179">Пример</span><span class="sxs-lookup"><span data-stu-id="885db-179">Example</span></span>

### <a name="request"></a><span data-ttu-id="885db-180">Запрос</span><span class="sxs-lookup"><span data-stu-id="885db-180">Request</span></span>
<span data-ttu-id="885db-181">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="885db-181">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="885db-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="885db-182">Response</span></span>
<span data-ttu-id="885db-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="885db-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





