---
title: Update deviceComplianceSettingState
description: Обновление свойств объекта deviceComplianceSettingState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e012df2ca7c9f88b38582de46ebc1dd341cfa44b
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39949548"
---
# <a name="update-devicecompliancesettingstate"></a><span data-ttu-id="4a453-103">Update deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="4a453-103">Update deviceComplianceSettingState</span></span>

> <span data-ttu-id="4a453-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a453-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4a453-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4a453-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a453-106">Обновление свойств объекта [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="4a453-106">Update the properties of a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4a453-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="4a453-107">Prerequisites</span></span>
<span data-ttu-id="4a453-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a453-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a453-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4a453-110">Permission type</span></span>|<span data-ttu-id="4a453-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4a453-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4a453-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4a453-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4a453-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a453-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4a453-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4a453-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a453-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a453-115">Not supported.</span></span>|
|<span data-ttu-id="4a453-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4a453-116">Application</span></span>|<span data-ttu-id="4a453-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a453-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a453-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4a453-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

## <a name="request-headers"></a><span data-ttu-id="4a453-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4a453-119">Request headers</span></span>
|<span data-ttu-id="4a453-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4a453-120">Header</span></span>|<span data-ttu-id="4a453-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4a453-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4a453-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4a453-122">Authorization</span></span>|<span data-ttu-id="4a453-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4a453-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4a453-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4a453-124">Accept</span></span>|<span data-ttu-id="4a453-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4a453-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a453-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4a453-126">Request body</span></span>
<span data-ttu-id="4a453-127">В теле запроса добавьте представление объекта [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4a453-127">In the request body, supply a JSON representation for the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

<span data-ttu-id="4a453-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="4a453-128">The following table shows the properties that are required when you create the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span></span>

|<span data-ttu-id="4a453-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4a453-129">Property</span></span>|<span data-ttu-id="4a453-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4a453-130">Type</span></span>|<span data-ttu-id="4a453-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4a453-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a453-132">id</span><span class="sxs-lookup"><span data-stu-id="4a453-132">id</span></span>|<span data-ttu-id="4a453-133">Строка</span><span class="sxs-lookup"><span data-stu-id="4a453-133">String</span></span>|<span data-ttu-id="4a453-134">Ключ объекта</span><span class="sxs-lookup"><span data-stu-id="4a453-134">Key of the entity</span></span>|
|<span data-ttu-id="4a453-135">platformType</span><span class="sxs-lookup"><span data-stu-id="4a453-135">platformType</span></span>|[<span data-ttu-id="4a453-136">deviceType</span><span class="sxs-lookup"><span data-stu-id="4a453-136">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="4a453-137">Тип платформы устройства.</span><span class="sxs-lookup"><span data-stu-id="4a453-137">Device platform type.</span></span> <span data-ttu-id="4a453-138">Возможные значения: `desktop`, `windowsRT`, `winMO6`, `nokia` `windowsPhone` `mac` `winCE` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `blackberry` `palm` `iSocConsumer` `unknown`,,,,,,,,,,,,,,,,,,,,,,,,. `winEmbedded` `iPhone` `iPad` `iPod` `android`</span><span class="sxs-lookup"><span data-stu-id="4a453-138">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="4a453-139">setting</span><span class="sxs-lookup"><span data-stu-id="4a453-139">setting</span></span>|<span data-ttu-id="4a453-140">Строка</span><span class="sxs-lookup"><span data-stu-id="4a453-140">String</span></span>|<span data-ttu-id="4a453-141">Имя класса параметров и свойства.</span><span class="sxs-lookup"><span data-stu-id="4a453-141">The setting class name and property name.</span></span>|
|<span data-ttu-id="4a453-142">settingName</span><span class="sxs-lookup"><span data-stu-id="4a453-142">settingName</span></span>|<span data-ttu-id="4a453-143">Строка</span><span class="sxs-lookup"><span data-stu-id="4a453-143">String</span></span>|<span data-ttu-id="4a453-144">Имя параметра в отчете</span><span class="sxs-lookup"><span data-stu-id="4a453-144">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="4a453-145">deviceId</span><span class="sxs-lookup"><span data-stu-id="4a453-145">deviceId</span></span>|<span data-ttu-id="4a453-146">Строка</span><span class="sxs-lookup"><span data-stu-id="4a453-146">String</span></span>|<span data-ttu-id="4a453-147">ИД устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="4a453-147">The Device Id that is being reported</span></span>|
|<span data-ttu-id="4a453-148">deviceName</span><span class="sxs-lookup"><span data-stu-id="4a453-148">deviceName</span></span>|<span data-ttu-id="4a453-149">Строка</span><span class="sxs-lookup"><span data-stu-id="4a453-149">String</span></span>|<span data-ttu-id="4a453-150">Имя устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="4a453-150">The Device Name that is being reported</span></span>|
|<span data-ttu-id="4a453-151">userId</span><span class="sxs-lookup"><span data-stu-id="4a453-151">userId</span></span>|<span data-ttu-id="4a453-152">String</span><span class="sxs-lookup"><span data-stu-id="4a453-152">String</span></span>|<span data-ttu-id="4a453-153">ИД пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="4a453-153">The user Id that is being reported</span></span>|
|<span data-ttu-id="4a453-154">userEmail</span><span class="sxs-lookup"><span data-stu-id="4a453-154">userEmail</span></span>|<span data-ttu-id="4a453-155">String</span><span class="sxs-lookup"><span data-stu-id="4a453-155">String</span></span>|<span data-ttu-id="4a453-156">Электронный адрес пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="4a453-156">The User email address that is being reported</span></span>|
|<span data-ttu-id="4a453-157">userName</span><span class="sxs-lookup"><span data-stu-id="4a453-157">userName</span></span>|<span data-ttu-id="4a453-158">Строка</span><span class="sxs-lookup"><span data-stu-id="4a453-158">String</span></span>|<span data-ttu-id="4a453-159">Имя пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="4a453-159">The User Name that is being reported</span></span>|
|<span data-ttu-id="4a453-160">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4a453-160">userPrincipalName</span></span>|<span data-ttu-id="4a453-161">String</span><span class="sxs-lookup"><span data-stu-id="4a453-161">String</span></span>|<span data-ttu-id="4a453-162">Имя участника-пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="4a453-162">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="4a453-163">deviceModel</span><span class="sxs-lookup"><span data-stu-id="4a453-163">deviceModel</span></span>|<span data-ttu-id="4a453-164">Строка</span><span class="sxs-lookup"><span data-stu-id="4a453-164">String</span></span>|<span data-ttu-id="4a453-165">Модель устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="4a453-165">The device model that is being reported</span></span>|
|<span data-ttu-id="4a453-166">state</span><span class="sxs-lookup"><span data-stu-id="4a453-166">state</span></span>|[<span data-ttu-id="4a453-167">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="4a453-167">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="4a453-168">Состояние соответствия для параметра.</span><span class="sxs-lookup"><span data-stu-id="4a453-168">The compliance state of the setting.</span></span> <span data-ttu-id="4a453-169">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="4a453-169">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="4a453-170">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="4a453-170">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="4a453-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a453-171">DateTimeOffset</span></span>|<span data-ttu-id="4a453-172">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="4a453-172">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="4a453-173">Ответ</span><span class="sxs-lookup"><span data-stu-id="4a453-173">Response</span></span>
<span data-ttu-id="4a453-174">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4a453-174">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a453-175">Пример</span><span class="sxs-lookup"><span data-stu-id="4a453-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="4a453-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a453-176">Request</span></span>
<span data-ttu-id="4a453-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4a453-177">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
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

### <a name="response"></a><span data-ttu-id="4a453-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a453-178">Response</span></span>
<span data-ttu-id="4a453-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4a453-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





