---
title: Update deviceComplianceSettingState
description: Обновление свойств объекта deviceComplianceSettingState.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ce9dbae6f3b0ffe3b84323018ff37036a554518f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398256"
---
# <a name="update-devicecompliancesettingstate"></a><span data-ttu-id="54c57-103">Update deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="54c57-103">Update deviceComplianceSettingState</span></span>

> <span data-ttu-id="54c57-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="54c57-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="54c57-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54c57-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="54c57-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="54c57-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54c57-107">Обновление свойств объекта [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="54c57-107">Update the properties of a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="54c57-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="54c57-108">Prerequisites</span></span>
<span data-ttu-id="54c57-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="54c57-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="54c57-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="54c57-111">Permission type</span></span>|<span data-ttu-id="54c57-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="54c57-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="54c57-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="54c57-113">Delegated (work or school account)</span></span>|<span data-ttu-id="54c57-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54c57-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="54c57-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="54c57-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="54c57-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54c57-116">Not supported.</span></span>|
|<span data-ttu-id="54c57-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="54c57-117">Application</span></span>|<span data-ttu-id="54c57-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54c57-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="54c57-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="54c57-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

## <a name="request-headers"></a><span data-ttu-id="54c57-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="54c57-120">Request headers</span></span>
|<span data-ttu-id="54c57-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="54c57-121">Header</span></span>|<span data-ttu-id="54c57-122">Значение</span><span class="sxs-lookup"><span data-stu-id="54c57-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="54c57-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="54c57-123">Authorization</span></span>|<span data-ttu-id="54c57-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="54c57-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="54c57-125">Accept</span><span class="sxs-lookup"><span data-stu-id="54c57-125">Accept</span></span>|<span data-ttu-id="54c57-126">application/json</span><span class="sxs-lookup"><span data-stu-id="54c57-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="54c57-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="54c57-127">Request body</span></span>
<span data-ttu-id="54c57-128">В теле запроса добавьте представление объекта [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="54c57-128">In the request body, supply a JSON representation for the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

<span data-ttu-id="54c57-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="54c57-129">The following table shows the properties that are required when you create the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span></span>

|<span data-ttu-id="54c57-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="54c57-130">Property</span></span>|<span data-ttu-id="54c57-131">Тип</span><span class="sxs-lookup"><span data-stu-id="54c57-131">Type</span></span>|<span data-ttu-id="54c57-132">Описание</span><span class="sxs-lookup"><span data-stu-id="54c57-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54c57-133">id</span><span class="sxs-lookup"><span data-stu-id="54c57-133">id</span></span>|<span data-ttu-id="54c57-134">String</span><span class="sxs-lookup"><span data-stu-id="54c57-134">String</span></span>|<span data-ttu-id="54c57-135">Ключ объекта</span><span class="sxs-lookup"><span data-stu-id="54c57-135">Key of the entity</span></span>|
|<span data-ttu-id="54c57-136">platformType</span><span class="sxs-lookup"><span data-stu-id="54c57-136">platformType</span></span>|[<span data-ttu-id="54c57-137">deviceType</span><span class="sxs-lookup"><span data-stu-id="54c57-137">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="54c57-138">Тип платформы устройства.</span><span class="sxs-lookup"><span data-stu-id="54c57-138">Device platform type.</span></span> <span data-ttu-id="54c57-139">Возможные значения: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="54c57-139">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="54c57-140">setting</span><span class="sxs-lookup"><span data-stu-id="54c57-140">setting</span></span>|<span data-ttu-id="54c57-141">String</span><span class="sxs-lookup"><span data-stu-id="54c57-141">String</span></span>|<span data-ttu-id="54c57-142">Имя класса параметров и свойства.</span><span class="sxs-lookup"><span data-stu-id="54c57-142">The setting class name and property name.</span></span>|
|<span data-ttu-id="54c57-143">settingName</span><span class="sxs-lookup"><span data-stu-id="54c57-143">settingName</span></span>|<span data-ttu-id="54c57-144">String</span><span class="sxs-lookup"><span data-stu-id="54c57-144">String</span></span>|<span data-ttu-id="54c57-145">Имя параметра в отчете.</span><span class="sxs-lookup"><span data-stu-id="54c57-145">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="54c57-146">deviceId</span><span class="sxs-lookup"><span data-stu-id="54c57-146">deviceId</span></span>|<span data-ttu-id="54c57-147">String</span><span class="sxs-lookup"><span data-stu-id="54c57-147">String</span></span>|<span data-ttu-id="54c57-148">Идентификатор устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="54c57-148">The Device Id that is being reported</span></span>|
|<span data-ttu-id="54c57-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="54c57-149">deviceName</span></span>|<span data-ttu-id="54c57-150">String</span><span class="sxs-lookup"><span data-stu-id="54c57-150">String</span></span>|<span data-ttu-id="54c57-151">Имя устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="54c57-151">The Device Name that is being reported</span></span>|
|<span data-ttu-id="54c57-152">userId</span><span class="sxs-lookup"><span data-stu-id="54c57-152">userId</span></span>|<span data-ttu-id="54c57-153">String</span><span class="sxs-lookup"><span data-stu-id="54c57-153">String</span></span>|<span data-ttu-id="54c57-154">Идентификатор пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="54c57-154">The user Id that is being reported</span></span>|
|<span data-ttu-id="54c57-155">userEmail</span><span class="sxs-lookup"><span data-stu-id="54c57-155">userEmail</span></span>|<span data-ttu-id="54c57-156">String</span><span class="sxs-lookup"><span data-stu-id="54c57-156">String</span></span>|<span data-ttu-id="54c57-157">Адрес электронной почты пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="54c57-157">The User email address that is being reported</span></span>|
|<span data-ttu-id="54c57-158">userName</span><span class="sxs-lookup"><span data-stu-id="54c57-158">userName</span></span>|<span data-ttu-id="54c57-159">String</span><span class="sxs-lookup"><span data-stu-id="54c57-159">String</span></span>|<span data-ttu-id="54c57-160">Имя пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="54c57-160">The User Name that is being reported</span></span>|
|<span data-ttu-id="54c57-161">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="54c57-161">userPrincipalName</span></span>|<span data-ttu-id="54c57-162">String</span><span class="sxs-lookup"><span data-stu-id="54c57-162">String</span></span>|<span data-ttu-id="54c57-163">Имя участника-пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="54c57-163">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="54c57-164">deviceModel</span><span class="sxs-lookup"><span data-stu-id="54c57-164">deviceModel</span></span>|<span data-ttu-id="54c57-165">String</span><span class="sxs-lookup"><span data-stu-id="54c57-165">String</span></span>|<span data-ttu-id="54c57-166">Модель устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="54c57-166">The device model that is being reported</span></span>|
|<span data-ttu-id="54c57-167">state</span><span class="sxs-lookup"><span data-stu-id="54c57-167">state</span></span>|[<span data-ttu-id="54c57-168">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="54c57-168">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="54c57-169">Соответствие требованиям состояние параметра.</span><span class="sxs-lookup"><span data-stu-id="54c57-169">The compliance state of the setting.</span></span> <span data-ttu-id="54c57-170">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="54c57-170">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="54c57-171">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="54c57-171">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="54c57-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54c57-172">DateTimeOffset</span></span>|<span data-ttu-id="54c57-173">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="54c57-173">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="54c57-174">Ответ</span><span class="sxs-lookup"><span data-stu-id="54c57-174">Response</span></span>
<span data-ttu-id="54c57-175">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="54c57-175">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54c57-176">Пример</span><span class="sxs-lookup"><span data-stu-id="54c57-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="54c57-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="54c57-177">Request</span></span>
<span data-ttu-id="54c57-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="54c57-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="54c57-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="54c57-179">Response</span></span>
<span data-ttu-id="54c57-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="54c57-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




