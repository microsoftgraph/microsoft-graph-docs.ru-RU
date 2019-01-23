---
title: Создание advancedThreatProtectionOnboardingDeviceSettingState
description: Создание нового объекта advancedThreatProtectionOnboardingDeviceSettingState.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 87db4f3c58a8f205ec6c72805d766e510dbb4188
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394693"
---
# <a name="create-advancedthreatprotectiononboardingdevicesettingstate"></a><span data-ttu-id="08fb1-103">Создание advancedThreatProtectionOnboardingDeviceSettingState</span><span class="sxs-lookup"><span data-stu-id="08fb1-103">Create advancedThreatProtectionOnboardingDeviceSettingState</span></span>

> <span data-ttu-id="08fb1-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="08fb1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="08fb1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08fb1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="08fb1-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="08fb1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08fb1-107">Создание нового объекта [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) .</span><span class="sxs-lookup"><span data-stu-id="08fb1-107">Create a new [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="08fb1-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="08fb1-108">Prerequisites</span></span>
<span data-ttu-id="08fb1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="08fb1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="08fb1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="08fb1-111">Permission type</span></span>|<span data-ttu-id="08fb1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="08fb1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08fb1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="08fb1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="08fb1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08fb1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="08fb1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="08fb1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08fb1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08fb1-116">Not supported.</span></span>|
|<span data-ttu-id="08fb1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="08fb1-117">Application</span></span>|<span data-ttu-id="08fb1-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08fb1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="08fb1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="08fb1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="08fb1-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="08fb1-120">Request headers</span></span>
|<span data-ttu-id="08fb1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="08fb1-121">Header</span></span>|<span data-ttu-id="08fb1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="08fb1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="08fb1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="08fb1-123">Authorization</span></span>|<span data-ttu-id="08fb1-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="08fb1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="08fb1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="08fb1-125">Accept</span></span>|<span data-ttu-id="08fb1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="08fb1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08fb1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="08fb1-127">Request body</span></span>
<span data-ttu-id="08fb1-128">В тексте запроса укажите представление JSON для объекта advancedThreatProtectionOnboardingDeviceSettingState.</span><span class="sxs-lookup"><span data-stu-id="08fb1-128">In the request body, supply a JSON representation for the advancedThreatProtectionOnboardingDeviceSettingState object.</span></span>

<span data-ttu-id="08fb1-129">В следующей таблице показаны свойства, которые необходимы для создания advancedThreatProtectionOnboardingDeviceSettingState.</span><span class="sxs-lookup"><span data-stu-id="08fb1-129">The following table shows the properties that are required when you create the advancedThreatProtectionOnboardingDeviceSettingState.</span></span>

|<span data-ttu-id="08fb1-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="08fb1-130">Property</span></span>|<span data-ttu-id="08fb1-131">Тип</span><span class="sxs-lookup"><span data-stu-id="08fb1-131">Type</span></span>|<span data-ttu-id="08fb1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="08fb1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08fb1-133">id</span><span class="sxs-lookup"><span data-stu-id="08fb1-133">id</span></span>|<span data-ttu-id="08fb1-134">String</span><span class="sxs-lookup"><span data-stu-id="08fb1-134">String</span></span>|<span data-ttu-id="08fb1-135">Ключ объекта</span><span class="sxs-lookup"><span data-stu-id="08fb1-135">Key of the entity</span></span>|
|<span data-ttu-id="08fb1-136">platformType</span><span class="sxs-lookup"><span data-stu-id="08fb1-136">platformType</span></span>|[<span data-ttu-id="08fb1-137">deviceType</span><span class="sxs-lookup"><span data-stu-id="08fb1-137">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="08fb1-138">Тип платформы устройства.</span><span class="sxs-lookup"><span data-stu-id="08fb1-138">Device platform type.</span></span> <span data-ttu-id="08fb1-139">Возможные значения: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="08fb1-139">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="08fb1-140">setting</span><span class="sxs-lookup"><span data-stu-id="08fb1-140">setting</span></span>|<span data-ttu-id="08fb1-141">String</span><span class="sxs-lookup"><span data-stu-id="08fb1-141">String</span></span>|<span data-ttu-id="08fb1-142">Имя класса параметров и свойства.</span><span class="sxs-lookup"><span data-stu-id="08fb1-142">The setting class name and property name.</span></span>|
|<span data-ttu-id="08fb1-143">settingName</span><span class="sxs-lookup"><span data-stu-id="08fb1-143">settingName</span></span>|<span data-ttu-id="08fb1-144">String</span><span class="sxs-lookup"><span data-stu-id="08fb1-144">String</span></span>|<span data-ttu-id="08fb1-145">Имя параметра в отчете.</span><span class="sxs-lookup"><span data-stu-id="08fb1-145">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="08fb1-146">deviceId</span><span class="sxs-lookup"><span data-stu-id="08fb1-146">deviceId</span></span>|<span data-ttu-id="08fb1-147">String</span><span class="sxs-lookup"><span data-stu-id="08fb1-147">String</span></span>|<span data-ttu-id="08fb1-148">Идентификатор устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="08fb1-148">The Device Id that is being reported</span></span>|
|<span data-ttu-id="08fb1-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="08fb1-149">deviceName</span></span>|<span data-ttu-id="08fb1-150">String</span><span class="sxs-lookup"><span data-stu-id="08fb1-150">String</span></span>|<span data-ttu-id="08fb1-151">Имя устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="08fb1-151">The Device Name that is being reported</span></span>|
|<span data-ttu-id="08fb1-152">userId</span><span class="sxs-lookup"><span data-stu-id="08fb1-152">userId</span></span>|<span data-ttu-id="08fb1-153">String</span><span class="sxs-lookup"><span data-stu-id="08fb1-153">String</span></span>|<span data-ttu-id="08fb1-154">Идентификатор пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="08fb1-154">The user Id that is being reported</span></span>|
|<span data-ttu-id="08fb1-155">userEmail</span><span class="sxs-lookup"><span data-stu-id="08fb1-155">userEmail</span></span>|<span data-ttu-id="08fb1-156">String</span><span class="sxs-lookup"><span data-stu-id="08fb1-156">String</span></span>|<span data-ttu-id="08fb1-157">Адрес электронной почты пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="08fb1-157">The User email address that is being reported</span></span>|
|<span data-ttu-id="08fb1-158">userName</span><span class="sxs-lookup"><span data-stu-id="08fb1-158">userName</span></span>|<span data-ttu-id="08fb1-159">String</span><span class="sxs-lookup"><span data-stu-id="08fb1-159">String</span></span>|<span data-ttu-id="08fb1-160">Имя пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="08fb1-160">The User Name that is being reported</span></span>|
|<span data-ttu-id="08fb1-161">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="08fb1-161">userPrincipalName</span></span>|<span data-ttu-id="08fb1-162">String</span><span class="sxs-lookup"><span data-stu-id="08fb1-162">String</span></span>|<span data-ttu-id="08fb1-163">Имя участника-пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="08fb1-163">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="08fb1-164">deviceModel</span><span class="sxs-lookup"><span data-stu-id="08fb1-164">deviceModel</span></span>|<span data-ttu-id="08fb1-165">String</span><span class="sxs-lookup"><span data-stu-id="08fb1-165">String</span></span>|<span data-ttu-id="08fb1-166">Модель устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="08fb1-166">The device model that is being reported</span></span>|
|<span data-ttu-id="08fb1-167">state</span><span class="sxs-lookup"><span data-stu-id="08fb1-167">state</span></span>|[<span data-ttu-id="08fb1-168">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="08fb1-168">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="08fb1-169">Соответствие требованиям состояние параметра.</span><span class="sxs-lookup"><span data-stu-id="08fb1-169">The compliance state of the setting.</span></span> <span data-ttu-id="08fb1-170">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="08fb1-170">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="08fb1-171">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="08fb1-171">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="08fb1-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08fb1-172">DateTimeOffset</span></span>|<span data-ttu-id="08fb1-173">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="08fb1-173">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="08fb1-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="08fb1-174">Response</span></span>
<span data-ttu-id="08fb1-175">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="08fb1-175">If successful, this method returns a `201 Created` response code and a [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08fb1-176">Пример</span><span class="sxs-lookup"><span data-stu-id="08fb1-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="08fb1-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="08fb1-177">Request</span></span>
<span data-ttu-id="08fb1-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="08fb1-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="08fb1-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="08fb1-179">Response</span></span>
<span data-ttu-id="08fb1-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="08fb1-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




