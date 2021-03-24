---
title: Обновление advancedThreatProtectionOnboardingDeviceSettingState
description: Обновление свойств объекта advancedThreatProtectionOnboardingDeviceSettingState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1db888112e3cea22cdf154662618474694a60b6e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51126866"
---
# <a name="update-advancedthreatprotectiononboardingdevicesettingstate"></a><span data-ttu-id="f6d86-103">Обновление advancedThreatProtectionOnboardingDeviceSettingState</span><span class="sxs-lookup"><span data-stu-id="f6d86-103">Update advancedThreatProtectionOnboardingDeviceSettingState</span></span>

<span data-ttu-id="f6d86-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6d86-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f6d86-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6d86-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f6d86-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f6d86-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6d86-107">Обновление свойств объекта [advancedThreatProtectionOnboardingDeviceSettingState.](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)</span><span class="sxs-lookup"><span data-stu-id="f6d86-107">Update the properties of a [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f6d86-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f6d86-108">Prerequisites</span></span>
<span data-ttu-id="f6d86-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6d86-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6d86-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f6d86-111">Permission type</span></span>|<span data-ttu-id="f6d86-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f6d86-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6d86-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f6d86-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f6d86-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6d86-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f6d86-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f6d86-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6d86-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6d86-116">Not supported.</span></span>|
|<span data-ttu-id="f6d86-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f6d86-117">Application</span></span>|<span data-ttu-id="f6d86-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6d86-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6d86-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f6d86-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates/{advancedThreatProtectionOnboardingDeviceSettingStateId}
```

## <a name="request-headers"></a><span data-ttu-id="f6d86-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f6d86-120">Request headers</span></span>
|<span data-ttu-id="f6d86-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f6d86-121">Header</span></span>|<span data-ttu-id="f6d86-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f6d86-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f6d86-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6d86-123">Authorization</span></span>|<span data-ttu-id="f6d86-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f6d86-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f6d86-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f6d86-125">Accept</span></span>|<span data-ttu-id="f6d86-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f6d86-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6d86-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f6d86-127">Request body</span></span>
<span data-ttu-id="f6d86-128">В теле запроса подарйте представление JSON для объекта [advancedThreatProtectionOnboardingDeviceSettingState.](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)</span><span class="sxs-lookup"><span data-stu-id="f6d86-128">In the request body, supply a JSON representation for the [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object.</span></span>

<span data-ttu-id="f6d86-129">В следующей таблице показаны свойства, необходимые при создании [advancedThreatProtectionOnboardingDeviceSettingState.](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)</span><span class="sxs-lookup"><span data-stu-id="f6d86-129">The following table shows the properties that are required when you create the [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md).</span></span>

|<span data-ttu-id="f6d86-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f6d86-130">Property</span></span>|<span data-ttu-id="f6d86-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f6d86-131">Type</span></span>|<span data-ttu-id="f6d86-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f6d86-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6d86-133">id</span><span class="sxs-lookup"><span data-stu-id="f6d86-133">id</span></span>|<span data-ttu-id="f6d86-134">Строка</span><span class="sxs-lookup"><span data-stu-id="f6d86-134">String</span></span>|<span data-ttu-id="f6d86-135">Ключ объекта</span><span class="sxs-lookup"><span data-stu-id="f6d86-135">Key of the entity</span></span>|
|<span data-ttu-id="f6d86-136">platformType</span><span class="sxs-lookup"><span data-stu-id="f6d86-136">platformType</span></span>|[<span data-ttu-id="f6d86-137">deviceType</span><span class="sxs-lookup"><span data-stu-id="f6d86-137">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="f6d86-138">Тип платформы устройства.</span><span class="sxs-lookup"><span data-stu-id="f6d86-138">Device platform type.</span></span> <span data-ttu-id="f6d86-139">Возможные значения: `desktop` `windowsRT` , `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `cloudPC` `blackberry` `palm` . `unknown`</span><span class="sxs-lookup"><span data-stu-id="f6d86-139">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `androidnGMS`, `cloudPC`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="f6d86-140">setting</span><span class="sxs-lookup"><span data-stu-id="f6d86-140">setting</span></span>|<span data-ttu-id="f6d86-141">String</span><span class="sxs-lookup"><span data-stu-id="f6d86-141">String</span></span>|<span data-ttu-id="f6d86-142">Имя класса параметров и свойства.</span><span class="sxs-lookup"><span data-stu-id="f6d86-142">The setting class name and property name.</span></span>|
|<span data-ttu-id="f6d86-143">settingName</span><span class="sxs-lookup"><span data-stu-id="f6d86-143">settingName</span></span>|<span data-ttu-id="f6d86-144">String</span><span class="sxs-lookup"><span data-stu-id="f6d86-144">String</span></span>|<span data-ttu-id="f6d86-145">Имя параметра в отчете</span><span class="sxs-lookup"><span data-stu-id="f6d86-145">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="f6d86-146">deviceId</span><span class="sxs-lookup"><span data-stu-id="f6d86-146">deviceId</span></span>|<span data-ttu-id="f6d86-147">String</span><span class="sxs-lookup"><span data-stu-id="f6d86-147">String</span></span>|<span data-ttu-id="f6d86-148">ИД устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="f6d86-148">The Device Id that is being reported</span></span>|
|<span data-ttu-id="f6d86-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="f6d86-149">deviceName</span></span>|<span data-ttu-id="f6d86-150">String</span><span class="sxs-lookup"><span data-stu-id="f6d86-150">String</span></span>|<span data-ttu-id="f6d86-151">Имя устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="f6d86-151">The Device Name that is being reported</span></span>|
|<span data-ttu-id="f6d86-152">userId</span><span class="sxs-lookup"><span data-stu-id="f6d86-152">userId</span></span>|<span data-ttu-id="f6d86-153">String</span><span class="sxs-lookup"><span data-stu-id="f6d86-153">String</span></span>|<span data-ttu-id="f6d86-154">ИД пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="f6d86-154">The user Id that is being reported</span></span>|
|<span data-ttu-id="f6d86-155">userEmail</span><span class="sxs-lookup"><span data-stu-id="f6d86-155">userEmail</span></span>|<span data-ttu-id="f6d86-156">String</span><span class="sxs-lookup"><span data-stu-id="f6d86-156">String</span></span>|<span data-ttu-id="f6d86-157">Электронный адрес пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="f6d86-157">The User email address that is being reported</span></span>|
|<span data-ttu-id="f6d86-158">userName</span><span class="sxs-lookup"><span data-stu-id="f6d86-158">userName</span></span>|<span data-ttu-id="f6d86-159">String</span><span class="sxs-lookup"><span data-stu-id="f6d86-159">String</span></span>|<span data-ttu-id="f6d86-160">Имя пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="f6d86-160">The User Name that is being reported</span></span>|
|<span data-ttu-id="f6d86-161">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f6d86-161">userPrincipalName</span></span>|<span data-ttu-id="f6d86-162">String</span><span class="sxs-lookup"><span data-stu-id="f6d86-162">String</span></span>|<span data-ttu-id="f6d86-163">Имя участника-пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="f6d86-163">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="f6d86-164">deviceModel</span><span class="sxs-lookup"><span data-stu-id="f6d86-164">deviceModel</span></span>|<span data-ttu-id="f6d86-165">String</span><span class="sxs-lookup"><span data-stu-id="f6d86-165">String</span></span>|<span data-ttu-id="f6d86-166">Модель устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="f6d86-166">The device model that is being reported</span></span>|
|<span data-ttu-id="f6d86-167">state</span><span class="sxs-lookup"><span data-stu-id="f6d86-167">state</span></span>|[<span data-ttu-id="f6d86-168">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="f6d86-168">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="f6d86-169">Состояние соответствия параметру.</span><span class="sxs-lookup"><span data-stu-id="f6d86-169">The compliance state of the setting.</span></span> <span data-ttu-id="f6d86-170">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="f6d86-170">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="f6d86-171">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f6d86-171">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="f6d86-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6d86-172">DateTimeOffset</span></span>|<span data-ttu-id="f6d86-173">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="f6d86-173">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="f6d86-174">Ответ</span><span class="sxs-lookup"><span data-stu-id="f6d86-174">Response</span></span>
<span data-ttu-id="f6d86-175">В случае успеха этот метод возвращает код ответа и обновленный расширенный `200 OK` [объектThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f6d86-175">If successful, this method returns a `200 OK` response code and an updated [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6d86-176">Пример</span><span class="sxs-lookup"><span data-stu-id="f6d86-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="f6d86-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="f6d86-177">Request</span></span>
<span data-ttu-id="f6d86-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f6d86-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f6d86-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6d86-179">Response</span></span>
<span data-ttu-id="f6d86-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f6d86-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




