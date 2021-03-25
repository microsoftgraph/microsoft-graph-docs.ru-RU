---
title: Обновление объекта deviceEnrollmentPlatformRestrictionsConfiguration
description: Обновление свойств объекта deviceEnrollmentPlatformRestrictionsConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fb36e187a54b91f1e05c9c8ad14fa58138dd111c
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51158873"
---
# <a name="update-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="71c21-103">Обновление объекта deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="71c21-103">Update deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

<span data-ttu-id="71c21-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71c21-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="71c21-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71c21-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="71c21-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="71c21-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71c21-107">Обновление свойств объекта [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="71c21-107">Update the properties of a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="71c21-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="71c21-108">Prerequisites</span></span>
<span data-ttu-id="71c21-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71c21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71c21-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71c21-111">Permission type</span></span>|<span data-ttu-id="71c21-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="71c21-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71c21-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71c21-113">Delegated (work or school account)</span></span>|<span data-ttu-id="71c21-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71c21-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="71c21-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71c21-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71c21-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71c21-116">Not supported.</span></span>|
|<span data-ttu-id="71c21-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="71c21-117">Application</span></span>|<span data-ttu-id="71c21-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71c21-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="71c21-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71c21-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="71c21-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="71c21-120">Request headers</span></span>
|<span data-ttu-id="71c21-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="71c21-121">Header</span></span>|<span data-ttu-id="71c21-122">Значение</span><span class="sxs-lookup"><span data-stu-id="71c21-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71c21-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="71c21-123">Authorization</span></span>|<span data-ttu-id="71c21-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="71c21-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71c21-125">Accept</span><span class="sxs-lookup"><span data-stu-id="71c21-125">Accept</span></span>|<span data-ttu-id="71c21-126">application/json</span><span class="sxs-lookup"><span data-stu-id="71c21-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71c21-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="71c21-127">Request body</span></span>
<span data-ttu-id="71c21-128">В теле запроса добавьте представление объекта [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="71c21-128">In the request body, supply a JSON representation for the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

<span data-ttu-id="71c21-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="71c21-129">The following table shows the properties that are required when you create the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).</span></span>

|<span data-ttu-id="71c21-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="71c21-130">Property</span></span>|<span data-ttu-id="71c21-131">Тип</span><span class="sxs-lookup"><span data-stu-id="71c21-131">Type</span></span>|<span data-ttu-id="71c21-132">Описание</span><span class="sxs-lookup"><span data-stu-id="71c21-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71c21-133">id</span><span class="sxs-lookup"><span data-stu-id="71c21-133">id</span></span>|<span data-ttu-id="71c21-134">Строка</span><span class="sxs-lookup"><span data-stu-id="71c21-134">String</span></span>|<span data-ttu-id="71c21-135">Уникальный идентификатор учетной записи, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71c21-135">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="71c21-136">displayName</span><span class="sxs-lookup"><span data-stu-id="71c21-136">displayName</span></span>|<span data-ttu-id="71c21-137">Строка</span><span class="sxs-lookup"><span data-stu-id="71c21-137">String</span></span>|<span data-ttu-id="71c21-138">Отображающее имя конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71c21-138">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="71c21-139">description</span><span class="sxs-lookup"><span data-stu-id="71c21-139">description</span></span>|<span data-ttu-id="71c21-140">Строка</span><span class="sxs-lookup"><span data-stu-id="71c21-140">String</span></span>|<span data-ttu-id="71c21-141">Описание конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71c21-141">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="71c21-142">priority</span><span class="sxs-lookup"><span data-stu-id="71c21-142">priority</span></span>|<span data-ttu-id="71c21-143">Int32</span><span class="sxs-lookup"><span data-stu-id="71c21-143">Int32</span></span>|<span data-ttu-id="71c21-144">Приоритет используется, когда пользователь существует в нескольких группах, которые назначены конфигурации регистрации.</span><span class="sxs-lookup"><span data-stu-id="71c21-144">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="71c21-145">Пользователи подчиняются только конфигурации с наименьшим значением приоритета.</span><span class="sxs-lookup"><span data-stu-id="71c21-145">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="71c21-146">Наследуется от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71c21-146">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="71c21-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="71c21-147">createdDateTime</span></span>|<span data-ttu-id="71c21-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71c21-148">DateTimeOffset</span></span>|<span data-ttu-id="71c21-149">Создано время даты в UTC конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71c21-149">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="71c21-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="71c21-150">lastModifiedDateTime</span></span>|<span data-ttu-id="71c21-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71c21-151">DateTimeOffset</span></span>|<span data-ttu-id="71c21-152">Последнее измененное время даты в UTC конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71c21-152">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="71c21-153">version</span><span class="sxs-lookup"><span data-stu-id="71c21-153">version</span></span>|<span data-ttu-id="71c21-154">Int32</span><span class="sxs-lookup"><span data-stu-id="71c21-154">Int32</span></span>|<span data-ttu-id="71c21-155">Версия конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71c21-155">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="71c21-156">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="71c21-156">roleScopeTagIds</span></span>|<span data-ttu-id="71c21-157">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="71c21-157">String collection</span></span>|<span data-ttu-id="71c21-158">Необязательные теги области ролей для ограничений регистрации.</span><span class="sxs-lookup"><span data-stu-id="71c21-158">Optional role scope tags for the enrollment restrictions.</span></span> <span data-ttu-id="71c21-159">Наследуется от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71c21-159">Inherited from [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="71c21-160">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="71c21-160">iosRestriction</span></span>|[<span data-ttu-id="71c21-161">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="71c21-161">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="71c21-162">Ограничения IOS на основе платформы, версии операционной системы платформы и владения устройствами</span><span class="sxs-lookup"><span data-stu-id="71c21-162">Ios restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="71c21-163">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="71c21-163">windowsRestriction</span></span>|[<span data-ttu-id="71c21-164">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="71c21-164">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="71c21-165">Ограничения Windows на основе платформы, версии операционной системы платформы и владения устройствами</span><span class="sxs-lookup"><span data-stu-id="71c21-165">Windows restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="71c21-166">windowsHomeSkuRestriction</span><span class="sxs-lookup"><span data-stu-id="71c21-166">windowsHomeSkuRestriction</span></span>|[<span data-ttu-id="71c21-167">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="71c21-167">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="71c21-168">Ограничения Windows Home Sku на основе платформы, версии операционной системы платформы и владения устройствами</span><span class="sxs-lookup"><span data-stu-id="71c21-168">Windows Home Sku restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="71c21-169">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="71c21-169">windowsMobileRestriction</span></span>|[<span data-ttu-id="71c21-170">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="71c21-170">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="71c21-171">Ограничения для мобильных устройств Windows на основе платформы, версии операционной системы платформы и владения устройствами</span><span class="sxs-lookup"><span data-stu-id="71c21-171">Windows mobile restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="71c21-172">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="71c21-172">androidRestriction</span></span>|[<span data-ttu-id="71c21-173">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="71c21-173">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="71c21-174">Ограничения для Android на основе платформы, версии операционной системы платформы и владения устройствами</span><span class="sxs-lookup"><span data-stu-id="71c21-174">Android restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="71c21-175">AndroidForWorkRestriction</span><span class="sxs-lookup"><span data-stu-id="71c21-175">androidForWorkRestriction</span></span>|[<span data-ttu-id="71c21-176">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="71c21-176">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="71c21-177">Ограничения для android для работы на основе платформы, версии операционной системы платформы и владения устройствами</span><span class="sxs-lookup"><span data-stu-id="71c21-177">Android for work restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="71c21-178">aospRestriction</span><span class="sxs-lookup"><span data-stu-id="71c21-178">aospRestriction</span></span>|[<span data-ttu-id="71c21-179">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="71c21-179">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="71c21-180">Ограничения AOSP на основе платформы, версии операционной системы платформы и владения устройствами</span><span class="sxs-lookup"><span data-stu-id="71c21-180">AOSP restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="71c21-181">macRestriction</span><span class="sxs-lookup"><span data-stu-id="71c21-181">macRestriction</span></span>|[<span data-ttu-id="71c21-182">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="71c21-182">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="71c21-183">Ограничения Mac на основе платформы, версии операционной системы платформы и владения устройствами</span><span class="sxs-lookup"><span data-stu-id="71c21-183">Mac restrictions based on platform, platform operating system version, and device ownership</span></span>|
|<span data-ttu-id="71c21-184">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="71c21-184">macOSRestriction</span></span>|[<span data-ttu-id="71c21-185">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="71c21-185">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|<span data-ttu-id="71c21-186">Ограничения Mac на основе платформы, версии операционной системы платформы и владения устройствами</span><span class="sxs-lookup"><span data-stu-id="71c21-186">Mac restrictions based on platform, platform operating system version, and device ownership</span></span>|



## <a name="response"></a><span data-ttu-id="71c21-187">Отклик</span><span class="sxs-lookup"><span data-stu-id="71c21-187">Response</span></span>
<span data-ttu-id="71c21-188">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="71c21-188">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71c21-189">Пример</span><span class="sxs-lookup"><span data-stu-id="71c21-189">Example</span></span>

### <a name="request"></a><span data-ttu-id="71c21-190">Запрос</span><span class="sxs-lookup"><span data-stu-id="71c21-190">Request</span></span>
<span data-ttu-id="71c21-191">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="71c21-191">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 4081

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
    ],
    "blockedSkus": [
      "Blocked Skus value"
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
    ],
    "blockedSkus": [
      "Blocked Skus value"
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
    ],
    "blockedSkus": [
      "Blocked Skus value"
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
    ],
    "blockedSkus": [
      "Blocked Skus value"
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
    ],
    "blockedSkus": [
      "Blocked Skus value"
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
    ],
    "blockedSkus": [
      "Blocked Skus value"
    ]
  },
  "aospRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "blockedManufacturers": [
      "Blocked Manufacturers value"
    ],
    "blockedSkus": [
      "Blocked Skus value"
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
    ],
    "blockedSkus": [
      "Blocked Skus value"
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
    ],
    "blockedSkus": [
      "Blocked Skus value"
    ]
  }
}
```

### <a name="response"></a><span data-ttu-id="71c21-192">Отклик</span><span class="sxs-lookup"><span data-stu-id="71c21-192">Response</span></span>
<span data-ttu-id="71c21-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="71c21-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4253

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
    ],
    "blockedSkus": [
      "Blocked Skus value"
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
    ],
    "blockedSkus": [
      "Blocked Skus value"
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
    ],
    "blockedSkus": [
      "Blocked Skus value"
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
    ],
    "blockedSkus": [
      "Blocked Skus value"
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
    ],
    "blockedSkus": [
      "Blocked Skus value"
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
    ],
    "blockedSkus": [
      "Blocked Skus value"
    ]
  },
  "aospRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "blockedManufacturers": [
      "Blocked Manufacturers value"
    ],
    "blockedSkus": [
      "Blocked Skus value"
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
    ],
    "blockedSkus": [
      "Blocked Skus value"
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
    ],
    "blockedSkus": [
      "Blocked Skus value"
    ]
  }
}
```




