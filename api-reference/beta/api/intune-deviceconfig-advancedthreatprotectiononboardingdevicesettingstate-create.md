---
title: Создание Адванцедсреатпротектиононбоардингдевицесеттингстате
description: Создание нового объекта Адванцедсреатпротектиононбоардингдевицесеттингстате.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 26130550d4a89368dfa29e22aedf9ca7bf1b67d5
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48714880"
---
# <a name="create-advancedthreatprotectiononboardingdevicesettingstate"></a><span data-ttu-id="8599b-103">Создание Адванцедсреатпротектиононбоардингдевицесеттингстате</span><span class="sxs-lookup"><span data-stu-id="8599b-103">Create advancedThreatProtectionOnboardingDeviceSettingState</span></span>

<span data-ttu-id="8599b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8599b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8599b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8599b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8599b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8599b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8599b-107">Создание нового объекта [адванцедсреатпротектиононбоардингдевицесеттингстате](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) .</span><span class="sxs-lookup"><span data-stu-id="8599b-107">Create a new [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8599b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8599b-108">Prerequisites</span></span>
<span data-ttu-id="8599b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8599b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8599b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8599b-111">Permission type</span></span>|<span data-ttu-id="8599b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8599b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8599b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8599b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8599b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8599b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8599b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8599b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8599b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8599b-116">Not supported.</span></span>|
|<span data-ttu-id="8599b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8599b-117">Application</span></span>|<span data-ttu-id="8599b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8599b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8599b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8599b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="8599b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8599b-120">Request headers</span></span>
|<span data-ttu-id="8599b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8599b-121">Header</span></span>|<span data-ttu-id="8599b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8599b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8599b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8599b-123">Authorization</span></span>|<span data-ttu-id="8599b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8599b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8599b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8599b-125">Accept</span></span>|<span data-ttu-id="8599b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8599b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8599b-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8599b-127">Request body</span></span>
<span data-ttu-id="8599b-128">В тексте запроса добавьте представление объекта Адванцедсреатпротектиононбоардингдевицесеттингстате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8599b-128">In the request body, supply a JSON representation for the advancedThreatProtectionOnboardingDeviceSettingState object.</span></span>

<span data-ttu-id="8599b-129">В следующей таблице приведены свойства, необходимые при создании Адванцедсреатпротектиононбоардингдевицесеттингстате.</span><span class="sxs-lookup"><span data-stu-id="8599b-129">The following table shows the properties that are required when you create the advancedThreatProtectionOnboardingDeviceSettingState.</span></span>

|<span data-ttu-id="8599b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8599b-130">Property</span></span>|<span data-ttu-id="8599b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8599b-131">Type</span></span>|<span data-ttu-id="8599b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8599b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8599b-133">id</span><span class="sxs-lookup"><span data-stu-id="8599b-133">id</span></span>|<span data-ttu-id="8599b-134">Строка</span><span class="sxs-lookup"><span data-stu-id="8599b-134">String</span></span>|<span data-ttu-id="8599b-135">Ключ объекта</span><span class="sxs-lookup"><span data-stu-id="8599b-135">Key of the entity</span></span>|
|<span data-ttu-id="8599b-136">platformType</span><span class="sxs-lookup"><span data-stu-id="8599b-136">platformType</span></span>|[<span data-ttu-id="8599b-137">deviceType</span><span class="sxs-lookup"><span data-stu-id="8599b-137">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="8599b-138">Тип платформы устройства.</span><span class="sxs-lookup"><span data-stu-id="8599b-138">Device platform type.</span></span> <span data-ttu-id="8599b-139">Возможные значения:,,,,,,,,,,, `desktop` `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` , `unix` , `macMDM` , `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `blackberry` `palm` `unknown` ,,,,,,,,,,,,,,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="8599b-139">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `androidnGMS`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="8599b-140">setting</span><span class="sxs-lookup"><span data-stu-id="8599b-140">setting</span></span>|<span data-ttu-id="8599b-141">String</span><span class="sxs-lookup"><span data-stu-id="8599b-141">String</span></span>|<span data-ttu-id="8599b-142">Имя класса параметров и свойства.</span><span class="sxs-lookup"><span data-stu-id="8599b-142">The setting class name and property name.</span></span>|
|<span data-ttu-id="8599b-143">settingName</span><span class="sxs-lookup"><span data-stu-id="8599b-143">settingName</span></span>|<span data-ttu-id="8599b-144">String</span><span class="sxs-lookup"><span data-stu-id="8599b-144">String</span></span>|<span data-ttu-id="8599b-145">Имя параметра в отчете</span><span class="sxs-lookup"><span data-stu-id="8599b-145">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="8599b-146">deviceId</span><span class="sxs-lookup"><span data-stu-id="8599b-146">deviceId</span></span>|<span data-ttu-id="8599b-147">String</span><span class="sxs-lookup"><span data-stu-id="8599b-147">String</span></span>|<span data-ttu-id="8599b-148">ИД устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="8599b-148">The Device Id that is being reported</span></span>|
|<span data-ttu-id="8599b-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="8599b-149">deviceName</span></span>|<span data-ttu-id="8599b-150">String</span><span class="sxs-lookup"><span data-stu-id="8599b-150">String</span></span>|<span data-ttu-id="8599b-151">Имя устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="8599b-151">The Device Name that is being reported</span></span>|
|<span data-ttu-id="8599b-152">userId</span><span class="sxs-lookup"><span data-stu-id="8599b-152">userId</span></span>|<span data-ttu-id="8599b-153">String</span><span class="sxs-lookup"><span data-stu-id="8599b-153">String</span></span>|<span data-ttu-id="8599b-154">ИД пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="8599b-154">The user Id that is being reported</span></span>|
|<span data-ttu-id="8599b-155">userEmail</span><span class="sxs-lookup"><span data-stu-id="8599b-155">userEmail</span></span>|<span data-ttu-id="8599b-156">String</span><span class="sxs-lookup"><span data-stu-id="8599b-156">String</span></span>|<span data-ttu-id="8599b-157">Электронный адрес пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="8599b-157">The User email address that is being reported</span></span>|
|<span data-ttu-id="8599b-158">userName</span><span class="sxs-lookup"><span data-stu-id="8599b-158">userName</span></span>|<span data-ttu-id="8599b-159">String</span><span class="sxs-lookup"><span data-stu-id="8599b-159">String</span></span>|<span data-ttu-id="8599b-160">Имя пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="8599b-160">The User Name that is being reported</span></span>|
|<span data-ttu-id="8599b-161">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8599b-161">userPrincipalName</span></span>|<span data-ttu-id="8599b-162">String</span><span class="sxs-lookup"><span data-stu-id="8599b-162">String</span></span>|<span data-ttu-id="8599b-163">Имя участника-пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="8599b-163">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="8599b-164">deviceModel</span><span class="sxs-lookup"><span data-stu-id="8599b-164">deviceModel</span></span>|<span data-ttu-id="8599b-165">String</span><span class="sxs-lookup"><span data-stu-id="8599b-165">String</span></span>|<span data-ttu-id="8599b-166">Модель устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="8599b-166">The device model that is being reported</span></span>|
|<span data-ttu-id="8599b-167">state</span><span class="sxs-lookup"><span data-stu-id="8599b-167">state</span></span>|[<span data-ttu-id="8599b-168">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="8599b-168">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="8599b-169">Состояние соответствия для параметра.</span><span class="sxs-lookup"><span data-stu-id="8599b-169">The compliance state of the setting.</span></span> <span data-ttu-id="8599b-170">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="8599b-170">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="8599b-171">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="8599b-171">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="8599b-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8599b-172">DateTimeOffset</span></span>|<span data-ttu-id="8599b-173">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="8599b-173">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="8599b-174">Ответ</span><span class="sxs-lookup"><span data-stu-id="8599b-174">Response</span></span>
<span data-ttu-id="8599b-175">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [адванцедсреатпротектиононбоардингдевицесеттингстате](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8599b-175">If successful, this method returns a `201 Created` response code and a [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8599b-176">Пример</span><span class="sxs-lookup"><span data-stu-id="8599b-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="8599b-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="8599b-177">Request</span></span>
<span data-ttu-id="8599b-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8599b-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8599b-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="8599b-179">Response</span></span>
<span data-ttu-id="8599b-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8599b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





