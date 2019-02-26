---
title: Update deviceComplianceSettingState
description: Обновление свойств объекта deviceComplianceSettingState.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c22c97d8e15e79419066392d3a984ee0899589b7
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258669"
---
# <a name="update-devicecompliancesettingstate"></a><span data-ttu-id="e7c87-103">Update deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="e7c87-103">Update deviceComplianceSettingState</span></span>

> <span data-ttu-id="e7c87-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e7c87-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7c87-105">Обновление свойств объекта [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="e7c87-105">Update the properties of a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e7c87-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="e7c87-106">Prerequisites</span></span>
<span data-ttu-id="e7c87-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e7c87-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e7c87-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e7c87-109">Permission type</span></span>|<span data-ttu-id="e7c87-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e7c87-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7c87-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e7c87-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e7c87-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7c87-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e7c87-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e7c87-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7c87-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7c87-114">Not supported.</span></span>|
|<span data-ttu-id="e7c87-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e7c87-115">Application</span></span>|<span data-ttu-id="e7c87-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7c87-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7c87-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e7c87-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

## <a name="request-headers"></a><span data-ttu-id="e7c87-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e7c87-118">Request headers</span></span>
|<span data-ttu-id="e7c87-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e7c87-119">Header</span></span>|<span data-ttu-id="e7c87-120">Значение</span><span class="sxs-lookup"><span data-stu-id="e7c87-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7c87-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7c87-121">Authorization</span></span>|<span data-ttu-id="e7c87-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e7c87-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7c87-123">Accept</span><span class="sxs-lookup"><span data-stu-id="e7c87-123">Accept</span></span>|<span data-ttu-id="e7c87-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e7c87-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7c87-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e7c87-125">Request body</span></span>
<span data-ttu-id="e7c87-126">В теле запроса добавьте представление объекта [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e7c87-126">In the request body, supply a JSON representation for the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

<span data-ttu-id="e7c87-127">Ниже показаны свойства, которые необходимо указывать при создании объекта [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="e7c87-127">The following table shows the properties that are required when you create the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span></span>

|<span data-ttu-id="e7c87-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="e7c87-128">Property</span></span>|<span data-ttu-id="e7c87-129">Тип</span><span class="sxs-lookup"><span data-stu-id="e7c87-129">Type</span></span>|<span data-ttu-id="e7c87-130">Описание</span><span class="sxs-lookup"><span data-stu-id="e7c87-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7c87-131">id</span><span class="sxs-lookup"><span data-stu-id="e7c87-131">id</span></span>|<span data-ttu-id="e7c87-132">String</span><span class="sxs-lookup"><span data-stu-id="e7c87-132">String</span></span>|<span data-ttu-id="e7c87-133">Ключ объекта</span><span class="sxs-lookup"><span data-stu-id="e7c87-133">Key of the entity</span></span>|
|<span data-ttu-id="e7c87-134">setting</span><span class="sxs-lookup"><span data-stu-id="e7c87-134">setting</span></span>|<span data-ttu-id="e7c87-135">String</span><span class="sxs-lookup"><span data-stu-id="e7c87-135">String</span></span>|<span data-ttu-id="e7c87-136">Имя класса параметров и свойства.</span><span class="sxs-lookup"><span data-stu-id="e7c87-136">The setting class name and property name.</span></span>|
|<span data-ttu-id="e7c87-137">settingName</span><span class="sxs-lookup"><span data-stu-id="e7c87-137">settingName</span></span>|<span data-ttu-id="e7c87-138">String</span><span class="sxs-lookup"><span data-stu-id="e7c87-138">String</span></span>|<span data-ttu-id="e7c87-139">Имя параметра в отчете.</span><span class="sxs-lookup"><span data-stu-id="e7c87-139">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="e7c87-140">deviceId</span><span class="sxs-lookup"><span data-stu-id="e7c87-140">deviceId</span></span>|<span data-ttu-id="e7c87-141">String</span><span class="sxs-lookup"><span data-stu-id="e7c87-141">String</span></span>|<span data-ttu-id="e7c87-142">Идентификатор устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="e7c87-142">The Device Id that is being reported</span></span>|
|<span data-ttu-id="e7c87-143">deviceName</span><span class="sxs-lookup"><span data-stu-id="e7c87-143">deviceName</span></span>|<span data-ttu-id="e7c87-144">String</span><span class="sxs-lookup"><span data-stu-id="e7c87-144">String</span></span>|<span data-ttu-id="e7c87-145">Имя устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="e7c87-145">The Device Name that is being reported</span></span>|
|<span data-ttu-id="e7c87-146">userId</span><span class="sxs-lookup"><span data-stu-id="e7c87-146">userId</span></span>|<span data-ttu-id="e7c87-147">String</span><span class="sxs-lookup"><span data-stu-id="e7c87-147">String</span></span>|<span data-ttu-id="e7c87-148">Идентификатор пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="e7c87-148">The user Id that is being reported</span></span>|
|<span data-ttu-id="e7c87-149">userEmail</span><span class="sxs-lookup"><span data-stu-id="e7c87-149">userEmail</span></span>|<span data-ttu-id="e7c87-150">String</span><span class="sxs-lookup"><span data-stu-id="e7c87-150">String</span></span>|<span data-ttu-id="e7c87-151">Адрес электронной почты пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="e7c87-151">The User email address that is being reported</span></span>|
|<span data-ttu-id="e7c87-152">userName</span><span class="sxs-lookup"><span data-stu-id="e7c87-152">userName</span></span>|<span data-ttu-id="e7c87-153">String</span><span class="sxs-lookup"><span data-stu-id="e7c87-153">String</span></span>|<span data-ttu-id="e7c87-154">Имя пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="e7c87-154">The User Name that is being reported</span></span>|
|<span data-ttu-id="e7c87-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e7c87-155">userPrincipalName</span></span>|<span data-ttu-id="e7c87-156">String</span><span class="sxs-lookup"><span data-stu-id="e7c87-156">String</span></span>|<span data-ttu-id="e7c87-157">Имя участника-пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="e7c87-157">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="e7c87-158">deviceModel</span><span class="sxs-lookup"><span data-stu-id="e7c87-158">deviceModel</span></span>|<span data-ttu-id="e7c87-159">String</span><span class="sxs-lookup"><span data-stu-id="e7c87-159">String</span></span>|<span data-ttu-id="e7c87-160">Модель устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="e7c87-160">The device model that is being reported</span></span>|
|<span data-ttu-id="e7c87-161">state</span><span class="sxs-lookup"><span data-stu-id="e7c87-161">state</span></span>|[<span data-ttu-id="e7c87-162">Комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="e7c87-162">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="e7c87-163">Состояние соответствия для параметра.</span><span class="sxs-lookup"><span data-stu-id="e7c87-163">The compliance state of the setting.</span></span> <span data-ttu-id="e7c87-164">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="e7c87-164">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="e7c87-165">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="e7c87-165">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="e7c87-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7c87-166">DateTimeOffset</span></span>|<span data-ttu-id="e7c87-167">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="e7c87-167">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="e7c87-168">Ответ</span><span class="sxs-lookup"><span data-stu-id="e7c87-168">Response</span></span>
<span data-ttu-id="e7c87-169">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e7c87-169">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7c87-170">Пример</span><span class="sxs-lookup"><span data-stu-id="e7c87-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="e7c87-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="e7c87-171">Request</span></span>
<span data-ttu-id="e7c87-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e7c87-172">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e7c87-173">Ответ</span><span class="sxs-lookup"><span data-stu-id="e7c87-173">Response</span></span>
<span data-ttu-id="e7c87-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e7c87-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



