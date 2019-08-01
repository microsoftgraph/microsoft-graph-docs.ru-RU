---
title: Создание объекта deviceComplianceSettingState
description: Создание объекта deviceComplianceSettingState.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b5e952ca051f7cc01ae5662e0a853b3c8f642f67
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36019298"
---
# <a name="create-devicecompliancesettingstate"></a><span data-ttu-id="6b982-103">Создание объекта deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="6b982-103">Create deviceComplianceSettingState</span></span>

> <span data-ttu-id="6b982-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6b982-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b982-105">Создание объекта [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="6b982-105">Create a new [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6b982-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6b982-106">Prerequisites</span></span>
<span data-ttu-id="6b982-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b982-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b982-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6b982-109">Permission type</span></span>|<span data-ttu-id="6b982-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6b982-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6b982-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6b982-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6b982-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b982-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6b982-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6b982-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b982-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b982-114">Not supported.</span></span>|
|<span data-ttu-id="6b982-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6b982-115">Application</span></span>|<span data-ttu-id="6b982-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b982-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b982-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6b982-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="6b982-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6b982-118">Request headers</span></span>
|<span data-ttu-id="6b982-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6b982-119">Header</span></span>|<span data-ttu-id="6b982-120">Значение</span><span class="sxs-lookup"><span data-stu-id="6b982-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6b982-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6b982-121">Authorization</span></span>|<span data-ttu-id="6b982-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6b982-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6b982-123">Accept</span><span class="sxs-lookup"><span data-stu-id="6b982-123">Accept</span></span>|<span data-ttu-id="6b982-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6b982-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b982-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6b982-125">Request body</span></span>
<span data-ttu-id="6b982-126">В тексте запроса добавьте представление объекта deviceComplianceSettingState в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6b982-126">In the request body, supply a JSON representation for the deviceComplianceSettingState object.</span></span>

<span data-ttu-id="6b982-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceComplianceSettingState.</span><span class="sxs-lookup"><span data-stu-id="6b982-127">The following table shows the properties that are required when you create the deviceComplianceSettingState.</span></span>

|<span data-ttu-id="6b982-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="6b982-128">Property</span></span>|<span data-ttu-id="6b982-129">Тип</span><span class="sxs-lookup"><span data-stu-id="6b982-129">Type</span></span>|<span data-ttu-id="6b982-130">Описание</span><span class="sxs-lookup"><span data-stu-id="6b982-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b982-131">id</span><span class="sxs-lookup"><span data-stu-id="6b982-131">id</span></span>|<span data-ttu-id="6b982-132">Строка</span><span class="sxs-lookup"><span data-stu-id="6b982-132">String</span></span>|<span data-ttu-id="6b982-133">Ключ объекта</span><span class="sxs-lookup"><span data-stu-id="6b982-133">Key of the entity</span></span>|
|<span data-ttu-id="6b982-134">setting</span><span class="sxs-lookup"><span data-stu-id="6b982-134">setting</span></span>|<span data-ttu-id="6b982-135">String</span><span class="sxs-lookup"><span data-stu-id="6b982-135">String</span></span>|<span data-ttu-id="6b982-136">Имя класса параметров и свойства.</span><span class="sxs-lookup"><span data-stu-id="6b982-136">The setting class name and property name.</span></span>|
|<span data-ttu-id="6b982-137">settingName</span><span class="sxs-lookup"><span data-stu-id="6b982-137">settingName</span></span>|<span data-ttu-id="6b982-138">String</span><span class="sxs-lookup"><span data-stu-id="6b982-138">String</span></span>|<span data-ttu-id="6b982-139">Имя параметра в отчете</span><span class="sxs-lookup"><span data-stu-id="6b982-139">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="6b982-140">deviceId</span><span class="sxs-lookup"><span data-stu-id="6b982-140">deviceId</span></span>|<span data-ttu-id="6b982-141">String</span><span class="sxs-lookup"><span data-stu-id="6b982-141">String</span></span>|<span data-ttu-id="6b982-142">ИД устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="6b982-142">The Device Id that is being reported</span></span>|
|<span data-ttu-id="6b982-143">deviceName</span><span class="sxs-lookup"><span data-stu-id="6b982-143">deviceName</span></span>|<span data-ttu-id="6b982-144">String</span><span class="sxs-lookup"><span data-stu-id="6b982-144">String</span></span>|<span data-ttu-id="6b982-145">Имя устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="6b982-145">The Device Name that is being reported</span></span>|
|<span data-ttu-id="6b982-146">userId</span><span class="sxs-lookup"><span data-stu-id="6b982-146">userId</span></span>|<span data-ttu-id="6b982-147">String</span><span class="sxs-lookup"><span data-stu-id="6b982-147">String</span></span>|<span data-ttu-id="6b982-148">ИД пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="6b982-148">The user Id that is being reported</span></span>|
|<span data-ttu-id="6b982-149">userEmail</span><span class="sxs-lookup"><span data-stu-id="6b982-149">userEmail</span></span>|<span data-ttu-id="6b982-150">String</span><span class="sxs-lookup"><span data-stu-id="6b982-150">String</span></span>|<span data-ttu-id="6b982-151">Электронный адрес пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="6b982-151">The User email address that is being reported</span></span>|
|<span data-ttu-id="6b982-152">userName</span><span class="sxs-lookup"><span data-stu-id="6b982-152">userName</span></span>|<span data-ttu-id="6b982-153">String</span><span class="sxs-lookup"><span data-stu-id="6b982-153">String</span></span>|<span data-ttu-id="6b982-154">Имя пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="6b982-154">The User Name that is being reported</span></span>|
|<span data-ttu-id="6b982-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6b982-155">userPrincipalName</span></span>|<span data-ttu-id="6b982-156">String</span><span class="sxs-lookup"><span data-stu-id="6b982-156">String</span></span>|<span data-ttu-id="6b982-157">Имя участника-пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="6b982-157">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="6b982-158">deviceModel</span><span class="sxs-lookup"><span data-stu-id="6b982-158">deviceModel</span></span>|<span data-ttu-id="6b982-159">String</span><span class="sxs-lookup"><span data-stu-id="6b982-159">String</span></span>|<span data-ttu-id="6b982-160">Модель устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="6b982-160">The device model that is being reported</span></span>|
|<span data-ttu-id="6b982-161">state</span><span class="sxs-lookup"><span data-stu-id="6b982-161">state</span></span>|[<span data-ttu-id="6b982-162">Комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="6b982-162">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="6b982-163">Состояние соответствия для параметра.</span><span class="sxs-lookup"><span data-stu-id="6b982-163">The compliance state of the setting.</span></span> <span data-ttu-id="6b982-164">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="6b982-164">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="6b982-165">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="6b982-165">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="6b982-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b982-166">DateTimeOffset</span></span>|<span data-ttu-id="6b982-167">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="6b982-167">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="6b982-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b982-168">Response</span></span>
<span data-ttu-id="6b982-169">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6b982-169">If successful, this method returns a `201 Created` response code and a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b982-170">Пример</span><span class="sxs-lookup"><span data-stu-id="6b982-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="6b982-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="6b982-171">Request</span></span>
<span data-ttu-id="6b982-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6b982-172">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6b982-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b982-173">Response</span></span>
<span data-ttu-id="6b982-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6b982-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



