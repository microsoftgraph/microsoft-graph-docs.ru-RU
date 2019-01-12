---
title: Создание объекта deviceComplianceSettingState
description: Создание объекта deviceComplianceSettingState.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e7c79676eac77cebe645c0c26785421dd0dc278b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27959086"
---
# <a name="create-devicecompliancesettingstate"></a><span data-ttu-id="f8520-103">Создание объекта deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="f8520-103">Create deviceComplianceSettingState</span></span>

> <span data-ttu-id="f8520-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f8520-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f8520-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8520-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f8520-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f8520-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f8520-107">Создание объекта [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="f8520-107">Create a new [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f8520-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f8520-108">Prerequisites</span></span>
<span data-ttu-id="f8520-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8520-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8520-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f8520-111">Permission type</span></span>|<span data-ttu-id="f8520-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f8520-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8520-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f8520-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f8520-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8520-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f8520-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f8520-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8520-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8520-116">Not supported.</span></span>|
|<span data-ttu-id="f8520-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f8520-117">Application</span></span>|<span data-ttu-id="f8520-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8520-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8520-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f8520-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="f8520-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f8520-120">Request headers</span></span>
|<span data-ttu-id="f8520-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f8520-121">Header</span></span>|<span data-ttu-id="f8520-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f8520-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8520-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8520-123">Authorization</span></span>|<span data-ttu-id="f8520-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f8520-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f8520-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f8520-125">Accept</span></span>|<span data-ttu-id="f8520-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f8520-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8520-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f8520-127">Request body</span></span>
<span data-ttu-id="f8520-128">В тексте запроса добавьте представление объекта deviceComplianceSettingState в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f8520-128">In the request body, supply a JSON representation for the deviceComplianceSettingState object.</span></span>

<span data-ttu-id="f8520-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceComplianceSettingState.</span><span class="sxs-lookup"><span data-stu-id="f8520-129">The following table shows the properties that are required when you create the deviceComplianceSettingState.</span></span>

|<span data-ttu-id="f8520-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f8520-130">Property</span></span>|<span data-ttu-id="f8520-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f8520-131">Type</span></span>|<span data-ttu-id="f8520-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f8520-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8520-133">id</span><span class="sxs-lookup"><span data-stu-id="f8520-133">id</span></span>|<span data-ttu-id="f8520-134">String</span><span class="sxs-lookup"><span data-stu-id="f8520-134">String</span></span>|<span data-ttu-id="f8520-135">Ключ объекта</span><span class="sxs-lookup"><span data-stu-id="f8520-135">Key of the entity</span></span>|
|<span data-ttu-id="f8520-136">platformType</span><span class="sxs-lookup"><span data-stu-id="f8520-136">platformType</span></span>|[<span data-ttu-id="f8520-137">deviceType</span><span class="sxs-lookup"><span data-stu-id="f8520-137">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="f8520-138">Тип платформы устройства.</span><span class="sxs-lookup"><span data-stu-id="f8520-138">Device platform type.</span></span> <span data-ttu-id="f8520-139">Возможные значения: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="f8520-139">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="f8520-140">setting</span><span class="sxs-lookup"><span data-stu-id="f8520-140">setting</span></span>|<span data-ttu-id="f8520-141">String</span><span class="sxs-lookup"><span data-stu-id="f8520-141">String</span></span>|<span data-ttu-id="f8520-142">Имя класса параметров и свойства.</span><span class="sxs-lookup"><span data-stu-id="f8520-142">The setting class name and property name.</span></span>|
|<span data-ttu-id="f8520-143">settingName</span><span class="sxs-lookup"><span data-stu-id="f8520-143">settingName</span></span>|<span data-ttu-id="f8520-144">String</span><span class="sxs-lookup"><span data-stu-id="f8520-144">String</span></span>|<span data-ttu-id="f8520-145">Имя параметра в отчете.</span><span class="sxs-lookup"><span data-stu-id="f8520-145">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="f8520-146">deviceId</span><span class="sxs-lookup"><span data-stu-id="f8520-146">deviceId</span></span>|<span data-ttu-id="f8520-147">String</span><span class="sxs-lookup"><span data-stu-id="f8520-147">String</span></span>|<span data-ttu-id="f8520-148">Идентификатор устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="f8520-148">The Device Id that is being reported</span></span>|
|<span data-ttu-id="f8520-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="f8520-149">deviceName</span></span>|<span data-ttu-id="f8520-150">String</span><span class="sxs-lookup"><span data-stu-id="f8520-150">String</span></span>|<span data-ttu-id="f8520-151">Имя устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="f8520-151">The Device Name that is being reported</span></span>|
|<span data-ttu-id="f8520-152">userId</span><span class="sxs-lookup"><span data-stu-id="f8520-152">userId</span></span>|<span data-ttu-id="f8520-153">String</span><span class="sxs-lookup"><span data-stu-id="f8520-153">String</span></span>|<span data-ttu-id="f8520-154">Идентификатор пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="f8520-154">The user Id that is being reported</span></span>|
|<span data-ttu-id="f8520-155">userEmail</span><span class="sxs-lookup"><span data-stu-id="f8520-155">userEmail</span></span>|<span data-ttu-id="f8520-156">String</span><span class="sxs-lookup"><span data-stu-id="f8520-156">String</span></span>|<span data-ttu-id="f8520-157">Адрес электронной почты пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="f8520-157">The User email address that is being reported</span></span>|
|<span data-ttu-id="f8520-158">userName</span><span class="sxs-lookup"><span data-stu-id="f8520-158">userName</span></span>|<span data-ttu-id="f8520-159">String</span><span class="sxs-lookup"><span data-stu-id="f8520-159">String</span></span>|<span data-ttu-id="f8520-160">Имя пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="f8520-160">The User Name that is being reported</span></span>|
|<span data-ttu-id="f8520-161">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f8520-161">userPrincipalName</span></span>|<span data-ttu-id="f8520-162">String</span><span class="sxs-lookup"><span data-stu-id="f8520-162">String</span></span>|<span data-ttu-id="f8520-163">Имя участника-пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="f8520-163">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="f8520-164">deviceModel</span><span class="sxs-lookup"><span data-stu-id="f8520-164">deviceModel</span></span>|<span data-ttu-id="f8520-165">String</span><span class="sxs-lookup"><span data-stu-id="f8520-165">String</span></span>|<span data-ttu-id="f8520-166">Модель устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="f8520-166">The device model that is being reported</span></span>|
|<span data-ttu-id="f8520-167">state</span><span class="sxs-lookup"><span data-stu-id="f8520-167">state</span></span>|[<span data-ttu-id="f8520-168">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="f8520-168">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="f8520-169">Соответствие требованиям состояние параметра.</span><span class="sxs-lookup"><span data-stu-id="f8520-169">The compliance state of the setting.</span></span> <span data-ttu-id="f8520-170">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="f8520-170">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="f8520-171">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f8520-171">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="f8520-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8520-172">DateTimeOffset</span></span>|<span data-ttu-id="f8520-173">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="f8520-173">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="f8520-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="f8520-174">Response</span></span>
<span data-ttu-id="f8520-175">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f8520-175">If successful, this method returns a `201 Created` response code and a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8520-176">Пример</span><span class="sxs-lookup"><span data-stu-id="f8520-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="f8520-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="f8520-177">Request</span></span>
<span data-ttu-id="f8520-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f8520-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f8520-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="f8520-179">Response</span></span>
<span data-ttu-id="f8520-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f8520-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





