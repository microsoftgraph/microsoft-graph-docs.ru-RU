---
title: Создание объекта deviceComplianceSettingState
description: Создание объекта deviceComplianceSettingState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7f31cf3bae143d92ba981cab2f6eea1391cb1044
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49213905"
---
# <a name="create-devicecompliancesettingstate"></a><span data-ttu-id="1b3c2-103">Создание объекта deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="1b3c2-103">Create deviceComplianceSettingState</span></span>

<span data-ttu-id="1b3c2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b3c2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1b3c2-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b3c2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1b3c2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1b3c2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b3c2-107">Создание объекта [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="1b3c2-107">Create a new [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1b3c2-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1b3c2-108">Prerequisites</span></span>
<span data-ttu-id="1b3c2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b3c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b3c2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1b3c2-111">Permission type</span></span>|<span data-ttu-id="1b3c2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1b3c2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1b3c2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1b3c2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1b3c2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b3c2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1b3c2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1b3c2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1b3c2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b3c2-116">Not supported.</span></span>|
|<span data-ttu-id="1b3c2-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="1b3c2-117">Application</span></span>|<span data-ttu-id="1b3c2-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b3c2-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1b3c2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1b3c2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="1b3c2-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1b3c2-120">Request headers</span></span>
|<span data-ttu-id="1b3c2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1b3c2-121">Header</span></span>|<span data-ttu-id="1b3c2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1b3c2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1b3c2-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1b3c2-123">Authorization</span></span>|<span data-ttu-id="1b3c2-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1b3c2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1b3c2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1b3c2-125">Accept</span></span>|<span data-ttu-id="1b3c2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1b3c2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b3c2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1b3c2-127">Request body</span></span>
<span data-ttu-id="1b3c2-128">В тексте запроса добавьте представление объекта deviceComplianceSettingState в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1b3c2-128">In the request body, supply a JSON representation for the deviceComplianceSettingState object.</span></span>

<span data-ttu-id="1b3c2-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceComplianceSettingState.</span><span class="sxs-lookup"><span data-stu-id="1b3c2-129">The following table shows the properties that are required when you create the deviceComplianceSettingState.</span></span>

|<span data-ttu-id="1b3c2-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1b3c2-130">Property</span></span>|<span data-ttu-id="1b3c2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1b3c2-131">Type</span></span>|<span data-ttu-id="1b3c2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1b3c2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b3c2-133">id</span><span class="sxs-lookup"><span data-stu-id="1b3c2-133">id</span></span>|<span data-ttu-id="1b3c2-134">String</span><span class="sxs-lookup"><span data-stu-id="1b3c2-134">String</span></span>|<span data-ttu-id="1b3c2-135">Ключ объекта</span><span class="sxs-lookup"><span data-stu-id="1b3c2-135">Key of the entity</span></span>|
|<span data-ttu-id="1b3c2-136">platformType</span><span class="sxs-lookup"><span data-stu-id="1b3c2-136">platformType</span></span>|[<span data-ttu-id="1b3c2-137">deviceType</span><span class="sxs-lookup"><span data-stu-id="1b3c2-137">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="1b3c2-138">Тип платформы устройства.</span><span class="sxs-lookup"><span data-stu-id="1b3c2-138">Device platform type.</span></span> <span data-ttu-id="1b3c2-139">Возможные значения:,,,,,,,,,,, `desktop` `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` , `unix` ,,, `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `cloudPC` `blackberry` `palm` ,, `unknown` ,,,,,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="1b3c2-139">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `androidnGMS`, `cloudPC`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="1b3c2-140">setting</span><span class="sxs-lookup"><span data-stu-id="1b3c2-140">setting</span></span>|<span data-ttu-id="1b3c2-141">String</span><span class="sxs-lookup"><span data-stu-id="1b3c2-141">String</span></span>|<span data-ttu-id="1b3c2-142">Имя класса параметров и свойства.</span><span class="sxs-lookup"><span data-stu-id="1b3c2-142">The setting class name and property name.</span></span>|
|<span data-ttu-id="1b3c2-143">settingName</span><span class="sxs-lookup"><span data-stu-id="1b3c2-143">settingName</span></span>|<span data-ttu-id="1b3c2-144">String</span><span class="sxs-lookup"><span data-stu-id="1b3c2-144">String</span></span>|<span data-ttu-id="1b3c2-145">Имя параметра в отчете</span><span class="sxs-lookup"><span data-stu-id="1b3c2-145">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="1b3c2-146">deviceId</span><span class="sxs-lookup"><span data-stu-id="1b3c2-146">deviceId</span></span>|<span data-ttu-id="1b3c2-147">String</span><span class="sxs-lookup"><span data-stu-id="1b3c2-147">String</span></span>|<span data-ttu-id="1b3c2-148">ИД устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="1b3c2-148">The Device Id that is being reported</span></span>|
|<span data-ttu-id="1b3c2-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="1b3c2-149">deviceName</span></span>|<span data-ttu-id="1b3c2-150">String</span><span class="sxs-lookup"><span data-stu-id="1b3c2-150">String</span></span>|<span data-ttu-id="1b3c2-151">Имя устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="1b3c2-151">The Device Name that is being reported</span></span>|
|<span data-ttu-id="1b3c2-152">userId</span><span class="sxs-lookup"><span data-stu-id="1b3c2-152">userId</span></span>|<span data-ttu-id="1b3c2-153">String</span><span class="sxs-lookup"><span data-stu-id="1b3c2-153">String</span></span>|<span data-ttu-id="1b3c2-154">ИД пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="1b3c2-154">The user Id that is being reported</span></span>|
|<span data-ttu-id="1b3c2-155">userEmail</span><span class="sxs-lookup"><span data-stu-id="1b3c2-155">userEmail</span></span>|<span data-ttu-id="1b3c2-156">String</span><span class="sxs-lookup"><span data-stu-id="1b3c2-156">String</span></span>|<span data-ttu-id="1b3c2-157">Электронный адрес пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="1b3c2-157">The User email address that is being reported</span></span>|
|<span data-ttu-id="1b3c2-158">userName</span><span class="sxs-lookup"><span data-stu-id="1b3c2-158">userName</span></span>|<span data-ttu-id="1b3c2-159">String</span><span class="sxs-lookup"><span data-stu-id="1b3c2-159">String</span></span>|<span data-ttu-id="1b3c2-160">Имя пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="1b3c2-160">The User Name that is being reported</span></span>|
|<span data-ttu-id="1b3c2-161">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1b3c2-161">userPrincipalName</span></span>|<span data-ttu-id="1b3c2-162">String</span><span class="sxs-lookup"><span data-stu-id="1b3c2-162">String</span></span>|<span data-ttu-id="1b3c2-163">Имя участника-пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="1b3c2-163">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="1b3c2-164">deviceModel</span><span class="sxs-lookup"><span data-stu-id="1b3c2-164">deviceModel</span></span>|<span data-ttu-id="1b3c2-165">String</span><span class="sxs-lookup"><span data-stu-id="1b3c2-165">String</span></span>|<span data-ttu-id="1b3c2-166">Модель устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="1b3c2-166">The device model that is being reported</span></span>|
|<span data-ttu-id="1b3c2-167">state</span><span class="sxs-lookup"><span data-stu-id="1b3c2-167">state</span></span>|[<span data-ttu-id="1b3c2-168">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="1b3c2-168">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="1b3c2-169">Состояние соответствия для параметра.</span><span class="sxs-lookup"><span data-stu-id="1b3c2-169">The compliance state of the setting.</span></span> <span data-ttu-id="1b3c2-170">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="1b3c2-170">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="1b3c2-171">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="1b3c2-171">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="1b3c2-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b3c2-172">DateTimeOffset</span></span>|<span data-ttu-id="1b3c2-173">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="1b3c2-173">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="1b3c2-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b3c2-174">Response</span></span>
<span data-ttu-id="1b3c2-175">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1b3c2-175">If successful, this method returns a `201 Created` response code and a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b3c2-176">Пример</span><span class="sxs-lookup"><span data-stu-id="1b3c2-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="1b3c2-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="1b3c2-177">Request</span></span>
<span data-ttu-id="1b3c2-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1b3c2-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1b3c2-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b3c2-179">Response</span></span>
<span data-ttu-id="1b3c2-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1b3c2-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




