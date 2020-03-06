---
title: Создание объекта deviceComplianceDeviceStatus
description: Создание объекта deviceComplianceDeviceStatus.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a19814ef1428adc70390bb1519cf4a26441f278d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42515128"
---
# <a name="create-devicecompliancedevicestatus"></a><span data-ttu-id="2753b-103">Создание объекта deviceComplianceDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="2753b-103">Create deviceComplianceDeviceStatus</span></span>

<span data-ttu-id="2753b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2753b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2753b-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2753b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2753b-106">Создание объекта [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="2753b-106">Create a new [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2753b-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2753b-107">Prerequisites</span></span>
<span data-ttu-id="2753b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2753b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2753b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2753b-110">Permission type</span></span>|<span data-ttu-id="2753b-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2753b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2753b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2753b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2753b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2753b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2753b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2753b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2753b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2753b-115">Not supported.</span></span>|
|<span data-ttu-id="2753b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2753b-116">Application</span></span>|<span data-ttu-id="2753b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2753b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2753b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2753b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="2753b-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2753b-119">Request headers</span></span>
|<span data-ttu-id="2753b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2753b-120">Header</span></span>|<span data-ttu-id="2753b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2753b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2753b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2753b-122">Authorization</span></span>|<span data-ttu-id="2753b-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2753b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2753b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="2753b-124">Accept</span></span>|<span data-ttu-id="2753b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2753b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2753b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2753b-126">Request body</span></span>
<span data-ttu-id="2753b-127">В тексте запроса добавьте представление объекта deviceComplianceDeviceStatus в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2753b-127">In the request body, supply a JSON representation for the deviceComplianceDeviceStatus object.</span></span>

<span data-ttu-id="2753b-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceComplianceDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="2753b-128">The following table shows the properties that are required when you create the deviceComplianceDeviceStatus.</span></span>

|<span data-ttu-id="2753b-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="2753b-129">Property</span></span>|<span data-ttu-id="2753b-130">Тип</span><span class="sxs-lookup"><span data-stu-id="2753b-130">Type</span></span>|<span data-ttu-id="2753b-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2753b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2753b-132">id</span><span class="sxs-lookup"><span data-stu-id="2753b-132">id</span></span>|<span data-ttu-id="2753b-133">Строка</span><span class="sxs-lookup"><span data-stu-id="2753b-133">String</span></span>|<span data-ttu-id="2753b-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2753b-134">Key of the entity.</span></span>|
|<span data-ttu-id="2753b-135">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="2753b-135">deviceDisplayName</span></span>|<span data-ttu-id="2753b-136">Строка</span><span class="sxs-lookup"><span data-stu-id="2753b-136">String</span></span>|<span data-ttu-id="2753b-137">Имя устройства в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="2753b-137">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="2753b-138">userName</span><span class="sxs-lookup"><span data-stu-id="2753b-138">userName</span></span>|<span data-ttu-id="2753b-139">Строка</span><span class="sxs-lookup"><span data-stu-id="2753b-139">String</span></span>|<span data-ttu-id="2753b-140">Имя пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="2753b-140">The User Name that is being reported</span></span>|
|<span data-ttu-id="2753b-141">deviceModel</span><span class="sxs-lookup"><span data-stu-id="2753b-141">deviceModel</span></span>|<span data-ttu-id="2753b-142">String</span><span class="sxs-lookup"><span data-stu-id="2753b-142">String</span></span>|<span data-ttu-id="2753b-143">Модель устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="2753b-143">The device model that is being reported</span></span>|
|<span data-ttu-id="2753b-144">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="2753b-144">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="2753b-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2753b-145">DateTimeOffset</span></span>|<span data-ttu-id="2753b-146">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="2753b-146">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="2753b-147">status</span><span class="sxs-lookup"><span data-stu-id="2753b-147">status</span></span>|[<span data-ttu-id="2753b-148">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="2753b-148">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="2753b-149">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="2753b-149">Compliance status of the policy report.</span></span> <span data-ttu-id="2753b-150">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="2753b-150">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="2753b-151">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="2753b-151">lastReportedDateTime</span></span>|<span data-ttu-id="2753b-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2753b-152">DateTimeOffset</span></span>|<span data-ttu-id="2753b-153">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="2753b-153">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="2753b-154">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2753b-154">userPrincipalName</span></span>|<span data-ttu-id="2753b-155">String</span><span class="sxs-lookup"><span data-stu-id="2753b-155">String</span></span>|<span data-ttu-id="2753b-156">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="2753b-156">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="2753b-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="2753b-157">Response</span></span>
<span data-ttu-id="2753b-158">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2753b-158">If successful, this method returns a `201 Created` response code and a [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2753b-159">Пример</span><span class="sxs-lookup"><span data-stu-id="2753b-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="2753b-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="2753b-160">Request</span></span>
<span data-ttu-id="2753b-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2753b-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
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

### <a name="response"></a><span data-ttu-id="2753b-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="2753b-162">Response</span></span>
<span data-ttu-id="2753b-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2753b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




