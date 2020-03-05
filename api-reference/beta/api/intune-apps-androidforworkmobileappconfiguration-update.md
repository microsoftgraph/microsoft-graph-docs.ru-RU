---
title: Обновление Андроидфорворкмобилеаппконфигуратион
description: Обновление свойств объекта Андроидфорворкмобилеаппконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b37272bc0b7b55a3476bf9dee059380298512644
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42445962"
---
# <a name="update-androidforworkmobileappconfiguration"></a><span data-ttu-id="b0501-103">Обновление Андроидфорворкмобилеаппконфигуратион</span><span class="sxs-lookup"><span data-stu-id="b0501-103">Update androidForWorkMobileAppConfiguration</span></span>

<span data-ttu-id="b0501-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b0501-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b0501-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0501-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0501-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b0501-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0501-107">Обновление свойств объекта [андроидфорворкмобилеаппконфигуратион](../resources/intune-apps-androidforworkmobileappconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="b0501-107">Update the properties of a [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b0501-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b0501-108">Prerequisites</span></span>
<span data-ttu-id="b0501-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0501-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0501-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b0501-111">Permission type</span></span>|<span data-ttu-id="b0501-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b0501-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0501-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b0501-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b0501-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0501-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b0501-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b0501-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0501-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0501-116">Not supported.</span></span>|
|<span data-ttu-id="b0501-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b0501-117">Application</span></span>|<span data-ttu-id="b0501-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0501-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0501-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b0501-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b0501-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b0501-120">Request headers</span></span>
|<span data-ttu-id="b0501-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b0501-121">Header</span></span>|<span data-ttu-id="b0501-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b0501-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0501-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0501-123">Authorization</span></span>|<span data-ttu-id="b0501-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b0501-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b0501-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b0501-125">Accept</span></span>|<span data-ttu-id="b0501-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b0501-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0501-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b0501-127">Request body</span></span>
<span data-ttu-id="b0501-128">В тексте запроса добавьте представление объекта [андроидфорворкмобилеаппконфигуратион](../resources/intune-apps-androidforworkmobileappconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b0501-128">In the request body, supply a JSON representation for the [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object.</span></span>

<span data-ttu-id="b0501-129">В следующей таблице приведены свойства, необходимые при создании [андроидфорворкмобилеаппконфигуратион](../resources/intune-apps-androidforworkmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b0501-129">The following table shows the properties that are required when you create the [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md).</span></span>

|<span data-ttu-id="b0501-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b0501-130">Property</span></span>|<span data-ttu-id="b0501-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b0501-131">Type</span></span>|<span data-ttu-id="b0501-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b0501-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0501-133">id</span><span class="sxs-lookup"><span data-stu-id="b0501-133">id</span></span>|<span data-ttu-id="b0501-134">Строка</span><span class="sxs-lookup"><span data-stu-id="b0501-134">String</span></span>|<span data-ttu-id="b0501-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b0501-135">Key of the entity.</span></span> <span data-ttu-id="b0501-136">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0501-136">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="b0501-137">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="b0501-137">targetedMobileApps</span></span>|<span data-ttu-id="b0501-138">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b0501-138">String collection</span></span>|<span data-ttu-id="b0501-139">приложение-обработчик</span><span class="sxs-lookup"><span data-stu-id="b0501-139">the associated app.</span></span> <span data-ttu-id="b0501-140">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0501-140">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="b0501-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b0501-141">roleScopeTagIds</span></span>|<span data-ttu-id="b0501-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b0501-142">String collection</span></span>|<span data-ttu-id="b0501-143">Список тегов областей для этой сущности конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="b0501-143">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="b0501-144">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0501-144">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="b0501-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b0501-145">createdDateTime</span></span>|<span data-ttu-id="b0501-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0501-146">DateTimeOffset</span></span>|<span data-ttu-id="b0501-147">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="b0501-147">DateTime the object was created.</span></span> <span data-ttu-id="b0501-148">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0501-148">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="b0501-149">description</span><span class="sxs-lookup"><span data-stu-id="b0501-149">description</span></span>|<span data-ttu-id="b0501-150">String</span><span class="sxs-lookup"><span data-stu-id="b0501-150">String</span></span>|<span data-ttu-id="b0501-151">Администратор предоставил описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b0501-151">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b0501-152">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0501-152">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="b0501-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b0501-153">lastModifiedDateTime</span></span>|<span data-ttu-id="b0501-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0501-154">DateTimeOffset</span></span>|<span data-ttu-id="b0501-155">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="b0501-155">DateTime the object was last modified.</span></span> <span data-ttu-id="b0501-156">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0501-156">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="b0501-157">displayName</span><span class="sxs-lookup"><span data-stu-id="b0501-157">displayName</span></span>|<span data-ttu-id="b0501-158">Строка</span><span class="sxs-lookup"><span data-stu-id="b0501-158">String</span></span>|<span data-ttu-id="b0501-159">Администратор предоставил название конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b0501-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b0501-160">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0501-160">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="b0501-161">версия</span><span class="sxs-lookup"><span data-stu-id="b0501-161">version</span></span>|<span data-ttu-id="b0501-162">Int32</span><span class="sxs-lookup"><span data-stu-id="b0501-162">Int32</span></span>|<span data-ttu-id="b0501-163">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b0501-163">Version of the device configuration.</span></span> <span data-ttu-id="b0501-164">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0501-164">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="b0501-165">packageId</span><span class="sxs-lookup"><span data-stu-id="b0501-165">packageId</span></span>|<span data-ttu-id="b0501-166">String</span><span class="sxs-lookup"><span data-stu-id="b0501-166">String</span></span>|<span data-ttu-id="b0501-167">Идентификатор пакета конфигурации приложения Android для рабочего приложения.</span><span class="sxs-lookup"><span data-stu-id="b0501-167">Android For Work app configuration package id.</span></span>|
|<span data-ttu-id="b0501-168">пайлоаджсон</span><span class="sxs-lookup"><span data-stu-id="b0501-168">payloadJson</span></span>|<span data-ttu-id="b0501-169">String</span><span class="sxs-lookup"><span data-stu-id="b0501-169">String</span></span>|<span data-ttu-id="b0501-170">Полезные данные JSON конфигурации приложения для Android для рабочего приложения.</span><span class="sxs-lookup"><span data-stu-id="b0501-170">Android For Work app configuration JSON payload.</span></span>|
|<span data-ttu-id="b0501-171">пермиссионактионс</span><span class="sxs-lookup"><span data-stu-id="b0501-171">permissionActions</span></span>|<span data-ttu-id="b0501-172">Коллекция [андроидпермиссионактион](../resources/intune-apps-androidpermissionaction.md)</span><span class="sxs-lookup"><span data-stu-id="b0501-172">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) collection</span></span>|<span data-ttu-id="b0501-173">Список разрешений приложений для Android и соответствующие действия с разрешениями.</span><span class="sxs-lookup"><span data-stu-id="b0501-173">List of Android app permissions and corresponding permission actions.</span></span>|



## <a name="response"></a><span data-ttu-id="b0501-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0501-174">Response</span></span>
<span data-ttu-id="b0501-175">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроидфорворкмобилеаппконфигуратион](../resources/intune-apps-androidforworkmobileappconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b0501-175">If successful, this method returns a `200 OK` response code and an updated [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0501-176">Пример</span><span class="sxs-lookup"><span data-stu-id="b0501-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="b0501-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="b0501-177">Request</span></span>
<span data-ttu-id="b0501-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b0501-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
Content-type: application/json
Content-length: 560

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
  ]
}
```

### <a name="response"></a><span data-ttu-id="b0501-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0501-179">Response</span></span>
<span data-ttu-id="b0501-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b0501-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 732

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
  ]
}
```





