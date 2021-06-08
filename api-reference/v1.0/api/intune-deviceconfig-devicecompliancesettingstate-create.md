---
title: Создание объекта deviceComplianceSettingState
description: Создание объекта deviceComplianceSettingState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0cb1deb234005cfdb7a206ddabbbc562f8e91299
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758381"
---
# <a name="create-devicecompliancesettingstate"></a><span data-ttu-id="146dc-103">Создание объекта deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="146dc-103">Create deviceComplianceSettingState</span></span>

<span data-ttu-id="146dc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="146dc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="146dc-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="146dc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="146dc-106">Создание объекта [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="146dc-106">Create a new [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="146dc-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="146dc-107">Prerequisites</span></span>
<span data-ttu-id="146dc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="146dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="146dc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="146dc-110">Permission type</span></span>|<span data-ttu-id="146dc-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="146dc-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="146dc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="146dc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="146dc-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="146dc-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="146dc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="146dc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="146dc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="146dc-115">Not supported.</span></span>|
|<span data-ttu-id="146dc-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="146dc-116">Application</span></span>|<span data-ttu-id="146dc-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="146dc-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="146dc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="146dc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="146dc-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="146dc-119">Request headers</span></span>
|<span data-ttu-id="146dc-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="146dc-120">Header</span></span>|<span data-ttu-id="146dc-121">Значение</span><span class="sxs-lookup"><span data-stu-id="146dc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="146dc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="146dc-122">Authorization</span></span>|<span data-ttu-id="146dc-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="146dc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="146dc-124">Accept</span><span class="sxs-lookup"><span data-stu-id="146dc-124">Accept</span></span>|<span data-ttu-id="146dc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="146dc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="146dc-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="146dc-126">Request body</span></span>
<span data-ttu-id="146dc-127">В тексте запроса добавьте представление объекта deviceComplianceSettingState в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="146dc-127">In the request body, supply a JSON representation for the deviceComplianceSettingState object.</span></span>

<span data-ttu-id="146dc-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceComplianceSettingState.</span><span class="sxs-lookup"><span data-stu-id="146dc-128">The following table shows the properties that are required when you create the deviceComplianceSettingState.</span></span>

|<span data-ttu-id="146dc-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="146dc-129">Property</span></span>|<span data-ttu-id="146dc-130">Тип</span><span class="sxs-lookup"><span data-stu-id="146dc-130">Type</span></span>|<span data-ttu-id="146dc-131">Описание</span><span class="sxs-lookup"><span data-stu-id="146dc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="146dc-132">id</span><span class="sxs-lookup"><span data-stu-id="146dc-132">id</span></span>|<span data-ttu-id="146dc-133">String</span><span class="sxs-lookup"><span data-stu-id="146dc-133">String</span></span>|<span data-ttu-id="146dc-134">Ключ объекта</span><span class="sxs-lookup"><span data-stu-id="146dc-134">Key of the entity</span></span>|
|<span data-ttu-id="146dc-135">setting</span><span class="sxs-lookup"><span data-stu-id="146dc-135">setting</span></span>|<span data-ttu-id="146dc-136">String</span><span class="sxs-lookup"><span data-stu-id="146dc-136">String</span></span>|<span data-ttu-id="146dc-137">Имя класса параметров и свойства.</span><span class="sxs-lookup"><span data-stu-id="146dc-137">The setting class name and property name.</span></span>|
|<span data-ttu-id="146dc-138">settingName</span><span class="sxs-lookup"><span data-stu-id="146dc-138">settingName</span></span>|<span data-ttu-id="146dc-139">String</span><span class="sxs-lookup"><span data-stu-id="146dc-139">String</span></span>|<span data-ttu-id="146dc-140">Имя параметра в отчете</span><span class="sxs-lookup"><span data-stu-id="146dc-140">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="146dc-141">deviceId</span><span class="sxs-lookup"><span data-stu-id="146dc-141">deviceId</span></span>|<span data-ttu-id="146dc-142">String</span><span class="sxs-lookup"><span data-stu-id="146dc-142">String</span></span>|<span data-ttu-id="146dc-143">ИД устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="146dc-143">The Device Id that is being reported</span></span>|
|<span data-ttu-id="146dc-144">deviceName</span><span class="sxs-lookup"><span data-stu-id="146dc-144">deviceName</span></span>|<span data-ttu-id="146dc-145">String</span><span class="sxs-lookup"><span data-stu-id="146dc-145">String</span></span>|<span data-ttu-id="146dc-146">Имя устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="146dc-146">The Device Name that is being reported</span></span>|
|<span data-ttu-id="146dc-147">userId</span><span class="sxs-lookup"><span data-stu-id="146dc-147">userId</span></span>|<span data-ttu-id="146dc-148">String</span><span class="sxs-lookup"><span data-stu-id="146dc-148">String</span></span>|<span data-ttu-id="146dc-149">ИД пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="146dc-149">The user Id that is being reported</span></span>|
|<span data-ttu-id="146dc-150">userEmail</span><span class="sxs-lookup"><span data-stu-id="146dc-150">userEmail</span></span>|<span data-ttu-id="146dc-151">String</span><span class="sxs-lookup"><span data-stu-id="146dc-151">String</span></span>|<span data-ttu-id="146dc-152">Электронный адрес пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="146dc-152">The User email address that is being reported</span></span>|
|<span data-ttu-id="146dc-153">userName</span><span class="sxs-lookup"><span data-stu-id="146dc-153">userName</span></span>|<span data-ttu-id="146dc-154">String</span><span class="sxs-lookup"><span data-stu-id="146dc-154">String</span></span>|<span data-ttu-id="146dc-155">Имя пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="146dc-155">The User Name that is being reported</span></span>|
|<span data-ttu-id="146dc-156">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="146dc-156">userPrincipalName</span></span>|<span data-ttu-id="146dc-157">String</span><span class="sxs-lookup"><span data-stu-id="146dc-157">String</span></span>|<span data-ttu-id="146dc-158">Имя участника-пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="146dc-158">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="146dc-159">deviceModel</span><span class="sxs-lookup"><span data-stu-id="146dc-159">deviceModel</span></span>|<span data-ttu-id="146dc-160">String</span><span class="sxs-lookup"><span data-stu-id="146dc-160">String</span></span>|<span data-ttu-id="146dc-161">Модель устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="146dc-161">The device model that is being reported</span></span>|
|<span data-ttu-id="146dc-162">state</span><span class="sxs-lookup"><span data-stu-id="146dc-162">state</span></span>|[<span data-ttu-id="146dc-163">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="146dc-163">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="146dc-164">Состояние соответствия параметру.</span><span class="sxs-lookup"><span data-stu-id="146dc-164">The compliance state of the setting.</span></span> <span data-ttu-id="146dc-165">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="146dc-165">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="146dc-166">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="146dc-166">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="146dc-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="146dc-167">DateTimeOffset</span></span>|<span data-ttu-id="146dc-168">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="146dc-168">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="146dc-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="146dc-169">Response</span></span>
<span data-ttu-id="146dc-170">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="146dc-170">If successful, this method returns a `201 Created` response code and a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="146dc-171">Пример</span><span class="sxs-lookup"><span data-stu-id="146dc-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="146dc-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="146dc-172">Request</span></span>
<span data-ttu-id="146dc-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="146dc-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
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

### <a name="response"></a><span data-ttu-id="146dc-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="146dc-174">Response</span></span>
<span data-ttu-id="146dc-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="146dc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




