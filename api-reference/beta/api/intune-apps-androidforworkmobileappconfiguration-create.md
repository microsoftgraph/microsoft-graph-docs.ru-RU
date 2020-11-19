---
title: Создание Андроидфорворкмобилеаппконфигуратион
description: Создание нового объекта Андроидфорворкмобилеаппконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7351556acfbb86ac27f399d1f6ce2fde186bc683
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49254064"
---
# <a name="create-androidforworkmobileappconfiguration"></a><span data-ttu-id="abb7a-103">Создание Андроидфорворкмобилеаппконфигуратион</span><span class="sxs-lookup"><span data-stu-id="abb7a-103">Create androidForWorkMobileAppConfiguration</span></span>

<span data-ttu-id="abb7a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="abb7a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="abb7a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="abb7a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="abb7a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="abb7a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="abb7a-107">Создание нового объекта [андроидфорворкмобилеаппконфигуратион](../resources/intune-apps-androidforworkmobileappconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="abb7a-107">Create a new [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="abb7a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="abb7a-108">Prerequisites</span></span>
<span data-ttu-id="abb7a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="abb7a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abb7a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="abb7a-111">Permission type</span></span>|<span data-ttu-id="abb7a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="abb7a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="abb7a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="abb7a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="abb7a-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="abb7a-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="abb7a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="abb7a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="abb7a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="abb7a-116">Not supported.</span></span>|
|<span data-ttu-id="abb7a-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="abb7a-117">Application</span></span>|<span data-ttu-id="abb7a-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="abb7a-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="abb7a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="abb7a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="abb7a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="abb7a-120">Request headers</span></span>
|<span data-ttu-id="abb7a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="abb7a-121">Header</span></span>|<span data-ttu-id="abb7a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="abb7a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="abb7a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="abb7a-123">Authorization</span></span>|<span data-ttu-id="abb7a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="abb7a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="abb7a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="abb7a-125">Accept</span></span>|<span data-ttu-id="abb7a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="abb7a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="abb7a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="abb7a-127">Request body</span></span>
<span data-ttu-id="abb7a-128">В тексте запроса добавьте представление объекта Андроидфорворкмобилеаппконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="abb7a-128">In the request body, supply a JSON representation for the androidForWorkMobileAppConfiguration object.</span></span>

<span data-ttu-id="abb7a-129">В следующей таблице приведены свойства, необходимые при создании Андроидфорворкмобилеаппконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="abb7a-129">The following table shows the properties that are required when you create the androidForWorkMobileAppConfiguration.</span></span>

|<span data-ttu-id="abb7a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="abb7a-130">Property</span></span>|<span data-ttu-id="abb7a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="abb7a-131">Type</span></span>|<span data-ttu-id="abb7a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="abb7a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="abb7a-133">id</span><span class="sxs-lookup"><span data-stu-id="abb7a-133">id</span></span>|<span data-ttu-id="abb7a-134">String</span><span class="sxs-lookup"><span data-stu-id="abb7a-134">String</span></span>|<span data-ttu-id="abb7a-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="abb7a-135">Key of the entity.</span></span> <span data-ttu-id="abb7a-136">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="abb7a-136">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="abb7a-137">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="abb7a-137">targetedMobileApps</span></span>|<span data-ttu-id="abb7a-138">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="abb7a-138">String collection</span></span>|<span data-ttu-id="abb7a-139">приложение-обработчик</span><span class="sxs-lookup"><span data-stu-id="abb7a-139">the associated app.</span></span> <span data-ttu-id="abb7a-140">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="abb7a-140">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="abb7a-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="abb7a-141">roleScopeTagIds</span></span>|<span data-ttu-id="abb7a-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="abb7a-142">String collection</span></span>|<span data-ttu-id="abb7a-143">Список тегов областей для этой сущности конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="abb7a-143">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="abb7a-144">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="abb7a-144">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="abb7a-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="abb7a-145">createdDateTime</span></span>|<span data-ttu-id="abb7a-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="abb7a-146">DateTimeOffset</span></span>|<span data-ttu-id="abb7a-147">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="abb7a-147">DateTime the object was created.</span></span> <span data-ttu-id="abb7a-148">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="abb7a-148">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="abb7a-149">description</span><span class="sxs-lookup"><span data-stu-id="abb7a-149">description</span></span>|<span data-ttu-id="abb7a-150">String</span><span class="sxs-lookup"><span data-stu-id="abb7a-150">String</span></span>|<span data-ttu-id="abb7a-151">Администратор предоставил описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="abb7a-151">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="abb7a-152">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="abb7a-152">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="abb7a-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="abb7a-153">lastModifiedDateTime</span></span>|<span data-ttu-id="abb7a-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="abb7a-154">DateTimeOffset</span></span>|<span data-ttu-id="abb7a-155">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="abb7a-155">DateTime the object was last modified.</span></span> <span data-ttu-id="abb7a-156">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="abb7a-156">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="abb7a-157">displayName</span><span class="sxs-lookup"><span data-stu-id="abb7a-157">displayName</span></span>|<span data-ttu-id="abb7a-158">String</span><span class="sxs-lookup"><span data-stu-id="abb7a-158">String</span></span>|<span data-ttu-id="abb7a-159">Администратор предоставил название конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="abb7a-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="abb7a-160">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="abb7a-160">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="abb7a-161">версия</span><span class="sxs-lookup"><span data-stu-id="abb7a-161">version</span></span>|<span data-ttu-id="abb7a-162">Int32</span><span class="sxs-lookup"><span data-stu-id="abb7a-162">Int32</span></span>|<span data-ttu-id="abb7a-163">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="abb7a-163">Version of the device configuration.</span></span> <span data-ttu-id="abb7a-164">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="abb7a-164">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="abb7a-165">packageId</span><span class="sxs-lookup"><span data-stu-id="abb7a-165">packageId</span></span>|<span data-ttu-id="abb7a-166">String</span><span class="sxs-lookup"><span data-stu-id="abb7a-166">String</span></span>|<span data-ttu-id="abb7a-167">Идентификатор пакета конфигурации приложения Android для рабочего приложения.</span><span class="sxs-lookup"><span data-stu-id="abb7a-167">Android For Work app configuration package id.</span></span>|
|<span data-ttu-id="abb7a-168">пайлоаджсон</span><span class="sxs-lookup"><span data-stu-id="abb7a-168">payloadJson</span></span>|<span data-ttu-id="abb7a-169">String</span><span class="sxs-lookup"><span data-stu-id="abb7a-169">String</span></span>|<span data-ttu-id="abb7a-170">Полезные данные JSON конфигурации приложения для Android для рабочего приложения.</span><span class="sxs-lookup"><span data-stu-id="abb7a-170">Android For Work app configuration JSON payload.</span></span>|
|<span data-ttu-id="abb7a-171">пермиссионактионс</span><span class="sxs-lookup"><span data-stu-id="abb7a-171">permissionActions</span></span>|<span data-ttu-id="abb7a-172">Коллекция [андроидпермиссионактион](../resources/intune-apps-androidpermissionaction.md)</span><span class="sxs-lookup"><span data-stu-id="abb7a-172">[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md) collection</span></span>|<span data-ttu-id="abb7a-173">Список разрешений приложений для Android и соответствующие действия с разрешениями.</span><span class="sxs-lookup"><span data-stu-id="abb7a-173">List of Android app permissions and corresponding permission actions.</span></span>|
|<span data-ttu-id="abb7a-174">профилеаппликабилити</span><span class="sxs-lookup"><span data-stu-id="abb7a-174">profileApplicability</span></span>|[<span data-ttu-id="abb7a-175">androidProfileApplicability</span><span class="sxs-lookup"><span data-stu-id="abb7a-175">androidProfileApplicability</span></span>](../resources/intune-apps-androidprofileapplicability.md)|<span data-ttu-id="abb7a-176">Применимость профиля предприятия Android (Андроидворкпрофиле, Девицеовнер или Default (применяется к обоим).</span><span class="sxs-lookup"><span data-stu-id="abb7a-176">Android Enterprise profile applicability (AndroidWorkProfile, DeviceOwner, or default (applies to both)).</span></span> <span data-ttu-id="abb7a-177">Возможные значения: `default`, `androidWorkProfile`, `androidDeviceOwner`.</span><span class="sxs-lookup"><span data-stu-id="abb7a-177">Possible values are: `default`, `androidWorkProfile`, `androidDeviceOwner`.</span></span>|



## <a name="response"></a><span data-ttu-id="abb7a-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="abb7a-178">Response</span></span>
<span data-ttu-id="abb7a-179">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроидфорворкмобилеаппконфигуратион](../resources/intune-apps-androidforworkmobileappconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="abb7a-179">If successful, this method returns a `201 Created` response code and a [androidForWorkMobileAppConfiguration](../resources/intune-apps-androidforworkmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="abb7a-180">Пример</span><span class="sxs-lookup"><span data-stu-id="abb7a-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="abb7a-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="abb7a-181">Request</span></span>
<span data-ttu-id="abb7a-182">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="abb7a-182">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations
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

### <a name="response"></a><span data-ttu-id="abb7a-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="abb7a-183">Response</span></span>
<span data-ttu-id="abb7a-p111">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="abb7a-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




