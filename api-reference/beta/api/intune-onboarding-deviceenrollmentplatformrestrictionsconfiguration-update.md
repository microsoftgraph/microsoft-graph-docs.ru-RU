---
title: Обновление объекта deviceEnrollmentPlatformRestrictionsConfiguration
description: Обновление свойств объекта deviceEnrollmentPlatformRestrictionsConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ba5b9fa4499bd3885c505342d911f9db5ef04486
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48725652"
---
# <a name="update-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="3d24f-103">Обновление объекта deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="3d24f-103">Update deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

<span data-ttu-id="3d24f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d24f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3d24f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d24f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3d24f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3d24f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d24f-107">Обновление свойств объекта [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3d24f-107">Update the properties of a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3d24f-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3d24f-108">Prerequisites</span></span>
<span data-ttu-id="3d24f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d24f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d24f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3d24f-111">Permission type</span></span>|<span data-ttu-id="3d24f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3d24f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3d24f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3d24f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3d24f-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d24f-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3d24f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3d24f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3d24f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d24f-116">Not supported.</span></span>|
|<span data-ttu-id="3d24f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3d24f-117">Application</span></span>|<span data-ttu-id="3d24f-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d24f-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3d24f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3d24f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="3d24f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3d24f-120">Request headers</span></span>
|<span data-ttu-id="3d24f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3d24f-121">Header</span></span>|<span data-ttu-id="3d24f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3d24f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3d24f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3d24f-123">Authorization</span></span>|<span data-ttu-id="3d24f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3d24f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3d24f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3d24f-125">Accept</span></span>|<span data-ttu-id="3d24f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3d24f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d24f-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3d24f-127">Request body</span></span>
<span data-ttu-id="3d24f-128">В теле запроса добавьте представление объекта [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3d24f-128">In the request body, supply a JSON representation for the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

<span data-ttu-id="3d24f-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3d24f-129">The following table shows the properties that are required when you create the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span></span>

|<span data-ttu-id="3d24f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3d24f-130">Property</span></span>|<span data-ttu-id="3d24f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3d24f-131">Type</span></span>|<span data-ttu-id="3d24f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3d24f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d24f-133">id</span><span class="sxs-lookup"><span data-stu-id="3d24f-133">id</span></span>|<span data-ttu-id="3d24f-134">Строка</span><span class="sxs-lookup"><span data-stu-id="3d24f-134">String</span></span>|<span data-ttu-id="3d24f-135">Уникальный идентификатор для учетной записи, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3d24f-135">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3d24f-136">displayName</span><span class="sxs-lookup"><span data-stu-id="3d24f-136">displayName</span></span>|<span data-ttu-id="3d24f-137">Строка</span><span class="sxs-lookup"><span data-stu-id="3d24f-137">String</span></span>|<span data-ttu-id="3d24f-138">Отображаемое имя конфигурации регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3d24f-138">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3d24f-139">description</span><span class="sxs-lookup"><span data-stu-id="3d24f-139">description</span></span>|<span data-ttu-id="3d24f-140">Строка</span><span class="sxs-lookup"><span data-stu-id="3d24f-140">String</span></span>|<span data-ttu-id="3d24f-141">Описание конфигурации регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3d24f-141">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3d24f-142">priority</span><span class="sxs-lookup"><span data-stu-id="3d24f-142">priority</span></span>|<span data-ttu-id="3d24f-143">Int32</span><span class="sxs-lookup"><span data-stu-id="3d24f-143">Int32</span></span>|<span data-ttu-id="3d24f-144">Priority используется, когда пользователь существует в нескольких группах, которым назначена Настройка регистрации.</span><span class="sxs-lookup"><span data-stu-id="3d24f-144">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="3d24f-145">Пользователи подчиняются только конфигурации с наименьшим значением приоритета.</span><span class="sxs-lookup"><span data-stu-id="3d24f-145">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="3d24f-146">Наследуется от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3d24f-146">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3d24f-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3d24f-147">createdDateTime</span></span>|<span data-ttu-id="3d24f-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d24f-148">DateTimeOffset</span></span>|<span data-ttu-id="3d24f-149">Созданная Дата и время в формате UTC для настройки регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3d24f-149">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3d24f-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3d24f-150">lastModifiedDateTime</span></span>|<span data-ttu-id="3d24f-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d24f-151">DateTimeOffset</span></span>|<span data-ttu-id="3d24f-152">Дата и время последнего изменения конфигурации регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3d24f-152">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3d24f-153">version</span><span class="sxs-lookup"><span data-stu-id="3d24f-153">version</span></span>|<span data-ttu-id="3d24f-154">Int32</span><span class="sxs-lookup"><span data-stu-id="3d24f-154">Int32</span></span>|<span data-ttu-id="3d24f-155">Версия конфигурации регистрации устройств, унаследованная от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3d24f-155">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3d24f-156">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3d24f-156">roleScopeTagIds</span></span>|<span data-ttu-id="3d24f-157">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="3d24f-157">String collection</span></span>|<span data-ttu-id="3d24f-158">Необязательные теги области применения роли для ограничений регистрации.</span><span class="sxs-lookup"><span data-stu-id="3d24f-158">Optional role scope tags for the enrollment restrictions.</span></span> <span data-ttu-id="3d24f-159">Наследуется от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3d24f-159">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="3d24f-160">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="3d24f-160">iosRestriction</span></span>|[<span data-ttu-id="3d24f-161">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="3d24f-161">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="3d24f-162">Ограничения iOS на основе платформы, версии операционной системы платформы и владельца устройств</span><span class="sxs-lookup"><span data-stu-id="3d24f-162">Ios restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="3d24f-163">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="3d24f-163">windowsRestriction</span></span>|[<span data-ttu-id="3d24f-164">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="3d24f-164">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="3d24f-165">Ограничения Windows на основе платформы, версии операционной системы платформы и владельца устройств</span><span class="sxs-lookup"><span data-stu-id="3d24f-165">Windows restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="3d24f-166">виндовшомескурестриктион</span><span class="sxs-lookup"><span data-stu-id="3d24f-166">windowsHomeSkuRestriction</span></span>|[<span data-ttu-id="3d24f-167">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="3d24f-167">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="3d24f-168">Ограничения для Windows Home SKU на основе платформы, версии операционной системы платформы и владельца устройств</span><span class="sxs-lookup"><span data-stu-id="3d24f-168">Windows Home Sku restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="3d24f-169">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="3d24f-169">windowsMobileRestriction</span></span>|[<span data-ttu-id="3d24f-170">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="3d24f-170">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="3d24f-171">Ограничения для Windows Mobile на основе платформы, версии операционной системы платформы и владельца устройств</span><span class="sxs-lookup"><span data-stu-id="3d24f-171">Windows mobile restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="3d24f-172">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="3d24f-172">androidRestriction</span></span>|[<span data-ttu-id="3d24f-173">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="3d24f-173">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="3d24f-174">Ограничения для Android на основе платформы, версии операционной системы платформы и владельца устройств</span><span class="sxs-lookup"><span data-stu-id="3d24f-174">Android restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="3d24f-175">андроидфорворкрестриктион</span><span class="sxs-lookup"><span data-stu-id="3d24f-175">androidForWorkRestriction</span></span>|[<span data-ttu-id="3d24f-176">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="3d24f-176">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="3d24f-177">Ограничения для Android для работы на основе платформы, версии операционной системы платформы и владельца устройств</span><span class="sxs-lookup"><span data-stu-id="3d24f-177">Android for work restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="3d24f-178">макрестриктион</span><span class="sxs-lookup"><span data-stu-id="3d24f-178">macRestriction</span></span>|[<span data-ttu-id="3d24f-179">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="3d24f-179">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="3d24f-180">Ограничения для MAC-адресов на основе платформы, версии операционной системы платформы и владельца устройств</span><span class="sxs-lookup"><span data-stu-id="3d24f-180">Mac restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="3d24f-181">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="3d24f-181">macOSRestriction</span></span>|[<span data-ttu-id="3d24f-182">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="3d24f-182">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="3d24f-183">Ограничения для MAC-адресов на основе платформы, версии операционной системы платформы и владельца устройств</span><span class="sxs-lookup"><span data-stu-id="3d24f-183">Mac restrictions based on platform, platform operating system version, and device ownership</span></span>|



## <a name="response"></a><span data-ttu-id="3d24f-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d24f-184">Response</span></span>
<span data-ttu-id="3d24f-185">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3d24f-185">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d24f-186">Пример</span><span class="sxs-lookup"><span data-stu-id="3d24f-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="3d24f-187">Запрос</span><span class="sxs-lookup"><span data-stu-id="3d24f-187">Request</span></span>
<span data-ttu-id="3d24f-188">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3d24f-188">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 3197

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestrictionsConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "version": 7,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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
  "windowsHomeSkuRestriction": {
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

### <a name="response"></a><span data-ttu-id="3d24f-189">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d24f-189">Response</span></span>
<span data-ttu-id="3d24f-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3d24f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3369

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestrictionsConfiguration",
  "id": "3acb2d75-2d75-3acb-752d-cb3a752dcb3a",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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
  "windowsHomeSkuRestriction": {
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





