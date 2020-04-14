---
title: Обновление Андроидманажедстореаппконфигуратион
description: Обновление свойств объекта Андроидманажедстореаппконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8dbcb5e73fbb672a80aef01e28978c8411f63831
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43417423"
---
# <a name="update-androidmanagedstoreappconfiguration"></a><span data-ttu-id="18244-103">Обновление Андроидманажедстореаппконфигуратион</span><span class="sxs-lookup"><span data-stu-id="18244-103">Update androidManagedStoreAppConfiguration</span></span>

<span data-ttu-id="18244-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18244-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="18244-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18244-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="18244-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="18244-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18244-107">Обновление свойств объекта [андроидманажедстореаппконфигуратион](../resources/intune-apps-androidmanagedstoreappconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="18244-107">Update the properties of a [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="18244-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="18244-108">Prerequisites</span></span>
<span data-ttu-id="18244-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18244-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18244-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="18244-111">Permission type</span></span>|<span data-ttu-id="18244-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="18244-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18244-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="18244-113">Delegated (work or school account)</span></span>|<span data-ttu-id="18244-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18244-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="18244-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="18244-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18244-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18244-116">Not supported.</span></span>|
|<span data-ttu-id="18244-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="18244-117">Application</span></span>|<span data-ttu-id="18244-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18244-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="18244-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="18244-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="18244-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="18244-120">Request headers</span></span>
|<span data-ttu-id="18244-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="18244-121">Header</span></span>|<span data-ttu-id="18244-122">Значение</span><span class="sxs-lookup"><span data-stu-id="18244-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18244-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="18244-123">Authorization</span></span>|<span data-ttu-id="18244-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="18244-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18244-125">Accept</span><span class="sxs-lookup"><span data-stu-id="18244-125">Accept</span></span>|<span data-ttu-id="18244-126">application/json</span><span class="sxs-lookup"><span data-stu-id="18244-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18244-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="18244-127">Request body</span></span>
<span data-ttu-id="18244-128">В тексте запроса добавьте представление объекта [андроидманажедстореаппконфигуратион](../resources/intune-apps-androidmanagedstoreappconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="18244-128">In the request body, supply a JSON representation for the [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object.</span></span>

<span data-ttu-id="18244-129">В следующей таблице приведены свойства, необходимые при создании [андроидманажедстореаппконфигуратион](../resources/intune-apps-androidmanagedstoreappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="18244-129">The following table shows the properties that are required when you create the [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md).</span></span>

|<span data-ttu-id="18244-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="18244-130">Property</span></span>|<span data-ttu-id="18244-131">Тип</span><span class="sxs-lookup"><span data-stu-id="18244-131">Type</span></span>|<span data-ttu-id="18244-132">Описание</span><span class="sxs-lookup"><span data-stu-id="18244-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18244-133">id</span><span class="sxs-lookup"><span data-stu-id="18244-133">id</span></span>|<span data-ttu-id="18244-134">Строка</span><span class="sxs-lookup"><span data-stu-id="18244-134">String</span></span>|<span data-ttu-id="18244-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="18244-135">Key of the entity.</span></span> <span data-ttu-id="18244-136">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18244-136">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="18244-137">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="18244-137">targetedMobileApps</span></span>|<span data-ttu-id="18244-138">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="18244-138">String collection</span></span>|<span data-ttu-id="18244-139">приложение-обработчик</span><span class="sxs-lookup"><span data-stu-id="18244-139">the associated app.</span></span> <span data-ttu-id="18244-140">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18244-140">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="18244-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="18244-141">roleScopeTagIds</span></span>|<span data-ttu-id="18244-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="18244-142">String collection</span></span>|<span data-ttu-id="18244-143">Список тегов областей для этой сущности конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="18244-143">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="18244-144">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18244-144">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="18244-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="18244-145">createdDateTime</span></span>|<span data-ttu-id="18244-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18244-146">DateTimeOffset</span></span>|<span data-ttu-id="18244-147">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="18244-147">DateTime the object was created.</span></span> <span data-ttu-id="18244-148">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18244-148">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="18244-149">description</span><span class="sxs-lookup"><span data-stu-id="18244-149">description</span></span>|<span data-ttu-id="18244-150">String</span><span class="sxs-lookup"><span data-stu-id="18244-150">String</span></span>|<span data-ttu-id="18244-151">Администратор предоставил описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="18244-151">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="18244-152">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18244-152">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="18244-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="18244-153">lastModifiedDateTime</span></span>|<span data-ttu-id="18244-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18244-154">DateTimeOffset</span></span>|<span data-ttu-id="18244-155">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="18244-155">DateTime the object was last modified.</span></span> <span data-ttu-id="18244-156">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18244-156">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="18244-157">displayName</span><span class="sxs-lookup"><span data-stu-id="18244-157">displayName</span></span>|<span data-ttu-id="18244-158">Строка</span><span class="sxs-lookup"><span data-stu-id="18244-158">String</span></span>|<span data-ttu-id="18244-159">Администратор предоставил название конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="18244-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="18244-160">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18244-160">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="18244-161">версия</span><span class="sxs-lookup"><span data-stu-id="18244-161">version</span></span>|<span data-ttu-id="18244-162">Int32</span><span class="sxs-lookup"><span data-stu-id="18244-162">Int32</span></span>|<span data-ttu-id="18244-163">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="18244-163">Version of the device configuration.</span></span> <span data-ttu-id="18244-164">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18244-164">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="18244-165">packageId</span><span class="sxs-lookup"><span data-stu-id="18244-165">packageId</span></span>|<span data-ttu-id="18244-166">String</span><span class="sxs-lookup"><span data-stu-id="18244-166">String</span></span>|<span data-ttu-id="18244-167">Идентификатор пакета конфигурации корпоративных приложений Android.</span><span class="sxs-lookup"><span data-stu-id="18244-167">Android Enterprise app configuration package id.</span></span>|
|<span data-ttu-id="18244-168">пайлоаджсон</span><span class="sxs-lookup"><span data-stu-id="18244-168">payloadJson</span></span>|<span data-ttu-id="18244-169">String</span><span class="sxs-lookup"><span data-stu-id="18244-169">String</span></span>|<span data-ttu-id="18244-170">Полезные данные JSON конфигурации корпоративных приложений Android.</span><span class="sxs-lookup"><span data-stu-id="18244-170">Android Enterprise app configuration JSON payload.</span></span>|
|<span data-ttu-id="18244-171">пермиссионактионс</span><span class="sxs-lookup"><span data-stu-id="18244-171">permissionActions</span></span>|<span data-ttu-id="18244-172">Коллекция [андроидпермиссионактион](../resources/intune-apps-androidpermissionaction.md)</span><span class="sxs-lookup"><span data-stu-id="18244-172">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) collection</span></span>|<span data-ttu-id="18244-173">Список разрешений приложений для Android и соответствующие действия с разрешениями.</span><span class="sxs-lookup"><span data-stu-id="18244-173">List of Android app permissions and corresponding permission actions.</span></span>|
|<span data-ttu-id="18244-174">аппсуппортсоемконфиг</span><span class="sxs-lookup"><span data-stu-id="18244-174">appSupportsOemConfig</span></span>|<span data-ttu-id="18244-175">Логическое</span><span class="sxs-lookup"><span data-stu-id="18244-175">Boolean</span></span>|<span data-ttu-id="18244-176">Указывает, является ли Аппконфиг политикой Оемконфиг.</span><span class="sxs-lookup"><span data-stu-id="18244-176">Whether or not this AppConfig is an OEMConfig policy.</span></span>|
|<span data-ttu-id="18244-177">профилеаппликабилити</span><span class="sxs-lookup"><span data-stu-id="18244-177">profileApplicability</span></span>|[<span data-ttu-id="18244-178">андроидпрофилеаппликабилити</span><span class="sxs-lookup"><span data-stu-id="18244-178">androidProfileApplicability</span></span>](../resources/intune-apps-androidprofileapplicability.md)|<span data-ttu-id="18244-179">Применимость профиля предприятия Android (Андроидворкпрофиле, Девицеовнер или Default (применяется к обоим).</span><span class="sxs-lookup"><span data-stu-id="18244-179">Android Enterprise profile applicability (AndroidWorkProfile, DeviceOwner, or default (applies to both)).</span></span> <span data-ttu-id="18244-180">Возможные значения: `default`, `androidWorkProfile`, `androidDeviceOwner`.</span><span class="sxs-lookup"><span data-stu-id="18244-180">Possible values are: `default`, `androidWorkProfile`, `androidDeviceOwner`.</span></span>|



## <a name="response"></a><span data-ttu-id="18244-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="18244-181">Response</span></span>
<span data-ttu-id="18244-182">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроидманажедстореаппконфигуратион](../resources/intune-apps-androidmanagedstoreappconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="18244-182">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18244-183">Пример</span><span class="sxs-lookup"><span data-stu-id="18244-183">Example</span></span>

### <a name="request"></a><span data-ttu-id="18244-184">Запрос</span><span class="sxs-lookup"><span data-stu-id="18244-184">Request</span></span>
<span data-ttu-id="18244-185">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="18244-185">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
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

### <a name="response"></a><span data-ttu-id="18244-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="18244-186">Response</span></span>
<span data-ttu-id="18244-p111">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="18244-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



