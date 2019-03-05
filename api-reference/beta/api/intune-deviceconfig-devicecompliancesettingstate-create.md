---
title: Создание объекта deviceComplianceSettingState
description: Создание объекта deviceComplianceSettingState.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8e28121ec0596d11bead62b0622d115c5c8f46d4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145481"
---
# <a name="create-devicecompliancesettingstate"></a><span data-ttu-id="fe9f0-103">Создание объекта deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="fe9f0-103">Create deviceComplianceSettingState</span></span>

> <span data-ttu-id="fe9f0-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe9f0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fe9f0-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fe9f0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe9f0-106">Создание объекта [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="fe9f0-106">Create a new [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fe9f0-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="fe9f0-107">Prerequisites</span></span>
<span data-ttu-id="fe9f0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="fe9f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fe9f0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fe9f0-110">Permission type</span></span>|<span data-ttu-id="fe9f0-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fe9f0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe9f0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fe9f0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fe9f0-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe9f0-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fe9f0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fe9f0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe9f0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe9f0-115">Not supported.</span></span>|
|<span data-ttu-id="fe9f0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fe9f0-116">Application</span></span>|<span data-ttu-id="fe9f0-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe9f0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe9f0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fe9f0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="fe9f0-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fe9f0-119">Request headers</span></span>
|<span data-ttu-id="fe9f0-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fe9f0-120">Header</span></span>|<span data-ttu-id="fe9f0-121">Значение</span><span class="sxs-lookup"><span data-stu-id="fe9f0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe9f0-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fe9f0-122">Authorization</span></span>|<span data-ttu-id="fe9f0-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="fe9f0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fe9f0-124">Accept</span><span class="sxs-lookup"><span data-stu-id="fe9f0-124">Accept</span></span>|<span data-ttu-id="fe9f0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fe9f0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe9f0-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fe9f0-126">Request body</span></span>
<span data-ttu-id="fe9f0-127">В тексте запроса добавьте представление объекта deviceComplianceSettingState в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fe9f0-127">In the request body, supply a JSON representation for the deviceComplianceSettingState object.</span></span>

<span data-ttu-id="fe9f0-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceComplianceSettingState.</span><span class="sxs-lookup"><span data-stu-id="fe9f0-128">The following table shows the properties that are required when you create the deviceComplianceSettingState.</span></span>

|<span data-ttu-id="fe9f0-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="fe9f0-129">Property</span></span>|<span data-ttu-id="fe9f0-130">Тип</span><span class="sxs-lookup"><span data-stu-id="fe9f0-130">Type</span></span>|<span data-ttu-id="fe9f0-131">Описание</span><span class="sxs-lookup"><span data-stu-id="fe9f0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe9f0-132">id</span><span class="sxs-lookup"><span data-stu-id="fe9f0-132">id</span></span>|<span data-ttu-id="fe9f0-133">String</span><span class="sxs-lookup"><span data-stu-id="fe9f0-133">String</span></span>|<span data-ttu-id="fe9f0-134">Ключ объекта</span><span class="sxs-lookup"><span data-stu-id="fe9f0-134">Key of the entity</span></span>|
|<span data-ttu-id="fe9f0-135">platformType</span><span class="sxs-lookup"><span data-stu-id="fe9f0-135">platformType</span></span>|[<span data-ttu-id="fe9f0-136">deviceType</span><span class="sxs-lookup"><span data-stu-id="fe9f0-136">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="fe9f0-137">Тип платформы устройства.</span><span class="sxs-lookup"><span data-stu-id="fe9f0-137">Device platform type.</span></span> <span data-ttu-id="fe9f0-138">Возможные значения: `desktop`, `windowsRT`, `winMO6`, `nokia` `windowsPhone` `mac` `winCE` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `android` `iSocConsumer`,,,,,,,,,,,,,,,,,,,,, `winEmbedded` `iPhone` `iPad` `iPod` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="fe9f0-138">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="fe9f0-139">setting</span><span class="sxs-lookup"><span data-stu-id="fe9f0-139">setting</span></span>|<span data-ttu-id="fe9f0-140">String</span><span class="sxs-lookup"><span data-stu-id="fe9f0-140">String</span></span>|<span data-ttu-id="fe9f0-141">Имя класса параметров и свойства.</span><span class="sxs-lookup"><span data-stu-id="fe9f0-141">The setting class name and property name.</span></span>|
|<span data-ttu-id="fe9f0-142">settingName</span><span class="sxs-lookup"><span data-stu-id="fe9f0-142">settingName</span></span>|<span data-ttu-id="fe9f0-143">String</span><span class="sxs-lookup"><span data-stu-id="fe9f0-143">String</span></span>|<span data-ttu-id="fe9f0-144">Имя параметра в отчете.</span><span class="sxs-lookup"><span data-stu-id="fe9f0-144">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="fe9f0-145">deviceId</span><span class="sxs-lookup"><span data-stu-id="fe9f0-145">deviceId</span></span>|<span data-ttu-id="fe9f0-146">String</span><span class="sxs-lookup"><span data-stu-id="fe9f0-146">String</span></span>|<span data-ttu-id="fe9f0-147">Идентификатор устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="fe9f0-147">The Device Id that is being reported</span></span>|
|<span data-ttu-id="fe9f0-148">deviceName</span><span class="sxs-lookup"><span data-stu-id="fe9f0-148">deviceName</span></span>|<span data-ttu-id="fe9f0-149">String</span><span class="sxs-lookup"><span data-stu-id="fe9f0-149">String</span></span>|<span data-ttu-id="fe9f0-150">Имя устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="fe9f0-150">The Device Name that is being reported</span></span>|
|<span data-ttu-id="fe9f0-151">userId</span><span class="sxs-lookup"><span data-stu-id="fe9f0-151">userId</span></span>|<span data-ttu-id="fe9f0-152">String</span><span class="sxs-lookup"><span data-stu-id="fe9f0-152">String</span></span>|<span data-ttu-id="fe9f0-153">Идентификатор пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="fe9f0-153">The user Id that is being reported</span></span>|
|<span data-ttu-id="fe9f0-154">userEmail</span><span class="sxs-lookup"><span data-stu-id="fe9f0-154">userEmail</span></span>|<span data-ttu-id="fe9f0-155">String</span><span class="sxs-lookup"><span data-stu-id="fe9f0-155">String</span></span>|<span data-ttu-id="fe9f0-156">Адрес электронной почты пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="fe9f0-156">The User email address that is being reported</span></span>|
|<span data-ttu-id="fe9f0-157">userName</span><span class="sxs-lookup"><span data-stu-id="fe9f0-157">userName</span></span>|<span data-ttu-id="fe9f0-158">String</span><span class="sxs-lookup"><span data-stu-id="fe9f0-158">String</span></span>|<span data-ttu-id="fe9f0-159">Имя пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="fe9f0-159">The User Name that is being reported</span></span>|
|<span data-ttu-id="fe9f0-160">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="fe9f0-160">userPrincipalName</span></span>|<span data-ttu-id="fe9f0-161">String</span><span class="sxs-lookup"><span data-stu-id="fe9f0-161">String</span></span>|<span data-ttu-id="fe9f0-162">Имя участника-пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="fe9f0-162">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="fe9f0-163">deviceModel</span><span class="sxs-lookup"><span data-stu-id="fe9f0-163">deviceModel</span></span>|<span data-ttu-id="fe9f0-164">String</span><span class="sxs-lookup"><span data-stu-id="fe9f0-164">String</span></span>|<span data-ttu-id="fe9f0-165">Модель устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="fe9f0-165">The device model that is being reported</span></span>|
|<span data-ttu-id="fe9f0-166">state</span><span class="sxs-lookup"><span data-stu-id="fe9f0-166">state</span></span>|[<span data-ttu-id="fe9f0-167">Комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="fe9f0-167">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="fe9f0-168">Состояние соответствия для параметра.</span><span class="sxs-lookup"><span data-stu-id="fe9f0-168">The compliance state of the setting.</span></span> <span data-ttu-id="fe9f0-169">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="fe9f0-169">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="fe9f0-170">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="fe9f0-170">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="fe9f0-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe9f0-171">DateTimeOffset</span></span>|<span data-ttu-id="fe9f0-172">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="fe9f0-172">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="fe9f0-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe9f0-173">Response</span></span>
<span data-ttu-id="fe9f0-174">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fe9f0-174">If successful, this method returns a `201 Created` response code and a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe9f0-175">Пример</span><span class="sxs-lookup"><span data-stu-id="fe9f0-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="fe9f0-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="fe9f0-176">Request</span></span>
<span data-ttu-id="fe9f0-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fe9f0-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
Content-type: application/json
Content-length: 549

{
  "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
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

### <a name="response"></a><span data-ttu-id="fe9f0-178">Ответ</span><span class="sxs-lookup"><span data-stu-id="fe9f0-178">Response</span></span>
<span data-ttu-id="fe9f0-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fe9f0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 598

{
  "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
  "id": "9905f955-f955-9905-55f9-059955f90599",
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




