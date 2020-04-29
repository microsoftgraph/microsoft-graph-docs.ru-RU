---
title: Update deviceComplianceSettingState
description: Обновление свойств объекта deviceComplianceSettingState.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2b1586a2501e16d796fbf44ee44527c8cb6ca2ab
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43399501"
---
# <a name="update-devicecompliancesettingstate"></a><span data-ttu-id="37a3a-103">Update deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="37a3a-103">Update deviceComplianceSettingState</span></span>

<span data-ttu-id="37a3a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37a3a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="37a3a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="37a3a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37a3a-106">Обновление свойств объекта [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="37a3a-106">Update the properties of a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="37a3a-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="37a3a-107">Prerequisites</span></span>
<span data-ttu-id="37a3a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37a3a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37a3a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="37a3a-110">Permission type</span></span>|<span data-ttu-id="37a3a-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="37a3a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37a3a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="37a3a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="37a3a-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37a3a-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="37a3a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="37a3a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37a3a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37a3a-115">Not supported.</span></span>|
|<span data-ttu-id="37a3a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="37a3a-116">Application</span></span>|<span data-ttu-id="37a3a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37a3a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="37a3a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="37a3a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

## <a name="request-headers"></a><span data-ttu-id="37a3a-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="37a3a-119">Request headers</span></span>
|<span data-ttu-id="37a3a-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="37a3a-120">Header</span></span>|<span data-ttu-id="37a3a-121">Значение</span><span class="sxs-lookup"><span data-stu-id="37a3a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="37a3a-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="37a3a-122">Authorization</span></span>|<span data-ttu-id="37a3a-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="37a3a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="37a3a-124">Accept</span><span class="sxs-lookup"><span data-stu-id="37a3a-124">Accept</span></span>|<span data-ttu-id="37a3a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="37a3a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="37a3a-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="37a3a-126">Request body</span></span>
<span data-ttu-id="37a3a-127">В теле запроса добавьте представление объекта [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="37a3a-127">In the request body, supply a JSON representation for the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

<span data-ttu-id="37a3a-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="37a3a-128">The following table shows the properties that are required when you create the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span></span>

|<span data-ttu-id="37a3a-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="37a3a-129">Property</span></span>|<span data-ttu-id="37a3a-130">Тип</span><span class="sxs-lookup"><span data-stu-id="37a3a-130">Type</span></span>|<span data-ttu-id="37a3a-131">Описание</span><span class="sxs-lookup"><span data-stu-id="37a3a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37a3a-132">id</span><span class="sxs-lookup"><span data-stu-id="37a3a-132">id</span></span>|<span data-ttu-id="37a3a-133">Строка</span><span class="sxs-lookup"><span data-stu-id="37a3a-133">String</span></span>|<span data-ttu-id="37a3a-134">Ключ объекта</span><span class="sxs-lookup"><span data-stu-id="37a3a-134">Key of the entity</span></span>|
|<span data-ttu-id="37a3a-135">setting</span><span class="sxs-lookup"><span data-stu-id="37a3a-135">setting</span></span>|<span data-ttu-id="37a3a-136">String</span><span class="sxs-lookup"><span data-stu-id="37a3a-136">String</span></span>|<span data-ttu-id="37a3a-137">Имя класса параметров и свойства.</span><span class="sxs-lookup"><span data-stu-id="37a3a-137">The setting class name and property name.</span></span>|
|<span data-ttu-id="37a3a-138">settingName</span><span class="sxs-lookup"><span data-stu-id="37a3a-138">settingName</span></span>|<span data-ttu-id="37a3a-139">String</span><span class="sxs-lookup"><span data-stu-id="37a3a-139">String</span></span>|<span data-ttu-id="37a3a-140">Имя параметра в отчете</span><span class="sxs-lookup"><span data-stu-id="37a3a-140">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="37a3a-141">deviceId</span><span class="sxs-lookup"><span data-stu-id="37a3a-141">deviceId</span></span>|<span data-ttu-id="37a3a-142">String</span><span class="sxs-lookup"><span data-stu-id="37a3a-142">String</span></span>|<span data-ttu-id="37a3a-143">ИД устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="37a3a-143">The Device Id that is being reported</span></span>|
|<span data-ttu-id="37a3a-144">deviceName</span><span class="sxs-lookup"><span data-stu-id="37a3a-144">deviceName</span></span>|<span data-ttu-id="37a3a-145">String</span><span class="sxs-lookup"><span data-stu-id="37a3a-145">String</span></span>|<span data-ttu-id="37a3a-146">Имя устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="37a3a-146">The Device Name that is being reported</span></span>|
|<span data-ttu-id="37a3a-147">userId</span><span class="sxs-lookup"><span data-stu-id="37a3a-147">userId</span></span>|<span data-ttu-id="37a3a-148">String</span><span class="sxs-lookup"><span data-stu-id="37a3a-148">String</span></span>|<span data-ttu-id="37a3a-149">ИД пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="37a3a-149">The user Id that is being reported</span></span>|
|<span data-ttu-id="37a3a-150">userEmail</span><span class="sxs-lookup"><span data-stu-id="37a3a-150">userEmail</span></span>|<span data-ttu-id="37a3a-151">String</span><span class="sxs-lookup"><span data-stu-id="37a3a-151">String</span></span>|<span data-ttu-id="37a3a-152">Электронный адрес пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="37a3a-152">The User email address that is being reported</span></span>|
|<span data-ttu-id="37a3a-153">userName</span><span class="sxs-lookup"><span data-stu-id="37a3a-153">userName</span></span>|<span data-ttu-id="37a3a-154">String</span><span class="sxs-lookup"><span data-stu-id="37a3a-154">String</span></span>|<span data-ttu-id="37a3a-155">Имя пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="37a3a-155">The User Name that is being reported</span></span>|
|<span data-ttu-id="37a3a-156">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="37a3a-156">userPrincipalName</span></span>|<span data-ttu-id="37a3a-157">String</span><span class="sxs-lookup"><span data-stu-id="37a3a-157">String</span></span>|<span data-ttu-id="37a3a-158">Имя участника-пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="37a3a-158">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="37a3a-159">deviceModel</span><span class="sxs-lookup"><span data-stu-id="37a3a-159">deviceModel</span></span>|<span data-ttu-id="37a3a-160">String</span><span class="sxs-lookup"><span data-stu-id="37a3a-160">String</span></span>|<span data-ttu-id="37a3a-161">Модель устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="37a3a-161">The device model that is being reported</span></span>|
|<span data-ttu-id="37a3a-162">state</span><span class="sxs-lookup"><span data-stu-id="37a3a-162">state</span></span>|[<span data-ttu-id="37a3a-163">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="37a3a-163">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="37a3a-164">Состояние соответствия для параметра.</span><span class="sxs-lookup"><span data-stu-id="37a3a-164">The compliance state of the setting.</span></span> <span data-ttu-id="37a3a-165">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="37a3a-165">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="37a3a-166">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="37a3a-166">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="37a3a-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37a3a-167">DateTimeOffset</span></span>|<span data-ttu-id="37a3a-168">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="37a3a-168">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="37a3a-169">Ответ</span><span class="sxs-lookup"><span data-stu-id="37a3a-169">Response</span></span>
<span data-ttu-id="37a3a-170">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="37a3a-170">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37a3a-171">Пример</span><span class="sxs-lookup"><span data-stu-id="37a3a-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="37a3a-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="37a3a-172">Request</span></span>
<span data-ttu-id="37a3a-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="37a3a-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
Content-type: application/json
Content-length: 517

{
  "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
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

### <a name="response"></a><span data-ttu-id="37a3a-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="37a3a-174">Response</span></span>
<span data-ttu-id="37a3a-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="37a3a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 566

{
  "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
  "id": "9905f955-f955-9905-55f9-059955f90599",
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






