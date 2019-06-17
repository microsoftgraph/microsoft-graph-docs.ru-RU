---
title: Обновление Адванцедсреатпротектиононбоардингдевицесеттингстате
description: Обновление свойств объекта Адванцедсреатпротектиононбоардингдевицесеттингстате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 288065c51d972dbcc5ea5e76053be07d55ceae71
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34971677"
---
# <a name="update-advancedthreatprotectiononboardingdevicesettingstate"></a><span data-ttu-id="b7f48-103">Обновление Адванцедсреатпротектиононбоардингдевицесеттингстате</span><span class="sxs-lookup"><span data-stu-id="b7f48-103">Update advancedThreatProtectionOnboardingDeviceSettingState</span></span>

> <span data-ttu-id="b7f48-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7f48-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b7f48-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b7f48-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7f48-106">Обновление свойств объекта [адванцедсреатпротектиононбоардингдевицесеттингстате](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) .</span><span class="sxs-lookup"><span data-stu-id="b7f48-106">Update the properties of a [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b7f48-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b7f48-107">Prerequisites</span></span>
<span data-ttu-id="b7f48-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7f48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7f48-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b7f48-110">Permission type</span></span>|<span data-ttu-id="b7f48-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b7f48-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b7f48-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b7f48-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b7f48-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7f48-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b7f48-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b7f48-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b7f48-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7f48-115">Not supported.</span></span>|
|<span data-ttu-id="b7f48-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b7f48-116">Application</span></span>|<span data-ttu-id="b7f48-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7f48-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b7f48-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b7f48-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates/{advancedThreatProtectionOnboardingDeviceSettingStateId}
```

## <a name="request-headers"></a><span data-ttu-id="b7f48-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b7f48-119">Request headers</span></span>
|<span data-ttu-id="b7f48-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b7f48-120">Header</span></span>|<span data-ttu-id="b7f48-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b7f48-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b7f48-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b7f48-122">Authorization</span></span>|<span data-ttu-id="b7f48-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b7f48-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b7f48-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b7f48-124">Accept</span></span>|<span data-ttu-id="b7f48-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b7f48-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7f48-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b7f48-126">Request body</span></span>
<span data-ttu-id="b7f48-127">В тексте запроса добавьте представление объекта [адванцедсреатпротектиононбоардингдевицесеттингстате](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b7f48-127">In the request body, supply a JSON representation for the [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object.</span></span>

<span data-ttu-id="b7f48-128">В следующей таблице приведены свойства, необходимые при создании [адванцедсреатпротектиононбоардингдевицесеттингстате](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="b7f48-128">The following table shows the properties that are required when you create the [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md).</span></span>

|<span data-ttu-id="b7f48-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b7f48-129">Property</span></span>|<span data-ttu-id="b7f48-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b7f48-130">Type</span></span>|<span data-ttu-id="b7f48-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b7f48-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7f48-132">id</span><span class="sxs-lookup"><span data-stu-id="b7f48-132">id</span></span>|<span data-ttu-id="b7f48-133">Строка</span><span class="sxs-lookup"><span data-stu-id="b7f48-133">String</span></span>|<span data-ttu-id="b7f48-134">Ключ объекта</span><span class="sxs-lookup"><span data-stu-id="b7f48-134">Key of the entity</span></span>|
|<span data-ttu-id="b7f48-135">platformType</span><span class="sxs-lookup"><span data-stu-id="b7f48-135">platformType</span></span>|[<span data-ttu-id="b7f48-136">deviceType</span><span class="sxs-lookup"><span data-stu-id="b7f48-136">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="b7f48-137">Тип платформы устройства.</span><span class="sxs-lookup"><span data-stu-id="b7f48-137">Device platform type.</span></span> <span data-ttu-id="b7f48-138">Возможные значения: `desktop`, `windowsRT`, `winMO6`, `nokia` `windowsPhone` `mac` `winCE` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `android` `iSocConsumer`,,,,,,,,,,,,,,,,,,,,, `winEmbedded` `iPhone` `iPad` `iPod` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="b7f48-138">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="b7f48-139">setting</span><span class="sxs-lookup"><span data-stu-id="b7f48-139">setting</span></span>|<span data-ttu-id="b7f48-140">String</span><span class="sxs-lookup"><span data-stu-id="b7f48-140">String</span></span>|<span data-ttu-id="b7f48-141">Имя класса параметров и свойства.</span><span class="sxs-lookup"><span data-stu-id="b7f48-141">The setting class name and property name.</span></span>|
|<span data-ttu-id="b7f48-142">settingName</span><span class="sxs-lookup"><span data-stu-id="b7f48-142">settingName</span></span>|<span data-ttu-id="b7f48-143">String</span><span class="sxs-lookup"><span data-stu-id="b7f48-143">String</span></span>|<span data-ttu-id="b7f48-144">Имя параметра в отчете</span><span class="sxs-lookup"><span data-stu-id="b7f48-144">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="b7f48-145">deviceId</span><span class="sxs-lookup"><span data-stu-id="b7f48-145">deviceId</span></span>|<span data-ttu-id="b7f48-146">String</span><span class="sxs-lookup"><span data-stu-id="b7f48-146">String</span></span>|<span data-ttu-id="b7f48-147">ИД устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="b7f48-147">The Device Id that is being reported</span></span>|
|<span data-ttu-id="b7f48-148">deviceName</span><span class="sxs-lookup"><span data-stu-id="b7f48-148">deviceName</span></span>|<span data-ttu-id="b7f48-149">String</span><span class="sxs-lookup"><span data-stu-id="b7f48-149">String</span></span>|<span data-ttu-id="b7f48-150">Имя устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="b7f48-150">The Device Name that is being reported</span></span>|
|<span data-ttu-id="b7f48-151">userId</span><span class="sxs-lookup"><span data-stu-id="b7f48-151">userId</span></span>|<span data-ttu-id="b7f48-152">String</span><span class="sxs-lookup"><span data-stu-id="b7f48-152">String</span></span>|<span data-ttu-id="b7f48-153">ИД пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="b7f48-153">The user Id that is being reported</span></span>|
|<span data-ttu-id="b7f48-154">userEmail</span><span class="sxs-lookup"><span data-stu-id="b7f48-154">userEmail</span></span>|<span data-ttu-id="b7f48-155">String</span><span class="sxs-lookup"><span data-stu-id="b7f48-155">String</span></span>|<span data-ttu-id="b7f48-156">Электронный адрес пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="b7f48-156">The User email address that is being reported</span></span>|
|<span data-ttu-id="b7f48-157">userName</span><span class="sxs-lookup"><span data-stu-id="b7f48-157">userName</span></span>|<span data-ttu-id="b7f48-158">String</span><span class="sxs-lookup"><span data-stu-id="b7f48-158">String</span></span>|<span data-ttu-id="b7f48-159">Имя пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="b7f48-159">The User Name that is being reported</span></span>|
|<span data-ttu-id="b7f48-160">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b7f48-160">userPrincipalName</span></span>|<span data-ttu-id="b7f48-161">String</span><span class="sxs-lookup"><span data-stu-id="b7f48-161">String</span></span>|<span data-ttu-id="b7f48-162">Имя участника-пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="b7f48-162">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="b7f48-163">deviceModel</span><span class="sxs-lookup"><span data-stu-id="b7f48-163">deviceModel</span></span>|<span data-ttu-id="b7f48-164">String</span><span class="sxs-lookup"><span data-stu-id="b7f48-164">String</span></span>|<span data-ttu-id="b7f48-165">Модель устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="b7f48-165">The device model that is being reported</span></span>|
|<span data-ttu-id="b7f48-166">state</span><span class="sxs-lookup"><span data-stu-id="b7f48-166">state</span></span>|[<span data-ttu-id="b7f48-167">Комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="b7f48-167">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="b7f48-168">Состояние соответствия для параметра.</span><span class="sxs-lookup"><span data-stu-id="b7f48-168">The compliance state of the setting.</span></span> <span data-ttu-id="b7f48-169">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="b7f48-169">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="b7f48-170">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="b7f48-170">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="b7f48-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b7f48-171">DateTimeOffset</span></span>|<span data-ttu-id="b7f48-172">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="b7f48-172">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="b7f48-173">Ответ</span><span class="sxs-lookup"><span data-stu-id="b7f48-173">Response</span></span>
<span data-ttu-id="b7f48-174">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [адванцедсреатпротектиононбоардингдевицесеттингстате](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b7f48-174">If successful, this method returns a `200 OK` response code and an updated [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7f48-175">Пример</span><span class="sxs-lookup"><span data-stu-id="b7f48-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="b7f48-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="b7f48-176">Request</span></span>
<span data-ttu-id="b7f48-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b7f48-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b7f48-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7f48-178">Response</span></span>
<span data-ttu-id="b7f48-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b7f48-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





