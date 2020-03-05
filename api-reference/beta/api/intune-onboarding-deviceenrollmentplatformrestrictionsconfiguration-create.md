---
title: Создание объекта deviceEnrollmentPlatformRestrictionsConfiguration
description: Создание объекта deviceEnrollmentPlatformRestrictionsConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 554dd2ccc5076c96f8ca0e239a3405e4509d474c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42462406"
---
# <a name="create-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="11827-103">Создание объекта deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="11827-103">Create deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

<span data-ttu-id="11827-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="11827-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="11827-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11827-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="11827-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="11827-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11827-107">Создание объекта [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="11827-107">Create a new [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="11827-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="11827-108">Prerequisites</span></span>
<span data-ttu-id="11827-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11827-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11827-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="11827-111">Permission type</span></span>|<span data-ttu-id="11827-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="11827-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="11827-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="11827-113">Delegated (work or school account)</span></span>|<span data-ttu-id="11827-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11827-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="11827-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="11827-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="11827-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11827-116">Not supported.</span></span>|
|<span data-ttu-id="11827-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="11827-117">Application</span></span>|<span data-ttu-id="11827-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11827-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="11827-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="11827-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="11827-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="11827-120">Request headers</span></span>
|<span data-ttu-id="11827-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="11827-121">Header</span></span>|<span data-ttu-id="11827-122">Значение</span><span class="sxs-lookup"><span data-stu-id="11827-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="11827-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="11827-123">Authorization</span></span>|<span data-ttu-id="11827-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="11827-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="11827-125">Accept</span><span class="sxs-lookup"><span data-stu-id="11827-125">Accept</span></span>|<span data-ttu-id="11827-126">application/json</span><span class="sxs-lookup"><span data-stu-id="11827-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="11827-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="11827-127">Request body</span></span>
<span data-ttu-id="11827-128">В теле запроса добавьте представление объекта deviceEnrollmentPlatformRestrictionsConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="11827-128">In the request body, supply a JSON representation for the deviceEnrollmentPlatformRestrictionsConfiguration object.</span></span>

<span data-ttu-id="11827-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceEnrollmentPlatformRestrictionsConfiguration.</span><span class="sxs-lookup"><span data-stu-id="11827-129">The following table shows the properties that are required when you create the deviceEnrollmentPlatformRestrictionsConfiguration.</span></span>

|<span data-ttu-id="11827-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="11827-130">Property</span></span>|<span data-ttu-id="11827-131">Тип</span><span class="sxs-lookup"><span data-stu-id="11827-131">Type</span></span>|<span data-ttu-id="11827-132">Описание</span><span class="sxs-lookup"><span data-stu-id="11827-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11827-133">id</span><span class="sxs-lookup"><span data-stu-id="11827-133">id</span></span>|<span data-ttu-id="11827-134">String</span><span class="sxs-lookup"><span data-stu-id="11827-134">String</span></span>|<span data-ttu-id="11827-135">Уникальный идентификатор для учетной записи, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="11827-135">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="11827-136">displayName</span><span class="sxs-lookup"><span data-stu-id="11827-136">displayName</span></span>|<span data-ttu-id="11827-137">Строка</span><span class="sxs-lookup"><span data-stu-id="11827-137">String</span></span>|<span data-ttu-id="11827-138">Отображаемое имя конфигурации регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="11827-138">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="11827-139">description</span><span class="sxs-lookup"><span data-stu-id="11827-139">description</span></span>|<span data-ttu-id="11827-140">String</span><span class="sxs-lookup"><span data-stu-id="11827-140">String</span></span>|<span data-ttu-id="11827-141">Описание конфигурации регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="11827-141">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="11827-142">priority</span><span class="sxs-lookup"><span data-stu-id="11827-142">priority</span></span>|<span data-ttu-id="11827-143">Int32</span><span class="sxs-lookup"><span data-stu-id="11827-143">Int32</span></span>|<span data-ttu-id="11827-144">Priority используется, когда пользователь существует в нескольких группах, которым назначена Настройка регистрации.</span><span class="sxs-lookup"><span data-stu-id="11827-144">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="11827-145">Пользователи подчиняются только конфигурации с наименьшим значением приоритета.</span><span class="sxs-lookup"><span data-stu-id="11827-145">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="11827-146">Наследуется от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="11827-146">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="11827-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="11827-147">createdDateTime</span></span>|<span data-ttu-id="11827-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11827-148">DateTimeOffset</span></span>|<span data-ttu-id="11827-149">Созданная Дата и время в формате UTC для настройки регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="11827-149">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="11827-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="11827-150">lastModifiedDateTime</span></span>|<span data-ttu-id="11827-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11827-151">DateTimeOffset</span></span>|<span data-ttu-id="11827-152">Дата и время последнего изменения конфигурации регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="11827-152">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="11827-153">version</span><span class="sxs-lookup"><span data-stu-id="11827-153">version</span></span>|<span data-ttu-id="11827-154">Int32</span><span class="sxs-lookup"><span data-stu-id="11827-154">Int32</span></span>|<span data-ttu-id="11827-155">Версия конфигурации регистрации устройств, унаследованная от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="11827-155">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="11827-156">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="11827-156">iosRestriction</span></span>|[<span data-ttu-id="11827-157">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="11827-157">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="11827-158">Ограничения iOS на основе платформы, версии операционной системы платформы и владельца устройств</span><span class="sxs-lookup"><span data-stu-id="11827-158">Ios restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="11827-159">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="11827-159">windowsRestriction</span></span>|[<span data-ttu-id="11827-160">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="11827-160">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="11827-161">Ограничения Windows на основе платформы, версии операционной системы платформы и владельца устройств</span><span class="sxs-lookup"><span data-stu-id="11827-161">Windows restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="11827-162">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="11827-162">windowsMobileRestriction</span></span>|[<span data-ttu-id="11827-163">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="11827-163">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="11827-164">Ограничения для Windows Mobile на основе платформы, версии операционной системы платформы и владельца устройств</span><span class="sxs-lookup"><span data-stu-id="11827-164">Windows mobile restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="11827-165">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="11827-165">androidRestriction</span></span>|[<span data-ttu-id="11827-166">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="11827-166">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="11827-167">Ограничения для Android на основе платформы, версии операционной системы платформы и владельца устройств</span><span class="sxs-lookup"><span data-stu-id="11827-167">Android restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="11827-168">андроидфорворкрестриктион</span><span class="sxs-lookup"><span data-stu-id="11827-168">androidForWorkRestriction</span></span>|[<span data-ttu-id="11827-169">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="11827-169">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="11827-170">Ограничения для Android для работы на основе платформы, версии операционной системы платформы и владельца устройств</span><span class="sxs-lookup"><span data-stu-id="11827-170">Android for work restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="11827-171">макрестриктион</span><span class="sxs-lookup"><span data-stu-id="11827-171">macRestriction</span></span>|[<span data-ttu-id="11827-172">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="11827-172">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="11827-173">Ограничения для MAC-адресов на основе платформы, версии операционной системы платформы и владельца устройств</span><span class="sxs-lookup"><span data-stu-id="11827-173">Mac restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="11827-174">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="11827-174">macOSRestriction</span></span>|[<span data-ttu-id="11827-175">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="11827-175">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="11827-176">Ограничения для MAC-адресов на основе платформы, версии операционной системы платформы и владельца устройств</span><span class="sxs-lookup"><span data-stu-id="11827-176">Mac restrictions based on platform, platform operating system version, and device ownership</span></span>|



## <a name="response"></a><span data-ttu-id="11827-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="11827-177">Response</span></span>
<span data-ttu-id="11827-178">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="11827-178">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11827-179">Пример</span><span class="sxs-lookup"><span data-stu-id="11827-179">Example</span></span>

### <a name="request"></a><span data-ttu-id="11827-180">Запрос</span><span class="sxs-lookup"><span data-stu-id="11827-180">Request</span></span>
<span data-ttu-id="11827-181">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="11827-181">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
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

### <a name="response"></a><span data-ttu-id="11827-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="11827-182">Response</span></span>
<span data-ttu-id="11827-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="11827-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





