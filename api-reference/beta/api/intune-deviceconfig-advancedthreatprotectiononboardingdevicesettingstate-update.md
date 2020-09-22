---
title: Обновление Адванцедсреатпротектиононбоардингдевицесеттингстате
description: Обновление свойств объекта Адванцедсреатпротектиононбоардингдевицесеттингстате.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f92b46fa868f88db74a90fe6cbdba10db0913ef3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48032399"
---
# <a name="update-advancedthreatprotectiononboardingdevicesettingstate"></a><span data-ttu-id="9d47d-103">Обновление Адванцедсреатпротектиононбоардингдевицесеттингстате</span><span class="sxs-lookup"><span data-stu-id="9d47d-103">Update advancedThreatProtectionOnboardingDeviceSettingState</span></span>

<span data-ttu-id="9d47d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d47d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9d47d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d47d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9d47d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9d47d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d47d-107">Обновление свойств объекта [адванцедсреатпротектиононбоардингдевицесеттингстате](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) .</span><span class="sxs-lookup"><span data-stu-id="9d47d-107">Update the properties of a [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9d47d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9d47d-108">Prerequisites</span></span>
<span data-ttu-id="9d47d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d47d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d47d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9d47d-111">Permission type</span></span>|<span data-ttu-id="9d47d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9d47d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9d47d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9d47d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9d47d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d47d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9d47d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9d47d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9d47d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d47d-116">Not supported.</span></span>|
|<span data-ttu-id="9d47d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9d47d-117">Application</span></span>|<span data-ttu-id="9d47d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d47d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9d47d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9d47d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates/{advancedThreatProtectionOnboardingDeviceSettingStateId}
```

## <a name="request-headers"></a><span data-ttu-id="9d47d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9d47d-120">Request headers</span></span>
|<span data-ttu-id="9d47d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9d47d-121">Header</span></span>|<span data-ttu-id="9d47d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9d47d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9d47d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d47d-123">Authorization</span></span>|<span data-ttu-id="9d47d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9d47d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9d47d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9d47d-125">Accept</span></span>|<span data-ttu-id="9d47d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9d47d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d47d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9d47d-127">Request body</span></span>
<span data-ttu-id="9d47d-128">В тексте запроса добавьте представление объекта [адванцедсреатпротектиононбоардингдевицесеттингстате](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9d47d-128">In the request body, supply a JSON representation for the [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object.</span></span>

<span data-ttu-id="9d47d-129">В следующей таблице приведены свойства, необходимые при создании [адванцедсреатпротектиононбоардингдевицесеттингстате](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="9d47d-129">The following table shows the properties that are required when you create the [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md).</span></span>

|<span data-ttu-id="9d47d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9d47d-130">Property</span></span>|<span data-ttu-id="9d47d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9d47d-131">Type</span></span>|<span data-ttu-id="9d47d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9d47d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d47d-133">id</span><span class="sxs-lookup"><span data-stu-id="9d47d-133">id</span></span>|<span data-ttu-id="9d47d-134">String</span><span class="sxs-lookup"><span data-stu-id="9d47d-134">String</span></span>|<span data-ttu-id="9d47d-135">Ключ объекта</span><span class="sxs-lookup"><span data-stu-id="9d47d-135">Key of the entity</span></span>|
|<span data-ttu-id="9d47d-136">platformType</span><span class="sxs-lookup"><span data-stu-id="9d47d-136">platformType</span></span>|[<span data-ttu-id="9d47d-137">deviceType</span><span class="sxs-lookup"><span data-stu-id="9d47d-137">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="9d47d-138">Тип платформы устройства.</span><span class="sxs-lookup"><span data-stu-id="9d47d-138">Device platform type.</span></span> <span data-ttu-id="9d47d-139">Возможные значения:,,,,,,,,,,, `desktop` `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` , `unix` , `macMDM` , `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `blackberry` `palm` `unknown` ,,,,,,,,,,,,,,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="9d47d-139">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `androidnGMS`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="9d47d-140">setting</span><span class="sxs-lookup"><span data-stu-id="9d47d-140">setting</span></span>|<span data-ttu-id="9d47d-141">String</span><span class="sxs-lookup"><span data-stu-id="9d47d-141">String</span></span>|<span data-ttu-id="9d47d-142">Имя класса параметров и свойства.</span><span class="sxs-lookup"><span data-stu-id="9d47d-142">The setting class name and property name.</span></span>|
|<span data-ttu-id="9d47d-143">settingName</span><span class="sxs-lookup"><span data-stu-id="9d47d-143">settingName</span></span>|<span data-ttu-id="9d47d-144">String</span><span class="sxs-lookup"><span data-stu-id="9d47d-144">String</span></span>|<span data-ttu-id="9d47d-145">Имя параметра в отчете</span><span class="sxs-lookup"><span data-stu-id="9d47d-145">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="9d47d-146">deviceId</span><span class="sxs-lookup"><span data-stu-id="9d47d-146">deviceId</span></span>|<span data-ttu-id="9d47d-147">String</span><span class="sxs-lookup"><span data-stu-id="9d47d-147">String</span></span>|<span data-ttu-id="9d47d-148">ИД устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="9d47d-148">The Device Id that is being reported</span></span>|
|<span data-ttu-id="9d47d-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="9d47d-149">deviceName</span></span>|<span data-ttu-id="9d47d-150">String</span><span class="sxs-lookup"><span data-stu-id="9d47d-150">String</span></span>|<span data-ttu-id="9d47d-151">Имя устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="9d47d-151">The Device Name that is being reported</span></span>|
|<span data-ttu-id="9d47d-152">userId</span><span class="sxs-lookup"><span data-stu-id="9d47d-152">userId</span></span>|<span data-ttu-id="9d47d-153">String</span><span class="sxs-lookup"><span data-stu-id="9d47d-153">String</span></span>|<span data-ttu-id="9d47d-154">ИД пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="9d47d-154">The user Id that is being reported</span></span>|
|<span data-ttu-id="9d47d-155">userEmail</span><span class="sxs-lookup"><span data-stu-id="9d47d-155">userEmail</span></span>|<span data-ttu-id="9d47d-156">String</span><span class="sxs-lookup"><span data-stu-id="9d47d-156">String</span></span>|<span data-ttu-id="9d47d-157">Электронный адрес пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="9d47d-157">The User email address that is being reported</span></span>|
|<span data-ttu-id="9d47d-158">userName</span><span class="sxs-lookup"><span data-stu-id="9d47d-158">userName</span></span>|<span data-ttu-id="9d47d-159">String</span><span class="sxs-lookup"><span data-stu-id="9d47d-159">String</span></span>|<span data-ttu-id="9d47d-160">Имя пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="9d47d-160">The User Name that is being reported</span></span>|
|<span data-ttu-id="9d47d-161">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9d47d-161">userPrincipalName</span></span>|<span data-ttu-id="9d47d-162">String</span><span class="sxs-lookup"><span data-stu-id="9d47d-162">String</span></span>|<span data-ttu-id="9d47d-163">Имя участника-пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="9d47d-163">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="9d47d-164">deviceModel</span><span class="sxs-lookup"><span data-stu-id="9d47d-164">deviceModel</span></span>|<span data-ttu-id="9d47d-165">String</span><span class="sxs-lookup"><span data-stu-id="9d47d-165">String</span></span>|<span data-ttu-id="9d47d-166">Модель устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="9d47d-166">The device model that is being reported</span></span>|
|<span data-ttu-id="9d47d-167">state</span><span class="sxs-lookup"><span data-stu-id="9d47d-167">state</span></span>|[<span data-ttu-id="9d47d-168">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="9d47d-168">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="9d47d-169">Состояние соответствия для параметра.</span><span class="sxs-lookup"><span data-stu-id="9d47d-169">The compliance state of the setting.</span></span> <span data-ttu-id="9d47d-170">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="9d47d-170">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="9d47d-171">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="9d47d-171">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="9d47d-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d47d-172">DateTimeOffset</span></span>|<span data-ttu-id="9d47d-173">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="9d47d-173">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="9d47d-174">Ответ</span><span class="sxs-lookup"><span data-stu-id="9d47d-174">Response</span></span>
<span data-ttu-id="9d47d-175">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [адванцедсреатпротектиононбоардингдевицесеттингстате](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9d47d-175">If successful, this method returns a `200 OK` response code and an updated [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d47d-176">Пример</span><span class="sxs-lookup"><span data-stu-id="9d47d-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="9d47d-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="9d47d-177">Request</span></span>
<span data-ttu-id="9d47d-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9d47d-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates/{advancedThreatProtectionOnboardingDeviceSettingStateId}
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

### <a name="response"></a><span data-ttu-id="9d47d-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d47d-179">Response</span></span>
<span data-ttu-id="9d47d-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9d47d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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






