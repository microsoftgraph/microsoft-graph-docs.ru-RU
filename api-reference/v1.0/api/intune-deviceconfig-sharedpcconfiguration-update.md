---
title: Обновление объекта sharedPCConfiguration
description: Обновляет свойства объекта sharedPCConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e4636a1b03a217cecb8857c7b4b710053ee11ec2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47968180"
---
# <a name="update-sharedpcconfiguration"></a><span data-ttu-id="2bfd1-103">Обновление объекта sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="2bfd1-103">Update sharedPCConfiguration</span></span>

<span data-ttu-id="2bfd1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2bfd1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2bfd1-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2bfd1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2bfd1-106">Обновляет свойства объекта [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2bfd1-106">Update the properties of a [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2bfd1-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2bfd1-107">Prerequisites</span></span>
<span data-ttu-id="2bfd1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2bfd1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2bfd1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2bfd1-110">Permission type</span></span>|<span data-ttu-id="2bfd1-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2bfd1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2bfd1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2bfd1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2bfd1-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2bfd1-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2bfd1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2bfd1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2bfd1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2bfd1-115">Not supported.</span></span>|
|<span data-ttu-id="2bfd1-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2bfd1-116">Application</span></span>|<span data-ttu-id="2bfd1-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2bfd1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2bfd1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2bfd1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2bfd1-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2bfd1-119">Request headers</span></span>
|<span data-ttu-id="2bfd1-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2bfd1-120">Header</span></span>|<span data-ttu-id="2bfd1-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2bfd1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2bfd1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2bfd1-122">Authorization</span></span>|<span data-ttu-id="2bfd1-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2bfd1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2bfd1-124">Accept</span><span class="sxs-lookup"><span data-stu-id="2bfd1-124">Accept</span></span>|<span data-ttu-id="2bfd1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2bfd1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2bfd1-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2bfd1-126">Request body</span></span>
<span data-ttu-id="2bfd1-127">В теле запроса добавьте представление объекта [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2bfd1-127">In the request body, supply a JSON representation for the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

<span data-ttu-id="2bfd1-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2bfd1-128">The following table shows the properties that are required when you create the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span></span>

|<span data-ttu-id="2bfd1-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="2bfd1-129">Property</span></span>|<span data-ttu-id="2bfd1-130">Тип</span><span class="sxs-lookup"><span data-stu-id="2bfd1-130">Type</span></span>|<span data-ttu-id="2bfd1-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2bfd1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2bfd1-132">id</span><span class="sxs-lookup"><span data-stu-id="2bfd1-132">id</span></span>|<span data-ttu-id="2bfd1-133">String</span><span class="sxs-lookup"><span data-stu-id="2bfd1-133">String</span></span>|<span data-ttu-id="2bfd1-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2bfd1-134">Key of the entity.</span></span> <span data-ttu-id="2bfd1-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2bfd1-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2bfd1-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2bfd1-136">lastModifiedDateTime</span></span>|<span data-ttu-id="2bfd1-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2bfd1-137">DateTimeOffset</span></span>|<span data-ttu-id="2bfd1-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="2bfd1-138">DateTime the object was last modified.</span></span> <span data-ttu-id="2bfd1-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2bfd1-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2bfd1-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2bfd1-140">createdDateTime</span></span>|<span data-ttu-id="2bfd1-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2bfd1-141">DateTimeOffset</span></span>|<span data-ttu-id="2bfd1-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="2bfd1-142">DateTime the object was created.</span></span> <span data-ttu-id="2bfd1-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2bfd1-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2bfd1-144">description</span><span class="sxs-lookup"><span data-stu-id="2bfd1-144">description</span></span>|<span data-ttu-id="2bfd1-145">String</span><span class="sxs-lookup"><span data-stu-id="2bfd1-145">String</span></span>|<span data-ttu-id="2bfd1-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2bfd1-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2bfd1-147">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2bfd1-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2bfd1-148">displayName</span><span class="sxs-lookup"><span data-stu-id="2bfd1-148">displayName</span></span>|<span data-ttu-id="2bfd1-149">String</span><span class="sxs-lookup"><span data-stu-id="2bfd1-149">String</span></span>|<span data-ttu-id="2bfd1-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2bfd1-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2bfd1-151">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2bfd1-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2bfd1-152">version</span><span class="sxs-lookup"><span data-stu-id="2bfd1-152">version</span></span>|<span data-ttu-id="2bfd1-153">Int32</span><span class="sxs-lookup"><span data-stu-id="2bfd1-153">Int32</span></span>|<span data-ttu-id="2bfd1-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2bfd1-154">Version of the device configuration.</span></span> <span data-ttu-id="2bfd1-155">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2bfd1-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2bfd1-156">accountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="2bfd1-156">accountManagerPolicy</span></span>|[<span data-ttu-id="2bfd1-157">sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="2bfd1-157">sharedPCAccountManagerPolicy</span></span>](../resources/intune-deviceconfig-sharedpcaccountmanagerpolicy.md)|<span data-ttu-id="2bfd1-158">Определяет способ управления учетными записями на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="2bfd1-158">Specifies how accounts are managed on a shared PC.</span></span> <span data-ttu-id="2bfd1-159">Применяется, только если для параметра disableAccountManager установлено значение false.</span><span class="sxs-lookup"><span data-stu-id="2bfd1-159">Only applies when disableAccountManager is false.</span></span>|
|<span data-ttu-id="2bfd1-160">allowedAccounts</span><span class="sxs-lookup"><span data-stu-id="2bfd1-160">allowedAccounts</span></span>|[<span data-ttu-id="2bfd1-161">шаредпкалловедаккаунттипе</span><span class="sxs-lookup"><span data-stu-id="2bfd1-161">sharedPCAllowedAccountType</span></span>](../resources/intune-deviceconfig-sharedpcallowedaccounttype.md)|<span data-ttu-id="2bfd1-162">Указывает тип учетных записей, которые можно использовать на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="2bfd1-162">Indicates which type of accounts are allowed to use on a shared PC.</span></span> <span data-ttu-id="2bfd1-163">Возможные значения: `guest`, `domain`.</span><span class="sxs-lookup"><span data-stu-id="2bfd1-163">Possible values are: `guest`, `domain`.</span></span>|
|<span data-ttu-id="2bfd1-164">allowLocalStorage</span><span class="sxs-lookup"><span data-stu-id="2bfd1-164">allowLocalStorage</span></span>|<span data-ttu-id="2bfd1-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bfd1-165">Boolean</span></span>|<span data-ttu-id="2bfd1-166">Определяет, разрешено ли на общем компьютере локальное хранилище.</span><span class="sxs-lookup"><span data-stu-id="2bfd1-166">Specifies whether local storage is allowed on a shared PC.</span></span>|
|<span data-ttu-id="2bfd1-167">disableAccountManager</span><span class="sxs-lookup"><span data-stu-id="2bfd1-167">disableAccountManager</span></span>|<span data-ttu-id="2bfd1-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bfd1-168">Boolean</span></span>|<span data-ttu-id="2bfd1-169">Отключает диспетчер учетных записей в режиме совместного использования компьютера.</span><span class="sxs-lookup"><span data-stu-id="2bfd1-169">Disables the account manager for shared PC mode.</span></span>|
|<span data-ttu-id="2bfd1-170">disableEduPolicies</span><span class="sxs-lookup"><span data-stu-id="2bfd1-170">disableEduPolicies</span></span>|<span data-ttu-id="2bfd1-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bfd1-171">Boolean</span></span>|<span data-ttu-id="2bfd1-172">Указывает, следует ли отключить стандартные политики среды совместного использования компьютера для образования.</span><span class="sxs-lookup"><span data-stu-id="2bfd1-172">Specifies whether the default shared PC education environment policies should be disabled.</span></span> <span data-ttu-id="2bfd1-173">Для Windows 10 RS2 и более поздних версий эта политика будет применяться без установки значения True для параметра Enabled.</span><span class="sxs-lookup"><span data-stu-id="2bfd1-173">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span>|
|<span data-ttu-id="2bfd1-174">disablePowerPolicies</span><span class="sxs-lookup"><span data-stu-id="2bfd1-174">disablePowerPolicies</span></span>|<span data-ttu-id="2bfd1-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bfd1-175">Boolean</span></span>|<span data-ttu-id="2bfd1-176">Указывает, следует ли отключить стандартные политики электропитания для общего компьютера.</span><span class="sxs-lookup"><span data-stu-id="2bfd1-176">Specifies whether the default shared PC power policies should be disabled.</span></span>|
|<span data-ttu-id="2bfd1-177">disableSignInOnResume</span><span class="sxs-lookup"><span data-stu-id="2bfd1-177">disableSignInOnResume</span></span>|<span data-ttu-id="2bfd1-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bfd1-178">Boolean</span></span>|<span data-ttu-id="2bfd1-179">Отключает обязательный вход в систему при выходе устройства из спящего режима.</span><span class="sxs-lookup"><span data-stu-id="2bfd1-179">Disables the requirement to sign in whenever the device wakes up from sleep mode.</span></span>|
|<span data-ttu-id="2bfd1-180">enabled</span><span class="sxs-lookup"><span data-stu-id="2bfd1-180">enabled</span></span>|<span data-ttu-id="2bfd1-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bfd1-181">Boolean</span></span>|<span data-ttu-id="2bfd1-182">Включает режим общего компьютера и применяет политики совместного использования ПК.</span><span class="sxs-lookup"><span data-stu-id="2bfd1-182">Enables shared PC mode and applies the shared pc policies.</span></span>|
|<span data-ttu-id="2bfd1-183">idleTimeBeforeSleepInSeconds</span><span class="sxs-lookup"><span data-stu-id="2bfd1-183">idleTimeBeforeSleepInSeconds</span></span>|<span data-ttu-id="2bfd1-184">Int32</span><span class="sxs-lookup"><span data-stu-id="2bfd1-184">Int32</span></span>|<span data-ttu-id="2bfd1-185">Определяет длительность (в секундах) пребывания устройства в режиме бездействия перед переходом в спящий режим.</span><span class="sxs-lookup"><span data-stu-id="2bfd1-185">Specifies the time in seconds that a device must sit idle before the PC goes to sleep.</span></span> <span data-ttu-id="2bfd1-186">Если задать значение 0, переход в спящий режим отключается.</span><span class="sxs-lookup"><span data-stu-id="2bfd1-186">Setting this value to 0 prevents the sleep timeout from occurring.</span></span>|
|<span data-ttu-id="2bfd1-187">kioskAppDisplayName</span><span class="sxs-lookup"><span data-stu-id="2bfd1-187">kioskAppDisplayName</span></span>|<span data-ttu-id="2bfd1-188">String</span><span class="sxs-lookup"><span data-stu-id="2bfd1-188">String</span></span>|<span data-ttu-id="2bfd1-189">Задает текст для учетной записи, который отображается на экране входа в систему и используется для запуска приложения, определяемого с помощью свойства SetKioskAppUserModelId.</span><span class="sxs-lookup"><span data-stu-id="2bfd1-189">Specifies the display text for the account shown on the sign-in screen which launches the app specified by SetKioskAppUserModelId.</span></span> <span data-ttu-id="2bfd1-190">Применяется, только если задано свойство KioskAppUserModelId.</span><span class="sxs-lookup"><span data-stu-id="2bfd1-190">Only applies when KioskAppUserModelId is set.</span></span>|
|<span data-ttu-id="2bfd1-191">kioskAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="2bfd1-191">kioskAppUserModelId</span></span>|<span data-ttu-id="2bfd1-192">String</span><span class="sxs-lookup"><span data-stu-id="2bfd1-192">String</span></span>|<span data-ttu-id="2bfd1-193">Определяет идентификатор пользовательской модели для приложения, используемого с ограниченным доступом.</span><span class="sxs-lookup"><span data-stu-id="2bfd1-193">Specifies the application user model ID of the app to use with assigned access.</span></span>|
|<span data-ttu-id="2bfd1-194">maintenanceStartTime</span><span class="sxs-lookup"><span data-stu-id="2bfd1-194">maintenanceStartTime</span></span>|<span data-ttu-id="2bfd1-195">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="2bfd1-195">TimeOfDay</span></span>|<span data-ttu-id="2bfd1-196">Указывает ежедневное время начала обслуживания.</span><span class="sxs-lookup"><span data-stu-id="2bfd1-196">Specifies the daily start time of maintenance hour.</span></span>|



## <a name="response"></a><span data-ttu-id="2bfd1-197">Отклик</span><span class="sxs-lookup"><span data-stu-id="2bfd1-197">Response</span></span>
<span data-ttu-id="2bfd1-198">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="2bfd1-198">If successful, this method returns a `200 OK` response code and an updated [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2bfd1-199">Пример</span><span class="sxs-lookup"><span data-stu-id="2bfd1-199">Example</span></span>

### <a name="request"></a><span data-ttu-id="2bfd1-200">Запрос</span><span class="sxs-lookup"><span data-stu-id="2bfd1-200">Request</span></span>
<span data-ttu-id="2bfd1-201">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2bfd1-201">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 860

{
  "@odata.type": "#microsoft.graph.sharedPCConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountManagerPolicy": {
    "@odata.type": "microsoft.graph.sharedPCAccountManagerPolicy",
    "accountDeletionPolicy": "diskSpaceThreshold",
    "cacheAccountsAboveDiskFreePercentage": 4,
    "inactiveThresholdDays": 5,
    "removeAccountsBelowDiskFreePercentage": 5
  },
  "allowedAccounts": "domain",
  "allowLocalStorage": true,
  "disableAccountManager": true,
  "disableEduPolicies": true,
  "disablePowerPolicies": true,
  "disableSignInOnResume": true,
  "enabled": true,
  "idleTimeBeforeSleepInSeconds": 12,
  "kioskAppDisplayName": "Kiosk App Display Name value",
  "kioskAppUserModelId": "Kiosk App User Model Id value",
  "maintenanceStartTime": "11:59:24.7240000"
}
```

### <a name="response"></a><span data-ttu-id="2bfd1-202">Отклик</span><span class="sxs-lookup"><span data-stu-id="2bfd1-202">Response</span></span>
<span data-ttu-id="2bfd1-p113">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2bfd1-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1032

{
  "@odata.type": "#microsoft.graph.sharedPCConfiguration",
  "id": "5206be3b-be3b-5206-3bbe-06523bbe0652",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountManagerPolicy": {
    "@odata.type": "microsoft.graph.sharedPCAccountManagerPolicy",
    "accountDeletionPolicy": "diskSpaceThreshold",
    "cacheAccountsAboveDiskFreePercentage": 4,
    "inactiveThresholdDays": 5,
    "removeAccountsBelowDiskFreePercentage": 5
  },
  "allowedAccounts": "domain",
  "allowLocalStorage": true,
  "disableAccountManager": true,
  "disableEduPolicies": true,
  "disablePowerPolicies": true,
  "disableSignInOnResume": true,
  "enabled": true,
  "idleTimeBeforeSleepInSeconds": 12,
  "kioskAppDisplayName": "Kiosk App Display Name value",
  "kioskAppUserModelId": "Kiosk App User Model Id value",
  "maintenanceStartTime": "11:59:24.7240000"
}
```









