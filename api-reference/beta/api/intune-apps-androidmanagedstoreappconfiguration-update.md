---
title: Обновление androidManagedStoreAppConfiguration
description: Обновление свойства объекта androidManagedStoreAppConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cf9a996b67a25bacce7ccb5f18efa05addde078f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406999"
---
# <a name="update-androidmanagedstoreappconfiguration"></a><span data-ttu-id="c11e1-103">Обновление androidManagedStoreAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="c11e1-103">Update androidManagedStoreAppConfiguration</span></span>

> <span data-ttu-id="c11e1-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c11e1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c11e1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c11e1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c11e1-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c11e1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c11e1-107">Обновление свойства объекта [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="c11e1-107">Update the properties of a [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c11e1-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="c11e1-108">Prerequisites</span></span>
<span data-ttu-id="c11e1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c11e1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c11e1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c11e1-111">Permission type</span></span>|<span data-ttu-id="c11e1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c11e1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c11e1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c11e1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c11e1-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c11e1-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c11e1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c11e1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c11e1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c11e1-116">Not supported.</span></span>|
|<span data-ttu-id="c11e1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c11e1-117">Application</span></span>|<span data-ttu-id="c11e1-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c11e1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c11e1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c11e1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c11e1-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c11e1-120">Request headers</span></span>
|<span data-ttu-id="c11e1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c11e1-121">Header</span></span>|<span data-ttu-id="c11e1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c11e1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c11e1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c11e1-123">Authorization</span></span>|<span data-ttu-id="c11e1-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c11e1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c11e1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c11e1-125">Accept</span></span>|<span data-ttu-id="c11e1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c11e1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c11e1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c11e1-127">Request body</span></span>
<span data-ttu-id="c11e1-128">В тексте запроса укажите представление JSON для объекта [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="c11e1-128">In the request body, supply a JSON representation for the [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object.</span></span>

<span data-ttu-id="c11e1-129">В следующей таблице показаны свойства, которые необходимы для создания [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c11e1-129">The following table shows the properties that are required when you create the [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md).</span></span>

|<span data-ttu-id="c11e1-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c11e1-130">Property</span></span>|<span data-ttu-id="c11e1-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c11e1-131">Type</span></span>|<span data-ttu-id="c11e1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c11e1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c11e1-133">id</span><span class="sxs-lookup"><span data-stu-id="c11e1-133">id</span></span>|<span data-ttu-id="c11e1-134">String</span><span class="sxs-lookup"><span data-stu-id="c11e1-134">String</span></span>|<span data-ttu-id="c11e1-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c11e1-135">Key of the entity.</span></span> <span data-ttu-id="c11e1-136">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="c11e1-136">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="c11e1-137">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="c11e1-137">targetedMobileApps</span></span>|<span data-ttu-id="c11e1-138">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c11e1-138">String collection</span></span>|<span data-ttu-id="c11e1-139">приложение-обработчик</span><span class="sxs-lookup"><span data-stu-id="c11e1-139">the associated app.</span></span> <span data-ttu-id="c11e1-140">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="c11e1-140">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="c11e1-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c11e1-141">roleScopeTagIds</span></span>|<span data-ttu-id="c11e1-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c11e1-142">String collection</span></span>|<span data-ttu-id="c11e1-143">Список областей теги для данного объекта конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="c11e1-143">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="c11e1-144">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="c11e1-144">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="c11e1-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c11e1-145">createdDateTime</span></span>|<span data-ttu-id="c11e1-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c11e1-146">DateTimeOffset</span></span>|<span data-ttu-id="c11e1-147">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c11e1-147">DateTime the object was created.</span></span> <span data-ttu-id="c11e1-148">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="c11e1-148">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="c11e1-149">описание</span><span class="sxs-lookup"><span data-stu-id="c11e1-149">description</span></span>|<span data-ttu-id="c11e1-150">String</span><span class="sxs-lookup"><span data-stu-id="c11e1-150">String</span></span>|<span data-ttu-id="c11e1-151">Администратор предоставил описание конфигурация устройства.</span><span class="sxs-lookup"><span data-stu-id="c11e1-151">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c11e1-152">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="c11e1-152">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="c11e1-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c11e1-153">lastModifiedDateTime</span></span>|<span data-ttu-id="c11e1-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c11e1-154">DateTimeOffset</span></span>|<span data-ttu-id="c11e1-155">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c11e1-155">DateTime the object was last modified.</span></span> <span data-ttu-id="c11e1-156">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="c11e1-156">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="c11e1-157">displayName</span><span class="sxs-lookup"><span data-stu-id="c11e1-157">displayName</span></span>|<span data-ttu-id="c11e1-158">String</span><span class="sxs-lookup"><span data-stu-id="c11e1-158">String</span></span>|<span data-ttu-id="c11e1-159">Администратор предоставил название конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c11e1-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c11e1-160">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="c11e1-160">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="c11e1-161">версия</span><span class="sxs-lookup"><span data-stu-id="c11e1-161">version</span></span>|<span data-ttu-id="c11e1-162">Int32</span><span class="sxs-lookup"><span data-stu-id="c11e1-162">Int32</span></span>|<span data-ttu-id="c11e1-163">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c11e1-163">Version of the device configuration.</span></span> <span data-ttu-id="c11e1-164">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="c11e1-164">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="c11e1-165">packageId</span><span class="sxs-lookup"><span data-stu-id="c11e1-165">packageId</span></span>|<span data-ttu-id="c11e1-166">String</span><span class="sxs-lookup"><span data-stu-id="c11e1-166">String</span></span>|<span data-ttu-id="c11e1-167">Идентификатор приложения пакета конфигурации Android предприятия.</span><span class="sxs-lookup"><span data-stu-id="c11e1-167">Android Enterprise app configuration package id.</span></span>|
|<span data-ttu-id="c11e1-168">payloadJson</span><span class="sxs-lookup"><span data-stu-id="c11e1-168">payloadJson</span></span>|<span data-ttu-id="c11e1-169">String</span><span class="sxs-lookup"><span data-stu-id="c11e1-169">String</span></span>|<span data-ttu-id="c11e1-170">Android корпоративного приложения конфигурации JSON полезных данных.</span><span class="sxs-lookup"><span data-stu-id="c11e1-170">Android Enterprise app configuration JSON payload.</span></span>|
|<span data-ttu-id="c11e1-171">permissionActions</span><span class="sxs-lookup"><span data-stu-id="c11e1-171">permissionActions</span></span>|<span data-ttu-id="c11e1-172">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="c11e1-172">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) collection</span></span>|<span data-ttu-id="c11e1-173">Список разрешений для Android и соответствующие действия разрешений.</span><span class="sxs-lookup"><span data-stu-id="c11e1-173">List of Android app permissions and corresponding permission actions.</span></span>|



## <a name="response"></a><span data-ttu-id="c11e1-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="c11e1-174">Response</span></span>
<span data-ttu-id="c11e1-175">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c11e1-175">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c11e1-176">Пример</span><span class="sxs-lookup"><span data-stu-id="c11e1-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="c11e1-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="c11e1-177">Request</span></span>
<span data-ttu-id="c11e1-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c11e1-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
Content-type: application/json
Content-length: 559

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
  ]
}
```

### <a name="response"></a><span data-ttu-id="c11e1-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="c11e1-179">Response</span></span>
<span data-ttu-id="c11e1-p111">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c11e1-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 731

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
  ]
}
```




