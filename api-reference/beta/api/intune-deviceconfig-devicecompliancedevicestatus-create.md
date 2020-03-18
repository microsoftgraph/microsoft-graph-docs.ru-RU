---
title: Создание объекта deviceComplianceDeviceStatus
description: Создание объекта deviceComplianceDeviceStatus.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: aa3d9ea5e68be8656a7702b7321d8ca982328468
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42756164"
---
# <a name="create-devicecompliancedevicestatus"></a><span data-ttu-id="ba903-103">Создание объекта deviceComplianceDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="ba903-103">Create deviceComplianceDeviceStatus</span></span>

> <span data-ttu-id="ba903-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba903-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba903-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ba903-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba903-106">Создание объекта [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="ba903-106">Create a new [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ba903-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ba903-107">Prerequisites</span></span>
<span data-ttu-id="ba903-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba903-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba903-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ba903-110">Permission type</span></span>|<span data-ttu-id="ba903-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ba903-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ba903-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ba903-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ba903-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba903-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ba903-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ba903-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ba903-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba903-115">Not supported.</span></span>|
|<span data-ttu-id="ba903-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="ba903-116">Application</span></span>|<span data-ttu-id="ba903-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba903-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba903-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ba903-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="ba903-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ba903-119">Request headers</span></span>
|<span data-ttu-id="ba903-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ba903-120">Header</span></span>|<span data-ttu-id="ba903-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ba903-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ba903-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba903-122">Authorization</span></span>|<span data-ttu-id="ba903-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ba903-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ba903-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ba903-124">Accept</span></span>|<span data-ttu-id="ba903-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ba903-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba903-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ba903-126">Request body</span></span>
<span data-ttu-id="ba903-127">В тексте запроса добавьте представление объекта deviceComplianceDeviceStatus в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ba903-127">In the request body, supply a JSON representation for the deviceComplianceDeviceStatus object.</span></span>

<span data-ttu-id="ba903-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceComplianceDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="ba903-128">The following table shows the properties that are required when you create the deviceComplianceDeviceStatus.</span></span>

|<span data-ttu-id="ba903-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ba903-129">Property</span></span>|<span data-ttu-id="ba903-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ba903-130">Type</span></span>|<span data-ttu-id="ba903-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ba903-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba903-132">id</span><span class="sxs-lookup"><span data-stu-id="ba903-132">id</span></span>|<span data-ttu-id="ba903-133">Строка</span><span class="sxs-lookup"><span data-stu-id="ba903-133">String</span></span>|<span data-ttu-id="ba903-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ba903-134">Key of the entity.</span></span>|
|<span data-ttu-id="ba903-135">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="ba903-135">deviceDisplayName</span></span>|<span data-ttu-id="ba903-136">String</span><span class="sxs-lookup"><span data-stu-id="ba903-136">String</span></span>|<span data-ttu-id="ba903-137">Имя устройства в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="ba903-137">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="ba903-138">userName</span><span class="sxs-lookup"><span data-stu-id="ba903-138">userName</span></span>|<span data-ttu-id="ba903-139">String</span><span class="sxs-lookup"><span data-stu-id="ba903-139">String</span></span>|<span data-ttu-id="ba903-140">Имя пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="ba903-140">The User Name that is being reported</span></span>|
|<span data-ttu-id="ba903-141">deviceModel</span><span class="sxs-lookup"><span data-stu-id="ba903-141">deviceModel</span></span>|<span data-ttu-id="ba903-142">String</span><span class="sxs-lookup"><span data-stu-id="ba903-142">String</span></span>|<span data-ttu-id="ba903-143">Модель устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="ba903-143">The device model that is being reported</span></span>|
|<span data-ttu-id="ba903-144">platform</span><span class="sxs-lookup"><span data-stu-id="ba903-144">platform</span></span>|<span data-ttu-id="ba903-145">Int32</span><span class="sxs-lookup"><span data-stu-id="ba903-145">Int32</span></span>|<span data-ttu-id="ba903-146">Платформа для устройства, о котором сообщается</span><span class="sxs-lookup"><span data-stu-id="ba903-146">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="ba903-147">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ba903-147">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="ba903-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba903-148">DateTimeOffset</span></span>|<span data-ttu-id="ba903-149">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="ba903-149">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="ba903-150">status</span><span class="sxs-lookup"><span data-stu-id="ba903-150">status</span></span>|[<span data-ttu-id="ba903-151">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="ba903-151">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="ba903-152">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="ba903-152">Compliance status of the policy report.</span></span> <span data-ttu-id="ba903-153">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="ba903-153">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="ba903-154">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="ba903-154">lastReportedDateTime</span></span>|<span data-ttu-id="ba903-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba903-155">DateTimeOffset</span></span>|<span data-ttu-id="ba903-156">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="ba903-156">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="ba903-157">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ba903-157">userPrincipalName</span></span>|<span data-ttu-id="ba903-158">String</span><span class="sxs-lookup"><span data-stu-id="ba903-158">String</span></span>|<span data-ttu-id="ba903-159">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="ba903-159">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="ba903-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba903-160">Response</span></span>
<span data-ttu-id="ba903-161">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ba903-161">If successful, this method returns a `201 Created` response code and a [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba903-162">Пример</span><span class="sxs-lookup"><span data-stu-id="ba903-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="ba903-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="ba903-163">Request</span></span>
<span data-ttu-id="ba903-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ba903-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
Content-type: application/json
Content-length: 444

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "platform": 8,
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="ba903-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba903-165">Response</span></span>
<span data-ttu-id="ba903-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ba903-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 493

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
  "id": "c6c78124-8124-c6c7-2481-c7c62481c7c6",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "platform": 8,
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```




