---
title: Обновление объекта deviceEnrollmentPlatformRestrictionsConfiguration
description: Обновление свойств объекта deviceEnrollmentPlatformRestrictionsConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1486450fe936394c04bff2f8d5144cc56f71d341
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37536611"
---
# <a name="update-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="46ff9-103">Обновление объекта deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="46ff9-103">Update deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="46ff9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46ff9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="46ff9-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="46ff9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46ff9-106">Обновление свойств объекта [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="46ff9-106">Update the properties of a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="46ff9-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="46ff9-107">Prerequisites</span></span>
<span data-ttu-id="46ff9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46ff9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46ff9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="46ff9-110">Permission type</span></span>|<span data-ttu-id="46ff9-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="46ff9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46ff9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="46ff9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="46ff9-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46ff9-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="46ff9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="46ff9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46ff9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46ff9-115">Not supported.</span></span>|
|<span data-ttu-id="46ff9-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="46ff9-116">Application</span></span>|<span data-ttu-id="46ff9-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46ff9-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="46ff9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="46ff9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="46ff9-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="46ff9-119">Request headers</span></span>
|<span data-ttu-id="46ff9-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="46ff9-120">Header</span></span>|<span data-ttu-id="46ff9-121">Значение</span><span class="sxs-lookup"><span data-stu-id="46ff9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46ff9-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="46ff9-122">Authorization</span></span>|<span data-ttu-id="46ff9-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="46ff9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46ff9-124">Accept</span><span class="sxs-lookup"><span data-stu-id="46ff9-124">Accept</span></span>|<span data-ttu-id="46ff9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="46ff9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46ff9-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="46ff9-126">Request body</span></span>
<span data-ttu-id="46ff9-127">В теле запроса добавьте представление объекта [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="46ff9-127">In the request body, supply a JSON representation for the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

<span data-ttu-id="46ff9-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="46ff9-128">The following table shows the properties that are required when you create the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span></span>

|<span data-ttu-id="46ff9-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="46ff9-129">Property</span></span>|<span data-ttu-id="46ff9-130">Тип</span><span class="sxs-lookup"><span data-stu-id="46ff9-130">Type</span></span>|<span data-ttu-id="46ff9-131">Описание</span><span class="sxs-lookup"><span data-stu-id="46ff9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46ff9-132">id</span><span class="sxs-lookup"><span data-stu-id="46ff9-132">id</span></span>|<span data-ttu-id="46ff9-133">String</span><span class="sxs-lookup"><span data-stu-id="46ff9-133">String</span></span>|<span data-ttu-id="46ff9-134">Уникальный идентификатор для учетной записи, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="46ff9-134">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="46ff9-135">displayName</span><span class="sxs-lookup"><span data-stu-id="46ff9-135">displayName</span></span>|<span data-ttu-id="46ff9-136">Строка</span><span class="sxs-lookup"><span data-stu-id="46ff9-136">String</span></span>|<span data-ttu-id="46ff9-137">Отображаемое имя конфигурации регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="46ff9-137">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="46ff9-138">description</span><span class="sxs-lookup"><span data-stu-id="46ff9-138">description</span></span>|<span data-ttu-id="46ff9-139">String</span><span class="sxs-lookup"><span data-stu-id="46ff9-139">String</span></span>|<span data-ttu-id="46ff9-140">Описание конфигурации регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="46ff9-140">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="46ff9-141">priority</span><span class="sxs-lookup"><span data-stu-id="46ff9-141">priority</span></span>|<span data-ttu-id="46ff9-142">Int32</span><span class="sxs-lookup"><span data-stu-id="46ff9-142">Int32</span></span>|<span data-ttu-id="46ff9-143">Priority используется, когда пользователь существует в нескольких группах, которым назначена Настройка регистрации.</span><span class="sxs-lookup"><span data-stu-id="46ff9-143">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="46ff9-144">Пользователи подчиняются только конфигурации с наименьшим значением приоритета.</span><span class="sxs-lookup"><span data-stu-id="46ff9-144">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="46ff9-145">Наследуется от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="46ff9-145">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="46ff9-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="46ff9-146">createdDateTime</span></span>|<span data-ttu-id="46ff9-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="46ff9-147">DateTimeOffset</span></span>|<span data-ttu-id="46ff9-148">Созданная Дата и время в формате UTC для настройки регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="46ff9-148">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="46ff9-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="46ff9-149">lastModifiedDateTime</span></span>|<span data-ttu-id="46ff9-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="46ff9-150">DateTimeOffset</span></span>|<span data-ttu-id="46ff9-151">Дата и время последнего изменения конфигурации регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="46ff9-151">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="46ff9-152">version</span><span class="sxs-lookup"><span data-stu-id="46ff9-152">version</span></span>|<span data-ttu-id="46ff9-153">Int32</span><span class="sxs-lookup"><span data-stu-id="46ff9-153">Int32</span></span>|<span data-ttu-id="46ff9-154">Версия конфигурации регистрации устройств, унаследованная от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="46ff9-154">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="46ff9-155">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="46ff9-155">iosRestriction</span></span>|[<span data-ttu-id="46ff9-156">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="46ff9-156">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="46ff9-157">Ограничения iOS на основе платформы, версии операционной системы платформы и владельца устройств</span><span class="sxs-lookup"><span data-stu-id="46ff9-157">Ios restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="46ff9-158">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="46ff9-158">windowsRestriction</span></span>|[<span data-ttu-id="46ff9-159">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="46ff9-159">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="46ff9-160">Ограничения Windows на основе платформы, версии операционной системы платформы и владельца устройств</span><span class="sxs-lookup"><span data-stu-id="46ff9-160">Windows restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="46ff9-161">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="46ff9-161">windowsMobileRestriction</span></span>|[<span data-ttu-id="46ff9-162">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="46ff9-162">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="46ff9-163">Ограничения для Windows Mobile на основе платформы, версии операционной системы платформы и владельца устройств</span><span class="sxs-lookup"><span data-stu-id="46ff9-163">Windows mobile restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="46ff9-164">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="46ff9-164">androidRestriction</span></span>|[<span data-ttu-id="46ff9-165">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="46ff9-165">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="46ff9-166">Ограничения для Android на основе платформы, версии операционной системы платформы и владельца устройств</span><span class="sxs-lookup"><span data-stu-id="46ff9-166">Android restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="46ff9-167">андроидфорворкрестриктион</span><span class="sxs-lookup"><span data-stu-id="46ff9-167">androidForWorkRestriction</span></span>|[<span data-ttu-id="46ff9-168">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="46ff9-168">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="46ff9-169">Ограничения для Android для работы на основе платформы, версии операционной системы платформы и владельца устройств</span><span class="sxs-lookup"><span data-stu-id="46ff9-169">Android for work restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="46ff9-170">макрестриктион</span><span class="sxs-lookup"><span data-stu-id="46ff9-170">macRestriction</span></span>|[<span data-ttu-id="46ff9-171">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="46ff9-171">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="46ff9-172">Ограничения для MAC-адресов на основе платформы, версии операционной системы платформы и владельца устройств</span><span class="sxs-lookup"><span data-stu-id="46ff9-172">Mac restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="46ff9-173">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="46ff9-173">macOSRestriction</span></span>|[<span data-ttu-id="46ff9-174">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="46ff9-174">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="46ff9-175">Ограничения для MAC-адресов на основе платформы, версии операционной системы платформы и владельца устройств</span><span class="sxs-lookup"><span data-stu-id="46ff9-175">Mac restrictions based on platform, platform operating system version, and device ownership</span></span>|



## <a name="response"></a><span data-ttu-id="46ff9-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="46ff9-176">Response</span></span>
<span data-ttu-id="46ff9-177">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="46ff9-177">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46ff9-178">Пример</span><span class="sxs-lookup"><span data-stu-id="46ff9-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="46ff9-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="46ff9-179">Request</span></span>
<span data-ttu-id="46ff9-180">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="46ff9-180">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 2231

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
  "androidForWorkRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "macRestriction": {
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

### <a name="response"></a><span data-ttu-id="46ff9-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="46ff9-181">Response</span></span>
<span data-ttu-id="46ff9-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="46ff9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2403

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
  "androidForWorkRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "macRestriction": {
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






