---
title: Обновление Андроидманажедстореаппконфигуратион
description: Обновление свойств объекта Андроидманажедстореаппконфигуратион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a6ab887cfa014d49bfb1359c5901e225d8a1a3ba
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30170492"
---
# <a name="update-androidmanagedstoreappconfiguration"></a><span data-ttu-id="5c978-103">Обновление Андроидманажедстореаппконфигуратион</span><span class="sxs-lookup"><span data-stu-id="5c978-103">Update androidManagedStoreAppConfiguration</span></span>

> <span data-ttu-id="5c978-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c978-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5c978-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5c978-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c978-106">Обновление свойств объекта [андроидманажедстореаппконфигуратион](../resources/intune-apps-androidmanagedstoreappconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="5c978-106">Update the properties of a [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5c978-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5c978-107">Prerequisites</span></span>
<span data-ttu-id="5c978-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="5c978-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5c978-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5c978-110">Permission type</span></span>|<span data-ttu-id="5c978-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5c978-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c978-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5c978-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5c978-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c978-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5c978-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5c978-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c978-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c978-115">Not supported.</span></span>|
|<span data-ttu-id="5c978-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5c978-116">Application</span></span>|<span data-ttu-id="5c978-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c978-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c978-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5c978-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="5c978-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5c978-119">Request headers</span></span>
|<span data-ttu-id="5c978-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5c978-120">Header</span></span>|<span data-ttu-id="5c978-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5c978-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c978-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5c978-122">Authorization</span></span>|<span data-ttu-id="5c978-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="5c978-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5c978-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5c978-124">Accept</span></span>|<span data-ttu-id="5c978-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5c978-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c978-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5c978-126">Request body</span></span>
<span data-ttu-id="5c978-127">В тексте запроса добавьте представление объекта [Андроидманажедстореаппконфигуратион](../resources/intune-apps-androidmanagedstoreappconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5c978-127">In the request body, supply a JSON representation for the [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object.</span></span>

<span data-ttu-id="5c978-128">В следующей таблице приведены свойства, необходимые при создании [андроидманажедстореаппконфигуратион](../resources/intune-apps-androidmanagedstoreappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5c978-128">The following table shows the properties that are required when you create the [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md).</span></span>

|<span data-ttu-id="5c978-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="5c978-129">Property</span></span>|<span data-ttu-id="5c978-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5c978-130">Type</span></span>|<span data-ttu-id="5c978-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5c978-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c978-132">id</span><span class="sxs-lookup"><span data-stu-id="5c978-132">id</span></span>|<span data-ttu-id="5c978-133">String</span><span class="sxs-lookup"><span data-stu-id="5c978-133">String</span></span>|<span data-ttu-id="5c978-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5c978-134">Key of the entity.</span></span> <span data-ttu-id="5c978-135">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="5c978-135">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="5c978-136">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="5c978-136">targetedMobileApps</span></span>|<span data-ttu-id="5c978-137">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="5c978-137">String collection</span></span>|<span data-ttu-id="5c978-138">приложение-обработчик</span><span class="sxs-lookup"><span data-stu-id="5c978-138">the associated app.</span></span> <span data-ttu-id="5c978-139">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="5c978-139">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="5c978-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5c978-140">roleScopeTagIds</span></span>|<span data-ttu-id="5c978-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="5c978-141">String collection</span></span>|<span data-ttu-id="5c978-142">Список тегов областей для этой сущности конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="5c978-142">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="5c978-143">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="5c978-143">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="5c978-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5c978-144">createdDateTime</span></span>|<span data-ttu-id="5c978-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c978-145">DateTimeOffset</span></span>|<span data-ttu-id="5c978-146">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="5c978-146">DateTime the object was created.</span></span> <span data-ttu-id="5c978-147">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="5c978-147">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="5c978-148">описание</span><span class="sxs-lookup"><span data-stu-id="5c978-148">description</span></span>|<span data-ttu-id="5c978-149">String</span><span class="sxs-lookup"><span data-stu-id="5c978-149">String</span></span>|<span data-ttu-id="5c978-150">Администратор предоставил описание конфигурация устройства.</span><span class="sxs-lookup"><span data-stu-id="5c978-150">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5c978-151">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="5c978-151">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="5c978-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5c978-152">lastModifiedDateTime</span></span>|<span data-ttu-id="5c978-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c978-153">DateTimeOffset</span></span>|<span data-ttu-id="5c978-154">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="5c978-154">DateTime the object was last modified.</span></span> <span data-ttu-id="5c978-155">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="5c978-155">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="5c978-156">displayName</span><span class="sxs-lookup"><span data-stu-id="5c978-156">displayName</span></span>|<span data-ttu-id="5c978-157">String</span><span class="sxs-lookup"><span data-stu-id="5c978-157">String</span></span>|<span data-ttu-id="5c978-158">Администратор предоставил название конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5c978-158">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5c978-159">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="5c978-159">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="5c978-160">версия</span><span class="sxs-lookup"><span data-stu-id="5c978-160">version</span></span>|<span data-ttu-id="5c978-161">Int32</span><span class="sxs-lookup"><span data-stu-id="5c978-161">Int32</span></span>|<span data-ttu-id="5c978-162">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5c978-162">Version of the device configuration.</span></span> <span data-ttu-id="5c978-163">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="5c978-163">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="5c978-164">packageId</span><span class="sxs-lookup"><span data-stu-id="5c978-164">packageId</span></span>|<span data-ttu-id="5c978-165">String</span><span class="sxs-lookup"><span data-stu-id="5c978-165">String</span></span>|<span data-ttu-id="5c978-166">Идентификатор пакета конфигурации корпоративных приложений Android.</span><span class="sxs-lookup"><span data-stu-id="5c978-166">Android Enterprise app configuration package id.</span></span>|
|<span data-ttu-id="5c978-167">Пайлоаджсон</span><span class="sxs-lookup"><span data-stu-id="5c978-167">payloadJson</span></span>|<span data-ttu-id="5c978-168">String</span><span class="sxs-lookup"><span data-stu-id="5c978-168">String</span></span>|<span data-ttu-id="5c978-169">Полезные данные JSON конфигурации корпоративных приложений Android.</span><span class="sxs-lookup"><span data-stu-id="5c978-169">Android Enterprise app configuration JSON payload.</span></span>|
|<span data-ttu-id="5c978-170">Пермиссионактионс</span><span class="sxs-lookup"><span data-stu-id="5c978-170">permissionActions</span></span>|<span data-ttu-id="5c978-171">Коллекция [андроидпермиссионактион](../resources/intune-apps-androidpermissionaction.md)</span><span class="sxs-lookup"><span data-stu-id="5c978-171">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) collection</span></span>|<span data-ttu-id="5c978-172">Список разрешений приложений для Android и соответствующие действия с разрешениями.</span><span class="sxs-lookup"><span data-stu-id="5c978-172">List of Android app permissions and corresponding permission actions.</span></span>|



## <a name="response"></a><span data-ttu-id="5c978-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c978-173">Response</span></span>
<span data-ttu-id="5c978-174">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроидманажедстореаппконфигуратион](../resources/intune-apps-androidmanagedstoreappconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5c978-174">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c978-175">Пример</span><span class="sxs-lookup"><span data-stu-id="5c978-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="5c978-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="5c978-176">Request</span></span>
<span data-ttu-id="5c978-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5c978-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5c978-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c978-178">Response</span></span>
<span data-ttu-id="5c978-p110">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5c978-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




