---
title: Обновление объекта sharedPCConfiguration
description: Обновляет свойства объекта sharedPCConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2163ae07a30d1a5c3dca616956fedce76ea6e96c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32558232"
---
# <a name="update-sharedpcconfiguration"></a><span data-ttu-id="029dc-103">Обновление объекта sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="029dc-103">Update sharedPCConfiguration</span></span>

> <span data-ttu-id="029dc-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="029dc-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="029dc-105">Обновляет свойства объекта [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="029dc-105">Update the properties of a [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="029dc-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="029dc-106">Prerequisites</span></span>
<span data-ttu-id="029dc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="029dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="029dc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="029dc-109">Permission type</span></span>|<span data-ttu-id="029dc-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="029dc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="029dc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="029dc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="029dc-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="029dc-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="029dc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="029dc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="029dc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="029dc-114">Not supported.</span></span>|
|<span data-ttu-id="029dc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="029dc-115">Application</span></span>|<span data-ttu-id="029dc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="029dc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="029dc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="029dc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="029dc-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="029dc-118">Request headers</span></span>
|<span data-ttu-id="029dc-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="029dc-119">Header</span></span>|<span data-ttu-id="029dc-120">Значение</span><span class="sxs-lookup"><span data-stu-id="029dc-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="029dc-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="029dc-121">Authorization</span></span>|<span data-ttu-id="029dc-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="029dc-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="029dc-123">Accept</span><span class="sxs-lookup"><span data-stu-id="029dc-123">Accept</span></span>|<span data-ttu-id="029dc-124">application/json</span><span class="sxs-lookup"><span data-stu-id="029dc-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="029dc-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="029dc-125">Request body</span></span>
<span data-ttu-id="029dc-126">В теле запроса добавьте представление объекта [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="029dc-126">In the request body, supply a JSON representation for the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

<span data-ttu-id="029dc-127">Ниже показаны свойства, которые необходимо указывать при создании объекта [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="029dc-127">The following table shows the properties that are required when you create the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span></span>

|<span data-ttu-id="029dc-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="029dc-128">Property</span></span>|<span data-ttu-id="029dc-129">Тип</span><span class="sxs-lookup"><span data-stu-id="029dc-129">Type</span></span>|<span data-ttu-id="029dc-130">Описание</span><span class="sxs-lookup"><span data-stu-id="029dc-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="029dc-131">id</span><span class="sxs-lookup"><span data-stu-id="029dc-131">id</span></span>|<span data-ttu-id="029dc-132">Строка</span><span class="sxs-lookup"><span data-stu-id="029dc-132">String</span></span>|<span data-ttu-id="029dc-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="029dc-133">Key of the entity.</span></span> <span data-ttu-id="029dc-134">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="029dc-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="029dc-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="029dc-135">lastModifiedDateTime</span></span>|<span data-ttu-id="029dc-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="029dc-136">DateTimeOffset</span></span>|<span data-ttu-id="029dc-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="029dc-137">DateTime the object was last modified.</span></span> <span data-ttu-id="029dc-138">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="029dc-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="029dc-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="029dc-139">createdDateTime</span></span>|<span data-ttu-id="029dc-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="029dc-140">DateTimeOffset</span></span>|<span data-ttu-id="029dc-141">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="029dc-141">DateTime the object was created.</span></span> <span data-ttu-id="029dc-142">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="029dc-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="029dc-143">description</span><span class="sxs-lookup"><span data-stu-id="029dc-143">description</span></span>|<span data-ttu-id="029dc-144">String</span><span class="sxs-lookup"><span data-stu-id="029dc-144">String</span></span>|<span data-ttu-id="029dc-145">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="029dc-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="029dc-146">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="029dc-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="029dc-147">displayName</span><span class="sxs-lookup"><span data-stu-id="029dc-147">displayName</span></span>|<span data-ttu-id="029dc-148">Строка</span><span class="sxs-lookup"><span data-stu-id="029dc-148">String</span></span>|<span data-ttu-id="029dc-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="029dc-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="029dc-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="029dc-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="029dc-151">version</span><span class="sxs-lookup"><span data-stu-id="029dc-151">version</span></span>|<span data-ttu-id="029dc-152">Int32</span><span class="sxs-lookup"><span data-stu-id="029dc-152">Int32</span></span>|<span data-ttu-id="029dc-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="029dc-153">Version of the device configuration.</span></span> <span data-ttu-id="029dc-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="029dc-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="029dc-155">accountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="029dc-155">accountManagerPolicy</span></span>|[<span data-ttu-id="029dc-156">sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="029dc-156">sharedPCAccountManagerPolicy</span></span>](../resources/intune-deviceconfig-sharedpcaccountmanagerpolicy.md)|<span data-ttu-id="029dc-157">Определяет способ управления учетными записями на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="029dc-157">Specifies how accounts are managed on a shared PC.</span></span> <span data-ttu-id="029dc-158">Применяется, только если для параметра disableAccountManager установлено значение false.</span><span class="sxs-lookup"><span data-stu-id="029dc-158">Only applies when disableAccountManager is false.</span></span>|
|<span data-ttu-id="029dc-159">allowedAccounts</span><span class="sxs-lookup"><span data-stu-id="029dc-159">allowedAccounts</span></span>|[<span data-ttu-id="029dc-160">Шаредпкалловедаккаунттипе</span><span class="sxs-lookup"><span data-stu-id="029dc-160">sharedPCAllowedAccountType</span></span>](../resources/intune-deviceconfig-sharedpcallowedaccounttype.md)|<span data-ttu-id="029dc-161">Указывает тип учетных записей, которые можно использовать на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="029dc-161">Indicates which type of accounts are allowed to use on a shared PC.</span></span> <span data-ttu-id="029dc-162">Возможные значения: `guest`, `domain`.</span><span class="sxs-lookup"><span data-stu-id="029dc-162">Possible values are: `guest`, `domain`.</span></span>|
|<span data-ttu-id="029dc-163">allowLocalStorage</span><span class="sxs-lookup"><span data-stu-id="029dc-163">allowLocalStorage</span></span>|<span data-ttu-id="029dc-164">Логический</span><span class="sxs-lookup"><span data-stu-id="029dc-164">Boolean</span></span>|<span data-ttu-id="029dc-165">Определяет, разрешено ли на общем компьютере локальное хранилище.</span><span class="sxs-lookup"><span data-stu-id="029dc-165">Specifies whether local storage is allowed on a shared PC.</span></span>|
|<span data-ttu-id="029dc-166">disableAccountManager</span><span class="sxs-lookup"><span data-stu-id="029dc-166">disableAccountManager</span></span>|<span data-ttu-id="029dc-167">Логический</span><span class="sxs-lookup"><span data-stu-id="029dc-167">Boolean</span></span>|<span data-ttu-id="029dc-168">Отключает диспетчер учетных записей в режиме совместного использования компьютера.</span><span class="sxs-lookup"><span data-stu-id="029dc-168">Disables the account manager for shared PC mode.</span></span>|
|<span data-ttu-id="029dc-169">disableEduPolicies</span><span class="sxs-lookup"><span data-stu-id="029dc-169">disableEduPolicies</span></span>|<span data-ttu-id="029dc-170">Логический</span><span class="sxs-lookup"><span data-stu-id="029dc-170">Boolean</span></span>|<span data-ttu-id="029dc-171">Указывает, следует ли отключить стандартные политики среды совместного использования компьютера для образования.</span><span class="sxs-lookup"><span data-stu-id="029dc-171">Specifies whether the default shared PC education environment policies should be disabled.</span></span> <span data-ttu-id="029dc-172">Для Windows 10 RS2 и более поздних версий эта политика будет применяться без установки значения True для параметра Enabled.</span><span class="sxs-lookup"><span data-stu-id="029dc-172">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span>|
|<span data-ttu-id="029dc-173">disablePowerPolicies</span><span class="sxs-lookup"><span data-stu-id="029dc-173">disablePowerPolicies</span></span>|<span data-ttu-id="029dc-174">Логический</span><span class="sxs-lookup"><span data-stu-id="029dc-174">Boolean</span></span>|<span data-ttu-id="029dc-175">Указывает, следует ли отключить стандартные политики электропитания для общего компьютера.</span><span class="sxs-lookup"><span data-stu-id="029dc-175">Specifies whether the default shared PC power policies should be disabled.</span></span>|
|<span data-ttu-id="029dc-176">disableSignInOnResume</span><span class="sxs-lookup"><span data-stu-id="029dc-176">disableSignInOnResume</span></span>|<span data-ttu-id="029dc-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="029dc-177">Boolean</span></span>|<span data-ttu-id="029dc-178">Отключает обязательный вход в систему при выходе устройства из спящего режима.</span><span class="sxs-lookup"><span data-stu-id="029dc-178">Disables the requirement to sign in whenever the device wakes up from sleep mode.</span></span>|
|<span data-ttu-id="029dc-179">enabled</span><span class="sxs-lookup"><span data-stu-id="029dc-179">enabled</span></span>|<span data-ttu-id="029dc-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="029dc-180">Boolean</span></span>|<span data-ttu-id="029dc-181">Включает режим общего компьютера и применяет политики совместного использования ПК.</span><span class="sxs-lookup"><span data-stu-id="029dc-181">Enables shared PC mode and applies the shared pc policies.</span></span>|
|<span data-ttu-id="029dc-182">idleTimeBeforeSleepInSeconds</span><span class="sxs-lookup"><span data-stu-id="029dc-182">idleTimeBeforeSleepInSeconds</span></span>|<span data-ttu-id="029dc-183">Int32</span><span class="sxs-lookup"><span data-stu-id="029dc-183">Int32</span></span>|<span data-ttu-id="029dc-184">Определяет длительность (в секундах) пребывания устройства в режиме бездействия перед переходом в спящий режим.</span><span class="sxs-lookup"><span data-stu-id="029dc-184">Specifies the time in seconds that a device must sit idle before the PC goes to sleep.</span></span> <span data-ttu-id="029dc-185">Если задать значение 0, переход в спящий режим отключается.</span><span class="sxs-lookup"><span data-stu-id="029dc-185">Setting this value to 0 prevents the sleep timeout from occurring.</span></span>|
|<span data-ttu-id="029dc-186">kioskAppDisplayName</span><span class="sxs-lookup"><span data-stu-id="029dc-186">kioskAppDisplayName</span></span>|<span data-ttu-id="029dc-187">String</span><span class="sxs-lookup"><span data-stu-id="029dc-187">String</span></span>|<span data-ttu-id="029dc-188">Задает текст для учетной записи, который отображается на экране входа в систему и используется для запуска приложения, определяемого с помощью свойства SetKioskAppUserModelId.</span><span class="sxs-lookup"><span data-stu-id="029dc-188">Specifies the display text for the account shown on the sign-in screen which launches the app specified by SetKioskAppUserModelId.</span></span> <span data-ttu-id="029dc-189">Применяется, только если задано свойство KioskAppUserModelId.</span><span class="sxs-lookup"><span data-stu-id="029dc-189">Only applies when KioskAppUserModelId is set.</span></span>|
|<span data-ttu-id="029dc-190">kioskAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="029dc-190">kioskAppUserModelId</span></span>|<span data-ttu-id="029dc-191">String</span><span class="sxs-lookup"><span data-stu-id="029dc-191">String</span></span>|<span data-ttu-id="029dc-192">Определяет идентификатор пользовательской модели для приложения, используемого с ограниченным доступом.</span><span class="sxs-lookup"><span data-stu-id="029dc-192">Specifies the application user model ID of the app to use with assigned access.</span></span>|
|<span data-ttu-id="029dc-193">maintenanceStartTime</span><span class="sxs-lookup"><span data-stu-id="029dc-193">maintenanceStartTime</span></span>|<span data-ttu-id="029dc-194">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="029dc-194">TimeOfDay</span></span>|<span data-ttu-id="029dc-195">Указывает ежедневное время начала обслуживания.</span><span class="sxs-lookup"><span data-stu-id="029dc-195">Specifies the daily start time of maintenance hour.</span></span>|



## <a name="response"></a><span data-ttu-id="029dc-196">Отклик</span><span class="sxs-lookup"><span data-stu-id="029dc-196">Response</span></span>
<span data-ttu-id="029dc-197">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="029dc-197">If successful, this method returns a `200 OK` response code and an updated [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="029dc-198">Пример</span><span class="sxs-lookup"><span data-stu-id="029dc-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="029dc-199">Запрос</span><span class="sxs-lookup"><span data-stu-id="029dc-199">Request</span></span>
<span data-ttu-id="029dc-200">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="029dc-200">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="029dc-201">Отклик</span><span class="sxs-lookup"><span data-stu-id="029dc-201">Response</span></span>
<span data-ttu-id="029dc-p113">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="029dc-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



