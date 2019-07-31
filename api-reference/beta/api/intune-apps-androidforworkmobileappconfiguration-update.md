---
title: Обновление Андроидфорворкмобилеаппконфигуратион
description: Обновление свойств объекта Андроидфорворкмобилеаппконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2a13d4ba462bac49096cfeb9da13af56d74921e4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35952340"
---
# <a name="update-androidforworkmobileappconfiguration"></a><span data-ttu-id="c34ac-103">Обновление Андроидфорворкмобилеаппконфигуратион</span><span class="sxs-lookup"><span data-stu-id="c34ac-103">Update androidForWorkMobileAppConfiguration</span></span>

> <span data-ttu-id="c34ac-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c34ac-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c34ac-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c34ac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c34ac-106">Обновление свойств объекта [андроидфорворкмобилеаппконфигуратион](../resources/intune-apps-androidforworkmobileappconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="c34ac-106">Update the properties of a [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c34ac-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c34ac-107">Prerequisites</span></span>
<span data-ttu-id="c34ac-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c34ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c34ac-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c34ac-110">Permission type</span></span>|<span data-ttu-id="c34ac-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c34ac-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c34ac-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c34ac-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c34ac-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c34ac-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c34ac-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c34ac-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c34ac-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c34ac-115">Not supported.</span></span>|
|<span data-ttu-id="c34ac-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c34ac-116">Application</span></span>|<span data-ttu-id="c34ac-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c34ac-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c34ac-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c34ac-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c34ac-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c34ac-119">Request headers</span></span>
|<span data-ttu-id="c34ac-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c34ac-120">Header</span></span>|<span data-ttu-id="c34ac-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c34ac-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c34ac-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c34ac-122">Authorization</span></span>|<span data-ttu-id="c34ac-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c34ac-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c34ac-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c34ac-124">Accept</span></span>|<span data-ttu-id="c34ac-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c34ac-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c34ac-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c34ac-126">Request body</span></span>
<span data-ttu-id="c34ac-127">В тексте запроса добавьте представление объекта [андроидфорворкмобилеаппконфигуратион](../resources/intune-apps-androidforworkmobileappconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c34ac-127">In the request body, supply a JSON representation for the [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object.</span></span>

<span data-ttu-id="c34ac-128">В следующей таблице приведены свойства, необходимые при создании [андроидфорворкмобилеаппконфигуратион](../resources/intune-apps-androidforworkmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c34ac-128">The following table shows the properties that are required when you create the [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md).</span></span>

|<span data-ttu-id="c34ac-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c34ac-129">Property</span></span>|<span data-ttu-id="c34ac-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c34ac-130">Type</span></span>|<span data-ttu-id="c34ac-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c34ac-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c34ac-132">id</span><span class="sxs-lookup"><span data-stu-id="c34ac-132">id</span></span>|<span data-ttu-id="c34ac-133">Строка</span><span class="sxs-lookup"><span data-stu-id="c34ac-133">String</span></span>|<span data-ttu-id="c34ac-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c34ac-134">Key of the entity.</span></span> <span data-ttu-id="c34ac-135">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c34ac-135">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="c34ac-136">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="c34ac-136">targetedMobileApps</span></span>|<span data-ttu-id="c34ac-137">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c34ac-137">String collection</span></span>|<span data-ttu-id="c34ac-138">приложение-обработчик</span><span class="sxs-lookup"><span data-stu-id="c34ac-138">the associated app.</span></span> <span data-ttu-id="c34ac-139">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c34ac-139">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="c34ac-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c34ac-140">roleScopeTagIds</span></span>|<span data-ttu-id="c34ac-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="c34ac-141">String collection</span></span>|<span data-ttu-id="c34ac-142">Список тегов областей для этой сущности конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="c34ac-142">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="c34ac-143">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c34ac-143">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="c34ac-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c34ac-144">createdDateTime</span></span>|<span data-ttu-id="c34ac-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c34ac-145">DateTimeOffset</span></span>|<span data-ttu-id="c34ac-146">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c34ac-146">DateTime the object was created.</span></span> <span data-ttu-id="c34ac-147">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c34ac-147">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="c34ac-148">description</span><span class="sxs-lookup"><span data-stu-id="c34ac-148">description</span></span>|<span data-ttu-id="c34ac-149">String</span><span class="sxs-lookup"><span data-stu-id="c34ac-149">String</span></span>|<span data-ttu-id="c34ac-150">Администратор предоставил описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c34ac-150">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c34ac-151">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c34ac-151">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="c34ac-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c34ac-152">lastModifiedDateTime</span></span>|<span data-ttu-id="c34ac-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c34ac-153">DateTimeOffset</span></span>|<span data-ttu-id="c34ac-154">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c34ac-154">DateTime the object was last modified.</span></span> <span data-ttu-id="c34ac-155">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c34ac-155">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="c34ac-156">displayName</span><span class="sxs-lookup"><span data-stu-id="c34ac-156">displayName</span></span>|<span data-ttu-id="c34ac-157">Строка</span><span class="sxs-lookup"><span data-stu-id="c34ac-157">String</span></span>|<span data-ttu-id="c34ac-158">Администратор предоставил название конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c34ac-158">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c34ac-159">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c34ac-159">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="c34ac-160">версия</span><span class="sxs-lookup"><span data-stu-id="c34ac-160">version</span></span>|<span data-ttu-id="c34ac-161">Int32</span><span class="sxs-lookup"><span data-stu-id="c34ac-161">Int32</span></span>|<span data-ttu-id="c34ac-162">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c34ac-162">Version of the device configuration.</span></span> <span data-ttu-id="c34ac-163">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c34ac-163">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="c34ac-164">packageId</span><span class="sxs-lookup"><span data-stu-id="c34ac-164">packageId</span></span>|<span data-ttu-id="c34ac-165">String</span><span class="sxs-lookup"><span data-stu-id="c34ac-165">String</span></span>|<span data-ttu-id="c34ac-166">Идентификатор пакета конфигурации приложения Android для рабочего приложения.</span><span class="sxs-lookup"><span data-stu-id="c34ac-166">Android For Work app configuration package id.</span></span>|
|<span data-ttu-id="c34ac-167">Пайлоаджсон</span><span class="sxs-lookup"><span data-stu-id="c34ac-167">payloadJson</span></span>|<span data-ttu-id="c34ac-168">String</span><span class="sxs-lookup"><span data-stu-id="c34ac-168">String</span></span>|<span data-ttu-id="c34ac-169">Полезные данные JSON конфигурации приложения для Android для рабочего приложения.</span><span class="sxs-lookup"><span data-stu-id="c34ac-169">Android For Work app configuration JSON payload.</span></span>|
|<span data-ttu-id="c34ac-170">Пермиссионактионс</span><span class="sxs-lookup"><span data-stu-id="c34ac-170">permissionActions</span></span>|<span data-ttu-id="c34ac-171">Коллекция [андроидпермиссионактион](../resources/intune-apps-androidpermissionaction.md)</span><span class="sxs-lookup"><span data-stu-id="c34ac-171">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) collection</span></span>|<span data-ttu-id="c34ac-172">Список разрешений приложений для Android и соответствующие действия с разрешениями.</span><span class="sxs-lookup"><span data-stu-id="c34ac-172">List of Android app permissions and corresponding permission actions.</span></span>|



## <a name="response"></a><span data-ttu-id="c34ac-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="c34ac-173">Response</span></span>
<span data-ttu-id="c34ac-174">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроидфорворкмобилеаппконфигуратион](../resources/intune-apps-androidforworkmobileappconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c34ac-174">If successful, this method returns a `200 OK` response code and an updated [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c34ac-175">Пример</span><span class="sxs-lookup"><span data-stu-id="c34ac-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="c34ac-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="c34ac-176">Request</span></span>
<span data-ttu-id="c34ac-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c34ac-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c34ac-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="c34ac-178">Response</span></span>
<span data-ttu-id="c34ac-p110">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c34ac-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





