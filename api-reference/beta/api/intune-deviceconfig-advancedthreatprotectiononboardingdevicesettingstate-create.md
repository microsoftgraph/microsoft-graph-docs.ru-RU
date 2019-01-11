---
title: Создание advancedThreatProtectionOnboardingDeviceSettingState
description: Создание нового объекта advancedThreatProtectionOnboardingDeviceSettingState.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 71a6e2f7c46acda723f1197a1c3b9302c63d47ae
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882259"
---
# <a name="create-advancedthreatprotectiononboardingdevicesettingstate"></a><span data-ttu-id="407a4-103">Создание advancedThreatProtectionOnboardingDeviceSettingState</span><span class="sxs-lookup"><span data-stu-id="407a4-103">Create advancedThreatProtectionOnboardingDeviceSettingState</span></span>

> <span data-ttu-id="407a4-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="407a4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="407a4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="407a4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="407a4-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="407a4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="407a4-107">Создание нового объекта [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) .</span><span class="sxs-lookup"><span data-stu-id="407a4-107">Create a new [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="407a4-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="407a4-108">Prerequisites</span></span>
<span data-ttu-id="407a4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="407a4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="407a4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="407a4-111">Permission type</span></span>|<span data-ttu-id="407a4-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="407a4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="407a4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="407a4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="407a4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="407a4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="407a4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="407a4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="407a4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="407a4-116">Not supported.</span></span>|
|<span data-ttu-id="407a4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="407a4-117">Application</span></span>|<span data-ttu-id="407a4-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="407a4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="407a4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="407a4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="407a4-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="407a4-120">Request headers</span></span>
|<span data-ttu-id="407a4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="407a4-121">Header</span></span>|<span data-ttu-id="407a4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="407a4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="407a4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="407a4-123">Authorization</span></span>|<span data-ttu-id="407a4-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="407a4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="407a4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="407a4-125">Accept</span></span>|<span data-ttu-id="407a4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="407a4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="407a4-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="407a4-127">Request body</span></span>
<span data-ttu-id="407a4-128">В тексте запроса укажите представление JSON для объекта advancedThreatProtectionOnboardingDeviceSettingState.</span><span class="sxs-lookup"><span data-stu-id="407a4-128">In the request body, supply a JSON representation for the advancedThreatProtectionOnboardingDeviceSettingState object.</span></span>

<span data-ttu-id="407a4-129">В следующей таблице показаны свойства, которые необходимы для создания advancedThreatProtectionOnboardingDeviceSettingState.</span><span class="sxs-lookup"><span data-stu-id="407a4-129">The following table shows the properties that are required when you create the advancedThreatProtectionOnboardingDeviceSettingState.</span></span>

|<span data-ttu-id="407a4-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="407a4-130">Property</span></span>|<span data-ttu-id="407a4-131">Тип</span><span class="sxs-lookup"><span data-stu-id="407a4-131">Type</span></span>|<span data-ttu-id="407a4-132">Описание</span><span class="sxs-lookup"><span data-stu-id="407a4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="407a4-133">id</span><span class="sxs-lookup"><span data-stu-id="407a4-133">id</span></span>|<span data-ttu-id="407a4-134">String</span><span class="sxs-lookup"><span data-stu-id="407a4-134">String</span></span>|<span data-ttu-id="407a4-135">Ключ объекта</span><span class="sxs-lookup"><span data-stu-id="407a4-135">Key of the entity</span></span>|
|<span data-ttu-id="407a4-136">platformType</span><span class="sxs-lookup"><span data-stu-id="407a4-136">platformType</span></span>|[<span data-ttu-id="407a4-137">deviceType</span><span class="sxs-lookup"><span data-stu-id="407a4-137">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="407a4-138">Тип платформы устройства.</span><span class="sxs-lookup"><span data-stu-id="407a4-138">Device platform type.</span></span> <span data-ttu-id="407a4-139">Возможные значения: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="407a4-139">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="407a4-140">setting</span><span class="sxs-lookup"><span data-stu-id="407a4-140">setting</span></span>|<span data-ttu-id="407a4-141">String</span><span class="sxs-lookup"><span data-stu-id="407a4-141">String</span></span>|<span data-ttu-id="407a4-142">Имя класса параметров и свойства.</span><span class="sxs-lookup"><span data-stu-id="407a4-142">The setting class name and property name.</span></span>|
|<span data-ttu-id="407a4-143">settingName</span><span class="sxs-lookup"><span data-stu-id="407a4-143">settingName</span></span>|<span data-ttu-id="407a4-144">String</span><span class="sxs-lookup"><span data-stu-id="407a4-144">String</span></span>|<span data-ttu-id="407a4-145">Имя параметра в отчете.</span><span class="sxs-lookup"><span data-stu-id="407a4-145">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="407a4-146">deviceId</span><span class="sxs-lookup"><span data-stu-id="407a4-146">deviceId</span></span>|<span data-ttu-id="407a4-147">String</span><span class="sxs-lookup"><span data-stu-id="407a4-147">String</span></span>|<span data-ttu-id="407a4-148">Идентификатор устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="407a4-148">The Device Id that is being reported</span></span>|
|<span data-ttu-id="407a4-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="407a4-149">deviceName</span></span>|<span data-ttu-id="407a4-150">String</span><span class="sxs-lookup"><span data-stu-id="407a4-150">String</span></span>|<span data-ttu-id="407a4-151">Имя устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="407a4-151">The Device Name that is being reported</span></span>|
|<span data-ttu-id="407a4-152">userId</span><span class="sxs-lookup"><span data-stu-id="407a4-152">userId</span></span>|<span data-ttu-id="407a4-153">String</span><span class="sxs-lookup"><span data-stu-id="407a4-153">String</span></span>|<span data-ttu-id="407a4-154">Идентификатор пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="407a4-154">The user Id that is being reported</span></span>|
|<span data-ttu-id="407a4-155">userEmail</span><span class="sxs-lookup"><span data-stu-id="407a4-155">userEmail</span></span>|<span data-ttu-id="407a4-156">String</span><span class="sxs-lookup"><span data-stu-id="407a4-156">String</span></span>|<span data-ttu-id="407a4-157">Адрес электронной почты пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="407a4-157">The User email address that is being reported</span></span>|
|<span data-ttu-id="407a4-158">userName</span><span class="sxs-lookup"><span data-stu-id="407a4-158">userName</span></span>|<span data-ttu-id="407a4-159">String</span><span class="sxs-lookup"><span data-stu-id="407a4-159">String</span></span>|<span data-ttu-id="407a4-160">Имя пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="407a4-160">The User Name that is being reported</span></span>|
|<span data-ttu-id="407a4-161">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="407a4-161">userPrincipalName</span></span>|<span data-ttu-id="407a4-162">String</span><span class="sxs-lookup"><span data-stu-id="407a4-162">String</span></span>|<span data-ttu-id="407a4-163">Имя участника-пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="407a4-163">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="407a4-164">deviceModel</span><span class="sxs-lookup"><span data-stu-id="407a4-164">deviceModel</span></span>|<span data-ttu-id="407a4-165">String</span><span class="sxs-lookup"><span data-stu-id="407a4-165">String</span></span>|<span data-ttu-id="407a4-166">Модель устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="407a4-166">The device model that is being reported</span></span>|
|<span data-ttu-id="407a4-167">state</span><span class="sxs-lookup"><span data-stu-id="407a4-167">state</span></span>|[<span data-ttu-id="407a4-168">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="407a4-168">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="407a4-169">Соответствие требованиям состояние параметра.</span><span class="sxs-lookup"><span data-stu-id="407a4-169">The compliance state of the setting.</span></span> <span data-ttu-id="407a4-170">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="407a4-170">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="407a4-171">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="407a4-171">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="407a4-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="407a4-172">DateTimeOffset</span></span>|<span data-ttu-id="407a4-173">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="407a4-173">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="407a4-174">Ответ</span><span class="sxs-lookup"><span data-stu-id="407a4-174">Response</span></span>
<span data-ttu-id="407a4-175">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="407a4-175">If successful, this method returns a `201 Created` response code and a [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="407a4-176">Пример</span><span class="sxs-lookup"><span data-stu-id="407a4-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="407a4-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="407a4-177">Request</span></span>
<span data-ttu-id="407a4-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="407a4-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="407a4-179">Ответ</span><span class="sxs-lookup"><span data-stu-id="407a4-179">Response</span></span>
<span data-ttu-id="407a4-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="407a4-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





