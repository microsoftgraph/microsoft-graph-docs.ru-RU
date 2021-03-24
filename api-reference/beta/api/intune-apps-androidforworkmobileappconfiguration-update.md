---
title: Обновление androidForWorkMobileAppConfiguration
description: Обновление свойств объекта AndroidForWorkMobileAppConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f723b05269bb01a7e5c0fc15bb21978bf817d7e2
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51144510"
---
# <a name="update-androidforworkmobileappconfiguration"></a><span data-ttu-id="5d57c-103">Обновление androidForWorkMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="5d57c-103">Update androidForWorkMobileAppConfiguration</span></span>

<span data-ttu-id="5d57c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d57c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5d57c-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d57c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5d57c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5d57c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5d57c-107">Обновление свойств объекта [AndroidForWorkMobileAppConfiguration.](../resources/intune-apps-androidforworkmobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5d57c-107">Update the properties of a [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5d57c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5d57c-108">Prerequisites</span></span>
<span data-ttu-id="5d57c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d57c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d57c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5d57c-111">Permission type</span></span>|<span data-ttu-id="5d57c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5d57c-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5d57c-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5d57c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5d57c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d57c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5d57c-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5d57c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5d57c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d57c-116">Not supported.</span></span>|
|<span data-ttu-id="5d57c-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="5d57c-117">Application</span></span>|<span data-ttu-id="5d57c-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d57c-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5d57c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5d57c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="5d57c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5d57c-120">Request headers</span></span>
|<span data-ttu-id="5d57c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5d57c-121">Header</span></span>|<span data-ttu-id="5d57c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5d57c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5d57c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d57c-123">Authorization</span></span>|<span data-ttu-id="5d57c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5d57c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5d57c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5d57c-125">Accept</span></span>|<span data-ttu-id="5d57c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5d57c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d57c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5d57c-127">Request body</span></span>
<span data-ttu-id="5d57c-128">В теле запроса предоставляем представление JSON для [объекта AndroidForWorkMobileAppConfiguration.](../resources/intune-apps-androidforworkmobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5d57c-128">In the request body, supply a JSON representation for the [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object.</span></span>

<span data-ttu-id="5d57c-129">В следующей таблице показаны свойства, необходимые при создании [androidForWorkMobileAppConfiguration.](../resources/intune-apps-androidforworkmobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5d57c-129">The following table shows the properties that are required when you create the [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md).</span></span>

|<span data-ttu-id="5d57c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5d57c-130">Property</span></span>|<span data-ttu-id="5d57c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5d57c-131">Type</span></span>|<span data-ttu-id="5d57c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5d57c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d57c-133">id</span><span class="sxs-lookup"><span data-stu-id="5d57c-133">id</span></span>|<span data-ttu-id="5d57c-134">Строка</span><span class="sxs-lookup"><span data-stu-id="5d57c-134">String</span></span>|<span data-ttu-id="5d57c-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5d57c-135">Key of the entity.</span></span> <span data-ttu-id="5d57c-136">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5d57c-136">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="5d57c-137">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="5d57c-137">targetedMobileApps</span></span>|<span data-ttu-id="5d57c-138">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="5d57c-138">String collection</span></span>|<span data-ttu-id="5d57c-139">приложение-обработчик</span><span class="sxs-lookup"><span data-stu-id="5d57c-139">the associated app.</span></span> <span data-ttu-id="5d57c-140">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5d57c-140">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="5d57c-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5d57c-141">roleScopeTagIds</span></span>|<span data-ttu-id="5d57c-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="5d57c-142">String collection</span></span>|<span data-ttu-id="5d57c-143">Список тегов области для этого объекта конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="5d57c-143">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="5d57c-144">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5d57c-144">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="5d57c-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5d57c-145">createdDateTime</span></span>|<span data-ttu-id="5d57c-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5d57c-146">DateTimeOffset</span></span>|<span data-ttu-id="5d57c-147">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="5d57c-147">DateTime the object was created.</span></span> <span data-ttu-id="5d57c-148">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5d57c-148">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="5d57c-149">description</span><span class="sxs-lookup"><span data-stu-id="5d57c-149">description</span></span>|<span data-ttu-id="5d57c-150">Строка</span><span class="sxs-lookup"><span data-stu-id="5d57c-150">String</span></span>|<span data-ttu-id="5d57c-151">Администратор предоставил описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5d57c-151">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5d57c-152">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5d57c-152">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="5d57c-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5d57c-153">lastModifiedDateTime</span></span>|<span data-ttu-id="5d57c-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5d57c-154">DateTimeOffset</span></span>|<span data-ttu-id="5d57c-155">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="5d57c-155">DateTime the object was last modified.</span></span> <span data-ttu-id="5d57c-156">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5d57c-156">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="5d57c-157">displayName</span><span class="sxs-lookup"><span data-stu-id="5d57c-157">displayName</span></span>|<span data-ttu-id="5d57c-158">Строка</span><span class="sxs-lookup"><span data-stu-id="5d57c-158">String</span></span>|<span data-ttu-id="5d57c-159">Администратор предоставил название конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5d57c-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5d57c-160">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5d57c-160">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="5d57c-161">версия</span><span class="sxs-lookup"><span data-stu-id="5d57c-161">version</span></span>|<span data-ttu-id="5d57c-162">Int32</span><span class="sxs-lookup"><span data-stu-id="5d57c-162">Int32</span></span>|<span data-ttu-id="5d57c-163">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5d57c-163">Version of the device configuration.</span></span> <span data-ttu-id="5d57c-164">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5d57c-164">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="5d57c-165">packageId</span><span class="sxs-lookup"><span data-stu-id="5d57c-165">packageId</span></span>|<span data-ttu-id="5d57c-166">String</span><span class="sxs-lookup"><span data-stu-id="5d57c-166">String</span></span>|<span data-ttu-id="5d57c-167">ID пакета конфигурации приложения Для Android for Work.</span><span class="sxs-lookup"><span data-stu-id="5d57c-167">Android For Work app configuration package id.</span></span>|
|<span data-ttu-id="5d57c-168">payloadJson</span><span class="sxs-lookup"><span data-stu-id="5d57c-168">payloadJson</span></span>|<span data-ttu-id="5d57c-169">Строка</span><span class="sxs-lookup"><span data-stu-id="5d57c-169">String</span></span>|<span data-ttu-id="5d57c-170">Конфигурация приложения Для Android для работы JSON полезной нагрузки.</span><span class="sxs-lookup"><span data-stu-id="5d57c-170">Android For Work app configuration JSON payload.</span></span>|
|<span data-ttu-id="5d57c-171">permissionActions</span><span class="sxs-lookup"><span data-stu-id="5d57c-171">permissionActions</span></span>|<span data-ttu-id="5d57c-172">[коллекция androidPermissionAction](../resources/intune-apps-androidpermissionaction.md)</span><span class="sxs-lookup"><span data-stu-id="5d57c-172">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) collection</span></span>|<span data-ttu-id="5d57c-173">Список разрешений на приложения Для Android и соответствующих действий разрешений.</span><span class="sxs-lookup"><span data-stu-id="5d57c-173">List of Android app permissions and corresponding permission actions.</span></span>|
|<span data-ttu-id="5d57c-174">profileApplicability</span><span class="sxs-lookup"><span data-stu-id="5d57c-174">profileApplicability</span></span>|[<span data-ttu-id="5d57c-175">androidProfileApplicability</span><span class="sxs-lookup"><span data-stu-id="5d57c-175">androidProfileApplicability</span></span>](../resources/intune-apps-androidprofileapplicability.md)|<span data-ttu-id="5d57c-176">Применимость профилей Android Enterprise (AndroidWorkProfile, DeviceOwner или по умолчанию (применяется к обоим)).</span><span class="sxs-lookup"><span data-stu-id="5d57c-176">Android Enterprise profile applicability (AndroidWorkProfile, DeviceOwner, or default (applies to both)).</span></span> <span data-ttu-id="5d57c-177">Возможные значения: `default`, `androidWorkProfile`, `androidDeviceOwner`.</span><span class="sxs-lookup"><span data-stu-id="5d57c-177">Possible values are: `default`, `androidWorkProfile`, `androidDeviceOwner`.</span></span>|



## <a name="response"></a><span data-ttu-id="5d57c-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="5d57c-178">Response</span></span>
<span data-ttu-id="5d57c-179">В случае успеха этот метод возвращает код отклика и обновленный `200 OK` [объект AndroidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="5d57c-179">If successful, this method returns a `200 OK` response code and an updated [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d57c-180">Пример</span><span class="sxs-lookup"><span data-stu-id="5d57c-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="5d57c-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="5d57c-181">Request</span></span>
<span data-ttu-id="5d57c-182">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5d57c-182">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
Content-type: application/json
Content-length: 609

{
  "@odata.type": "#microsoft.graph.androidForWorkMobileAppConfiguration",
  "targetedMobileApps": [
    "Targeted Mobile Apps value"
  ],
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "packageId": "Package Id value",
  "payloadJson": "Payload Json value",
  "permissionActions": [
    {
      "@odata.type": "microsoft.graph.androidPermissionAction",
      "permission": "Permission value",
      "action": "autoGrant"
    }
  ],
  "profileApplicability": "androidWorkProfile"
}
```

### <a name="response"></a><span data-ttu-id="5d57c-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="5d57c-183">Response</span></span>
<span data-ttu-id="5d57c-p111">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5d57c-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 781

{
  "@odata.type": "#microsoft.graph.androidForWorkMobileAppConfiguration",
  "id": "6204ae6d-ae6d-6204-6dae-04626dae0462",
  "targetedMobileApps": [
    "Targeted Mobile Apps value"
  ],
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "packageId": "Package Id value",
  "payloadJson": "Payload Json value",
  "permissionActions": [
    {
      "@odata.type": "microsoft.graph.androidPermissionAction",
      "permission": "Permission value",
      "action": "autoGrant"
    }
  ],
  "profileApplicability": "androidWorkProfile"
}
```




