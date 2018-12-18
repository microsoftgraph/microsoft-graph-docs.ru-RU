---
title: Обновление advancedThreatProtectionOnboardingDeviceSettingState
description: Обновление свойства объекта advancedThreatProtectionOnboardingDeviceSettingState.
author: tfitzmac
ms.openlocfilehash: 0194eca0c9d36c7d0e4e24cca6eb276beb7d49e3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321695"
---
# <a name="update-advancedthreatprotectiononboardingdevicesettingstate"></a><span data-ttu-id="eecde-103">Обновление advancedThreatProtectionOnboardingDeviceSettingState</span><span class="sxs-lookup"><span data-stu-id="eecde-103">Update advancedThreatProtectionOnboardingDeviceSettingState</span></span>

> <span data-ttu-id="eecde-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="eecde-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eecde-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eecde-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="eecde-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="eecde-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eecde-107">Обновление свойства объекта [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) .</span><span class="sxs-lookup"><span data-stu-id="eecde-107">Update the properties of a [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="eecde-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="eecde-108">Prerequisites</span></span>
<span data-ttu-id="eecde-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eecde-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eecde-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eecde-111">Permission type</span></span>|<span data-ttu-id="eecde-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="eecde-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eecde-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eecde-113">Delegated (work or school account)</span></span>|<span data-ttu-id="eecde-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eecde-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="eecde-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eecde-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eecde-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eecde-116">Not supported.</span></span>|
|<span data-ttu-id="eecde-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eecde-117">Application</span></span>|<span data-ttu-id="eecde-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eecde-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eecde-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eecde-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates/{advancedThreatProtectionOnboardingDeviceSettingStateId}
```

## <a name="request-headers"></a><span data-ttu-id="eecde-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eecde-120">Request headers</span></span>
|<span data-ttu-id="eecde-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="eecde-121">Header</span></span>|<span data-ttu-id="eecde-122">Значение</span><span class="sxs-lookup"><span data-stu-id="eecde-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eecde-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eecde-123">Authorization</span></span>|<span data-ttu-id="eecde-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="eecde-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eecde-125">Accept</span><span class="sxs-lookup"><span data-stu-id="eecde-125">Accept</span></span>|<span data-ttu-id="eecde-126">application/json</span><span class="sxs-lookup"><span data-stu-id="eecde-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eecde-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eecde-127">Request body</span></span>
<span data-ttu-id="eecde-128">В тексте запроса укажите представление JSON для объекта [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) .</span><span class="sxs-lookup"><span data-stu-id="eecde-128">In the request body, supply a JSON representation for the [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object.</span></span>

<span data-ttu-id="eecde-129">В следующей таблице показаны свойства, которые необходимы для создания [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="eecde-129">The following table shows the properties that are required when you create the [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md).</span></span>

|<span data-ttu-id="eecde-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="eecde-130">Property</span></span>|<span data-ttu-id="eecde-131">Тип</span><span class="sxs-lookup"><span data-stu-id="eecde-131">Type</span></span>|<span data-ttu-id="eecde-132">Описание</span><span class="sxs-lookup"><span data-stu-id="eecde-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eecde-133">id</span><span class="sxs-lookup"><span data-stu-id="eecde-133">id</span></span>|<span data-ttu-id="eecde-134">String</span><span class="sxs-lookup"><span data-stu-id="eecde-134">String</span></span>|<span data-ttu-id="eecde-135">Ключ объекта</span><span class="sxs-lookup"><span data-stu-id="eecde-135">Key of the entity</span></span>|
|<span data-ttu-id="eecde-136">platformType</span><span class="sxs-lookup"><span data-stu-id="eecde-136">platformType</span></span>|[<span data-ttu-id="eecde-137">deviceType</span><span class="sxs-lookup"><span data-stu-id="eecde-137">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="eecde-138">Тип платформы устройства.</span><span class="sxs-lookup"><span data-stu-id="eecde-138">Device platform type.</span></span> <span data-ttu-id="eecde-139">Возможные значения: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="eecde-139">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="eecde-140">setting</span><span class="sxs-lookup"><span data-stu-id="eecde-140">setting</span></span>|<span data-ttu-id="eecde-141">String</span><span class="sxs-lookup"><span data-stu-id="eecde-141">String</span></span>|<span data-ttu-id="eecde-142">Имя класса параметров и свойства.</span><span class="sxs-lookup"><span data-stu-id="eecde-142">The setting class name and property name.</span></span>|
|<span data-ttu-id="eecde-143">settingName</span><span class="sxs-lookup"><span data-stu-id="eecde-143">settingName</span></span>|<span data-ttu-id="eecde-144">String</span><span class="sxs-lookup"><span data-stu-id="eecde-144">String</span></span>|<span data-ttu-id="eecde-145">Имя параметра в отчете.</span><span class="sxs-lookup"><span data-stu-id="eecde-145">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="eecde-146">deviceId</span><span class="sxs-lookup"><span data-stu-id="eecde-146">deviceId</span></span>|<span data-ttu-id="eecde-147">String</span><span class="sxs-lookup"><span data-stu-id="eecde-147">String</span></span>|<span data-ttu-id="eecde-148">Идентификатор устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="eecde-148">The Device Id that is being reported</span></span>|
|<span data-ttu-id="eecde-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="eecde-149">deviceName</span></span>|<span data-ttu-id="eecde-150">String</span><span class="sxs-lookup"><span data-stu-id="eecde-150">String</span></span>|<span data-ttu-id="eecde-151">Имя устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="eecde-151">The Device Name that is being reported</span></span>|
|<span data-ttu-id="eecde-152">userId</span><span class="sxs-lookup"><span data-stu-id="eecde-152">userId</span></span>|<span data-ttu-id="eecde-153">String</span><span class="sxs-lookup"><span data-stu-id="eecde-153">String</span></span>|<span data-ttu-id="eecde-154">Идентификатор пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="eecde-154">The user Id that is being reported</span></span>|
|<span data-ttu-id="eecde-155">userEmail</span><span class="sxs-lookup"><span data-stu-id="eecde-155">userEmail</span></span>|<span data-ttu-id="eecde-156">String</span><span class="sxs-lookup"><span data-stu-id="eecde-156">String</span></span>|<span data-ttu-id="eecde-157">Адрес электронной почты пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="eecde-157">The User email address that is being reported</span></span>|
|<span data-ttu-id="eecde-158">userName</span><span class="sxs-lookup"><span data-stu-id="eecde-158">userName</span></span>|<span data-ttu-id="eecde-159">String</span><span class="sxs-lookup"><span data-stu-id="eecde-159">String</span></span>|<span data-ttu-id="eecde-160">Имя пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="eecde-160">The User Name that is being reported</span></span>|
|<span data-ttu-id="eecde-161">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="eecde-161">userPrincipalName</span></span>|<span data-ttu-id="eecde-162">String</span><span class="sxs-lookup"><span data-stu-id="eecde-162">String</span></span>|<span data-ttu-id="eecde-163">Имя участника-пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="eecde-163">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="eecde-164">deviceModel</span><span class="sxs-lookup"><span data-stu-id="eecde-164">deviceModel</span></span>|<span data-ttu-id="eecde-165">String</span><span class="sxs-lookup"><span data-stu-id="eecde-165">String</span></span>|<span data-ttu-id="eecde-166">Модель устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="eecde-166">The device model that is being reported</span></span>|
|<span data-ttu-id="eecde-167">state</span><span class="sxs-lookup"><span data-stu-id="eecde-167">state</span></span>|[<span data-ttu-id="eecde-168">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="eecde-168">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="eecde-169">Соответствие требованиям состояние параметра.</span><span class="sxs-lookup"><span data-stu-id="eecde-169">The compliance state of the setting.</span></span> <span data-ttu-id="eecde-170">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="eecde-170">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="eecde-171">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="eecde-171">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="eecde-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eecde-172">DateTimeOffset</span></span>|<span data-ttu-id="eecde-173">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="eecde-173">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="eecde-174">Ответ</span><span class="sxs-lookup"><span data-stu-id="eecde-174">Response</span></span>
<span data-ttu-id="eecde-175">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="eecde-175">If successful, this method returns a `200 OK` response code and an updated [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eecde-176">Пример</span><span class="sxs-lookup"><span data-stu-id="eecde-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="eecde-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="eecde-177">Request</span></span>
<span data-ttu-id="eecde-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eecde-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates/{advancedThreatProtectionOnboardingDeviceSettingStateId}
Content-type: application/json
Content-length: 482

{
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

### <a name="response"></a><span data-ttu-id="eecde-179">Ответ</span><span class="sxs-lookup"><span data-stu-id="eecde-179">Response</span></span>
<span data-ttu-id="eecde-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="eecde-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





