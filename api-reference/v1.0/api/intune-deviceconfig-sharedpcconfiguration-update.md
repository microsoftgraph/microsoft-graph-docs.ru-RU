---
title: Обновление объекта sharedPCConfiguration
description: Обновляет свойства объекта sharedPCConfiguration.
ms.openlocfilehash: b18ebcf49af71ae77d21d2fd2d9d0a9b97d27eae
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027080"
---
# <a name="update-sharedpcconfiguration"></a><span data-ttu-id="4ed9a-103">Обновление объекта sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="4ed9a-103">Update sharedPCConfiguration</span></span>

> <span data-ttu-id="4ed9a-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4ed9a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4ed9a-105">Обновляет свойства объекта [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4ed9a-105">Update the properties of a [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4ed9a-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4ed9a-106">Prerequisites</span></span>
<span data-ttu-id="4ed9a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ed9a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ed9a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4ed9a-109">Permission type</span></span>|<span data-ttu-id="4ed9a-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4ed9a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ed9a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4ed9a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4ed9a-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ed9a-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4ed9a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4ed9a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ed9a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ed9a-114">Not supported.</span></span>|
|<span data-ttu-id="4ed9a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4ed9a-115">Application</span></span>|<span data-ttu-id="4ed9a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ed9a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ed9a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4ed9a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="4ed9a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4ed9a-118">Request headers</span></span>
|<span data-ttu-id="4ed9a-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4ed9a-119">Header</span></span>|<span data-ttu-id="4ed9a-120">Значение</span><span class="sxs-lookup"><span data-stu-id="4ed9a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4ed9a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ed9a-121">Authorization</span></span>|<span data-ttu-id="4ed9a-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4ed9a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4ed9a-123">Accept</span><span class="sxs-lookup"><span data-stu-id="4ed9a-123">Accept</span></span>|<span data-ttu-id="4ed9a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4ed9a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ed9a-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4ed9a-125">Request body</span></span>
<span data-ttu-id="4ed9a-126">В теле запроса добавьте представление объекта [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4ed9a-126">In the request body, supply a JSON representation for the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

<span data-ttu-id="4ed9a-127">Ниже показаны свойства, которые необходимо указывать при создании объекта [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4ed9a-127">The following table shows the properties that are required when you create the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span></span>

|<span data-ttu-id="4ed9a-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="4ed9a-128">Property</span></span>|<span data-ttu-id="4ed9a-129">Тип</span><span class="sxs-lookup"><span data-stu-id="4ed9a-129">Type</span></span>|<span data-ttu-id="4ed9a-130">Описание</span><span class="sxs-lookup"><span data-stu-id="4ed9a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ed9a-131">id</span><span class="sxs-lookup"><span data-stu-id="4ed9a-131">id</span></span>|<span data-ttu-id="4ed9a-132">String</span><span class="sxs-lookup"><span data-stu-id="4ed9a-132">String</span></span>|<span data-ttu-id="4ed9a-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4ed9a-133">Key of the entity.</span></span> <span data-ttu-id="4ed9a-134">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4ed9a-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ed9a-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4ed9a-135">lastModifiedDateTime</span></span>|<span data-ttu-id="4ed9a-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ed9a-136">DateTimeOffset</span></span>|<span data-ttu-id="4ed9a-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="4ed9a-137">DateTime the object was last modified.</span></span> <span data-ttu-id="4ed9a-138">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4ed9a-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ed9a-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4ed9a-139">createdDateTime</span></span>|<span data-ttu-id="4ed9a-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ed9a-140">DateTimeOffset</span></span>|<span data-ttu-id="4ed9a-141">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="4ed9a-141">DateTime the object was created.</span></span> <span data-ttu-id="4ed9a-142">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4ed9a-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ed9a-143">описание</span><span class="sxs-lookup"><span data-stu-id="4ed9a-143">description</span></span>|<span data-ttu-id="4ed9a-144">String</span><span class="sxs-lookup"><span data-stu-id="4ed9a-144">String</span></span>|<span data-ttu-id="4ed9a-145">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4ed9a-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4ed9a-146">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4ed9a-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ed9a-147">displayName</span><span class="sxs-lookup"><span data-stu-id="4ed9a-147">displayName</span></span>|<span data-ttu-id="4ed9a-148">String</span><span class="sxs-lookup"><span data-stu-id="4ed9a-148">String</span></span>|<span data-ttu-id="4ed9a-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4ed9a-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4ed9a-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4ed9a-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ed9a-151">version</span><span class="sxs-lookup"><span data-stu-id="4ed9a-151">version</span></span>|<span data-ttu-id="4ed9a-152">Int32</span><span class="sxs-lookup"><span data-stu-id="4ed9a-152">Int32</span></span>|<span data-ttu-id="4ed9a-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4ed9a-153">Version of the device configuration.</span></span> <span data-ttu-id="4ed9a-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ed9a-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ed9a-155">accountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="4ed9a-155">accountManagerPolicy</span></span>|[<span data-ttu-id="4ed9a-156">sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="4ed9a-156">sharedPCAccountManagerPolicy</span></span>](../resources/intune-deviceconfig-sharedpcaccountmanagerpolicy.md)|<span data-ttu-id="4ed9a-157">Задает способ управления учетными записями на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="4ed9a-157">Specifies how accounts are managed on a shared PC.</span></span> <span data-ttu-id="4ed9a-158">Применяется, только если для параметра disableAccountManager задано значение false.</span><span class="sxs-lookup"><span data-stu-id="4ed9a-158">Only applies when disableAccountManager is false.</span></span>|
|<span data-ttu-id="4ed9a-159">allowedAccounts</span><span class="sxs-lookup"><span data-stu-id="4ed9a-159">allowedAccounts</span></span>|[<span data-ttu-id="4ed9a-160">sharedPCAllowedAccountType</span><span class="sxs-lookup"><span data-stu-id="4ed9a-160">sharedPCAllowedAccountType</span></span>](../resources/intune-deviceconfig-sharedpcallowedaccounttype.md)|<span data-ttu-id="4ed9a-161">Указывает тип учетных записей, которые можно использовать на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="4ed9a-161">Indicates which type of accounts are allowed to use on a shared PC.</span></span> <span data-ttu-id="4ed9a-162">Возможные значения: `guest`, `domain`.</span><span class="sxs-lookup"><span data-stu-id="4ed9a-162">Possible values are: `guest`, `domain`.</span></span>|
|<span data-ttu-id="4ed9a-163">allowLocalStorage</span><span class="sxs-lookup"><span data-stu-id="4ed9a-163">allowLocalStorage</span></span>|<span data-ttu-id="4ed9a-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ed9a-164">Boolean</span></span>|<span data-ttu-id="4ed9a-165">Указывает, можно ли разместить локальное хранилище на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="4ed9a-165">Specifies whether local storage is allowed on a shared PC.</span></span>|
|<span data-ttu-id="4ed9a-166">disableAccountManager</span><span class="sxs-lookup"><span data-stu-id="4ed9a-166">disableAccountManager</span></span>|<span data-ttu-id="4ed9a-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ed9a-167">Boolean</span></span>|<span data-ttu-id="4ed9a-168">Отключает диспетчер учетных записей в режиме совместного использования компьютера.</span><span class="sxs-lookup"><span data-stu-id="4ed9a-168">Disables the account manager for shared PC mode.</span></span>|
|<span data-ttu-id="4ed9a-169">disableEduPolicies</span><span class="sxs-lookup"><span data-stu-id="4ed9a-169">disableEduPolicies</span></span>|<span data-ttu-id="4ed9a-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ed9a-170">Boolean</span></span>|<span data-ttu-id="4ed9a-171">Указывает, следует ли отключить стандартные политики среды совместного использования компьютера для образования.</span><span class="sxs-lookup"><span data-stu-id="4ed9a-171">Specifies whether the default shared PC education environment policies should be disabled.</span></span> <span data-ttu-id="4ed9a-172">Для Windows 10 RS2 и более поздних версий эта политика будет применяться без установки значения True для параметра Enabled.</span><span class="sxs-lookup"><span data-stu-id="4ed9a-172">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span>|
|<span data-ttu-id="4ed9a-173">disablePowerPolicies</span><span class="sxs-lookup"><span data-stu-id="4ed9a-173">disablePowerPolicies</span></span>|<span data-ttu-id="4ed9a-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ed9a-174">Boolean</span></span>|<span data-ttu-id="4ed9a-175">Указывает, следует ли отключить стандартные политики электропитания для общего компьютера.</span><span class="sxs-lookup"><span data-stu-id="4ed9a-175">Specifies whether the default shared PC power policies should be disabled.</span></span>|
|<span data-ttu-id="4ed9a-176">disableSignInOnResume</span><span class="sxs-lookup"><span data-stu-id="4ed9a-176">disableSignInOnResume</span></span>|<span data-ttu-id="4ed9a-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ed9a-177">Boolean</span></span>|<span data-ttu-id="4ed9a-178">Отключает обязательный вход в систему при выходе устройства из спящего режима.</span><span class="sxs-lookup"><span data-stu-id="4ed9a-178">Disables the requirement to sign in whenever the device wakes up from sleep mode.</span></span>|
|<span data-ttu-id="4ed9a-179">enabled</span><span class="sxs-lookup"><span data-stu-id="4ed9a-179">enabled</span></span>|<span data-ttu-id="4ed9a-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ed9a-180">Boolean</span></span>|<span data-ttu-id="4ed9a-181">Включает режим общего компьютера и применяет политики совместного использования ПК.</span><span class="sxs-lookup"><span data-stu-id="4ed9a-181">Enables shared PC mode and applies the shared pc policies.</span></span>|
|<span data-ttu-id="4ed9a-182">idleTimeBeforeSleepInSeconds</span><span class="sxs-lookup"><span data-stu-id="4ed9a-182">idleTimeBeforeSleepInSeconds</span></span>|<span data-ttu-id="4ed9a-183">Int32</span><span class="sxs-lookup"><span data-stu-id="4ed9a-183">Int32</span></span>|<span data-ttu-id="4ed9a-184">Определяет длительность (в секундах) простоя устройства перед переходом в спящий режим.</span><span class="sxs-lookup"><span data-stu-id="4ed9a-184">Specifies the time in seconds that a device must sit idle before the PC goes to sleep.</span></span> <span data-ttu-id="4ed9a-185">Если задать значение 0, переход в спящий режим отключается.</span><span class="sxs-lookup"><span data-stu-id="4ed9a-185">Setting this value to 0 prevents the sleep timeout from occurring.</span></span>|
|<span data-ttu-id="4ed9a-186">kioskAppDisplayName</span><span class="sxs-lookup"><span data-stu-id="4ed9a-186">kioskAppDisplayName</span></span>|<span data-ttu-id="4ed9a-187">String</span><span class="sxs-lookup"><span data-stu-id="4ed9a-187">String</span></span>|<span data-ttu-id="4ed9a-188">Задает текст для учетной записи, который отображается на экране входа в систему и используется для запуска приложения, указанного в свойстве SetKioskAppUserModelId.</span><span class="sxs-lookup"><span data-stu-id="4ed9a-188">Specifies the display text for the account shown on the sign-in screen which launches the app specified by SetKioskAppUserModelId.</span></span> <span data-ttu-id="4ed9a-189">Применяется, только если задано свойство KioskAppUserModelId.</span><span class="sxs-lookup"><span data-stu-id="4ed9a-189">Only applies when KioskAppUserModelId is set.</span></span>|
|<span data-ttu-id="4ed9a-190">kioskAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="4ed9a-190">kioskAppUserModelId</span></span>|<span data-ttu-id="4ed9a-191">String</span><span class="sxs-lookup"><span data-stu-id="4ed9a-191">String</span></span>|<span data-ttu-id="4ed9a-192">Задает ИД пользовательской модели для приложения, используемый с ограниченным доступом.</span><span class="sxs-lookup"><span data-stu-id="4ed9a-192">Specifies the application user model ID of the app to use with assigned access.</span></span>|
|<span data-ttu-id="4ed9a-193">maintenanceStartTime</span><span class="sxs-lookup"><span data-stu-id="4ed9a-193">maintenanceStartTime</span></span>|<span data-ttu-id="4ed9a-194">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="4ed9a-194">TimeOfDay</span></span>|<span data-ttu-id="4ed9a-195">Задает ежедневное время начала обслуживания.</span><span class="sxs-lookup"><span data-stu-id="4ed9a-195">Specifies the daily start time of maintenance hour.</span></span>|



## <a name="response"></a><span data-ttu-id="4ed9a-196">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ed9a-196">Response</span></span>
<span data-ttu-id="4ed9a-197">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4ed9a-197">If successful, this method returns a `200 OK` response code and an updated [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ed9a-198">Пример</span><span class="sxs-lookup"><span data-stu-id="4ed9a-198">Example</span></span>
### <a name="request"></a><span data-ttu-id="4ed9a-199">Запрос</span><span class="sxs-lookup"><span data-stu-id="4ed9a-199">Request</span></span>
<span data-ttu-id="4ed9a-200">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4ed9a-200">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4ed9a-201">Ответ</span><span class="sxs-lookup"><span data-stu-id="4ed9a-201">Response</span></span>
<span data-ttu-id="4ed9a-p113">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="4ed9a-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



