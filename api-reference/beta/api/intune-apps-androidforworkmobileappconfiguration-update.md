---
title: Обновление Андроидфорворкмобилеаппконфигуратион
description: Обновление свойств объекта Андроидфорворкмобилеаппконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 64b208535ac03ffcc3f8b63425efabe896def3df
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43395267"
---
# <a name="update-androidforworkmobileappconfiguration"></a><span data-ttu-id="941b5-103">Обновление Андроидфорворкмобилеаппконфигуратион</span><span class="sxs-lookup"><span data-stu-id="941b5-103">Update androidForWorkMobileAppConfiguration</span></span>

<span data-ttu-id="941b5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="941b5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="941b5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="941b5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="941b5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="941b5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="941b5-107">Обновление свойств объекта [андроидфорворкмобилеаппконфигуратион](../resources/intune-apps-androidforworkmobileappconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="941b5-107">Update the properties of a [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="941b5-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="941b5-108">Prerequisites</span></span>
<span data-ttu-id="941b5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="941b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="941b5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="941b5-111">Permission type</span></span>|<span data-ttu-id="941b5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="941b5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="941b5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="941b5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="941b5-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="941b5-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="941b5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="941b5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="941b5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="941b5-116">Not supported.</span></span>|
|<span data-ttu-id="941b5-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="941b5-117">Application</span></span>|<span data-ttu-id="941b5-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="941b5-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="941b5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="941b5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="941b5-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="941b5-120">Request headers</span></span>
|<span data-ttu-id="941b5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="941b5-121">Header</span></span>|<span data-ttu-id="941b5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="941b5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="941b5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="941b5-123">Authorization</span></span>|<span data-ttu-id="941b5-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="941b5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="941b5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="941b5-125">Accept</span></span>|<span data-ttu-id="941b5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="941b5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="941b5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="941b5-127">Request body</span></span>
<span data-ttu-id="941b5-128">В тексте запроса добавьте представление объекта [андроидфорворкмобилеаппконфигуратион](../resources/intune-apps-androidforworkmobileappconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="941b5-128">In the request body, supply a JSON representation for the [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object.</span></span>

<span data-ttu-id="941b5-129">В следующей таблице приведены свойства, необходимые при создании [андроидфорворкмобилеаппконфигуратион](../resources/intune-apps-androidforworkmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="941b5-129">The following table shows the properties that are required when you create the [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md).</span></span>

|<span data-ttu-id="941b5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="941b5-130">Property</span></span>|<span data-ttu-id="941b5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="941b5-131">Type</span></span>|<span data-ttu-id="941b5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="941b5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="941b5-133">id</span><span class="sxs-lookup"><span data-stu-id="941b5-133">id</span></span>|<span data-ttu-id="941b5-134">Строка</span><span class="sxs-lookup"><span data-stu-id="941b5-134">String</span></span>|<span data-ttu-id="941b5-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="941b5-135">Key of the entity.</span></span> <span data-ttu-id="941b5-136">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="941b5-136">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="941b5-137">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="941b5-137">targetedMobileApps</span></span>|<span data-ttu-id="941b5-138">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="941b5-138">String collection</span></span>|<span data-ttu-id="941b5-139">приложение-обработчик</span><span class="sxs-lookup"><span data-stu-id="941b5-139">the associated app.</span></span> <span data-ttu-id="941b5-140">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="941b5-140">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="941b5-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="941b5-141">roleScopeTagIds</span></span>|<span data-ttu-id="941b5-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="941b5-142">String collection</span></span>|<span data-ttu-id="941b5-143">Список тегов областей для этой сущности конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="941b5-143">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="941b5-144">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="941b5-144">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="941b5-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="941b5-145">createdDateTime</span></span>|<span data-ttu-id="941b5-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="941b5-146">DateTimeOffset</span></span>|<span data-ttu-id="941b5-147">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="941b5-147">DateTime the object was created.</span></span> <span data-ttu-id="941b5-148">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="941b5-148">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="941b5-149">description</span><span class="sxs-lookup"><span data-stu-id="941b5-149">description</span></span>|<span data-ttu-id="941b5-150">String</span><span class="sxs-lookup"><span data-stu-id="941b5-150">String</span></span>|<span data-ttu-id="941b5-151">Администратор предоставил описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="941b5-151">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="941b5-152">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="941b5-152">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="941b5-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="941b5-153">lastModifiedDateTime</span></span>|<span data-ttu-id="941b5-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="941b5-154">DateTimeOffset</span></span>|<span data-ttu-id="941b5-155">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="941b5-155">DateTime the object was last modified.</span></span> <span data-ttu-id="941b5-156">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="941b5-156">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="941b5-157">displayName</span><span class="sxs-lookup"><span data-stu-id="941b5-157">displayName</span></span>|<span data-ttu-id="941b5-158">Строка</span><span class="sxs-lookup"><span data-stu-id="941b5-158">String</span></span>|<span data-ttu-id="941b5-159">Администратор предоставил название конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="941b5-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="941b5-160">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="941b5-160">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="941b5-161">версия</span><span class="sxs-lookup"><span data-stu-id="941b5-161">version</span></span>|<span data-ttu-id="941b5-162">Int32</span><span class="sxs-lookup"><span data-stu-id="941b5-162">Int32</span></span>|<span data-ttu-id="941b5-163">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="941b5-163">Version of the device configuration.</span></span> <span data-ttu-id="941b5-164">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="941b5-164">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="941b5-165">packageId</span><span class="sxs-lookup"><span data-stu-id="941b5-165">packageId</span></span>|<span data-ttu-id="941b5-166">String</span><span class="sxs-lookup"><span data-stu-id="941b5-166">String</span></span>|<span data-ttu-id="941b5-167">Идентификатор пакета конфигурации приложения Android для рабочего приложения.</span><span class="sxs-lookup"><span data-stu-id="941b5-167">Android For Work app configuration package id.</span></span>|
|<span data-ttu-id="941b5-168">пайлоаджсон</span><span class="sxs-lookup"><span data-stu-id="941b5-168">payloadJson</span></span>|<span data-ttu-id="941b5-169">String</span><span class="sxs-lookup"><span data-stu-id="941b5-169">String</span></span>|<span data-ttu-id="941b5-170">Полезные данные JSON конфигурации приложения для Android для рабочего приложения.</span><span class="sxs-lookup"><span data-stu-id="941b5-170">Android For Work app configuration JSON payload.</span></span>|
|<span data-ttu-id="941b5-171">пермиссионактионс</span><span class="sxs-lookup"><span data-stu-id="941b5-171">permissionActions</span></span>|<span data-ttu-id="941b5-172">Коллекция [андроидпермиссионактион](../resources/intune-apps-androidpermissionaction.md)</span><span class="sxs-lookup"><span data-stu-id="941b5-172">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) collection</span></span>|<span data-ttu-id="941b5-173">Список разрешений приложений для Android и соответствующие действия с разрешениями.</span><span class="sxs-lookup"><span data-stu-id="941b5-173">List of Android app permissions and corresponding permission actions.</span></span>|
|<span data-ttu-id="941b5-174">профилеаппликабилити</span><span class="sxs-lookup"><span data-stu-id="941b5-174">profileApplicability</span></span>|[<span data-ttu-id="941b5-175">андроидпрофилеаппликабилити</span><span class="sxs-lookup"><span data-stu-id="941b5-175">androidProfileApplicability</span></span>](../resources/intune-apps-androidprofileapplicability.md)|<span data-ttu-id="941b5-176">Применимость профиля предприятия Android (Андроидворкпрофиле, Девицеовнер или Default (применяется к обоим).</span><span class="sxs-lookup"><span data-stu-id="941b5-176">Android Enterprise profile applicability (AndroidWorkProfile, DeviceOwner, or default (applies to both)).</span></span> <span data-ttu-id="941b5-177">Возможные значения: `default`, `androidWorkProfile`, `androidDeviceOwner`.</span><span class="sxs-lookup"><span data-stu-id="941b5-177">Possible values are: `default`, `androidWorkProfile`, `androidDeviceOwner`.</span></span>|



## <a name="response"></a><span data-ttu-id="941b5-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="941b5-178">Response</span></span>
<span data-ttu-id="941b5-179">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроидфорворкмобилеаппконфигуратион](../resources/intune-apps-androidforworkmobileappconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="941b5-179">If successful, this method returns a `200 OK` response code and an updated [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="941b5-180">Пример</span><span class="sxs-lookup"><span data-stu-id="941b5-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="941b5-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="941b5-181">Request</span></span>
<span data-ttu-id="941b5-182">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="941b5-182">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="941b5-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="941b5-183">Response</span></span>
<span data-ttu-id="941b5-p111">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="941b5-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



