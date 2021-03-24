---
title: Создание androidManagedStoreAppConfiguration
description: Создайте новый объект AndroidManagedStoreAppConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ac28b6d1e02edb9e1513bda9ccc616126eb13cca
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51140975"
---
# <a name="create-androidmanagedstoreappconfiguration"></a><span data-ttu-id="54859-103">Создание androidManagedStoreAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="54859-103">Create androidManagedStoreAppConfiguration</span></span>

<span data-ttu-id="54859-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54859-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="54859-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54859-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="54859-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="54859-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54859-107">Создайте новый [объект AndroidManagedStoreAppConfiguration.](../resources/intune-apps-androidmanagedstoreappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54859-107">Create a new [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="54859-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="54859-108">Prerequisites</span></span>
<span data-ttu-id="54859-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54859-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54859-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="54859-111">Permission type</span></span>|<span data-ttu-id="54859-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="54859-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="54859-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="54859-113">Delegated (work or school account)</span></span>|<span data-ttu-id="54859-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54859-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="54859-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="54859-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="54859-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54859-116">Not supported.</span></span>|
|<span data-ttu-id="54859-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="54859-117">Application</span></span>|<span data-ttu-id="54859-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54859-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="54859-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="54859-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="54859-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="54859-120">Request headers</span></span>
|<span data-ttu-id="54859-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="54859-121">Header</span></span>|<span data-ttu-id="54859-122">Значение</span><span class="sxs-lookup"><span data-stu-id="54859-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="54859-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="54859-123">Authorization</span></span>|<span data-ttu-id="54859-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="54859-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="54859-125">Accept</span><span class="sxs-lookup"><span data-stu-id="54859-125">Accept</span></span>|<span data-ttu-id="54859-126">application/json</span><span class="sxs-lookup"><span data-stu-id="54859-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="54859-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="54859-127">Request body</span></span>
<span data-ttu-id="54859-128">В теле запроса предоставляем представление JSON для объекта AndroidManagedStoreAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="54859-128">In the request body, supply a JSON representation for the androidManagedStoreAppConfiguration object.</span></span>

<span data-ttu-id="54859-129">В следующей таблице показаны свойства, необходимые при создании androidManagedStoreAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="54859-129">The following table shows the properties that are required when you create the androidManagedStoreAppConfiguration.</span></span>

|<span data-ttu-id="54859-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="54859-130">Property</span></span>|<span data-ttu-id="54859-131">Тип</span><span class="sxs-lookup"><span data-stu-id="54859-131">Type</span></span>|<span data-ttu-id="54859-132">Описание</span><span class="sxs-lookup"><span data-stu-id="54859-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54859-133">id</span><span class="sxs-lookup"><span data-stu-id="54859-133">id</span></span>|<span data-ttu-id="54859-134">Строка</span><span class="sxs-lookup"><span data-stu-id="54859-134">String</span></span>|<span data-ttu-id="54859-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="54859-135">Key of the entity.</span></span> <span data-ttu-id="54859-136">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54859-136">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="54859-137">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="54859-137">targetedMobileApps</span></span>|<span data-ttu-id="54859-138">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="54859-138">String collection</span></span>|<span data-ttu-id="54859-139">приложение-обработчик</span><span class="sxs-lookup"><span data-stu-id="54859-139">the associated app.</span></span> <span data-ttu-id="54859-140">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54859-140">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="54859-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="54859-141">roleScopeTagIds</span></span>|<span data-ttu-id="54859-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="54859-142">String collection</span></span>|<span data-ttu-id="54859-143">Список тегов области для этого объекта конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="54859-143">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="54859-144">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54859-144">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="54859-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="54859-145">createdDateTime</span></span>|<span data-ttu-id="54859-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54859-146">DateTimeOffset</span></span>|<span data-ttu-id="54859-147">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="54859-147">DateTime the object was created.</span></span> <span data-ttu-id="54859-148">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54859-148">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="54859-149">description</span><span class="sxs-lookup"><span data-stu-id="54859-149">description</span></span>|<span data-ttu-id="54859-150">Строка</span><span class="sxs-lookup"><span data-stu-id="54859-150">String</span></span>|<span data-ttu-id="54859-151">Администратор предоставил описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="54859-151">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="54859-152">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54859-152">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="54859-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="54859-153">lastModifiedDateTime</span></span>|<span data-ttu-id="54859-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54859-154">DateTimeOffset</span></span>|<span data-ttu-id="54859-155">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="54859-155">DateTime the object was last modified.</span></span> <span data-ttu-id="54859-156">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54859-156">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="54859-157">displayName</span><span class="sxs-lookup"><span data-stu-id="54859-157">displayName</span></span>|<span data-ttu-id="54859-158">Строка</span><span class="sxs-lookup"><span data-stu-id="54859-158">String</span></span>|<span data-ttu-id="54859-159">Администратор предоставил название конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="54859-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="54859-160">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54859-160">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="54859-161">версия</span><span class="sxs-lookup"><span data-stu-id="54859-161">version</span></span>|<span data-ttu-id="54859-162">Int32</span><span class="sxs-lookup"><span data-stu-id="54859-162">Int32</span></span>|<span data-ttu-id="54859-163">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="54859-163">Version of the device configuration.</span></span> <span data-ttu-id="54859-164">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54859-164">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="54859-165">packageId</span><span class="sxs-lookup"><span data-stu-id="54859-165">packageId</span></span>|<span data-ttu-id="54859-166">String</span><span class="sxs-lookup"><span data-stu-id="54859-166">String</span></span>|<span data-ttu-id="54859-167">ID пакета конфигурации приложений для Android Enterprise.</span><span class="sxs-lookup"><span data-stu-id="54859-167">Android Enterprise app configuration package id.</span></span>|
|<span data-ttu-id="54859-168">payloadJson</span><span class="sxs-lookup"><span data-stu-id="54859-168">payloadJson</span></span>|<span data-ttu-id="54859-169">Строка</span><span class="sxs-lookup"><span data-stu-id="54859-169">String</span></span>|<span data-ttu-id="54859-170">Конфигурация приложения для Android Enterprise JSON полезной нагрузки.</span><span class="sxs-lookup"><span data-stu-id="54859-170">Android Enterprise app configuration JSON payload.</span></span>|
|<span data-ttu-id="54859-171">permissionActions</span><span class="sxs-lookup"><span data-stu-id="54859-171">permissionActions</span></span>|<span data-ttu-id="54859-172">[коллекция androidPermissionAction](../resources/intune-apps-androidpermissionaction.md)</span><span class="sxs-lookup"><span data-stu-id="54859-172">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) collection</span></span>|<span data-ttu-id="54859-173">Список разрешений на приложения Для Android и соответствующих действий разрешений.</span><span class="sxs-lookup"><span data-stu-id="54859-173">List of Android app permissions and corresponding permission actions.</span></span>|
|<span data-ttu-id="54859-174">appSupportsOemConfig</span><span class="sxs-lookup"><span data-stu-id="54859-174">appSupportsOemConfig</span></span>|<span data-ttu-id="54859-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="54859-175">Boolean</span></span>|<span data-ttu-id="54859-176">Является ли этот AppConfig политикой OEMConfig.</span><span class="sxs-lookup"><span data-stu-id="54859-176">Whether or not this AppConfig is an OEMConfig policy.</span></span>|
|<span data-ttu-id="54859-177">profileApplicability</span><span class="sxs-lookup"><span data-stu-id="54859-177">profileApplicability</span></span>|[<span data-ttu-id="54859-178">androidProfileApplicability</span><span class="sxs-lookup"><span data-stu-id="54859-178">androidProfileApplicability</span></span>](../resources/intune-apps-androidprofileapplicability.md)|<span data-ttu-id="54859-179">Применимость профилей Android Enterprise (AndroidWorkProfile, DeviceOwner или по умолчанию (применяется к обоим)).</span><span class="sxs-lookup"><span data-stu-id="54859-179">Android Enterprise profile applicability (AndroidWorkProfile, DeviceOwner, or default (applies to both)).</span></span> <span data-ttu-id="54859-180">Возможные значения: `default`, `androidWorkProfile`, `androidDeviceOwner`.</span><span class="sxs-lookup"><span data-stu-id="54859-180">Possible values are: `default`, `androidWorkProfile`, `androidDeviceOwner`.</span></span>|



## <a name="response"></a><span data-ttu-id="54859-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="54859-181">Response</span></span>
<span data-ttu-id="54859-182">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект AndroidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="54859-182">If successful, this method returns a `201 Created` response code and a [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54859-183">Пример</span><span class="sxs-lookup"><span data-stu-id="54859-183">Example</span></span>

### <a name="request"></a><span data-ttu-id="54859-184">Запрос</span><span class="sxs-lookup"><span data-stu-id="54859-184">Request</span></span>
<span data-ttu-id="54859-185">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="54859-185">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations
Content-type: application/json
Content-length: 641

{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppConfiguration",
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
  "appSupportsOemConfig": true,
  "profileApplicability": "androidWorkProfile"
}
```

### <a name="response"></a><span data-ttu-id="54859-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="54859-186">Response</span></span>
<span data-ttu-id="54859-p111">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="54859-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 813

{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppConfiguration",
  "id": "919a9335-9335-919a-3593-9a9135939a91",
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
  "appSupportsOemConfig": true,
  "profileApplicability": "androidWorkProfile"
}
```




