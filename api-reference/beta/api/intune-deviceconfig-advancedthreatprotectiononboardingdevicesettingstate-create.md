---
title: Создание advancedThreatProtectionOnboardingDeviceSettingState
description: Создайте новый расширенный объектThreatProtectionOnboardingDeviceSettingState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 682954bc04f1660b3c8bf651ced705e58dada259
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51126922"
---
# <a name="create-advancedthreatprotectiononboardingdevicesettingstate"></a><span data-ttu-id="b2322-103">Создание advancedThreatProtectionOnboardingDeviceSettingState</span><span class="sxs-lookup"><span data-stu-id="b2322-103">Create advancedThreatProtectionOnboardingDeviceSettingState</span></span>

<span data-ttu-id="b2322-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2322-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b2322-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2322-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2322-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b2322-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2322-107">Создайте новый [расширенный объектThreatProtectionOnboardingDeviceSettingState.](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)</span><span class="sxs-lookup"><span data-stu-id="b2322-107">Create a new [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b2322-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b2322-108">Prerequisites</span></span>
<span data-ttu-id="b2322-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2322-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2322-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b2322-111">Permission type</span></span>|<span data-ttu-id="b2322-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b2322-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2322-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b2322-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b2322-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2322-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b2322-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b2322-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2322-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2322-116">Not supported.</span></span>|
|<span data-ttu-id="b2322-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="b2322-117">Application</span></span>|<span data-ttu-id="b2322-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2322-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2322-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b2322-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="b2322-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b2322-120">Request headers</span></span>
|<span data-ttu-id="b2322-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b2322-121">Header</span></span>|<span data-ttu-id="b2322-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b2322-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2322-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2322-123">Authorization</span></span>|<span data-ttu-id="b2322-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b2322-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2322-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b2322-125">Accept</span></span>|<span data-ttu-id="b2322-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b2322-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2322-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b2322-127">Request body</span></span>
<span data-ttu-id="b2322-128">В теле запроса подарйте представление JSON для объекта advancedThreatProtectionOnboardingDeviceSettingState.</span><span class="sxs-lookup"><span data-stu-id="b2322-128">In the request body, supply a JSON representation for the advancedThreatProtectionOnboardingDeviceSettingState object.</span></span>

<span data-ttu-id="b2322-129">В следующей таблице показаны свойства, необходимые при создании advancedThreatProtectionOnboardingDeviceSettingState.</span><span class="sxs-lookup"><span data-stu-id="b2322-129">The following table shows the properties that are required when you create the advancedThreatProtectionOnboardingDeviceSettingState.</span></span>

|<span data-ttu-id="b2322-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b2322-130">Property</span></span>|<span data-ttu-id="b2322-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b2322-131">Type</span></span>|<span data-ttu-id="b2322-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b2322-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2322-133">id</span><span class="sxs-lookup"><span data-stu-id="b2322-133">id</span></span>|<span data-ttu-id="b2322-134">Строка</span><span class="sxs-lookup"><span data-stu-id="b2322-134">String</span></span>|<span data-ttu-id="b2322-135">Ключ объекта</span><span class="sxs-lookup"><span data-stu-id="b2322-135">Key of the entity</span></span>|
|<span data-ttu-id="b2322-136">platformType</span><span class="sxs-lookup"><span data-stu-id="b2322-136">platformType</span></span>|[<span data-ttu-id="b2322-137">deviceType</span><span class="sxs-lookup"><span data-stu-id="b2322-137">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="b2322-138">Тип платформы устройства.</span><span class="sxs-lookup"><span data-stu-id="b2322-138">Device platform type.</span></span> <span data-ttu-id="b2322-139">Возможные значения: `desktop` `windowsRT` , `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `cloudPC` `blackberry` `palm` . `unknown`</span><span class="sxs-lookup"><span data-stu-id="b2322-139">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `androidnGMS`, `cloudPC`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="b2322-140">setting</span><span class="sxs-lookup"><span data-stu-id="b2322-140">setting</span></span>|<span data-ttu-id="b2322-141">String</span><span class="sxs-lookup"><span data-stu-id="b2322-141">String</span></span>|<span data-ttu-id="b2322-142">Имя класса параметров и свойства.</span><span class="sxs-lookup"><span data-stu-id="b2322-142">The setting class name and property name.</span></span>|
|<span data-ttu-id="b2322-143">settingName</span><span class="sxs-lookup"><span data-stu-id="b2322-143">settingName</span></span>|<span data-ttu-id="b2322-144">String</span><span class="sxs-lookup"><span data-stu-id="b2322-144">String</span></span>|<span data-ttu-id="b2322-145">Имя параметра в отчете</span><span class="sxs-lookup"><span data-stu-id="b2322-145">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="b2322-146">deviceId</span><span class="sxs-lookup"><span data-stu-id="b2322-146">deviceId</span></span>|<span data-ttu-id="b2322-147">String</span><span class="sxs-lookup"><span data-stu-id="b2322-147">String</span></span>|<span data-ttu-id="b2322-148">ИД устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="b2322-148">The Device Id that is being reported</span></span>|
|<span data-ttu-id="b2322-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="b2322-149">deviceName</span></span>|<span data-ttu-id="b2322-150">String</span><span class="sxs-lookup"><span data-stu-id="b2322-150">String</span></span>|<span data-ttu-id="b2322-151">Имя устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="b2322-151">The Device Name that is being reported</span></span>|
|<span data-ttu-id="b2322-152">userId</span><span class="sxs-lookup"><span data-stu-id="b2322-152">userId</span></span>|<span data-ttu-id="b2322-153">String</span><span class="sxs-lookup"><span data-stu-id="b2322-153">String</span></span>|<span data-ttu-id="b2322-154">ИД пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="b2322-154">The user Id that is being reported</span></span>|
|<span data-ttu-id="b2322-155">userEmail</span><span class="sxs-lookup"><span data-stu-id="b2322-155">userEmail</span></span>|<span data-ttu-id="b2322-156">String</span><span class="sxs-lookup"><span data-stu-id="b2322-156">String</span></span>|<span data-ttu-id="b2322-157">Электронный адрес пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="b2322-157">The User email address that is being reported</span></span>|
|<span data-ttu-id="b2322-158">userName</span><span class="sxs-lookup"><span data-stu-id="b2322-158">userName</span></span>|<span data-ttu-id="b2322-159">String</span><span class="sxs-lookup"><span data-stu-id="b2322-159">String</span></span>|<span data-ttu-id="b2322-160">Имя пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="b2322-160">The User Name that is being reported</span></span>|
|<span data-ttu-id="b2322-161">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b2322-161">userPrincipalName</span></span>|<span data-ttu-id="b2322-162">String</span><span class="sxs-lookup"><span data-stu-id="b2322-162">String</span></span>|<span data-ttu-id="b2322-163">Имя участника-пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="b2322-163">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="b2322-164">deviceModel</span><span class="sxs-lookup"><span data-stu-id="b2322-164">deviceModel</span></span>|<span data-ttu-id="b2322-165">String</span><span class="sxs-lookup"><span data-stu-id="b2322-165">String</span></span>|<span data-ttu-id="b2322-166">Модель устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="b2322-166">The device model that is being reported</span></span>|
|<span data-ttu-id="b2322-167">state</span><span class="sxs-lookup"><span data-stu-id="b2322-167">state</span></span>|[<span data-ttu-id="b2322-168">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="b2322-168">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="b2322-169">Состояние соответствия параметру.</span><span class="sxs-lookup"><span data-stu-id="b2322-169">The compliance state of the setting.</span></span> <span data-ttu-id="b2322-170">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="b2322-170">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="b2322-171">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="b2322-171">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="b2322-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2322-172">DateTimeOffset</span></span>|<span data-ttu-id="b2322-173">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="b2322-173">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="b2322-174">Ответ</span><span class="sxs-lookup"><span data-stu-id="b2322-174">Response</span></span>
<span data-ttu-id="b2322-175">В случае успешной работы этот метод возвращает код ответа и расширенный `201 Created` [объектThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b2322-175">If successful, this method returns a `201 Created` response code and a [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2322-176">Пример</span><span class="sxs-lookup"><span data-stu-id="b2322-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="b2322-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="b2322-177">Request</span></span>
<span data-ttu-id="b2322-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b2322-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b2322-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2322-179">Response</span></span>
<span data-ttu-id="b2322-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b2322-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




