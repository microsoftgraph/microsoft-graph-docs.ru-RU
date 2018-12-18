---
title: Update deviceComplianceSettingState
description: Обновление свойств объекта deviceComplianceSettingState.
author: tfitzmac
ms.openlocfilehash: 7183493e8b45198c4f1cadd1e8fbc2e7e738478d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330151"
---
# <a name="update-devicecompliancesettingstate"></a><span data-ttu-id="d4c9f-103">Update deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="d4c9f-103">Update deviceComplianceSettingState</span></span>

> <span data-ttu-id="d4c9f-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d4c9f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d4c9f-105">Обновление свойств объекта [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="d4c9f-105">Update the properties of a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d4c9f-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="d4c9f-106">Prerequisites</span></span>
<span data-ttu-id="d4c9f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4c9f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4c9f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d4c9f-109">Permission type</span></span>|<span data-ttu-id="d4c9f-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d4c9f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4c9f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d4c9f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d4c9f-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4c9f-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d4c9f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d4c9f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4c9f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4c9f-114">Not supported.</span></span>|
|<span data-ttu-id="d4c9f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d4c9f-115">Application</span></span>|<span data-ttu-id="d4c9f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4c9f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4c9f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d4c9f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

## <a name="request-headers"></a><span data-ttu-id="d4c9f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d4c9f-118">Request headers</span></span>
|<span data-ttu-id="d4c9f-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d4c9f-119">Header</span></span>|<span data-ttu-id="d4c9f-120">Значение</span><span class="sxs-lookup"><span data-stu-id="d4c9f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4c9f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d4c9f-121">Authorization</span></span>|<span data-ttu-id="d4c9f-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="d4c9f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4c9f-123">Accept</span><span class="sxs-lookup"><span data-stu-id="d4c9f-123">Accept</span></span>|<span data-ttu-id="d4c9f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d4c9f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4c9f-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d4c9f-125">Request body</span></span>
<span data-ttu-id="d4c9f-126">В теле запроса добавьте представление объекта [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d4c9f-126">In the request body, supply a JSON representation for the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

<span data-ttu-id="d4c9f-127">Ниже показаны свойства, которые необходимо указывать при создании объекта [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="d4c9f-127">The following table shows the properties that are required when you create the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span></span>

|<span data-ttu-id="d4c9f-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="d4c9f-128">Property</span></span>|<span data-ttu-id="d4c9f-129">Тип</span><span class="sxs-lookup"><span data-stu-id="d4c9f-129">Type</span></span>|<span data-ttu-id="d4c9f-130">Описание</span><span class="sxs-lookup"><span data-stu-id="d4c9f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4c9f-131">id</span><span class="sxs-lookup"><span data-stu-id="d4c9f-131">id</span></span>|<span data-ttu-id="d4c9f-132">String</span><span class="sxs-lookup"><span data-stu-id="d4c9f-132">String</span></span>|<span data-ttu-id="d4c9f-133">Ключ объекта</span><span class="sxs-lookup"><span data-stu-id="d4c9f-133">Key of the entity</span></span>|
|<span data-ttu-id="d4c9f-134">setting</span><span class="sxs-lookup"><span data-stu-id="d4c9f-134">setting</span></span>|<span data-ttu-id="d4c9f-135">String</span><span class="sxs-lookup"><span data-stu-id="d4c9f-135">String</span></span>|<span data-ttu-id="d4c9f-136">Имя класса параметров и свойства.</span><span class="sxs-lookup"><span data-stu-id="d4c9f-136">The setting class name and property name.</span></span>|
|<span data-ttu-id="d4c9f-137">settingName</span><span class="sxs-lookup"><span data-stu-id="d4c9f-137">settingName</span></span>|<span data-ttu-id="d4c9f-138">String</span><span class="sxs-lookup"><span data-stu-id="d4c9f-138">String</span></span>|<span data-ttu-id="d4c9f-139">Имя параметра в отчете.</span><span class="sxs-lookup"><span data-stu-id="d4c9f-139">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="d4c9f-140">deviceId</span><span class="sxs-lookup"><span data-stu-id="d4c9f-140">deviceId</span></span>|<span data-ttu-id="d4c9f-141">String</span><span class="sxs-lookup"><span data-stu-id="d4c9f-141">String</span></span>|<span data-ttu-id="d4c9f-142">Идентификатор устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="d4c9f-142">The Device Id that is being reported</span></span>|
|<span data-ttu-id="d4c9f-143">deviceName</span><span class="sxs-lookup"><span data-stu-id="d4c9f-143">deviceName</span></span>|<span data-ttu-id="d4c9f-144">String</span><span class="sxs-lookup"><span data-stu-id="d4c9f-144">String</span></span>|<span data-ttu-id="d4c9f-145">Имя устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="d4c9f-145">The Device Name that is being reported</span></span>|
|<span data-ttu-id="d4c9f-146">userId</span><span class="sxs-lookup"><span data-stu-id="d4c9f-146">userId</span></span>|<span data-ttu-id="d4c9f-147">String</span><span class="sxs-lookup"><span data-stu-id="d4c9f-147">String</span></span>|<span data-ttu-id="d4c9f-148">Идентификатор пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="d4c9f-148">The user Id that is being reported</span></span>|
|<span data-ttu-id="d4c9f-149">userEmail</span><span class="sxs-lookup"><span data-stu-id="d4c9f-149">userEmail</span></span>|<span data-ttu-id="d4c9f-150">String</span><span class="sxs-lookup"><span data-stu-id="d4c9f-150">String</span></span>|<span data-ttu-id="d4c9f-151">Адрес электронной почты пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="d4c9f-151">The User email address that is being reported</span></span>|
|<span data-ttu-id="d4c9f-152">userName</span><span class="sxs-lookup"><span data-stu-id="d4c9f-152">userName</span></span>|<span data-ttu-id="d4c9f-153">String</span><span class="sxs-lookup"><span data-stu-id="d4c9f-153">String</span></span>|<span data-ttu-id="d4c9f-154">Имя пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="d4c9f-154">The User Name that is being reported</span></span>|
|<span data-ttu-id="d4c9f-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d4c9f-155">userPrincipalName</span></span>|<span data-ttu-id="d4c9f-156">String</span><span class="sxs-lookup"><span data-stu-id="d4c9f-156">String</span></span>|<span data-ttu-id="d4c9f-157">Имя участника-пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="d4c9f-157">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="d4c9f-158">deviceModel</span><span class="sxs-lookup"><span data-stu-id="d4c9f-158">deviceModel</span></span>|<span data-ttu-id="d4c9f-159">String</span><span class="sxs-lookup"><span data-stu-id="d4c9f-159">String</span></span>|<span data-ttu-id="d4c9f-160">Модель устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="d4c9f-160">The device model that is being reported</span></span>|
|<span data-ttu-id="d4c9f-161">state</span><span class="sxs-lookup"><span data-stu-id="d4c9f-161">state</span></span>|[<span data-ttu-id="d4c9f-162">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="d4c9f-162">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="d4c9f-163">Соответствие требованиям состояние параметра.</span><span class="sxs-lookup"><span data-stu-id="d4c9f-163">The compliance state of the setting.</span></span> <span data-ttu-id="d4c9f-164">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="d4c9f-164">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="d4c9f-165">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d4c9f-165">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="d4c9f-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4c9f-166">DateTimeOffset</span></span>|<span data-ttu-id="d4c9f-167">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="d4c9f-167">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="d4c9f-168">Ответ</span><span class="sxs-lookup"><span data-stu-id="d4c9f-168">Response</span></span>
<span data-ttu-id="d4c9f-169">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d4c9f-169">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4c9f-170">Пример</span><span class="sxs-lookup"><span data-stu-id="d4c9f-170">Example</span></span>
### <a name="request"></a><span data-ttu-id="d4c9f-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="d4c9f-171">Request</span></span>
<span data-ttu-id="d4c9f-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d4c9f-172">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d4c9f-173">Ответ</span><span class="sxs-lookup"><span data-stu-id="d4c9f-173">Response</span></span>
<span data-ttu-id="d4c9f-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d4c9f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



