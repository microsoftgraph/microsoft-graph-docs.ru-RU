---
title: Обновление объекта deviceComplianceDeviceStatus
description: Обновление свойств объекта deviceComplianceDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 28643c5e308f026f6aca0b0c600387a35acf4f4f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968997"
---
# <a name="update-devicecompliancedevicestatus"></a><span data-ttu-id="866bb-103">Обновление объекта deviceComplianceDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="866bb-103">Update deviceComplianceDeviceStatus</span></span>

> <span data-ttu-id="866bb-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="866bb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="866bb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="866bb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="866bb-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="866bb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="866bb-107">Обновление свойств объекта [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="866bb-107">Update the properties of a [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="866bb-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="866bb-108">Prerequisites</span></span>
<span data-ttu-id="866bb-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="866bb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="866bb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="866bb-111">Permission type</span></span>|<span data-ttu-id="866bb-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="866bb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="866bb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="866bb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="866bb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="866bb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="866bb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="866bb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="866bb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="866bb-116">Not supported.</span></span>|
|<span data-ttu-id="866bb-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="866bb-117">Application</span></span>|<span data-ttu-id="866bb-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="866bb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="866bb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="866bb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="866bb-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="866bb-120">Request headers</span></span>
|<span data-ttu-id="866bb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="866bb-121">Header</span></span>|<span data-ttu-id="866bb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="866bb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="866bb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="866bb-123">Authorization</span></span>|<span data-ttu-id="866bb-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="866bb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="866bb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="866bb-125">Accept</span></span>|<span data-ttu-id="866bb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="866bb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="866bb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="866bb-127">Request body</span></span>
<span data-ttu-id="866bb-128">В тексте запроса добавьте представление объекта [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="866bb-128">In the request body, supply a JSON representation for the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>

<span data-ttu-id="866bb-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="866bb-129">The following table shows the properties that are required when you create the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span></span>

|<span data-ttu-id="866bb-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="866bb-130">Property</span></span>|<span data-ttu-id="866bb-131">Тип</span><span class="sxs-lookup"><span data-stu-id="866bb-131">Type</span></span>|<span data-ttu-id="866bb-132">Описание</span><span class="sxs-lookup"><span data-stu-id="866bb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="866bb-133">id</span><span class="sxs-lookup"><span data-stu-id="866bb-133">id</span></span>|<span data-ttu-id="866bb-134">Строка</span><span class="sxs-lookup"><span data-stu-id="866bb-134">String</span></span>|<span data-ttu-id="866bb-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="866bb-135">Key of the entity.</span></span>|
|<span data-ttu-id="866bb-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="866bb-136">deviceDisplayName</span></span>|<span data-ttu-id="866bb-137">String</span><span class="sxs-lookup"><span data-stu-id="866bb-137">String</span></span>|<span data-ttu-id="866bb-138">Имя устройства в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="866bb-138">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="866bb-139">userName</span><span class="sxs-lookup"><span data-stu-id="866bb-139">userName</span></span>|<span data-ttu-id="866bb-140">String</span><span class="sxs-lookup"><span data-stu-id="866bb-140">String</span></span>|<span data-ttu-id="866bb-141">Имя пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="866bb-141">The User Name that is being reported</span></span>|
|<span data-ttu-id="866bb-142">deviceModel</span><span class="sxs-lookup"><span data-stu-id="866bb-142">deviceModel</span></span>|<span data-ttu-id="866bb-143">String</span><span class="sxs-lookup"><span data-stu-id="866bb-143">String</span></span>|<span data-ttu-id="866bb-144">Модель устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="866bb-144">The device model that is being reported</span></span>|
|<span data-ttu-id="866bb-145">platform</span><span class="sxs-lookup"><span data-stu-id="866bb-145">platform</span></span>|<span data-ttu-id="866bb-146">Int32</span><span class="sxs-lookup"><span data-stu-id="866bb-146">Int32</span></span>|<span data-ttu-id="866bb-147">Платформа устройства, предоставленные</span><span class="sxs-lookup"><span data-stu-id="866bb-147">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="866bb-148">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="866bb-148">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="866bb-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="866bb-149">DateTimeOffset</span></span>|<span data-ttu-id="866bb-150">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="866bb-150">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="866bb-151">status</span><span class="sxs-lookup"><span data-stu-id="866bb-151">status</span></span>|[<span data-ttu-id="866bb-152">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="866bb-152">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="866bb-153">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="866bb-153">Compliance status of the policy report.</span></span> <span data-ttu-id="866bb-154">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="866bb-154">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="866bb-155">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="866bb-155">lastReportedDateTime</span></span>|<span data-ttu-id="866bb-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="866bb-156">DateTimeOffset</span></span>|<span data-ttu-id="866bb-157">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="866bb-157">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="866bb-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="866bb-158">userPrincipalName</span></span>|<span data-ttu-id="866bb-159">String</span><span class="sxs-lookup"><span data-stu-id="866bb-159">String</span></span>|<span data-ttu-id="866bb-160">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="866bb-160">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="866bb-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="866bb-161">Response</span></span>
<span data-ttu-id="866bb-162">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="866bb-162">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="866bb-163">Пример</span><span class="sxs-lookup"><span data-stu-id="866bb-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="866bb-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="866bb-164">Request</span></span>
<span data-ttu-id="866bb-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="866bb-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
Content-type: application/json
Content-length: 377

{
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

### <a name="response"></a><span data-ttu-id="866bb-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="866bb-166">Response</span></span>
<span data-ttu-id="866bb-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="866bb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





