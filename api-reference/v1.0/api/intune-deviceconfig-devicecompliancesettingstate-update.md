---
title: Update deviceComplianceSettingState
description: Обновление свойств объекта deviceComplianceSettingState.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: de5c9bf9b2f19bf60bf35391a918916dd02ca9d9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42514917"
---
# <a name="update-devicecompliancesettingstate"></a><span data-ttu-id="18fd4-103">Update deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="18fd4-103">Update deviceComplianceSettingState</span></span>

<span data-ttu-id="18fd4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18fd4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="18fd4-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="18fd4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18fd4-106">Обновление свойств объекта [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="18fd4-106">Update the properties of a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="18fd4-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="18fd4-107">Prerequisites</span></span>
<span data-ttu-id="18fd4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18fd4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18fd4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="18fd4-110">Permission type</span></span>|<span data-ttu-id="18fd4-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="18fd4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18fd4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="18fd4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="18fd4-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18fd4-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="18fd4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="18fd4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18fd4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18fd4-115">Not supported.</span></span>|
|<span data-ttu-id="18fd4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="18fd4-116">Application</span></span>|<span data-ttu-id="18fd4-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18fd4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="18fd4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="18fd4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

## <a name="request-headers"></a><span data-ttu-id="18fd4-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="18fd4-119">Request headers</span></span>
|<span data-ttu-id="18fd4-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="18fd4-120">Header</span></span>|<span data-ttu-id="18fd4-121">Значение</span><span class="sxs-lookup"><span data-stu-id="18fd4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18fd4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="18fd4-122">Authorization</span></span>|<span data-ttu-id="18fd4-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="18fd4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18fd4-124">Accept</span><span class="sxs-lookup"><span data-stu-id="18fd4-124">Accept</span></span>|<span data-ttu-id="18fd4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="18fd4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18fd4-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="18fd4-126">Request body</span></span>
<span data-ttu-id="18fd4-127">В теле запроса добавьте представление объекта [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="18fd4-127">In the request body, supply a JSON representation for the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

<span data-ttu-id="18fd4-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="18fd4-128">The following table shows the properties that are required when you create the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span></span>

|<span data-ttu-id="18fd4-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="18fd4-129">Property</span></span>|<span data-ttu-id="18fd4-130">Тип</span><span class="sxs-lookup"><span data-stu-id="18fd4-130">Type</span></span>|<span data-ttu-id="18fd4-131">Описание</span><span class="sxs-lookup"><span data-stu-id="18fd4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18fd4-132">id</span><span class="sxs-lookup"><span data-stu-id="18fd4-132">id</span></span>|<span data-ttu-id="18fd4-133">Строка</span><span class="sxs-lookup"><span data-stu-id="18fd4-133">String</span></span>|<span data-ttu-id="18fd4-134">Ключ объекта</span><span class="sxs-lookup"><span data-stu-id="18fd4-134">Key of the entity</span></span>|
|<span data-ttu-id="18fd4-135">setting</span><span class="sxs-lookup"><span data-stu-id="18fd4-135">setting</span></span>|<span data-ttu-id="18fd4-136">Строка</span><span class="sxs-lookup"><span data-stu-id="18fd4-136">String</span></span>|<span data-ttu-id="18fd4-137">Имя класса параметров и свойства.</span><span class="sxs-lookup"><span data-stu-id="18fd4-137">The setting class name and property name.</span></span>|
|<span data-ttu-id="18fd4-138">settingName</span><span class="sxs-lookup"><span data-stu-id="18fd4-138">settingName</span></span>|<span data-ttu-id="18fd4-139">Строка</span><span class="sxs-lookup"><span data-stu-id="18fd4-139">String</span></span>|<span data-ttu-id="18fd4-140">Имя параметра в отчете</span><span class="sxs-lookup"><span data-stu-id="18fd4-140">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="18fd4-141">deviceId</span><span class="sxs-lookup"><span data-stu-id="18fd4-141">deviceId</span></span>|<span data-ttu-id="18fd4-142">Строка</span><span class="sxs-lookup"><span data-stu-id="18fd4-142">String</span></span>|<span data-ttu-id="18fd4-143">ИД устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="18fd4-143">The Device Id that is being reported</span></span>|
|<span data-ttu-id="18fd4-144">deviceName</span><span class="sxs-lookup"><span data-stu-id="18fd4-144">deviceName</span></span>|<span data-ttu-id="18fd4-145">Строка</span><span class="sxs-lookup"><span data-stu-id="18fd4-145">String</span></span>|<span data-ttu-id="18fd4-146">Имя устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="18fd4-146">The Device Name that is being reported</span></span>|
|<span data-ttu-id="18fd4-147">userId</span><span class="sxs-lookup"><span data-stu-id="18fd4-147">userId</span></span>|<span data-ttu-id="18fd4-148">String</span><span class="sxs-lookup"><span data-stu-id="18fd4-148">String</span></span>|<span data-ttu-id="18fd4-149">ИД пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="18fd4-149">The user Id that is being reported</span></span>|
|<span data-ttu-id="18fd4-150">userEmail</span><span class="sxs-lookup"><span data-stu-id="18fd4-150">userEmail</span></span>|<span data-ttu-id="18fd4-151">String</span><span class="sxs-lookup"><span data-stu-id="18fd4-151">String</span></span>|<span data-ttu-id="18fd4-152">Электронный адрес пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="18fd4-152">The User email address that is being reported</span></span>|
|<span data-ttu-id="18fd4-153">userName</span><span class="sxs-lookup"><span data-stu-id="18fd4-153">userName</span></span>|<span data-ttu-id="18fd4-154">Строка</span><span class="sxs-lookup"><span data-stu-id="18fd4-154">String</span></span>|<span data-ttu-id="18fd4-155">Имя пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="18fd4-155">The User Name that is being reported</span></span>|
|<span data-ttu-id="18fd4-156">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="18fd4-156">userPrincipalName</span></span>|<span data-ttu-id="18fd4-157">String</span><span class="sxs-lookup"><span data-stu-id="18fd4-157">String</span></span>|<span data-ttu-id="18fd4-158">Имя участника-пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="18fd4-158">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="18fd4-159">deviceModel</span><span class="sxs-lookup"><span data-stu-id="18fd4-159">deviceModel</span></span>|<span data-ttu-id="18fd4-160">Строка</span><span class="sxs-lookup"><span data-stu-id="18fd4-160">String</span></span>|<span data-ttu-id="18fd4-161">Модель устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="18fd4-161">The device model that is being reported</span></span>|
|<span data-ttu-id="18fd4-162">state</span><span class="sxs-lookup"><span data-stu-id="18fd4-162">state</span></span>|[<span data-ttu-id="18fd4-163">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="18fd4-163">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="18fd4-164">Состояние соответствия для параметра.</span><span class="sxs-lookup"><span data-stu-id="18fd4-164">The compliance state of the setting.</span></span> <span data-ttu-id="18fd4-165">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="18fd4-165">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="18fd4-166">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="18fd4-166">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="18fd4-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18fd4-167">DateTimeOffset</span></span>|<span data-ttu-id="18fd4-168">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="18fd4-168">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="18fd4-169">Ответ</span><span class="sxs-lookup"><span data-stu-id="18fd4-169">Response</span></span>
<span data-ttu-id="18fd4-170">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="18fd4-170">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18fd4-171">Пример</span><span class="sxs-lookup"><span data-stu-id="18fd4-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="18fd4-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="18fd4-172">Request</span></span>
<span data-ttu-id="18fd4-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="18fd4-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="18fd4-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="18fd4-174">Response</span></span>
<span data-ttu-id="18fd4-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="18fd4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




