---
title: Create sharedPCConfiguration
description: Создание объекта sharedPCConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8aa0d11513e7f66c910e4d8b8fe994e62c218df9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36017049"
---
# <a name="create-sharedpcconfiguration"></a><span data-ttu-id="f2b33-103">Create sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="f2b33-103">Create sharedPCConfiguration</span></span>

> <span data-ttu-id="f2b33-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f2b33-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2b33-105">Создание объекта [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f2b33-105">Create a new [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f2b33-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="f2b33-106">Prerequisites</span></span>
<span data-ttu-id="f2b33-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2b33-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2b33-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f2b33-109">Permission type</span></span>|<span data-ttu-id="f2b33-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f2b33-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2b33-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f2b33-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f2b33-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2b33-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f2b33-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f2b33-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2b33-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2b33-114">Not supported.</span></span>|
|<span data-ttu-id="f2b33-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f2b33-115">Application</span></span>|<span data-ttu-id="f2b33-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2b33-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2b33-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f2b33-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f2b33-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f2b33-118">Request headers</span></span>
|<span data-ttu-id="f2b33-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f2b33-119">Header</span></span>|<span data-ttu-id="f2b33-120">Значение</span><span class="sxs-lookup"><span data-stu-id="f2b33-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2b33-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f2b33-121">Authorization</span></span>|<span data-ttu-id="f2b33-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f2b33-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2b33-123">Accept</span><span class="sxs-lookup"><span data-stu-id="f2b33-123">Accept</span></span>|<span data-ttu-id="f2b33-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f2b33-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2b33-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f2b33-125">Request body</span></span>
<span data-ttu-id="f2b33-126">В тексте запроса добавьте представление объекта sharedPCConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f2b33-126">In the request body, supply a JSON representation for the sharedPCConfiguration object.</span></span>

<span data-ttu-id="f2b33-127">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта sharedPCConfiguration.</span><span class="sxs-lookup"><span data-stu-id="f2b33-127">The following table shows the properties that are required when you create the sharedPCConfiguration.</span></span>

|<span data-ttu-id="f2b33-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="f2b33-128">Property</span></span>|<span data-ttu-id="f2b33-129">Тип</span><span class="sxs-lookup"><span data-stu-id="f2b33-129">Type</span></span>|<span data-ttu-id="f2b33-130">Описание</span><span class="sxs-lookup"><span data-stu-id="f2b33-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2b33-131">id</span><span class="sxs-lookup"><span data-stu-id="f2b33-131">id</span></span>|<span data-ttu-id="f2b33-132">Строка</span><span class="sxs-lookup"><span data-stu-id="f2b33-132">String</span></span>|<span data-ttu-id="f2b33-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f2b33-133">Key of the entity.</span></span> <span data-ttu-id="f2b33-134">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f2b33-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2b33-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f2b33-135">lastModifiedDateTime</span></span>|<span data-ttu-id="f2b33-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2b33-136">DateTimeOffset</span></span>|<span data-ttu-id="f2b33-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f2b33-137">DateTime the object was last modified.</span></span> <span data-ttu-id="f2b33-138">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f2b33-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2b33-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f2b33-139">createdDateTime</span></span>|<span data-ttu-id="f2b33-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2b33-140">DateTimeOffset</span></span>|<span data-ttu-id="f2b33-141">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="f2b33-141">DateTime the object was created.</span></span> <span data-ttu-id="f2b33-142">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f2b33-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2b33-143">description</span><span class="sxs-lookup"><span data-stu-id="f2b33-143">description</span></span>|<span data-ttu-id="f2b33-144">String</span><span class="sxs-lookup"><span data-stu-id="f2b33-144">String</span></span>|<span data-ttu-id="f2b33-145">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f2b33-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f2b33-146">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f2b33-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2b33-147">displayName</span><span class="sxs-lookup"><span data-stu-id="f2b33-147">displayName</span></span>|<span data-ttu-id="f2b33-148">Строка</span><span class="sxs-lookup"><span data-stu-id="f2b33-148">String</span></span>|<span data-ttu-id="f2b33-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f2b33-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f2b33-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f2b33-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2b33-151">version</span><span class="sxs-lookup"><span data-stu-id="f2b33-151">version</span></span>|<span data-ttu-id="f2b33-152">Int32</span><span class="sxs-lookup"><span data-stu-id="f2b33-152">Int32</span></span>|<span data-ttu-id="f2b33-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f2b33-153">Version of the device configuration.</span></span> <span data-ttu-id="f2b33-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f2b33-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2b33-155">accountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="f2b33-155">accountManagerPolicy</span></span>|[<span data-ttu-id="f2b33-156">sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="f2b33-156">sharedPCAccountManagerPolicy</span></span>](../resources/intune-deviceconfig-sharedpcaccountmanagerpolicy.md)|<span data-ttu-id="f2b33-157">Определяет способ управления учетными записями на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="f2b33-157">Specifies how accounts are managed on a shared PC.</span></span> <span data-ttu-id="f2b33-158">Применяется, только если для параметра disableAccountManager установлено значение false.</span><span class="sxs-lookup"><span data-stu-id="f2b33-158">Only applies when disableAccountManager is false.</span></span>|
|<span data-ttu-id="f2b33-159">allowedAccounts</span><span class="sxs-lookup"><span data-stu-id="f2b33-159">allowedAccounts</span></span>|[<span data-ttu-id="f2b33-160">Шаредпкалловедаккаунттипе</span><span class="sxs-lookup"><span data-stu-id="f2b33-160">sharedPCAllowedAccountType</span></span>](../resources/intune-deviceconfig-sharedpcallowedaccounttype.md)|<span data-ttu-id="f2b33-161">Указывает тип учетных записей, которые можно использовать на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="f2b33-161">Indicates which type of accounts are allowed to use on a shared PC.</span></span> <span data-ttu-id="f2b33-162">Возможные значения: `guest`, `domain`.</span><span class="sxs-lookup"><span data-stu-id="f2b33-162">Possible values are: `guest`, `domain`.</span></span>|
|<span data-ttu-id="f2b33-163">allowLocalStorage</span><span class="sxs-lookup"><span data-stu-id="f2b33-163">allowLocalStorage</span></span>|<span data-ttu-id="f2b33-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="f2b33-164">Boolean</span></span>|<span data-ttu-id="f2b33-165">Определяет, разрешено ли на общем компьютере локальное хранилище.</span><span class="sxs-lookup"><span data-stu-id="f2b33-165">Specifies whether local storage is allowed on a shared PC.</span></span>|
|<span data-ttu-id="f2b33-166">disableAccountManager</span><span class="sxs-lookup"><span data-stu-id="f2b33-166">disableAccountManager</span></span>|<span data-ttu-id="f2b33-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="f2b33-167">Boolean</span></span>|<span data-ttu-id="f2b33-168">Отключает диспетчер учетных записей в режиме совместного использования компьютера.</span><span class="sxs-lookup"><span data-stu-id="f2b33-168">Disables the account manager for shared PC mode.</span></span>|
|<span data-ttu-id="f2b33-169">disableEduPolicies</span><span class="sxs-lookup"><span data-stu-id="f2b33-169">disableEduPolicies</span></span>|<span data-ttu-id="f2b33-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="f2b33-170">Boolean</span></span>|<span data-ttu-id="f2b33-171">Указывает, следует ли отключить стандартные политики среды совместного использования компьютера для образования.</span><span class="sxs-lookup"><span data-stu-id="f2b33-171">Specifies whether the default shared PC education environment policies should be disabled.</span></span> <span data-ttu-id="f2b33-172">Для Windows 10 RS2 и более поздних версий эта политика будет применяться без установки значения True для параметра Enabled.</span><span class="sxs-lookup"><span data-stu-id="f2b33-172">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span>|
|<span data-ttu-id="f2b33-173">disablePowerPolicies</span><span class="sxs-lookup"><span data-stu-id="f2b33-173">disablePowerPolicies</span></span>|<span data-ttu-id="f2b33-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="f2b33-174">Boolean</span></span>|<span data-ttu-id="f2b33-175">Указывает, следует ли отключить стандартные политики электропитания для общего компьютера.</span><span class="sxs-lookup"><span data-stu-id="f2b33-175">Specifies whether the default shared PC power policies should be disabled.</span></span>|
|<span data-ttu-id="f2b33-176">disableSignInOnResume</span><span class="sxs-lookup"><span data-stu-id="f2b33-176">disableSignInOnResume</span></span>|<span data-ttu-id="f2b33-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="f2b33-177">Boolean</span></span>|<span data-ttu-id="f2b33-178">Отключает обязательный вход в систему при выходе устройства из спящего режима.</span><span class="sxs-lookup"><span data-stu-id="f2b33-178">Disables the requirement to sign in whenever the device wakes up from sleep mode.</span></span>|
|<span data-ttu-id="f2b33-179">enabled</span><span class="sxs-lookup"><span data-stu-id="f2b33-179">enabled</span></span>|<span data-ttu-id="f2b33-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="f2b33-180">Boolean</span></span>|<span data-ttu-id="f2b33-181">Включает режим общего компьютера и применяет политики совместного использования ПК.</span><span class="sxs-lookup"><span data-stu-id="f2b33-181">Enables shared PC mode and applies the shared pc policies.</span></span>|
|<span data-ttu-id="f2b33-182">idleTimeBeforeSleepInSeconds</span><span class="sxs-lookup"><span data-stu-id="f2b33-182">idleTimeBeforeSleepInSeconds</span></span>|<span data-ttu-id="f2b33-183">Int32</span><span class="sxs-lookup"><span data-stu-id="f2b33-183">Int32</span></span>|<span data-ttu-id="f2b33-184">Определяет длительность (в секундах) пребывания устройства в режиме бездействия перед переходом в спящий режим.</span><span class="sxs-lookup"><span data-stu-id="f2b33-184">Specifies the time in seconds that a device must sit idle before the PC goes to sleep.</span></span> <span data-ttu-id="f2b33-185">Если задать значение 0, переход в спящий режим отключается.</span><span class="sxs-lookup"><span data-stu-id="f2b33-185">Setting this value to 0 prevents the sleep timeout from occurring.</span></span>|
|<span data-ttu-id="f2b33-186">kioskAppDisplayName</span><span class="sxs-lookup"><span data-stu-id="f2b33-186">kioskAppDisplayName</span></span>|<span data-ttu-id="f2b33-187">String</span><span class="sxs-lookup"><span data-stu-id="f2b33-187">String</span></span>|<span data-ttu-id="f2b33-188">Задает текст для учетной записи, который отображается на экране входа в систему и используется для запуска приложения, определяемого с помощью свойства SetKioskAppUserModelId.</span><span class="sxs-lookup"><span data-stu-id="f2b33-188">Specifies the display text for the account shown on the sign-in screen which launches the app specified by SetKioskAppUserModelId.</span></span> <span data-ttu-id="f2b33-189">Применяется, только если задано свойство KioskAppUserModelId.</span><span class="sxs-lookup"><span data-stu-id="f2b33-189">Only applies when KioskAppUserModelId is set.</span></span>|
|<span data-ttu-id="f2b33-190">kioskAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="f2b33-190">kioskAppUserModelId</span></span>|<span data-ttu-id="f2b33-191">String</span><span class="sxs-lookup"><span data-stu-id="f2b33-191">String</span></span>|<span data-ttu-id="f2b33-192">Определяет идентификатор пользовательской модели для приложения, используемого с ограниченным доступом.</span><span class="sxs-lookup"><span data-stu-id="f2b33-192">Specifies the application user model ID of the app to use with assigned access.</span></span>|
|<span data-ttu-id="f2b33-193">maintenanceStartTime</span><span class="sxs-lookup"><span data-stu-id="f2b33-193">maintenanceStartTime</span></span>|<span data-ttu-id="f2b33-194">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="f2b33-194">TimeOfDay</span></span>|<span data-ttu-id="f2b33-195">Указывает ежедневное время начала обслуживания.</span><span class="sxs-lookup"><span data-stu-id="f2b33-195">Specifies the daily start time of maintenance hour.</span></span>|



## <a name="response"></a><span data-ttu-id="f2b33-196">Ответ</span><span class="sxs-lookup"><span data-stu-id="f2b33-196">Response</span></span>
<span data-ttu-id="f2b33-197">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f2b33-197">If successful, this method returns a `201 Created` response code and a [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2b33-198">Пример</span><span class="sxs-lookup"><span data-stu-id="f2b33-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="f2b33-199">Запрос</span><span class="sxs-lookup"><span data-stu-id="f2b33-199">Request</span></span>
<span data-ttu-id="f2b33-200">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f2b33-200">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="f2b33-201">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2b33-201">Response</span></span>
<span data-ttu-id="f2b33-p113">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f2b33-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



