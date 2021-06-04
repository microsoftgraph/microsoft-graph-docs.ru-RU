---
title: Обновление объекта deviceEnrollmentPlatformRestrictionsConfiguration
description: Обновление свойств объекта deviceEnrollmentPlatformRestrictionsConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bc975ab57cd3ed81ab71c9260c66e717fd37faea
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52743730"
---
# <a name="update-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="13250-103">Обновление объекта deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="13250-103">Update deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

<span data-ttu-id="13250-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13250-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="13250-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="13250-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13250-106">Обновление свойств объекта [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="13250-106">Update the properties of a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13250-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="13250-107">Prerequisites</span></span>
<span data-ttu-id="13250-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13250-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13250-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="13250-110">Permission type</span></span>|<span data-ttu-id="13250-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="13250-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13250-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="13250-112">Delegated (work or school account)</span></span>|<span data-ttu-id="13250-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13250-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="13250-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="13250-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13250-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13250-115">Not supported.</span></span>|
|<span data-ttu-id="13250-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="13250-116">Application</span></span>|<span data-ttu-id="13250-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13250-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="13250-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="13250-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="13250-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="13250-119">Request headers</span></span>
|<span data-ttu-id="13250-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="13250-120">Header</span></span>|<span data-ttu-id="13250-121">Значение</span><span class="sxs-lookup"><span data-stu-id="13250-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13250-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="13250-122">Authorization</span></span>|<span data-ttu-id="13250-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="13250-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13250-124">Accept</span><span class="sxs-lookup"><span data-stu-id="13250-124">Accept</span></span>|<span data-ttu-id="13250-125">application/json</span><span class="sxs-lookup"><span data-stu-id="13250-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13250-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="13250-126">Request body</span></span>
<span data-ttu-id="13250-127">В теле запроса добавьте представление объекта [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="13250-127">In the request body, supply a JSON representation for the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

<span data-ttu-id="13250-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="13250-128">The following table shows the properties that are required when you create the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span></span>

|<span data-ttu-id="13250-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="13250-129">Property</span></span>|<span data-ttu-id="13250-130">Тип</span><span class="sxs-lookup"><span data-stu-id="13250-130">Type</span></span>|<span data-ttu-id="13250-131">Описание</span><span class="sxs-lookup"><span data-stu-id="13250-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13250-132">id</span><span class="sxs-lookup"><span data-stu-id="13250-132">id</span></span>|<span data-ttu-id="13250-133">String</span><span class="sxs-lookup"><span data-stu-id="13250-133">String</span></span>|<span data-ttu-id="13250-134">Уникальный идентификатор учетной записи, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="13250-134">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="13250-135">displayName</span><span class="sxs-lookup"><span data-stu-id="13250-135">displayName</span></span>|<span data-ttu-id="13250-136">String</span><span class="sxs-lookup"><span data-stu-id="13250-136">String</span></span>|<span data-ttu-id="13250-137">Отображающее имя конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="13250-137">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="13250-138">description</span><span class="sxs-lookup"><span data-stu-id="13250-138">description</span></span>|<span data-ttu-id="13250-139">String</span><span class="sxs-lookup"><span data-stu-id="13250-139">String</span></span>|<span data-ttu-id="13250-140">Описание конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="13250-140">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="13250-141">priority</span><span class="sxs-lookup"><span data-stu-id="13250-141">priority</span></span>|<span data-ttu-id="13250-142">Int32</span><span class="sxs-lookup"><span data-stu-id="13250-142">Int32</span></span>|<span data-ttu-id="13250-143">Приоритет используется, когда пользователь существует в нескольких группах, которые назначены конфигурации регистрации.</span><span class="sxs-lookup"><span data-stu-id="13250-143">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="13250-144">Пользователи подчиняются только конфигурации с наименьшим значением приоритета.</span><span class="sxs-lookup"><span data-stu-id="13250-144">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="13250-145">Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="13250-145">Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="13250-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="13250-146">createdDateTime</span></span>|<span data-ttu-id="13250-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13250-147">DateTimeOffset</span></span>|<span data-ttu-id="13250-148">Создано время даты в UTC конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="13250-148">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="13250-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="13250-149">lastModifiedDateTime</span></span>|<span data-ttu-id="13250-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13250-150">DateTimeOffset</span></span>|<span data-ttu-id="13250-151">Последнее измененное время даты в UTC конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="13250-151">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="13250-152">version</span><span class="sxs-lookup"><span data-stu-id="13250-152">version</span></span>|<span data-ttu-id="13250-153">Int32</span><span class="sxs-lookup"><span data-stu-id="13250-153">Int32</span></span>|<span data-ttu-id="13250-154">Версия конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="13250-154">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="13250-155">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="13250-155">iosRestriction</span></span>|[<span data-ttu-id="13250-156">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="13250-156">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="13250-157">Ограничения IOS на основе платформы, версии операционной системы платформы и владения устройствами</span><span class="sxs-lookup"><span data-stu-id="13250-157">Ios restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="13250-158">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="13250-158">windowsRestriction</span></span>|[<span data-ttu-id="13250-159">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="13250-159">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="13250-160">Windows на основе платформы, версии операционной системы платформы и владения устройствами</span><span class="sxs-lookup"><span data-stu-id="13250-160">Windows restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="13250-161">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="13250-161">windowsMobileRestriction</span></span>|[<span data-ttu-id="13250-162">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="13250-162">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="13250-163">Windows на основе платформы, версии операционной системы платформы и владения устройствами</span><span class="sxs-lookup"><span data-stu-id="13250-163">Windows mobile restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="13250-164">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="13250-164">androidRestriction</span></span>|[<span data-ttu-id="13250-165">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="13250-165">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="13250-166">Ограничения для Android на основе платформы, версии операционной системы платформы и владения устройствами</span><span class="sxs-lookup"><span data-stu-id="13250-166">Android restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="13250-167">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="13250-167">macOSRestriction</span></span>|[<span data-ttu-id="13250-168">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="13250-168">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="13250-169">Ограничения Mac на основе платформы, версии операционной системы платформы и владения устройствами</span><span class="sxs-lookup"><span data-stu-id="13250-169">Mac restrictions based on platform, platform operating system version, and device ownership</span></span>|



## <a name="response"></a><span data-ttu-id="13250-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="13250-170">Response</span></span>
<span data-ttu-id="13250-171">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="13250-171">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13250-172">Пример</span><span class="sxs-lookup"><span data-stu-id="13250-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="13250-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="13250-173">Request</span></span>
<span data-ttu-id="13250-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="13250-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 1650

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
    "osMaximumVersion": "Os Maximum Version value"
  },
  "windowsRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "windowsMobileRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "androidRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "macOSRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  }
}
```

### <a name="response"></a><span data-ttu-id="13250-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="13250-175">Response</span></span>
<span data-ttu-id="13250-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="13250-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1822

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
    "osMaximumVersion": "Os Maximum Version value"
  },
  "windowsRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "windowsMobileRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "androidRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "macOSRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  }
}
```




