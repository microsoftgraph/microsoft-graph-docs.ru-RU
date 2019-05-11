---
title: Обновление Андроидфорворкмобилеаппконфигуратион
description: Обновление свойств объекта Андроидфорворкмобилеаппконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8666d179d2b51419b934915ed38b760c192a5329
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33937472"
---
# <a name="update-androidforworkmobileappconfiguration"></a><span data-ttu-id="1ecd2-103">Обновление Андроидфорворкмобилеаппконфигуратион</span><span class="sxs-lookup"><span data-stu-id="1ecd2-103">Update androidForWorkMobileAppConfiguration</span></span>

> <span data-ttu-id="1ecd2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ecd2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1ecd2-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1ecd2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ecd2-106">Обновление свойств объекта [андроидфорворкмобилеаппконфигуратион](../resources/intune-apps-androidforworkmobileappconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="1ecd2-106">Update the properties of a [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1ecd2-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1ecd2-107">Prerequisites</span></span>
<span data-ttu-id="1ecd2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ecd2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ecd2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1ecd2-110">Permission type</span></span>|<span data-ttu-id="1ecd2-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1ecd2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ecd2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1ecd2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1ecd2-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ecd2-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1ecd2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1ecd2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ecd2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ecd2-115">Not supported.</span></span>|
|<span data-ttu-id="1ecd2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1ecd2-116">Application</span></span>|<span data-ttu-id="1ecd2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ecd2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ecd2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1ecd2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="1ecd2-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1ecd2-119">Request headers</span></span>
|<span data-ttu-id="1ecd2-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1ecd2-120">Header</span></span>|<span data-ttu-id="1ecd2-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1ecd2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1ecd2-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1ecd2-122">Authorization</span></span>|<span data-ttu-id="1ecd2-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1ecd2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1ecd2-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1ecd2-124">Accept</span></span>|<span data-ttu-id="1ecd2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1ecd2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ecd2-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1ecd2-126">Request body</span></span>
<span data-ttu-id="1ecd2-127">В тексте запроса добавьте представление объекта [Андроидфорворкмобилеаппконфигуратион](../resources/intune-apps-androidforworkmobileappconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1ecd2-127">In the request body, supply a JSON representation for the [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object.</span></span>

<span data-ttu-id="1ecd2-128">В следующей таблице приведены свойства, необходимые при создании [андроидфорворкмобилеаппконфигуратион](../resources/intune-apps-androidforworkmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1ecd2-128">The following table shows the properties that are required when you create the [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md).</span></span>

|<span data-ttu-id="1ecd2-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="1ecd2-129">Property</span></span>|<span data-ttu-id="1ecd2-130">Тип</span><span class="sxs-lookup"><span data-stu-id="1ecd2-130">Type</span></span>|<span data-ttu-id="1ecd2-131">Описание</span><span class="sxs-lookup"><span data-stu-id="1ecd2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ecd2-132">id</span><span class="sxs-lookup"><span data-stu-id="1ecd2-132">id</span></span>|<span data-ttu-id="1ecd2-133">Строка</span><span class="sxs-lookup"><span data-stu-id="1ecd2-133">String</span></span>|<span data-ttu-id="1ecd2-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1ecd2-134">Key of the entity.</span></span> <span data-ttu-id="1ecd2-135">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ecd2-135">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="1ecd2-136">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="1ecd2-136">targetedMobileApps</span></span>|<span data-ttu-id="1ecd2-137">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1ecd2-137">String collection</span></span>|<span data-ttu-id="1ecd2-138">приложение-обработчик</span><span class="sxs-lookup"><span data-stu-id="1ecd2-138">the associated app.</span></span> <span data-ttu-id="1ecd2-139">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ecd2-139">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="1ecd2-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1ecd2-140">roleScopeTagIds</span></span>|<span data-ttu-id="1ecd2-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="1ecd2-141">String collection</span></span>|<span data-ttu-id="1ecd2-142">Список тегов областей для этой сущности конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="1ecd2-142">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="1ecd2-143">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ecd2-143">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="1ecd2-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1ecd2-144">createdDateTime</span></span>|<span data-ttu-id="1ecd2-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ecd2-145">DateTimeOffset</span></span>|<span data-ttu-id="1ecd2-146">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="1ecd2-146">DateTime the object was created.</span></span> <span data-ttu-id="1ecd2-147">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ecd2-147">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="1ecd2-148">description</span><span class="sxs-lookup"><span data-stu-id="1ecd2-148">description</span></span>|<span data-ttu-id="1ecd2-149">String</span><span class="sxs-lookup"><span data-stu-id="1ecd2-149">String</span></span>|<span data-ttu-id="1ecd2-150">Администратор предоставил описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1ecd2-150">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1ecd2-151">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ecd2-151">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="1ecd2-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1ecd2-152">lastModifiedDateTime</span></span>|<span data-ttu-id="1ecd2-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ecd2-153">DateTimeOffset</span></span>|<span data-ttu-id="1ecd2-154">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="1ecd2-154">DateTime the object was last modified.</span></span> <span data-ttu-id="1ecd2-155">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ecd2-155">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="1ecd2-156">displayName</span><span class="sxs-lookup"><span data-stu-id="1ecd2-156">displayName</span></span>|<span data-ttu-id="1ecd2-157">Строка</span><span class="sxs-lookup"><span data-stu-id="1ecd2-157">String</span></span>|<span data-ttu-id="1ecd2-158">Администратор предоставил название конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1ecd2-158">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1ecd2-159">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ecd2-159">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="1ecd2-160">версия</span><span class="sxs-lookup"><span data-stu-id="1ecd2-160">version</span></span>|<span data-ttu-id="1ecd2-161">Int32</span><span class="sxs-lookup"><span data-stu-id="1ecd2-161">Int32</span></span>|<span data-ttu-id="1ecd2-162">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1ecd2-162">Version of the device configuration.</span></span> <span data-ttu-id="1ecd2-163">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ecd2-163">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="1ecd2-164">packageId</span><span class="sxs-lookup"><span data-stu-id="1ecd2-164">packageId</span></span>|<span data-ttu-id="1ecd2-165">String</span><span class="sxs-lookup"><span data-stu-id="1ecd2-165">String</span></span>|<span data-ttu-id="1ecd2-166">Идентификатор пакета конфигурации приложения Android для рабочего приложения.</span><span class="sxs-lookup"><span data-stu-id="1ecd2-166">Android For Work app configuration package id.</span></span>|
|<span data-ttu-id="1ecd2-167">Пайлоаджсон</span><span class="sxs-lookup"><span data-stu-id="1ecd2-167">payloadJson</span></span>|<span data-ttu-id="1ecd2-168">Строка</span><span class="sxs-lookup"><span data-stu-id="1ecd2-168">String</span></span>|<span data-ttu-id="1ecd2-169">Полезные данные JSON конфигурации приложения для Android для рабочего приложения.</span><span class="sxs-lookup"><span data-stu-id="1ecd2-169">Android For Work app configuration JSON payload.</span></span>|
|<span data-ttu-id="1ecd2-170">Пермиссионактионс</span><span class="sxs-lookup"><span data-stu-id="1ecd2-170">permissionActions</span></span>|<span data-ttu-id="1ecd2-171">Коллекция [андроидпермиссионактион](../resources/intune-apps-androidpermissionaction.md)</span><span class="sxs-lookup"><span data-stu-id="1ecd2-171">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) collection</span></span>|<span data-ttu-id="1ecd2-172">Список разрешений приложений для Android и соответствующие действия с разрешениями.</span><span class="sxs-lookup"><span data-stu-id="1ecd2-172">List of Android app permissions and corresponding permission actions.</span></span>|



## <a name="response"></a><span data-ttu-id="1ecd2-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ecd2-173">Response</span></span>
<span data-ttu-id="1ecd2-174">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроидфорворкмобилеаппконфигуратион](../resources/intune-apps-androidforworkmobileappconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1ecd2-174">If successful, this method returns a `200 OK` response code and an updated [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ecd2-175">Пример</span><span class="sxs-lookup"><span data-stu-id="1ecd2-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="1ecd2-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="1ecd2-176">Request</span></span>
<span data-ttu-id="1ecd2-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1ecd2-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1ecd2-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ecd2-178">Response</span></span>
<span data-ttu-id="1ecd2-p110">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1ecd2-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




