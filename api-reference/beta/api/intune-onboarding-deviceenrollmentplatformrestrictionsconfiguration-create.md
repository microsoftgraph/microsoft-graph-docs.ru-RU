---
title: Создание объекта deviceEnrollmentPlatformRestrictionsConfiguration
description: Создание объекта deviceEnrollmentPlatformRestrictionsConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 87d2bf92540e15b2f27675580b4a0b2ecafc5365
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43450433"
---
# <a name="create-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="7c2a0-103">Создание объекта deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="7c2a0-103">Create deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

<span data-ttu-id="7c2a0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c2a0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7c2a0-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c2a0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7c2a0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7c2a0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c2a0-107">Создание объекта [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7c2a0-107">Create a new [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7c2a0-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7c2a0-108">Prerequisites</span></span>
<span data-ttu-id="7c2a0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c2a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c2a0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7c2a0-111">Permission type</span></span>|<span data-ttu-id="7c2a0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7c2a0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c2a0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7c2a0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7c2a0-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c2a0-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7c2a0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7c2a0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c2a0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c2a0-116">Not supported.</span></span>|
|<span data-ttu-id="7c2a0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7c2a0-117">Application</span></span>|<span data-ttu-id="7c2a0-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c2a0-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c2a0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7c2a0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7c2a0-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7c2a0-120">Request headers</span></span>
|<span data-ttu-id="7c2a0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7c2a0-121">Header</span></span>|<span data-ttu-id="7c2a0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7c2a0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c2a0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c2a0-123">Authorization</span></span>|<span data-ttu-id="7c2a0-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7c2a0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c2a0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7c2a0-125">Accept</span></span>|<span data-ttu-id="7c2a0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7c2a0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c2a0-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7c2a0-127">Request body</span></span>
<span data-ttu-id="7c2a0-128">В теле запроса добавьте представление объекта deviceEnrollmentPlatformRestrictionsConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7c2a0-128">In the request body, supply a JSON representation for the deviceEnrollmentPlatformRestrictionsConfiguration object.</span></span>

<span data-ttu-id="7c2a0-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceEnrollmentPlatformRestrictionsConfiguration.</span><span class="sxs-lookup"><span data-stu-id="7c2a0-129">The following table shows the properties that are required when you create the deviceEnrollmentPlatformRestrictionsConfiguration.</span></span>

|<span data-ttu-id="7c2a0-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7c2a0-130">Property</span></span>|<span data-ttu-id="7c2a0-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7c2a0-131">Type</span></span>|<span data-ttu-id="7c2a0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7c2a0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c2a0-133">id</span><span class="sxs-lookup"><span data-stu-id="7c2a0-133">id</span></span>|<span data-ttu-id="7c2a0-134">String</span><span class="sxs-lookup"><span data-stu-id="7c2a0-134">String</span></span>|<span data-ttu-id="7c2a0-135">Уникальный идентификатор для учетной записи, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7c2a0-135">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7c2a0-136">displayName</span><span class="sxs-lookup"><span data-stu-id="7c2a0-136">displayName</span></span>|<span data-ttu-id="7c2a0-137">Строка</span><span class="sxs-lookup"><span data-stu-id="7c2a0-137">String</span></span>|<span data-ttu-id="7c2a0-138">Отображаемое имя конфигурации регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7c2a0-138">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7c2a0-139">description</span><span class="sxs-lookup"><span data-stu-id="7c2a0-139">description</span></span>|<span data-ttu-id="7c2a0-140">String</span><span class="sxs-lookup"><span data-stu-id="7c2a0-140">String</span></span>|<span data-ttu-id="7c2a0-141">Описание конфигурации регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7c2a0-141">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7c2a0-142">priority</span><span class="sxs-lookup"><span data-stu-id="7c2a0-142">priority</span></span>|<span data-ttu-id="7c2a0-143">Int32</span><span class="sxs-lookup"><span data-stu-id="7c2a0-143">Int32</span></span>|<span data-ttu-id="7c2a0-144">Priority используется, когда пользователь существует в нескольких группах, которым назначена Настройка регистрации.</span><span class="sxs-lookup"><span data-stu-id="7c2a0-144">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="7c2a0-145">Пользователи подчиняются только конфигурации с наименьшим значением приоритета.</span><span class="sxs-lookup"><span data-stu-id="7c2a0-145">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="7c2a0-146">Наследуется от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7c2a0-146">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7c2a0-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7c2a0-147">createdDateTime</span></span>|<span data-ttu-id="7c2a0-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c2a0-148">DateTimeOffset</span></span>|<span data-ttu-id="7c2a0-149">Созданная Дата и время в формате UTC для настройки регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7c2a0-149">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7c2a0-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7c2a0-150">lastModifiedDateTime</span></span>|<span data-ttu-id="7c2a0-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c2a0-151">DateTimeOffset</span></span>|<span data-ttu-id="7c2a0-152">Дата и время последнего изменения конфигурации регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7c2a0-152">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7c2a0-153">version</span><span class="sxs-lookup"><span data-stu-id="7c2a0-153">version</span></span>|<span data-ttu-id="7c2a0-154">Int32</span><span class="sxs-lookup"><span data-stu-id="7c2a0-154">Int32</span></span>|<span data-ttu-id="7c2a0-155">Версия конфигурации регистрации устройств, унаследованная от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7c2a0-155">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7c2a0-156">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="7c2a0-156">iosRestriction</span></span>|[<span data-ttu-id="7c2a0-157">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="7c2a0-157">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="7c2a0-158">Ограничения iOS на основе платформы, версии операционной системы платформы и владельца устройств</span><span class="sxs-lookup"><span data-stu-id="7c2a0-158">Ios restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="7c2a0-159">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="7c2a0-159">windowsRestriction</span></span>|[<span data-ttu-id="7c2a0-160">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="7c2a0-160">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="7c2a0-161">Ограничения Windows на основе платформы, версии операционной системы платформы и владельца устройств</span><span class="sxs-lookup"><span data-stu-id="7c2a0-161">Windows restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="7c2a0-162">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="7c2a0-162">windowsMobileRestriction</span></span>|[<span data-ttu-id="7c2a0-163">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="7c2a0-163">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="7c2a0-164">Ограничения для Windows Mobile на основе платформы, версии операционной системы платформы и владельца устройств</span><span class="sxs-lookup"><span data-stu-id="7c2a0-164">Windows mobile restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="7c2a0-165">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="7c2a0-165">androidRestriction</span></span>|[<span data-ttu-id="7c2a0-166">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="7c2a0-166">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="7c2a0-167">Ограничения для Android на основе платформы, версии операционной системы платформы и владельца устройств</span><span class="sxs-lookup"><span data-stu-id="7c2a0-167">Android restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="7c2a0-168">андроидфорворкрестриктион</span><span class="sxs-lookup"><span data-stu-id="7c2a0-168">androidForWorkRestriction</span></span>|[<span data-ttu-id="7c2a0-169">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="7c2a0-169">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="7c2a0-170">Ограничения для Android для работы на основе платформы, версии операционной системы платформы и владельца устройств</span><span class="sxs-lookup"><span data-stu-id="7c2a0-170">Android for work restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="7c2a0-171">макрестриктион</span><span class="sxs-lookup"><span data-stu-id="7c2a0-171">macRestriction</span></span>|[<span data-ttu-id="7c2a0-172">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="7c2a0-172">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="7c2a0-173">Ограничения для MAC-адресов на основе платформы, версии операционной системы платформы и владельца устройств</span><span class="sxs-lookup"><span data-stu-id="7c2a0-173">Mac restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="7c2a0-174">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="7c2a0-174">macOSRestriction</span></span>|[<span data-ttu-id="7c2a0-175">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="7c2a0-175">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="7c2a0-176">Ограничения для MAC-адресов на основе платформы, версии операционной системы платформы и владельца устройств</span><span class="sxs-lookup"><span data-stu-id="7c2a0-176">Mac restrictions based on platform, platform operating system version, and device ownership</span></span>|



## <a name="response"></a><span data-ttu-id="7c2a0-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c2a0-177">Response</span></span>
<span data-ttu-id="7c2a0-178">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7c2a0-178">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c2a0-179">Пример</span><span class="sxs-lookup"><span data-stu-id="7c2a0-179">Example</span></span>

### <a name="request"></a><span data-ttu-id="7c2a0-180">Запрос</span><span class="sxs-lookup"><span data-stu-id="7c2a0-180">Request</span></span>
<span data-ttu-id="7c2a0-181">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7c2a0-181">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7c2a0-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c2a0-182">Response</span></span>
<span data-ttu-id="7c2a0-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7c2a0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



