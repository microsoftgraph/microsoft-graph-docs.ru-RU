---
title: Update deviceComplianceSettingState
description: Обновление свойств объекта deviceComplianceSettingState.
author: tfitzmac
ms.openlocfilehash: 699ddfebe1e333c97d6fc186e4d65e40c4f367aa
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348211"
---
# <a name="update-devicecompliancesettingstate"></a><span data-ttu-id="3923c-103">Update deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="3923c-103">Update deviceComplianceSettingState</span></span>

> <span data-ttu-id="3923c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3923c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3923c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3923c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3923c-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3923c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3923c-107">Обновление свойств объекта [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="3923c-107">Update the properties of a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3923c-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="3923c-108">Prerequisites</span></span>
<span data-ttu-id="3923c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3923c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3923c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3923c-111">Permission type</span></span>|<span data-ttu-id="3923c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3923c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3923c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3923c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3923c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3923c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3923c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3923c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3923c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3923c-116">Not supported.</span></span>|
|<span data-ttu-id="3923c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3923c-117">Application</span></span>|<span data-ttu-id="3923c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3923c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3923c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3923c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

## <a name="request-headers"></a><span data-ttu-id="3923c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3923c-120">Request headers</span></span>
|<span data-ttu-id="3923c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3923c-121">Header</span></span>|<span data-ttu-id="3923c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3923c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3923c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3923c-123">Authorization</span></span>|<span data-ttu-id="3923c-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3923c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3923c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3923c-125">Accept</span></span>|<span data-ttu-id="3923c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3923c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3923c-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3923c-127">Request body</span></span>
<span data-ttu-id="3923c-128">В теле запроса добавьте представление объекта [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3923c-128">In the request body, supply a JSON representation for the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

<span data-ttu-id="3923c-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="3923c-129">The following table shows the properties that are required when you create the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span></span>

|<span data-ttu-id="3923c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3923c-130">Property</span></span>|<span data-ttu-id="3923c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3923c-131">Type</span></span>|<span data-ttu-id="3923c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3923c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3923c-133">id</span><span class="sxs-lookup"><span data-stu-id="3923c-133">id</span></span>|<span data-ttu-id="3923c-134">String</span><span class="sxs-lookup"><span data-stu-id="3923c-134">String</span></span>|<span data-ttu-id="3923c-135">Ключ объекта</span><span class="sxs-lookup"><span data-stu-id="3923c-135">Key of the entity</span></span>|
|<span data-ttu-id="3923c-136">platformType</span><span class="sxs-lookup"><span data-stu-id="3923c-136">platformType</span></span>|[<span data-ttu-id="3923c-137">deviceType</span><span class="sxs-lookup"><span data-stu-id="3923c-137">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="3923c-138">Тип платформы устройства.</span><span class="sxs-lookup"><span data-stu-id="3923c-138">Device platform type.</span></span> <span data-ttu-id="3923c-139">Возможные значения: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="3923c-139">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="3923c-140">setting</span><span class="sxs-lookup"><span data-stu-id="3923c-140">setting</span></span>|<span data-ttu-id="3923c-141">String</span><span class="sxs-lookup"><span data-stu-id="3923c-141">String</span></span>|<span data-ttu-id="3923c-142">Имя класса параметров и свойства.</span><span class="sxs-lookup"><span data-stu-id="3923c-142">The setting class name and property name.</span></span>|
|<span data-ttu-id="3923c-143">settingName</span><span class="sxs-lookup"><span data-stu-id="3923c-143">settingName</span></span>|<span data-ttu-id="3923c-144">String</span><span class="sxs-lookup"><span data-stu-id="3923c-144">String</span></span>|<span data-ttu-id="3923c-145">Имя параметра в отчете.</span><span class="sxs-lookup"><span data-stu-id="3923c-145">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="3923c-146">deviceId</span><span class="sxs-lookup"><span data-stu-id="3923c-146">deviceId</span></span>|<span data-ttu-id="3923c-147">String</span><span class="sxs-lookup"><span data-stu-id="3923c-147">String</span></span>|<span data-ttu-id="3923c-148">Идентификатор устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="3923c-148">The Device Id that is being reported</span></span>|
|<span data-ttu-id="3923c-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="3923c-149">deviceName</span></span>|<span data-ttu-id="3923c-150">String</span><span class="sxs-lookup"><span data-stu-id="3923c-150">String</span></span>|<span data-ttu-id="3923c-151">Имя устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="3923c-151">The Device Name that is being reported</span></span>|
|<span data-ttu-id="3923c-152">userId</span><span class="sxs-lookup"><span data-stu-id="3923c-152">userId</span></span>|<span data-ttu-id="3923c-153">String</span><span class="sxs-lookup"><span data-stu-id="3923c-153">String</span></span>|<span data-ttu-id="3923c-154">Идентификатор пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="3923c-154">The user Id that is being reported</span></span>|
|<span data-ttu-id="3923c-155">userEmail</span><span class="sxs-lookup"><span data-stu-id="3923c-155">userEmail</span></span>|<span data-ttu-id="3923c-156">String</span><span class="sxs-lookup"><span data-stu-id="3923c-156">String</span></span>|<span data-ttu-id="3923c-157">Адрес электронной почты пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="3923c-157">The User email address that is being reported</span></span>|
|<span data-ttu-id="3923c-158">userName</span><span class="sxs-lookup"><span data-stu-id="3923c-158">userName</span></span>|<span data-ttu-id="3923c-159">String</span><span class="sxs-lookup"><span data-stu-id="3923c-159">String</span></span>|<span data-ttu-id="3923c-160">Имя пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="3923c-160">The User Name that is being reported</span></span>|
|<span data-ttu-id="3923c-161">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3923c-161">userPrincipalName</span></span>|<span data-ttu-id="3923c-162">String</span><span class="sxs-lookup"><span data-stu-id="3923c-162">String</span></span>|<span data-ttu-id="3923c-163">Имя участника-пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="3923c-163">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="3923c-164">deviceModel</span><span class="sxs-lookup"><span data-stu-id="3923c-164">deviceModel</span></span>|<span data-ttu-id="3923c-165">String</span><span class="sxs-lookup"><span data-stu-id="3923c-165">String</span></span>|<span data-ttu-id="3923c-166">Модель устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="3923c-166">The device model that is being reported</span></span>|
|<span data-ttu-id="3923c-167">state</span><span class="sxs-lookup"><span data-stu-id="3923c-167">state</span></span>|[<span data-ttu-id="3923c-168">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="3923c-168">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="3923c-169">Соответствие требованиям состояние параметра.</span><span class="sxs-lookup"><span data-stu-id="3923c-169">The compliance state of the setting.</span></span> <span data-ttu-id="3923c-170">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="3923c-170">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="3923c-171">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="3923c-171">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="3923c-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3923c-172">DateTimeOffset</span></span>|<span data-ttu-id="3923c-173">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="3923c-173">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="3923c-174">Ответ</span><span class="sxs-lookup"><span data-stu-id="3923c-174">Response</span></span>
<span data-ttu-id="3923c-175">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3923c-175">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3923c-176">Пример</span><span class="sxs-lookup"><span data-stu-id="3923c-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="3923c-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="3923c-177">Request</span></span>
<span data-ttu-id="3923c-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3923c-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
Content-type: application/json
Content-length: 482

{
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

### <a name="response"></a><span data-ttu-id="3923c-179">Ответ</span><span class="sxs-lookup"><span data-stu-id="3923c-179">Response</span></span>
<span data-ttu-id="3923c-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3923c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





