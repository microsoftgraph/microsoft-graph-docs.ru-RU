---
title: Создание Адванцедсреатпротектиононбоардингдевицесеттингстате
description: Создание нового объекта Адванцедсреатпротектиононбоардингдевицесеттингстате.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 576ac7eaf5e44cdd3539c1d4a281c3612880e733
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793152"
---
# <a name="create-advancedthreatprotectiononboardingdevicesettingstate"></a><span data-ttu-id="bd4c0-103">Создание Адванцедсреатпротектиононбоардингдевицесеттингстате</span><span class="sxs-lookup"><span data-stu-id="bd4c0-103">Create advancedThreatProtectionOnboardingDeviceSettingState</span></span>

<span data-ttu-id="bd4c0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd4c0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bd4c0-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd4c0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bd4c0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bd4c0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd4c0-107">Создание нового объекта [адванцедсреатпротектиононбоардингдевицесеттингстате](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) .</span><span class="sxs-lookup"><span data-stu-id="bd4c0-107">Create a new [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bd4c0-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bd4c0-108">Prerequisites</span></span>
<span data-ttu-id="bd4c0-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="bd4c0-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="bd4c0-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd4c0-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd4c0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bd4c0-111">Permission type</span></span>|<span data-ttu-id="bd4c0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bd4c0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bd4c0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bd4c0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bd4c0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd4c0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bd4c0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bd4c0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bd4c0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd4c0-116">Not supported.</span></span>|
|<span data-ttu-id="bd4c0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bd4c0-117">Application</span></span>|<span data-ttu-id="bd4c0-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd4c0-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bd4c0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bd4c0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="bd4c0-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bd4c0-120">Request headers</span></span>
|<span data-ttu-id="bd4c0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bd4c0-121">Header</span></span>|<span data-ttu-id="bd4c0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="bd4c0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bd4c0-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bd4c0-123">Authorization</span></span>|<span data-ttu-id="bd4c0-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bd4c0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bd4c0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bd4c0-125">Accept</span></span>|<span data-ttu-id="bd4c0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bd4c0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd4c0-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bd4c0-127">Request body</span></span>
<span data-ttu-id="bd4c0-128">В тексте запроса добавьте представление объекта Адванцедсреатпротектиононбоардингдевицесеттингстате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bd4c0-128">In the request body, supply a JSON representation for the advancedThreatProtectionOnboardingDeviceSettingState object.</span></span>

<span data-ttu-id="bd4c0-129">В следующей таблице приведены свойства, необходимые при создании Адванцедсреатпротектиононбоардингдевицесеттингстате.</span><span class="sxs-lookup"><span data-stu-id="bd4c0-129">The following table shows the properties that are required when you create the advancedThreatProtectionOnboardingDeviceSettingState.</span></span>

|<span data-ttu-id="bd4c0-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="bd4c0-130">Property</span></span>|<span data-ttu-id="bd4c0-131">Тип</span><span class="sxs-lookup"><span data-stu-id="bd4c0-131">Type</span></span>|<span data-ttu-id="bd4c0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="bd4c0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd4c0-133">id</span><span class="sxs-lookup"><span data-stu-id="bd4c0-133">id</span></span>|<span data-ttu-id="bd4c0-134">Строка</span><span class="sxs-lookup"><span data-stu-id="bd4c0-134">String</span></span>|<span data-ttu-id="bd4c0-135">Ключ объекта</span><span class="sxs-lookup"><span data-stu-id="bd4c0-135">Key of the entity</span></span>|
|<span data-ttu-id="bd4c0-136">platformType</span><span class="sxs-lookup"><span data-stu-id="bd4c0-136">platformType</span></span>|[<span data-ttu-id="bd4c0-137">deviceType</span><span class="sxs-lookup"><span data-stu-id="bd4c0-137">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="bd4c0-138">Тип платформы устройства.</span><span class="sxs-lookup"><span data-stu-id="bd4c0-138">Device platform type.</span></span> <span data-ttu-id="bd4c0-139">Возможные значения:,,,,,,,,,,, `desktop` `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` , `unix` , `macMDM` , `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `blackberry` `palm` `unknown` ,,,,,,,,,,,,,,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="bd4c0-139">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `androidnGMS`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="bd4c0-140">setting</span><span class="sxs-lookup"><span data-stu-id="bd4c0-140">setting</span></span>|<span data-ttu-id="bd4c0-141">String</span><span class="sxs-lookup"><span data-stu-id="bd4c0-141">String</span></span>|<span data-ttu-id="bd4c0-142">Имя класса параметров и свойства.</span><span class="sxs-lookup"><span data-stu-id="bd4c0-142">The setting class name and property name.</span></span>|
|<span data-ttu-id="bd4c0-143">settingName</span><span class="sxs-lookup"><span data-stu-id="bd4c0-143">settingName</span></span>|<span data-ttu-id="bd4c0-144">String</span><span class="sxs-lookup"><span data-stu-id="bd4c0-144">String</span></span>|<span data-ttu-id="bd4c0-145">Имя параметра в отчете</span><span class="sxs-lookup"><span data-stu-id="bd4c0-145">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="bd4c0-146">deviceId</span><span class="sxs-lookup"><span data-stu-id="bd4c0-146">deviceId</span></span>|<span data-ttu-id="bd4c0-147">String</span><span class="sxs-lookup"><span data-stu-id="bd4c0-147">String</span></span>|<span data-ttu-id="bd4c0-148">ИД устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="bd4c0-148">The Device Id that is being reported</span></span>|
|<span data-ttu-id="bd4c0-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="bd4c0-149">deviceName</span></span>|<span data-ttu-id="bd4c0-150">String</span><span class="sxs-lookup"><span data-stu-id="bd4c0-150">String</span></span>|<span data-ttu-id="bd4c0-151">Имя устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="bd4c0-151">The Device Name that is being reported</span></span>|
|<span data-ttu-id="bd4c0-152">userId</span><span class="sxs-lookup"><span data-stu-id="bd4c0-152">userId</span></span>|<span data-ttu-id="bd4c0-153">String</span><span class="sxs-lookup"><span data-stu-id="bd4c0-153">String</span></span>|<span data-ttu-id="bd4c0-154">ИД пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="bd4c0-154">The user Id that is being reported</span></span>|
|<span data-ttu-id="bd4c0-155">userEmail</span><span class="sxs-lookup"><span data-stu-id="bd4c0-155">userEmail</span></span>|<span data-ttu-id="bd4c0-156">String</span><span class="sxs-lookup"><span data-stu-id="bd4c0-156">String</span></span>|<span data-ttu-id="bd4c0-157">Электронный адрес пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="bd4c0-157">The User email address that is being reported</span></span>|
|<span data-ttu-id="bd4c0-158">userName</span><span class="sxs-lookup"><span data-stu-id="bd4c0-158">userName</span></span>|<span data-ttu-id="bd4c0-159">String</span><span class="sxs-lookup"><span data-stu-id="bd4c0-159">String</span></span>|<span data-ttu-id="bd4c0-160">Имя пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="bd4c0-160">The User Name that is being reported</span></span>|
|<span data-ttu-id="bd4c0-161">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="bd4c0-161">userPrincipalName</span></span>|<span data-ttu-id="bd4c0-162">String</span><span class="sxs-lookup"><span data-stu-id="bd4c0-162">String</span></span>|<span data-ttu-id="bd4c0-163">Имя участника-пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="bd4c0-163">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="bd4c0-164">deviceModel</span><span class="sxs-lookup"><span data-stu-id="bd4c0-164">deviceModel</span></span>|<span data-ttu-id="bd4c0-165">String</span><span class="sxs-lookup"><span data-stu-id="bd4c0-165">String</span></span>|<span data-ttu-id="bd4c0-166">Модель устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="bd4c0-166">The device model that is being reported</span></span>|
|<span data-ttu-id="bd4c0-167">state</span><span class="sxs-lookup"><span data-stu-id="bd4c0-167">state</span></span>|[<span data-ttu-id="bd4c0-168">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="bd4c0-168">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="bd4c0-169">Состояние соответствия для параметра.</span><span class="sxs-lookup"><span data-stu-id="bd4c0-169">The compliance state of the setting.</span></span> <span data-ttu-id="bd4c0-170">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="bd4c0-170">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="bd4c0-171">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="bd4c0-171">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="bd4c0-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd4c0-172">DateTimeOffset</span></span>|<span data-ttu-id="bd4c0-173">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="bd4c0-173">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="bd4c0-174">Ответ</span><span class="sxs-lookup"><span data-stu-id="bd4c0-174">Response</span></span>
<span data-ttu-id="bd4c0-175">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [адванцедсреатпротектиононбоардингдевицесеттингстате](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bd4c0-175">If successful, this method returns a `201 Created` response code and a [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd4c0-176">Пример</span><span class="sxs-lookup"><span data-stu-id="bd4c0-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="bd4c0-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="bd4c0-177">Request</span></span>
<span data-ttu-id="bd4c0-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bd4c0-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates
Content-type: application/json
Content-length: 573

{
  "@odata.type": "#microsoft.graph.advancedThreatProtectionOnboardingDeviceSettingState",
  "platformType": "windowsRT",
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "deviceId": "Device Id value",
  "deviceName": "Device Name value",
  "userId": "User Id value",
  "userEmail": "User Email value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "deviceModel": "Device Model value",
  "state": "notApplicable",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00"
}
```

### <a name="response"></a><span data-ttu-id="bd4c0-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd4c0-179">Response</span></span>
<span data-ttu-id="bd4c0-180">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="bd4c0-180">Here is an example of the response.</span></span> <span data-ttu-id="bd4c0-181">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="bd4c0-181">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="bd4c0-182">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="bd4c0-182">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 622

{
  "@odata.type": "#microsoft.graph.advancedThreatProtectionOnboardingDeviceSettingState",
  "id": "63593fc6-3fc6-6359-c63f-5963c63f5963",
  "platformType": "windowsRT",
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "deviceId": "Device Id value",
  "deviceName": "Device Name value",
  "userId": "User Id value",
  "userEmail": "User Email value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "deviceModel": "Device Model value",
  "state": "notApplicable",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00"
}
```



