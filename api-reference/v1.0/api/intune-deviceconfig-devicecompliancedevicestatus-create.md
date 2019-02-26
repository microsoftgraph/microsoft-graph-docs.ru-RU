---
title: Создание объекта deviceComplianceDeviceStatus
description: Создание объекта deviceComplianceDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e34a792989e60e9b2655ff2efa7dd3c2b15da0cd
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253192"
---
# <a name="create-devicecompliancedevicestatus"></a><span data-ttu-id="5babb-103">Создание объекта deviceComplianceDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="5babb-103">Create deviceComplianceDeviceStatus</span></span>

> <span data-ttu-id="5babb-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5babb-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5babb-105">Создание объекта [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="5babb-105">Create a new [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5babb-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5babb-106">Prerequisites</span></span>
<span data-ttu-id="5babb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="5babb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5babb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5babb-109">Permission type</span></span>|<span data-ttu-id="5babb-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5babb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5babb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5babb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5babb-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5babb-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5babb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5babb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5babb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5babb-114">Not supported.</span></span>|
|<span data-ttu-id="5babb-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5babb-115">Application</span></span>|<span data-ttu-id="5babb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5babb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5babb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5babb-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="5babb-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5babb-118">Request headers</span></span>
|<span data-ttu-id="5babb-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5babb-119">Header</span></span>|<span data-ttu-id="5babb-120">Значение</span><span class="sxs-lookup"><span data-stu-id="5babb-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5babb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5babb-121">Authorization</span></span>|<span data-ttu-id="5babb-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="5babb-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5babb-123">Accept</span><span class="sxs-lookup"><span data-stu-id="5babb-123">Accept</span></span>|<span data-ttu-id="5babb-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5babb-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5babb-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5babb-125">Request body</span></span>
<span data-ttu-id="5babb-126">В тексте запроса добавьте представление объекта deviceComplianceDeviceStatus в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5babb-126">In the request body, supply a JSON representation for the deviceComplianceDeviceStatus object.</span></span>

<span data-ttu-id="5babb-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceComplianceDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="5babb-127">The following table shows the properties that are required when you create the deviceComplianceDeviceStatus.</span></span>

|<span data-ttu-id="5babb-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="5babb-128">Property</span></span>|<span data-ttu-id="5babb-129">Тип</span><span class="sxs-lookup"><span data-stu-id="5babb-129">Type</span></span>|<span data-ttu-id="5babb-130">Описание</span><span class="sxs-lookup"><span data-stu-id="5babb-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5babb-131">id</span><span class="sxs-lookup"><span data-stu-id="5babb-131">id</span></span>|<span data-ttu-id="5babb-132">Строка</span><span class="sxs-lookup"><span data-stu-id="5babb-132">String</span></span>|<span data-ttu-id="5babb-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5babb-133">Key of the entity.</span></span>|
|<span data-ttu-id="5babb-134">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="5babb-134">deviceDisplayName</span></span>|<span data-ttu-id="5babb-135">String</span><span class="sxs-lookup"><span data-stu-id="5babb-135">String</span></span>|<span data-ttu-id="5babb-136">Имя устройства в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="5babb-136">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="5babb-137">userName</span><span class="sxs-lookup"><span data-stu-id="5babb-137">userName</span></span>|<span data-ttu-id="5babb-138">String</span><span class="sxs-lookup"><span data-stu-id="5babb-138">String</span></span>|<span data-ttu-id="5babb-139">Имя пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="5babb-139">The User Name that is being reported</span></span>|
|<span data-ttu-id="5babb-140">deviceModel</span><span class="sxs-lookup"><span data-stu-id="5babb-140">deviceModel</span></span>|<span data-ttu-id="5babb-141">String</span><span class="sxs-lookup"><span data-stu-id="5babb-141">String</span></span>|<span data-ttu-id="5babb-142">Модель устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="5babb-142">The device model that is being reported</span></span>|
|<span data-ttu-id="5babb-143">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="5babb-143">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="5babb-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5babb-144">DateTimeOffset</span></span>|<span data-ttu-id="5babb-145">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="5babb-145">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="5babb-146">status</span><span class="sxs-lookup"><span data-stu-id="5babb-146">status</span></span>|[<span data-ttu-id="5babb-147">Комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="5babb-147">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="5babb-148">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="5babb-148">Compliance status of the policy report.</span></span> <span data-ttu-id="5babb-149">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="5babb-149">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="5babb-150">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="5babb-150">lastReportedDateTime</span></span>|<span data-ttu-id="5babb-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5babb-151">DateTimeOffset</span></span>|<span data-ttu-id="5babb-152">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="5babb-152">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="5babb-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5babb-153">userPrincipalName</span></span>|<span data-ttu-id="5babb-154">Строка</span><span class="sxs-lookup"><span data-stu-id="5babb-154">String</span></span>|<span data-ttu-id="5babb-155">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="5babb-155">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="5babb-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="5babb-156">Response</span></span>
<span data-ttu-id="5babb-157">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5babb-157">If successful, this method returns a `201 Created` response code and a [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5babb-158">Пример</span><span class="sxs-lookup"><span data-stu-id="5babb-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="5babb-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="5babb-159">Request</span></span>
<span data-ttu-id="5babb-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5babb-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5babb-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="5babb-161">Response</span></span>
<span data-ttu-id="5babb-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5babb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



