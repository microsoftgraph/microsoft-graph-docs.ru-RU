---
title: Создание объекта deviceComplianceDeviceStatus
description: Создание объекта deviceComplianceDeviceStatus.
ms.openlocfilehash: c3c43b6c6ee49f0c4b962cd35d0cead9d4900bf6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026162"
---
# <a name="create-devicecompliancedevicestatus"></a><span data-ttu-id="32396-103">Создание объекта deviceComplianceDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="32396-103">Create deviceComplianceDeviceStatus</span></span>

> <span data-ttu-id="32396-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="32396-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="32396-105">Создание объекта [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="32396-105">Create a new [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="32396-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="32396-106">Prerequisites</span></span>
<span data-ttu-id="32396-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32396-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32396-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="32396-109">Permission type</span></span>|<span data-ttu-id="32396-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="32396-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32396-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="32396-111">Delegated (work or school account)</span></span>|<span data-ttu-id="32396-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32396-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="32396-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="32396-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32396-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32396-114">Not supported.</span></span>|
|<span data-ttu-id="32396-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="32396-115">Application</span></span>|<span data-ttu-id="32396-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32396-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="32396-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="32396-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="32396-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="32396-118">Request headers</span></span>
|<span data-ttu-id="32396-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="32396-119">Header</span></span>|<span data-ttu-id="32396-120">Значение</span><span class="sxs-lookup"><span data-stu-id="32396-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="32396-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="32396-121">Authorization</span></span>|<span data-ttu-id="32396-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="32396-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="32396-123">Accept</span><span class="sxs-lookup"><span data-stu-id="32396-123">Accept</span></span>|<span data-ttu-id="32396-124">application/json</span><span class="sxs-lookup"><span data-stu-id="32396-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="32396-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="32396-125">Request body</span></span>
<span data-ttu-id="32396-126">В тексте запроса добавьте представление объекта deviceComplianceDeviceStatus в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="32396-126">In the request body, supply a JSON representation for the deviceComplianceDeviceStatus object.</span></span>

<span data-ttu-id="32396-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceComplianceDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="32396-127">The following table shows the properties that are required when you create the deviceComplianceDeviceStatus.</span></span>

|<span data-ttu-id="32396-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="32396-128">Property</span></span>|<span data-ttu-id="32396-129">Тип</span><span class="sxs-lookup"><span data-stu-id="32396-129">Type</span></span>|<span data-ttu-id="32396-130">Описание</span><span class="sxs-lookup"><span data-stu-id="32396-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32396-131">id</span><span class="sxs-lookup"><span data-stu-id="32396-131">id</span></span>|<span data-ttu-id="32396-132">String</span><span class="sxs-lookup"><span data-stu-id="32396-132">String</span></span>|<span data-ttu-id="32396-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="32396-133">Key of the entity.</span></span>|
|<span data-ttu-id="32396-134">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="32396-134">deviceDisplayName</span></span>|<span data-ttu-id="32396-135">String</span><span class="sxs-lookup"><span data-stu-id="32396-135">String</span></span>|<span data-ttu-id="32396-136">Имя устройства в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="32396-136">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="32396-137">userName</span><span class="sxs-lookup"><span data-stu-id="32396-137">userName</span></span>|<span data-ttu-id="32396-138">String</span><span class="sxs-lookup"><span data-stu-id="32396-138">String</span></span>|<span data-ttu-id="32396-139">Имя пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="32396-139">The User Name that is being reported</span></span>|
|<span data-ttu-id="32396-140">deviceModel</span><span class="sxs-lookup"><span data-stu-id="32396-140">deviceModel</span></span>|<span data-ttu-id="32396-141">String</span><span class="sxs-lookup"><span data-stu-id="32396-141">String</span></span>|<span data-ttu-id="32396-142">Модель устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="32396-142">The device model that is being reported</span></span>|
|<span data-ttu-id="32396-143">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="32396-143">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="32396-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32396-144">DateTimeOffset</span></span>|<span data-ttu-id="32396-145">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="32396-145">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="32396-146">status</span><span class="sxs-lookup"><span data-stu-id="32396-146">status</span></span>|[<span data-ttu-id="32396-147">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="32396-147">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="32396-148">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="32396-148">Compliance status of the policy report.</span></span> <span data-ttu-id="32396-149">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="32396-149">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="32396-150">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="32396-150">lastReportedDateTime</span></span>|<span data-ttu-id="32396-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32396-151">DateTimeOffset</span></span>|<span data-ttu-id="32396-152">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="32396-152">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="32396-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="32396-153">userPrincipalName</span></span>|<span data-ttu-id="32396-154">String</span><span class="sxs-lookup"><span data-stu-id="32396-154">String</span></span>|<span data-ttu-id="32396-155">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="32396-155">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="32396-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="32396-156">Response</span></span>
<span data-ttu-id="32396-157">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="32396-157">If successful, this method returns a `201 Created` response code and a [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32396-158">Пример</span><span class="sxs-lookup"><span data-stu-id="32396-158">Example</span></span>
### <a name="request"></a><span data-ttu-id="32396-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="32396-159">Request</span></span>
<span data-ttu-id="32396-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="32396-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="32396-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="32396-161">Response</span></span>
<span data-ttu-id="32396-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="32396-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



