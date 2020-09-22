---
title: Обновление объекта deviceComplianceUserStatus
description: Обновление свойств объекта deviceComplianceUserStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 720158bf7cc86db30bc3ecae3486a9b2bc3540d8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48011545"
---
# <a name="update-devicecomplianceuserstatus"></a><span data-ttu-id="49393-103">Обновление объекта deviceComplianceUserStatus</span><span class="sxs-lookup"><span data-stu-id="49393-103">Update deviceComplianceUserStatus</span></span>

<span data-ttu-id="49393-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49393-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="49393-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49393-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="49393-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="49393-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49393-107">Обновление свойств объекта [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="49393-107">Update the properties of a [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="49393-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="49393-108">Prerequisites</span></span>
<span data-ttu-id="49393-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49393-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49393-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="49393-111">Permission type</span></span>|<span data-ttu-id="49393-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="49393-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49393-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="49393-113">Delegated (work or school account)</span></span>|<span data-ttu-id="49393-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49393-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="49393-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="49393-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49393-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49393-116">Not supported.</span></span>|
|<span data-ttu-id="49393-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="49393-117">Application</span></span>|<span data-ttu-id="49393-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49393-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="49393-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="49393-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses/{deviceComplianceUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="49393-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="49393-120">Request headers</span></span>
|<span data-ttu-id="49393-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="49393-121">Header</span></span>|<span data-ttu-id="49393-122">Значение</span><span class="sxs-lookup"><span data-stu-id="49393-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49393-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="49393-123">Authorization</span></span>|<span data-ttu-id="49393-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="49393-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49393-125">Accept</span><span class="sxs-lookup"><span data-stu-id="49393-125">Accept</span></span>|<span data-ttu-id="49393-126">application/json</span><span class="sxs-lookup"><span data-stu-id="49393-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49393-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="49393-127">Request body</span></span>
<span data-ttu-id="49393-128">В тексте запроса добавьте представление объекта [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="49393-128">In the request body, supply a JSON representation for the [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object.</span></span>

<span data-ttu-id="49393-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="49393-129">The following table shows the properties that are required when you create the [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span></span>

|<span data-ttu-id="49393-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="49393-130">Property</span></span>|<span data-ttu-id="49393-131">Тип</span><span class="sxs-lookup"><span data-stu-id="49393-131">Type</span></span>|<span data-ttu-id="49393-132">Описание</span><span class="sxs-lookup"><span data-stu-id="49393-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49393-133">id</span><span class="sxs-lookup"><span data-stu-id="49393-133">id</span></span>|<span data-ttu-id="49393-134">String</span><span class="sxs-lookup"><span data-stu-id="49393-134">String</span></span>|<span data-ttu-id="49393-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="49393-135">Key of the entity.</span></span>|
|<span data-ttu-id="49393-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="49393-136">userDisplayName</span></span>|<span data-ttu-id="49393-137">String</span><span class="sxs-lookup"><span data-stu-id="49393-137">String</span></span>|<span data-ttu-id="49393-138">Имя пользователя в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="49393-138">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="49393-139">devicesCount</span><span class="sxs-lookup"><span data-stu-id="49393-139">devicesCount</span></span>|<span data-ttu-id="49393-140">Int32</span><span class="sxs-lookup"><span data-stu-id="49393-140">Int32</span></span>|<span data-ttu-id="49393-141">Количество устройств для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="49393-141">Devices count for that user.</span></span>|
|<span data-ttu-id="49393-142">status</span><span class="sxs-lookup"><span data-stu-id="49393-142">status</span></span>|[<span data-ttu-id="49393-143">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="49393-143">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="49393-144">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="49393-144">Compliance status of the policy report.</span></span> <span data-ttu-id="49393-145">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="49393-145">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="49393-146">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="49393-146">lastReportedDateTime</span></span>|<span data-ttu-id="49393-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49393-147">DateTimeOffset</span></span>|<span data-ttu-id="49393-148">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="49393-148">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="49393-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="49393-149">userPrincipalName</span></span>|<span data-ttu-id="49393-150">String</span><span class="sxs-lookup"><span data-stu-id="49393-150">String</span></span>|<span data-ttu-id="49393-151">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="49393-151">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="49393-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="49393-152">Response</span></span>
<span data-ttu-id="49393-153">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="49393-153">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49393-154">Пример</span><span class="sxs-lookup"><span data-stu-id="49393-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="49393-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="49393-155">Request</span></span>
<span data-ttu-id="49393-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="49393-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses/{deviceComplianceUserStatusId}
Content-type: application/json
Content-length: 287

{
  "@odata.type": "#microsoft.graph.deviceComplianceUserStatus",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="49393-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="49393-157">Response</span></span>
<span data-ttu-id="49393-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="49393-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 336

{
  "@odata.type": "#microsoft.graph.deviceComplianceUserStatus",
  "id": "a0b566cd-66cd-a0b5-cd66-b5a0cd66b5a0",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```






