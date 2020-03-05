---
title: Обновление Андроидманажедстореаппконфигуратион
description: Обновление свойств объекта Андроидманажедстореаппконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6c8ade082cd4334710acc2347aed9b9160e7947a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42445871"
---
# <a name="update-androidmanagedstoreappconfiguration"></a><span data-ttu-id="ff4ae-103">Обновление Андроидманажедстореаппконфигуратион</span><span class="sxs-lookup"><span data-stu-id="ff4ae-103">Update androidManagedStoreAppConfiguration</span></span>

<span data-ttu-id="ff4ae-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ff4ae-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ff4ae-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff4ae-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff4ae-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ff4ae-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff4ae-107">Обновление свойств объекта [андроидманажедстореаппконфигуратион](../resources/intune-apps-androidmanagedstoreappconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="ff4ae-107">Update the properties of a [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ff4ae-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ff4ae-108">Prerequisites</span></span>
<span data-ttu-id="ff4ae-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff4ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff4ae-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ff4ae-111">Permission type</span></span>|<span data-ttu-id="ff4ae-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ff4ae-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff4ae-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ff4ae-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ff4ae-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff4ae-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ff4ae-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ff4ae-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff4ae-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff4ae-116">Not supported.</span></span>|
|<span data-ttu-id="ff4ae-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ff4ae-117">Application</span></span>|<span data-ttu-id="ff4ae-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff4ae-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff4ae-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ff4ae-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ff4ae-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ff4ae-120">Request headers</span></span>
|<span data-ttu-id="ff4ae-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ff4ae-121">Header</span></span>|<span data-ttu-id="ff4ae-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ff4ae-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff4ae-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff4ae-123">Authorization</span></span>|<span data-ttu-id="ff4ae-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ff4ae-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff4ae-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ff4ae-125">Accept</span></span>|<span data-ttu-id="ff4ae-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ff4ae-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff4ae-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ff4ae-127">Request body</span></span>
<span data-ttu-id="ff4ae-128">В тексте запроса добавьте представление объекта [андроидманажедстореаппконфигуратион](../resources/intune-apps-androidmanagedstoreappconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ff4ae-128">In the request body, supply a JSON representation for the [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object.</span></span>

<span data-ttu-id="ff4ae-129">В следующей таблице приведены свойства, необходимые при создании [андроидманажедстореаппконфигуратион](../resources/intune-apps-androidmanagedstoreappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ff4ae-129">The following table shows the properties that are required when you create the [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md).</span></span>

|<span data-ttu-id="ff4ae-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ff4ae-130">Property</span></span>|<span data-ttu-id="ff4ae-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ff4ae-131">Type</span></span>|<span data-ttu-id="ff4ae-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ff4ae-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff4ae-133">id</span><span class="sxs-lookup"><span data-stu-id="ff4ae-133">id</span></span>|<span data-ttu-id="ff4ae-134">Строка</span><span class="sxs-lookup"><span data-stu-id="ff4ae-134">String</span></span>|<span data-ttu-id="ff4ae-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ff4ae-135">Key of the entity.</span></span> <span data-ttu-id="ff4ae-136">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff4ae-136">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="ff4ae-137">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="ff4ae-137">targetedMobileApps</span></span>|<span data-ttu-id="ff4ae-138">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ff4ae-138">String collection</span></span>|<span data-ttu-id="ff4ae-139">приложение-обработчик</span><span class="sxs-lookup"><span data-stu-id="ff4ae-139">the associated app.</span></span> <span data-ttu-id="ff4ae-140">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff4ae-140">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="ff4ae-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ff4ae-141">roleScopeTagIds</span></span>|<span data-ttu-id="ff4ae-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ff4ae-142">String collection</span></span>|<span data-ttu-id="ff4ae-143">Список тегов областей для этой сущности конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="ff4ae-143">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="ff4ae-144">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff4ae-144">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="ff4ae-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ff4ae-145">createdDateTime</span></span>|<span data-ttu-id="ff4ae-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff4ae-146">DateTimeOffset</span></span>|<span data-ttu-id="ff4ae-147">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="ff4ae-147">DateTime the object was created.</span></span> <span data-ttu-id="ff4ae-148">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff4ae-148">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="ff4ae-149">description</span><span class="sxs-lookup"><span data-stu-id="ff4ae-149">description</span></span>|<span data-ttu-id="ff4ae-150">String</span><span class="sxs-lookup"><span data-stu-id="ff4ae-150">String</span></span>|<span data-ttu-id="ff4ae-151">Администратор предоставил описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ff4ae-151">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ff4ae-152">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff4ae-152">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="ff4ae-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ff4ae-153">lastModifiedDateTime</span></span>|<span data-ttu-id="ff4ae-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff4ae-154">DateTimeOffset</span></span>|<span data-ttu-id="ff4ae-155">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ff4ae-155">DateTime the object was last modified.</span></span> <span data-ttu-id="ff4ae-156">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff4ae-156">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="ff4ae-157">displayName</span><span class="sxs-lookup"><span data-stu-id="ff4ae-157">displayName</span></span>|<span data-ttu-id="ff4ae-158">Строка</span><span class="sxs-lookup"><span data-stu-id="ff4ae-158">String</span></span>|<span data-ttu-id="ff4ae-159">Администратор предоставил название конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ff4ae-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ff4ae-160">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff4ae-160">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="ff4ae-161">версия</span><span class="sxs-lookup"><span data-stu-id="ff4ae-161">version</span></span>|<span data-ttu-id="ff4ae-162">Int32</span><span class="sxs-lookup"><span data-stu-id="ff4ae-162">Int32</span></span>|<span data-ttu-id="ff4ae-163">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ff4ae-163">Version of the device configuration.</span></span> <span data-ttu-id="ff4ae-164">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff4ae-164">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="ff4ae-165">packageId</span><span class="sxs-lookup"><span data-stu-id="ff4ae-165">packageId</span></span>|<span data-ttu-id="ff4ae-166">String</span><span class="sxs-lookup"><span data-stu-id="ff4ae-166">String</span></span>|<span data-ttu-id="ff4ae-167">Идентификатор пакета конфигурации корпоративных приложений Android.</span><span class="sxs-lookup"><span data-stu-id="ff4ae-167">Android Enterprise app configuration package id.</span></span>|
|<span data-ttu-id="ff4ae-168">пайлоаджсон</span><span class="sxs-lookup"><span data-stu-id="ff4ae-168">payloadJson</span></span>|<span data-ttu-id="ff4ae-169">String</span><span class="sxs-lookup"><span data-stu-id="ff4ae-169">String</span></span>|<span data-ttu-id="ff4ae-170">Полезные данные JSON конфигурации корпоративных приложений Android.</span><span class="sxs-lookup"><span data-stu-id="ff4ae-170">Android Enterprise app configuration JSON payload.</span></span>|
|<span data-ttu-id="ff4ae-171">пермиссионактионс</span><span class="sxs-lookup"><span data-stu-id="ff4ae-171">permissionActions</span></span>|<span data-ttu-id="ff4ae-172">Коллекция [андроидпермиссионактион](../resources/intune-apps-androidpermissionaction.md)</span><span class="sxs-lookup"><span data-stu-id="ff4ae-172">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) collection</span></span>|<span data-ttu-id="ff4ae-173">Список разрешений приложений для Android и соответствующие действия с разрешениями.</span><span class="sxs-lookup"><span data-stu-id="ff4ae-173">List of Android app permissions and corresponding permission actions.</span></span>|
|<span data-ttu-id="ff4ae-174">аппсуппортсоемконфиг</span><span class="sxs-lookup"><span data-stu-id="ff4ae-174">appSupportsOemConfig</span></span>|<span data-ttu-id="ff4ae-175">Логический</span><span class="sxs-lookup"><span data-stu-id="ff4ae-175">Boolean</span></span>|<span data-ttu-id="ff4ae-176">Указывает, является ли Аппконфиг политикой Оемконфиг.</span><span class="sxs-lookup"><span data-stu-id="ff4ae-176">Whether or not this AppConfig is an OEMConfig policy.</span></span>|



## <a name="response"></a><span data-ttu-id="ff4ae-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff4ae-177">Response</span></span>
<span data-ttu-id="ff4ae-178">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроидманажедстореаппконфигуратион](../resources/intune-apps-androidmanagedstoreappconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ff4ae-178">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff4ae-179">Пример</span><span class="sxs-lookup"><span data-stu-id="ff4ae-179">Example</span></span>

### <a name="request"></a><span data-ttu-id="ff4ae-180">Запрос</span><span class="sxs-lookup"><span data-stu-id="ff4ae-180">Request</span></span>
<span data-ttu-id="ff4ae-181">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ff4ae-181">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
Content-type: application/json
Content-length: 592

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
  "appSupportsOemConfig": true
}
```

### <a name="response"></a><span data-ttu-id="ff4ae-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff4ae-182">Response</span></span>
<span data-ttu-id="ff4ae-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ff4ae-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 764

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
  "appSupportsOemConfig": true
}
```





