---
title: Создание объекта deviceConfigurationDeviceStatus
description: Создание объекта deviceConfigurationDeviceStatus.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 817dabc8e2a75b7e0cecbc60064a311f0cafb320
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37368710"
---
# <a name="create-deviceconfigurationdevicestatus"></a><span data-ttu-id="9cc74-103">Создание объекта deviceConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="9cc74-103">Create deviceConfigurationDeviceStatus</span></span>

> <span data-ttu-id="9cc74-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9cc74-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9cc74-105">Создание объекта [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="9cc74-105">Create a new [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9cc74-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9cc74-106">Prerequisites</span></span>
<span data-ttu-id="9cc74-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9cc74-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9cc74-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9cc74-109">Permission type</span></span>|<span data-ttu-id="9cc74-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9cc74-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9cc74-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9cc74-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9cc74-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9cc74-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9cc74-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9cc74-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9cc74-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9cc74-114">Not supported.</span></span>|
|<span data-ttu-id="9cc74-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9cc74-115">Application</span></span>|<span data-ttu-id="9cc74-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9cc74-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9cc74-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9cc74-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="9cc74-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9cc74-118">Request headers</span></span>
|<span data-ttu-id="9cc74-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9cc74-119">Header</span></span>|<span data-ttu-id="9cc74-120">Значение</span><span class="sxs-lookup"><span data-stu-id="9cc74-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9cc74-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9cc74-121">Authorization</span></span>|<span data-ttu-id="9cc74-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9cc74-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9cc74-123">Accept</span><span class="sxs-lookup"><span data-stu-id="9cc74-123">Accept</span></span>|<span data-ttu-id="9cc74-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9cc74-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9cc74-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9cc74-125">Request body</span></span>
<span data-ttu-id="9cc74-126">В теле запроса добавьте представление объекта deviceConfigurationDeviceStatus в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9cc74-126">In the request body, supply a JSON representation for the deviceConfigurationDeviceStatus object.</span></span>

<span data-ttu-id="9cc74-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="9cc74-127">The following table shows the properties that are required when you create the deviceConfigurationDeviceStatus.</span></span>

|<span data-ttu-id="9cc74-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="9cc74-128">Property</span></span>|<span data-ttu-id="9cc74-129">Тип</span><span class="sxs-lookup"><span data-stu-id="9cc74-129">Type</span></span>|<span data-ttu-id="9cc74-130">Описание</span><span class="sxs-lookup"><span data-stu-id="9cc74-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9cc74-131">id</span><span class="sxs-lookup"><span data-stu-id="9cc74-131">id</span></span>|<span data-ttu-id="9cc74-132">Строка</span><span class="sxs-lookup"><span data-stu-id="9cc74-132">String</span></span>|<span data-ttu-id="9cc74-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9cc74-133">Key of the entity.</span></span>|
|<span data-ttu-id="9cc74-134">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="9cc74-134">deviceDisplayName</span></span>|<span data-ttu-id="9cc74-135">String</span><span class="sxs-lookup"><span data-stu-id="9cc74-135">String</span></span>|<span data-ttu-id="9cc74-136">Имя устройства в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="9cc74-136">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="9cc74-137">userName</span><span class="sxs-lookup"><span data-stu-id="9cc74-137">userName</span></span>|<span data-ttu-id="9cc74-138">String</span><span class="sxs-lookup"><span data-stu-id="9cc74-138">String</span></span>|<span data-ttu-id="9cc74-139">Имя пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="9cc74-139">The User Name that is being reported</span></span>|
|<span data-ttu-id="9cc74-140">deviceModel</span><span class="sxs-lookup"><span data-stu-id="9cc74-140">deviceModel</span></span>|<span data-ttu-id="9cc74-141">String</span><span class="sxs-lookup"><span data-stu-id="9cc74-141">String</span></span>|<span data-ttu-id="9cc74-142">Модель устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="9cc74-142">The device model that is being reported</span></span>|
|<span data-ttu-id="9cc74-143">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="9cc74-143">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="9cc74-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9cc74-144">DateTimeOffset</span></span>|<span data-ttu-id="9cc74-145">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="9cc74-145">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="9cc74-146">status</span><span class="sxs-lookup"><span data-stu-id="9cc74-146">status</span></span>|[<span data-ttu-id="9cc74-147">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="9cc74-147">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="9cc74-148">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="9cc74-148">Compliance status of the policy report.</span></span> <span data-ttu-id="9cc74-149">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="9cc74-149">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="9cc74-150">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="9cc74-150">lastReportedDateTime</span></span>|<span data-ttu-id="9cc74-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9cc74-151">DateTimeOffset</span></span>|<span data-ttu-id="9cc74-152">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="9cc74-152">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="9cc74-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9cc74-153">userPrincipalName</span></span>|<span data-ttu-id="9cc74-154">String</span><span class="sxs-lookup"><span data-stu-id="9cc74-154">String</span></span>|<span data-ttu-id="9cc74-155">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="9cc74-155">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="9cc74-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="9cc74-156">Response</span></span>
<span data-ttu-id="9cc74-157">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9cc74-157">If successful, this method returns a `201 Created` response code and a [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9cc74-158">Пример</span><span class="sxs-lookup"><span data-stu-id="9cc74-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="9cc74-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="9cc74-159">Request</span></span>
<span data-ttu-id="9cc74-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9cc74-160">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
Content-type: application/json
Content-length: 429

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="9cc74-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="9cc74-161">Response</span></span>
<span data-ttu-id="9cc74-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9cc74-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 478

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
  "id": "674e98e5-98e5-674e-e598-4e67e5984e67",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```




