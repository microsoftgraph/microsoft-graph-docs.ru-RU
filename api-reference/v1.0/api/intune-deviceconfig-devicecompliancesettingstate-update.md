---
title: Update deviceComplianceSettingState
description: Обновление свойств объекта deviceComplianceSettingState.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2452998bb521053a888d348ac5abc4626a62e266
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37368948"
---
# <a name="update-devicecompliancesettingstate"></a><span data-ttu-id="f3bd8-103">Update deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="f3bd8-103">Update deviceComplianceSettingState</span></span>

> <span data-ttu-id="f3bd8-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f3bd8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3bd8-105">Обновление свойств объекта [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="f3bd8-105">Update the properties of a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f3bd8-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="f3bd8-106">Prerequisites</span></span>
<span data-ttu-id="f3bd8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3bd8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3bd8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f3bd8-109">Permission type</span></span>|<span data-ttu-id="f3bd8-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f3bd8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3bd8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f3bd8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f3bd8-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3bd8-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f3bd8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f3bd8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3bd8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3bd8-114">Not supported.</span></span>|
|<span data-ttu-id="f3bd8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f3bd8-115">Application</span></span>|<span data-ttu-id="f3bd8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3bd8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3bd8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f3bd8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

## <a name="request-headers"></a><span data-ttu-id="f3bd8-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f3bd8-118">Request headers</span></span>
|<span data-ttu-id="f3bd8-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f3bd8-119">Header</span></span>|<span data-ttu-id="f3bd8-120">Значение</span><span class="sxs-lookup"><span data-stu-id="f3bd8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3bd8-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f3bd8-121">Authorization</span></span>|<span data-ttu-id="f3bd8-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f3bd8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3bd8-123">Accept</span><span class="sxs-lookup"><span data-stu-id="f3bd8-123">Accept</span></span>|<span data-ttu-id="f3bd8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f3bd8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3bd8-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f3bd8-125">Request body</span></span>
<span data-ttu-id="f3bd8-126">В теле запроса добавьте представление объекта [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f3bd8-126">In the request body, supply a JSON representation for the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

<span data-ttu-id="f3bd8-127">Ниже показаны свойства, которые необходимо указывать при создании объекта [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="f3bd8-127">The following table shows the properties that are required when you create the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span></span>

|<span data-ttu-id="f3bd8-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="f3bd8-128">Property</span></span>|<span data-ttu-id="f3bd8-129">Тип</span><span class="sxs-lookup"><span data-stu-id="f3bd8-129">Type</span></span>|<span data-ttu-id="f3bd8-130">Описание</span><span class="sxs-lookup"><span data-stu-id="f3bd8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3bd8-131">id</span><span class="sxs-lookup"><span data-stu-id="f3bd8-131">id</span></span>|<span data-ttu-id="f3bd8-132">Строка</span><span class="sxs-lookup"><span data-stu-id="f3bd8-132">String</span></span>|<span data-ttu-id="f3bd8-133">Ключ объекта</span><span class="sxs-lookup"><span data-stu-id="f3bd8-133">Key of the entity</span></span>|
|<span data-ttu-id="f3bd8-134">setting</span><span class="sxs-lookup"><span data-stu-id="f3bd8-134">setting</span></span>|<span data-ttu-id="f3bd8-135">String</span><span class="sxs-lookup"><span data-stu-id="f3bd8-135">String</span></span>|<span data-ttu-id="f3bd8-136">Имя класса параметров и свойства.</span><span class="sxs-lookup"><span data-stu-id="f3bd8-136">The setting class name and property name.</span></span>|
|<span data-ttu-id="f3bd8-137">settingName</span><span class="sxs-lookup"><span data-stu-id="f3bd8-137">settingName</span></span>|<span data-ttu-id="f3bd8-138">String</span><span class="sxs-lookup"><span data-stu-id="f3bd8-138">String</span></span>|<span data-ttu-id="f3bd8-139">Имя параметра в отчете</span><span class="sxs-lookup"><span data-stu-id="f3bd8-139">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="f3bd8-140">deviceId</span><span class="sxs-lookup"><span data-stu-id="f3bd8-140">deviceId</span></span>|<span data-ttu-id="f3bd8-141">String</span><span class="sxs-lookup"><span data-stu-id="f3bd8-141">String</span></span>|<span data-ttu-id="f3bd8-142">ИД устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="f3bd8-142">The Device Id that is being reported</span></span>|
|<span data-ttu-id="f3bd8-143">deviceName</span><span class="sxs-lookup"><span data-stu-id="f3bd8-143">deviceName</span></span>|<span data-ttu-id="f3bd8-144">String</span><span class="sxs-lookup"><span data-stu-id="f3bd8-144">String</span></span>|<span data-ttu-id="f3bd8-145">Имя устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="f3bd8-145">The Device Name that is being reported</span></span>|
|<span data-ttu-id="f3bd8-146">userId</span><span class="sxs-lookup"><span data-stu-id="f3bd8-146">userId</span></span>|<span data-ttu-id="f3bd8-147">String</span><span class="sxs-lookup"><span data-stu-id="f3bd8-147">String</span></span>|<span data-ttu-id="f3bd8-148">ИД пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="f3bd8-148">The user Id that is being reported</span></span>|
|<span data-ttu-id="f3bd8-149">userEmail</span><span class="sxs-lookup"><span data-stu-id="f3bd8-149">userEmail</span></span>|<span data-ttu-id="f3bd8-150">String</span><span class="sxs-lookup"><span data-stu-id="f3bd8-150">String</span></span>|<span data-ttu-id="f3bd8-151">Электронный адрес пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="f3bd8-151">The User email address that is being reported</span></span>|
|<span data-ttu-id="f3bd8-152">userName</span><span class="sxs-lookup"><span data-stu-id="f3bd8-152">userName</span></span>|<span data-ttu-id="f3bd8-153">String</span><span class="sxs-lookup"><span data-stu-id="f3bd8-153">String</span></span>|<span data-ttu-id="f3bd8-154">Имя пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="f3bd8-154">The User Name that is being reported</span></span>|
|<span data-ttu-id="f3bd8-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f3bd8-155">userPrincipalName</span></span>|<span data-ttu-id="f3bd8-156">String</span><span class="sxs-lookup"><span data-stu-id="f3bd8-156">String</span></span>|<span data-ttu-id="f3bd8-157">Имя участника-пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="f3bd8-157">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="f3bd8-158">deviceModel</span><span class="sxs-lookup"><span data-stu-id="f3bd8-158">deviceModel</span></span>|<span data-ttu-id="f3bd8-159">String</span><span class="sxs-lookup"><span data-stu-id="f3bd8-159">String</span></span>|<span data-ttu-id="f3bd8-160">Модель устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="f3bd8-160">The device model that is being reported</span></span>|
|<span data-ttu-id="f3bd8-161">state</span><span class="sxs-lookup"><span data-stu-id="f3bd8-161">state</span></span>|[<span data-ttu-id="f3bd8-162">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="f3bd8-162">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="f3bd8-163">Состояние соответствия для параметра.</span><span class="sxs-lookup"><span data-stu-id="f3bd8-163">The compliance state of the setting.</span></span> <span data-ttu-id="f3bd8-164">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="f3bd8-164">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="f3bd8-165">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f3bd8-165">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="f3bd8-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3bd8-166">DateTimeOffset</span></span>|<span data-ttu-id="f3bd8-167">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="f3bd8-167">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="f3bd8-168">Ответ</span><span class="sxs-lookup"><span data-stu-id="f3bd8-168">Response</span></span>
<span data-ttu-id="f3bd8-169">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f3bd8-169">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3bd8-170">Пример</span><span class="sxs-lookup"><span data-stu-id="f3bd8-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3bd8-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="f3bd8-171">Request</span></span>
<span data-ttu-id="f3bd8-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f3bd8-172">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f3bd8-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3bd8-173">Response</span></span>
<span data-ttu-id="f3bd8-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f3bd8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




