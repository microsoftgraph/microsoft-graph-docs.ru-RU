---
title: Update deviceComplianceSettingState
description: Обновление свойств объекта deviceComplianceSettingState.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 646e69d1bc637dde947ddddf03eb62d25c07148f
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31783033"
---
# <a name="update-devicecompliancesettingstate"></a><span data-ttu-id="5e7f5-103">Update deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="5e7f5-103">Update deviceComplianceSettingState</span></span>

> <span data-ttu-id="5e7f5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e7f5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5e7f5-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5e7f5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e7f5-106">Обновление свойств объекта [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="5e7f5-106">Update the properties of a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5e7f5-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="5e7f5-107">Prerequisites</span></span>
<span data-ttu-id="5e7f5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e7f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e7f5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5e7f5-110">Permission type</span></span>|<span data-ttu-id="5e7f5-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5e7f5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5e7f5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5e7f5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5e7f5-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e7f5-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5e7f5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5e7f5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e7f5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e7f5-115">Not supported.</span></span>|
|<span data-ttu-id="5e7f5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5e7f5-116">Application</span></span>|<span data-ttu-id="5e7f5-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e7f5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5e7f5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5e7f5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

## <a name="request-headers"></a><span data-ttu-id="5e7f5-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5e7f5-119">Request headers</span></span>
|<span data-ttu-id="5e7f5-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5e7f5-120">Header</span></span>|<span data-ttu-id="5e7f5-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5e7f5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5e7f5-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5e7f5-122">Authorization</span></span>|<span data-ttu-id="5e7f5-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5e7f5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5e7f5-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5e7f5-124">Accept</span></span>|<span data-ttu-id="5e7f5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5e7f5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e7f5-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5e7f5-126">Request body</span></span>
<span data-ttu-id="5e7f5-127">В теле запроса добавьте представление объекта [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5e7f5-127">In the request body, supply a JSON representation for the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

<span data-ttu-id="5e7f5-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="5e7f5-128">The following table shows the properties that are required when you create the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span></span>

|<span data-ttu-id="5e7f5-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="5e7f5-129">Property</span></span>|<span data-ttu-id="5e7f5-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5e7f5-130">Type</span></span>|<span data-ttu-id="5e7f5-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5e7f5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e7f5-132">id</span><span class="sxs-lookup"><span data-stu-id="5e7f5-132">id</span></span>|<span data-ttu-id="5e7f5-133">Строка</span><span class="sxs-lookup"><span data-stu-id="5e7f5-133">String</span></span>|<span data-ttu-id="5e7f5-134">Ключ объекта</span><span class="sxs-lookup"><span data-stu-id="5e7f5-134">Key of the entity</span></span>|
|<span data-ttu-id="5e7f5-135">platformType</span><span class="sxs-lookup"><span data-stu-id="5e7f5-135">platformType</span></span>|[<span data-ttu-id="5e7f5-136">deviceType</span><span class="sxs-lookup"><span data-stu-id="5e7f5-136">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="5e7f5-137">Тип платформы устройства.</span><span class="sxs-lookup"><span data-stu-id="5e7f5-137">Device platform type.</span></span> <span data-ttu-id="5e7f5-138">Возможные значения: `desktop`, `windowsRT`, `winMO6`, `nokia` `windowsPhone` `mac` `winCE` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `android` `iSocConsumer`,,,,,,,,,,,,,,,,,,,,, `winEmbedded` `iPhone` `iPad` `iPod` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="5e7f5-138">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="5e7f5-139">setting</span><span class="sxs-lookup"><span data-stu-id="5e7f5-139">setting</span></span>|<span data-ttu-id="5e7f5-140">String</span><span class="sxs-lookup"><span data-stu-id="5e7f5-140">String</span></span>|<span data-ttu-id="5e7f5-141">Имя класса параметров и свойства.</span><span class="sxs-lookup"><span data-stu-id="5e7f5-141">The setting class name and property name.</span></span>|
|<span data-ttu-id="5e7f5-142">settingName</span><span class="sxs-lookup"><span data-stu-id="5e7f5-142">settingName</span></span>|<span data-ttu-id="5e7f5-143">String</span><span class="sxs-lookup"><span data-stu-id="5e7f5-143">String</span></span>|<span data-ttu-id="5e7f5-144">Имя параметра в отчете</span><span class="sxs-lookup"><span data-stu-id="5e7f5-144">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="5e7f5-145">deviceId</span><span class="sxs-lookup"><span data-stu-id="5e7f5-145">deviceId</span></span>|<span data-ttu-id="5e7f5-146">String</span><span class="sxs-lookup"><span data-stu-id="5e7f5-146">String</span></span>|<span data-ttu-id="5e7f5-147">ИД устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="5e7f5-147">The Device Id that is being reported</span></span>|
|<span data-ttu-id="5e7f5-148">deviceName</span><span class="sxs-lookup"><span data-stu-id="5e7f5-148">deviceName</span></span>|<span data-ttu-id="5e7f5-149">String</span><span class="sxs-lookup"><span data-stu-id="5e7f5-149">String</span></span>|<span data-ttu-id="5e7f5-150">Имя устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="5e7f5-150">The Device Name that is being reported</span></span>|
|<span data-ttu-id="5e7f5-151">userId</span><span class="sxs-lookup"><span data-stu-id="5e7f5-151">userId</span></span>|<span data-ttu-id="5e7f5-152">String</span><span class="sxs-lookup"><span data-stu-id="5e7f5-152">String</span></span>|<span data-ttu-id="5e7f5-153">ИД пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="5e7f5-153">The user Id that is being reported</span></span>|
|<span data-ttu-id="5e7f5-154">userEmail</span><span class="sxs-lookup"><span data-stu-id="5e7f5-154">userEmail</span></span>|<span data-ttu-id="5e7f5-155">String</span><span class="sxs-lookup"><span data-stu-id="5e7f5-155">String</span></span>|<span data-ttu-id="5e7f5-156">Электронный адрес пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="5e7f5-156">The User email address that is being reported</span></span>|
|<span data-ttu-id="5e7f5-157">userName</span><span class="sxs-lookup"><span data-stu-id="5e7f5-157">userName</span></span>|<span data-ttu-id="5e7f5-158">String</span><span class="sxs-lookup"><span data-stu-id="5e7f5-158">String</span></span>|<span data-ttu-id="5e7f5-159">Имя пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="5e7f5-159">The User Name that is being reported</span></span>|
|<span data-ttu-id="5e7f5-160">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5e7f5-160">userPrincipalName</span></span>|<span data-ttu-id="5e7f5-161">String</span><span class="sxs-lookup"><span data-stu-id="5e7f5-161">String</span></span>|<span data-ttu-id="5e7f5-162">Имя участника-пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="5e7f5-162">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="5e7f5-163">deviceModel</span><span class="sxs-lookup"><span data-stu-id="5e7f5-163">deviceModel</span></span>|<span data-ttu-id="5e7f5-164">String</span><span class="sxs-lookup"><span data-stu-id="5e7f5-164">String</span></span>|<span data-ttu-id="5e7f5-165">Модель устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="5e7f5-165">The device model that is being reported</span></span>|
|<span data-ttu-id="5e7f5-166">state</span><span class="sxs-lookup"><span data-stu-id="5e7f5-166">state</span></span>|[<span data-ttu-id="5e7f5-167">Комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="5e7f5-167">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="5e7f5-168">Состояние соответствия для параметра.</span><span class="sxs-lookup"><span data-stu-id="5e7f5-168">The compliance state of the setting.</span></span> <span data-ttu-id="5e7f5-169">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="5e7f5-169">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="5e7f5-170">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="5e7f5-170">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="5e7f5-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e7f5-171">DateTimeOffset</span></span>|<span data-ttu-id="5e7f5-172">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="5e7f5-172">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="5e7f5-173">Ответ</span><span class="sxs-lookup"><span data-stu-id="5e7f5-173">Response</span></span>
<span data-ttu-id="5e7f5-174">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="5e7f5-174">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e7f5-175">Пример</span><span class="sxs-lookup"><span data-stu-id="5e7f5-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="5e7f5-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="5e7f5-176">Request</span></span>
<span data-ttu-id="5e7f5-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5e7f5-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5e7f5-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="5e7f5-178">Response</span></span>
<span data-ttu-id="5e7f5-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5e7f5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





