---
title: Обновление объекта deviceComplianceDeviceStatus
description: Обновление свойств объекта deviceComplianceDeviceStatus.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 28fee9e63744a9b841d8f09e36290513ea8db09e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43400181"
---
# <a name="update-devicecompliancedevicestatus"></a><span data-ttu-id="b0381-103">Обновление объекта deviceComplianceDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="b0381-103">Update deviceComplianceDeviceStatus</span></span>

<span data-ttu-id="b0381-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0381-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b0381-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b0381-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0381-106">Обновление свойств объекта [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="b0381-106">Update the properties of a [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b0381-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b0381-107">Prerequisites</span></span>
<span data-ttu-id="b0381-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0381-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0381-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b0381-110">Permission type</span></span>|<span data-ttu-id="b0381-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b0381-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0381-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b0381-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b0381-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0381-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b0381-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b0381-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0381-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0381-115">Not supported.</span></span>|
|<span data-ttu-id="b0381-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b0381-116">Application</span></span>|<span data-ttu-id="b0381-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0381-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0381-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b0381-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="b0381-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b0381-119">Request headers</span></span>
|<span data-ttu-id="b0381-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b0381-120">Header</span></span>|<span data-ttu-id="b0381-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b0381-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0381-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b0381-122">Authorization</span></span>|<span data-ttu-id="b0381-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b0381-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b0381-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b0381-124">Accept</span></span>|<span data-ttu-id="b0381-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b0381-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0381-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b0381-126">Request body</span></span>
<span data-ttu-id="b0381-127">В тексте запроса добавьте представление объекта [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b0381-127">In the request body, supply a JSON representation for the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>

<span data-ttu-id="b0381-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="b0381-128">The following table shows the properties that are required when you create the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span></span>

|<span data-ttu-id="b0381-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b0381-129">Property</span></span>|<span data-ttu-id="b0381-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b0381-130">Type</span></span>|<span data-ttu-id="b0381-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b0381-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0381-132">id</span><span class="sxs-lookup"><span data-stu-id="b0381-132">id</span></span>|<span data-ttu-id="b0381-133">Строка</span><span class="sxs-lookup"><span data-stu-id="b0381-133">String</span></span>|<span data-ttu-id="b0381-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b0381-134">Key of the entity.</span></span>|
|<span data-ttu-id="b0381-135">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="b0381-135">deviceDisplayName</span></span>|<span data-ttu-id="b0381-136">String</span><span class="sxs-lookup"><span data-stu-id="b0381-136">String</span></span>|<span data-ttu-id="b0381-137">Имя устройства в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="b0381-137">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="b0381-138">userName</span><span class="sxs-lookup"><span data-stu-id="b0381-138">userName</span></span>|<span data-ttu-id="b0381-139">String</span><span class="sxs-lookup"><span data-stu-id="b0381-139">String</span></span>|<span data-ttu-id="b0381-140">Имя пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="b0381-140">The User Name that is being reported</span></span>|
|<span data-ttu-id="b0381-141">deviceModel</span><span class="sxs-lookup"><span data-stu-id="b0381-141">deviceModel</span></span>|<span data-ttu-id="b0381-142">String</span><span class="sxs-lookup"><span data-stu-id="b0381-142">String</span></span>|<span data-ttu-id="b0381-143">Модель устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="b0381-143">The device model that is being reported</span></span>|
|<span data-ttu-id="b0381-144">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="b0381-144">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="b0381-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0381-145">DateTimeOffset</span></span>|<span data-ttu-id="b0381-146">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="b0381-146">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="b0381-147">status</span><span class="sxs-lookup"><span data-stu-id="b0381-147">status</span></span>|[<span data-ttu-id="b0381-148">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="b0381-148">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="b0381-149">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="b0381-149">Compliance status of the policy report.</span></span> <span data-ttu-id="b0381-150">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="b0381-150">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="b0381-151">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="b0381-151">lastReportedDateTime</span></span>|<span data-ttu-id="b0381-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0381-152">DateTimeOffset</span></span>|<span data-ttu-id="b0381-153">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="b0381-153">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="b0381-154">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b0381-154">userPrincipalName</span></span>|<span data-ttu-id="b0381-155">String</span><span class="sxs-lookup"><span data-stu-id="b0381-155">String</span></span>|<span data-ttu-id="b0381-156">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="b0381-156">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="b0381-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0381-157">Response</span></span>
<span data-ttu-id="b0381-158">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b0381-158">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0381-159">Пример</span><span class="sxs-lookup"><span data-stu-id="b0381-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="b0381-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="b0381-160">Request</span></span>
<span data-ttu-id="b0381-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b0381-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
Content-type: application/json
Content-length: 426

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="b0381-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0381-162">Response</span></span>
<span data-ttu-id="b0381-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b0381-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 475

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
  "id": "c6c78124-8124-c6c7-2481-c7c62481c7c6",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```






