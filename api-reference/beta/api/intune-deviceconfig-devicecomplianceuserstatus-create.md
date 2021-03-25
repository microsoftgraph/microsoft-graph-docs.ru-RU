---
title: Создание объекта deviceComplianceUserStatus
description: Создание объекта deviceComplianceUserStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 72ae447feabf20db707781aca54ef323679d89f4
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51151517"
---
# <a name="create-devicecomplianceuserstatus"></a><span data-ttu-id="2e4ff-103">Создание объекта deviceComplianceUserStatus</span><span class="sxs-lookup"><span data-stu-id="2e4ff-103">Create deviceComplianceUserStatus</span></span>

<span data-ttu-id="2e4ff-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e4ff-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2e4ff-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e4ff-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2e4ff-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2e4ff-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e4ff-107">Создание объекта [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="2e4ff-107">Create a new [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2e4ff-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2e4ff-108">Prerequisites</span></span>
<span data-ttu-id="2e4ff-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e4ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e4ff-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2e4ff-111">Permission type</span></span>|<span data-ttu-id="2e4ff-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2e4ff-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2e4ff-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2e4ff-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2e4ff-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e4ff-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2e4ff-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2e4ff-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2e4ff-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e4ff-116">Not supported.</span></span>|
|<span data-ttu-id="2e4ff-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="2e4ff-117">Application</span></span>|<span data-ttu-id="2e4ff-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e4ff-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2e4ff-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2e4ff-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="2e4ff-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2e4ff-120">Request headers</span></span>
|<span data-ttu-id="2e4ff-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2e4ff-121">Header</span></span>|<span data-ttu-id="2e4ff-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2e4ff-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2e4ff-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e4ff-123">Authorization</span></span>|<span data-ttu-id="2e4ff-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2e4ff-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2e4ff-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2e4ff-125">Accept</span></span>|<span data-ttu-id="2e4ff-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2e4ff-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e4ff-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2e4ff-127">Request body</span></span>
<span data-ttu-id="2e4ff-128">В тексте запроса добавьте представление объекта deviceComplianceUserStatus в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2e4ff-128">In the request body, supply a JSON representation for the deviceComplianceUserStatus object.</span></span>

<span data-ttu-id="2e4ff-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceComplianceUserStatus.</span><span class="sxs-lookup"><span data-stu-id="2e4ff-129">The following table shows the properties that are required when you create the deviceComplianceUserStatus.</span></span>

|<span data-ttu-id="2e4ff-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2e4ff-130">Property</span></span>|<span data-ttu-id="2e4ff-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2e4ff-131">Type</span></span>|<span data-ttu-id="2e4ff-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2e4ff-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e4ff-133">id</span><span class="sxs-lookup"><span data-stu-id="2e4ff-133">id</span></span>|<span data-ttu-id="2e4ff-134">Строка</span><span class="sxs-lookup"><span data-stu-id="2e4ff-134">String</span></span>|<span data-ttu-id="2e4ff-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2e4ff-135">Key of the entity.</span></span>|
|<span data-ttu-id="2e4ff-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="2e4ff-136">userDisplayName</span></span>|<span data-ttu-id="2e4ff-137">String</span><span class="sxs-lookup"><span data-stu-id="2e4ff-137">String</span></span>|<span data-ttu-id="2e4ff-138">Имя пользователя в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="2e4ff-138">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="2e4ff-139">devicesCount</span><span class="sxs-lookup"><span data-stu-id="2e4ff-139">devicesCount</span></span>|<span data-ttu-id="2e4ff-140">Int32</span><span class="sxs-lookup"><span data-stu-id="2e4ff-140">Int32</span></span>|<span data-ttu-id="2e4ff-141">Количество устройств для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="2e4ff-141">Devices count for that user.</span></span>|
|<span data-ttu-id="2e4ff-142">status</span><span class="sxs-lookup"><span data-stu-id="2e4ff-142">status</span></span>|[<span data-ttu-id="2e4ff-143">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="2e4ff-143">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="2e4ff-144">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="2e4ff-144">Compliance status of the policy report.</span></span> <span data-ttu-id="2e4ff-145">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="2e4ff-145">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="2e4ff-146">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="2e4ff-146">lastReportedDateTime</span></span>|<span data-ttu-id="2e4ff-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e4ff-147">DateTimeOffset</span></span>|<span data-ttu-id="2e4ff-148">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="2e4ff-148">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="2e4ff-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2e4ff-149">userPrincipalName</span></span>|<span data-ttu-id="2e4ff-150">String</span><span class="sxs-lookup"><span data-stu-id="2e4ff-150">String</span></span>|<span data-ttu-id="2e4ff-151">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="2e4ff-151">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="2e4ff-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e4ff-152">Response</span></span>
<span data-ttu-id="2e4ff-153">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2e4ff-153">If successful, this method returns a `201 Created` response code and a [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e4ff-154">Пример</span><span class="sxs-lookup"><span data-stu-id="2e4ff-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="2e4ff-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="2e4ff-155">Request</span></span>
<span data-ttu-id="2e4ff-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2e4ff-156">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
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

### <a name="response"></a><span data-ttu-id="2e4ff-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e4ff-157">Response</span></span>
<span data-ttu-id="2e4ff-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2e4ff-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




