---
title: Создание объекта deviceComplianceDeviceStatus
description: Создание объекта deviceComplianceDeviceStatus.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0b9e7a7049c656c42f2ad843bedafcc6f9975619
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417576"
---
# <a name="create-devicecompliancedevicestatus"></a><span data-ttu-id="12997-103">Создание объекта deviceComplianceDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="12997-103">Create deviceComplianceDeviceStatus</span></span>

> <span data-ttu-id="12997-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="12997-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="12997-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12997-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="12997-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="12997-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12997-107">Создание объекта [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="12997-107">Create a new [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="12997-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="12997-108">Prerequisites</span></span>
<span data-ttu-id="12997-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="12997-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="12997-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="12997-111">Permission type</span></span>|<span data-ttu-id="12997-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="12997-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12997-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="12997-113">Delegated (work or school account)</span></span>|<span data-ttu-id="12997-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12997-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="12997-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="12997-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12997-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12997-116">Not supported.</span></span>|
|<span data-ttu-id="12997-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="12997-117">Application</span></span>|<span data-ttu-id="12997-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12997-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="12997-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="12997-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="12997-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="12997-120">Request headers</span></span>
|<span data-ttu-id="12997-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="12997-121">Header</span></span>|<span data-ttu-id="12997-122">Значение</span><span class="sxs-lookup"><span data-stu-id="12997-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12997-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="12997-123">Authorization</span></span>|<span data-ttu-id="12997-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="12997-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12997-125">Accept</span><span class="sxs-lookup"><span data-stu-id="12997-125">Accept</span></span>|<span data-ttu-id="12997-126">application/json</span><span class="sxs-lookup"><span data-stu-id="12997-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12997-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="12997-127">Request body</span></span>
<span data-ttu-id="12997-128">В тексте запроса добавьте представление объекта deviceComplianceDeviceStatus в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="12997-128">In the request body, supply a JSON representation for the deviceComplianceDeviceStatus object.</span></span>

<span data-ttu-id="12997-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceComplianceDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="12997-129">The following table shows the properties that are required when you create the deviceComplianceDeviceStatus.</span></span>

|<span data-ttu-id="12997-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="12997-130">Property</span></span>|<span data-ttu-id="12997-131">Тип</span><span class="sxs-lookup"><span data-stu-id="12997-131">Type</span></span>|<span data-ttu-id="12997-132">Описание</span><span class="sxs-lookup"><span data-stu-id="12997-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12997-133">id</span><span class="sxs-lookup"><span data-stu-id="12997-133">id</span></span>|<span data-ttu-id="12997-134">String</span><span class="sxs-lookup"><span data-stu-id="12997-134">String</span></span>|<span data-ttu-id="12997-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="12997-135">Key of the entity.</span></span>|
|<span data-ttu-id="12997-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="12997-136">deviceDisplayName</span></span>|<span data-ttu-id="12997-137">String</span><span class="sxs-lookup"><span data-stu-id="12997-137">String</span></span>|<span data-ttu-id="12997-138">Имя устройства в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="12997-138">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="12997-139">userName</span><span class="sxs-lookup"><span data-stu-id="12997-139">userName</span></span>|<span data-ttu-id="12997-140">String</span><span class="sxs-lookup"><span data-stu-id="12997-140">String</span></span>|<span data-ttu-id="12997-141">Имя пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="12997-141">The User Name that is being reported</span></span>|
|<span data-ttu-id="12997-142">deviceModel</span><span class="sxs-lookup"><span data-stu-id="12997-142">deviceModel</span></span>|<span data-ttu-id="12997-143">String</span><span class="sxs-lookup"><span data-stu-id="12997-143">String</span></span>|<span data-ttu-id="12997-144">Модель устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="12997-144">The device model that is being reported</span></span>|
|<span data-ttu-id="12997-145">platform</span><span class="sxs-lookup"><span data-stu-id="12997-145">platform</span></span>|<span data-ttu-id="12997-146">Int32</span><span class="sxs-lookup"><span data-stu-id="12997-146">Int32</span></span>|<span data-ttu-id="12997-147">Платформа устройства, предоставленные</span><span class="sxs-lookup"><span data-stu-id="12997-147">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="12997-148">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="12997-148">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="12997-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12997-149">DateTimeOffset</span></span>|<span data-ttu-id="12997-150">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="12997-150">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="12997-151">status</span><span class="sxs-lookup"><span data-stu-id="12997-151">status</span></span>|[<span data-ttu-id="12997-152">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="12997-152">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="12997-153">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="12997-153">Compliance status of the policy report.</span></span> <span data-ttu-id="12997-154">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="12997-154">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="12997-155">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="12997-155">lastReportedDateTime</span></span>|<span data-ttu-id="12997-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12997-156">DateTimeOffset</span></span>|<span data-ttu-id="12997-157">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="12997-157">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="12997-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="12997-158">userPrincipalName</span></span>|<span data-ttu-id="12997-159">String</span><span class="sxs-lookup"><span data-stu-id="12997-159">String</span></span>|<span data-ttu-id="12997-160">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="12997-160">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="12997-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="12997-161">Response</span></span>
<span data-ttu-id="12997-162">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="12997-162">If successful, this method returns a `201 Created` response code and a [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12997-163">Пример</span><span class="sxs-lookup"><span data-stu-id="12997-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="12997-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="12997-164">Request</span></span>
<span data-ttu-id="12997-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="12997-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="12997-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="12997-166">Response</span></span>
<span data-ttu-id="12997-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="12997-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




