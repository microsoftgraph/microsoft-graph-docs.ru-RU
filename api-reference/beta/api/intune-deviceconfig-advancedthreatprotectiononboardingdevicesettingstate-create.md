---
title: Создание Адванцедсреатпротектиононбоардингдевицесеттингстате
description: Создание нового объекта Адванцедсреатпротектиононбоардингдевицесеттингстате.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d877edcdc82cee35c7fc75c556ca5ac0035221ad
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30980665"
---
# <a name="create-advancedthreatprotectiononboardingdevicesettingstate"></a><span data-ttu-id="eda10-103">Создание Адванцедсреатпротектиононбоардингдевицесеттингстате</span><span class="sxs-lookup"><span data-stu-id="eda10-103">Create advancedThreatProtectionOnboardingDeviceSettingState</span></span>

> <span data-ttu-id="eda10-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eda10-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eda10-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eda10-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eda10-106">Создание нового объекта [адванцедсреатпротектиононбоардингдевицесеттингстате](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) .</span><span class="sxs-lookup"><span data-stu-id="eda10-106">Create a new [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eda10-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="eda10-107">Prerequisites</span></span>
<span data-ttu-id="eda10-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eda10-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eda10-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eda10-110">Permission type</span></span>|<span data-ttu-id="eda10-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="eda10-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eda10-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eda10-112">Delegated (work or school account)</span></span>|<span data-ttu-id="eda10-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eda10-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="eda10-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eda10-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eda10-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eda10-115">Not supported.</span></span>|
|<span data-ttu-id="eda10-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eda10-116">Application</span></span>|<span data-ttu-id="eda10-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eda10-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eda10-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eda10-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="eda10-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eda10-119">Request headers</span></span>
|<span data-ttu-id="eda10-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="eda10-120">Header</span></span>|<span data-ttu-id="eda10-121">Значение</span><span class="sxs-lookup"><span data-stu-id="eda10-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eda10-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eda10-122">Authorization</span></span>|<span data-ttu-id="eda10-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eda10-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eda10-124">Accept</span><span class="sxs-lookup"><span data-stu-id="eda10-124">Accept</span></span>|<span data-ttu-id="eda10-125">application/json</span><span class="sxs-lookup"><span data-stu-id="eda10-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eda10-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eda10-126">Request body</span></span>
<span data-ttu-id="eda10-127">В тексте запроса добавьте представление объекта Адванцедсреатпротектиононбоардингдевицесеттингстате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eda10-127">In the request body, supply a JSON representation for the advancedThreatProtectionOnboardingDeviceSettingState object.</span></span>

<span data-ttu-id="eda10-128">В следующей таблице приведены свойства, необходимые при создании Адванцедсреатпротектиононбоардингдевицесеттингстате.</span><span class="sxs-lookup"><span data-stu-id="eda10-128">The following table shows the properties that are required when you create the advancedThreatProtectionOnboardingDeviceSettingState.</span></span>

|<span data-ttu-id="eda10-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="eda10-129">Property</span></span>|<span data-ttu-id="eda10-130">Тип</span><span class="sxs-lookup"><span data-stu-id="eda10-130">Type</span></span>|<span data-ttu-id="eda10-131">Описание</span><span class="sxs-lookup"><span data-stu-id="eda10-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eda10-132">id</span><span class="sxs-lookup"><span data-stu-id="eda10-132">id</span></span>|<span data-ttu-id="eda10-133">Строка</span><span class="sxs-lookup"><span data-stu-id="eda10-133">String</span></span>|<span data-ttu-id="eda10-134">Ключ объекта</span><span class="sxs-lookup"><span data-stu-id="eda10-134">Key of the entity</span></span>|
|<span data-ttu-id="eda10-135">platformType</span><span class="sxs-lookup"><span data-stu-id="eda10-135">platformType</span></span>|[<span data-ttu-id="eda10-136">deviceType</span><span class="sxs-lookup"><span data-stu-id="eda10-136">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="eda10-137">Тип платформы устройства.</span><span class="sxs-lookup"><span data-stu-id="eda10-137">Device platform type.</span></span> <span data-ttu-id="eda10-138">Возможные значения: `desktop`, `windowsRT`, `winMO6`, `nokia` `windowsPhone` `mac` `winCE` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `android` `iSocConsumer`,,,,,,,,,,,,,,,,,,,,, `winEmbedded` `iPhone` `iPad` `iPod` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="eda10-138">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="eda10-139">setting</span><span class="sxs-lookup"><span data-stu-id="eda10-139">setting</span></span>|<span data-ttu-id="eda10-140">String</span><span class="sxs-lookup"><span data-stu-id="eda10-140">String</span></span>|<span data-ttu-id="eda10-141">Имя класса параметров и свойства.</span><span class="sxs-lookup"><span data-stu-id="eda10-141">The setting class name and property name.</span></span>|
|<span data-ttu-id="eda10-142">settingName</span><span class="sxs-lookup"><span data-stu-id="eda10-142">settingName</span></span>|<span data-ttu-id="eda10-143">String</span><span class="sxs-lookup"><span data-stu-id="eda10-143">String</span></span>|<span data-ttu-id="eda10-144">Имя параметра в отчете</span><span class="sxs-lookup"><span data-stu-id="eda10-144">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="eda10-145">deviceId</span><span class="sxs-lookup"><span data-stu-id="eda10-145">deviceId</span></span>|<span data-ttu-id="eda10-146">String</span><span class="sxs-lookup"><span data-stu-id="eda10-146">String</span></span>|<span data-ttu-id="eda10-147">ИД устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="eda10-147">The Device Id that is being reported</span></span>|
|<span data-ttu-id="eda10-148">deviceName</span><span class="sxs-lookup"><span data-stu-id="eda10-148">deviceName</span></span>|<span data-ttu-id="eda10-149">String</span><span class="sxs-lookup"><span data-stu-id="eda10-149">String</span></span>|<span data-ttu-id="eda10-150">Имя устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="eda10-150">The Device Name that is being reported</span></span>|
|<span data-ttu-id="eda10-151">userId</span><span class="sxs-lookup"><span data-stu-id="eda10-151">userId</span></span>|<span data-ttu-id="eda10-152">String</span><span class="sxs-lookup"><span data-stu-id="eda10-152">String</span></span>|<span data-ttu-id="eda10-153">ИД пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="eda10-153">The user Id that is being reported</span></span>|
|<span data-ttu-id="eda10-154">userEmail</span><span class="sxs-lookup"><span data-stu-id="eda10-154">userEmail</span></span>|<span data-ttu-id="eda10-155">String</span><span class="sxs-lookup"><span data-stu-id="eda10-155">String</span></span>|<span data-ttu-id="eda10-156">Электронный адрес пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="eda10-156">The User email address that is being reported</span></span>|
|<span data-ttu-id="eda10-157">userName</span><span class="sxs-lookup"><span data-stu-id="eda10-157">userName</span></span>|<span data-ttu-id="eda10-158">String</span><span class="sxs-lookup"><span data-stu-id="eda10-158">String</span></span>|<span data-ttu-id="eda10-159">Имя пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="eda10-159">The User Name that is being reported</span></span>|
|<span data-ttu-id="eda10-160">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="eda10-160">userPrincipalName</span></span>|<span data-ttu-id="eda10-161">String</span><span class="sxs-lookup"><span data-stu-id="eda10-161">String</span></span>|<span data-ttu-id="eda10-162">Имя участника-пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="eda10-162">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="eda10-163">deviceModel</span><span class="sxs-lookup"><span data-stu-id="eda10-163">deviceModel</span></span>|<span data-ttu-id="eda10-164">String</span><span class="sxs-lookup"><span data-stu-id="eda10-164">String</span></span>|<span data-ttu-id="eda10-165">Модель устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="eda10-165">The device model that is being reported</span></span>|
|<span data-ttu-id="eda10-166">state</span><span class="sxs-lookup"><span data-stu-id="eda10-166">state</span></span>|[<span data-ttu-id="eda10-167">Комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="eda10-167">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="eda10-168">Состояние соответствия для параметра.</span><span class="sxs-lookup"><span data-stu-id="eda10-168">The compliance state of the setting.</span></span> <span data-ttu-id="eda10-169">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="eda10-169">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="eda10-170">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="eda10-170">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="eda10-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eda10-171">DateTimeOffset</span></span>|<span data-ttu-id="eda10-172">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="eda10-172">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="eda10-173">Ответ</span><span class="sxs-lookup"><span data-stu-id="eda10-173">Response</span></span>
<span data-ttu-id="eda10-174">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [адванцедсреатпротектиононбоардингдевицесеттингстате](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="eda10-174">If successful, this method returns a `201 Created` response code and a [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eda10-175">Пример</span><span class="sxs-lookup"><span data-stu-id="eda10-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="eda10-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="eda10-176">Request</span></span>
<span data-ttu-id="eda10-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eda10-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="eda10-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="eda10-178">Response</span></span>
<span data-ttu-id="eda10-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="eda10-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




