---
title: Обновление объекта deviceConfigurationUserStatus
description: Обновление свойств объекта deviceConfigurationUserStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2c793551f22c33f45d9967ae7effb710afa02e39
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51128056"
---
# <a name="update-deviceconfigurationuserstatus"></a><span data-ttu-id="f1ca4-103">Обновление объекта deviceConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="f1ca4-103">Update deviceConfigurationUserStatus</span></span>

<span data-ttu-id="f1ca4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1ca4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f1ca4-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1ca4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1ca4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f1ca4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1ca4-107">Обновление свойств объекта [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="f1ca4-107">Update the properties of a [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f1ca4-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f1ca4-108">Prerequisites</span></span>
<span data-ttu-id="f1ca4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1ca4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1ca4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f1ca4-111">Permission type</span></span>|<span data-ttu-id="f1ca4-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f1ca4-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1ca4-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f1ca4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f1ca4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1ca4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f1ca4-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f1ca4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1ca4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1ca4-116">Not supported.</span></span>|
|<span data-ttu-id="f1ca4-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f1ca4-117">Application</span></span>|<span data-ttu-id="f1ca4-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1ca4-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1ca4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f1ca4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/userStatuses/{deviceConfigurationUserStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/userStatuses/{deviceConfigurationUserStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/userStatuses/{deviceConfigurationUserStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/userStatuses/{deviceConfigurationUserStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/userStatuses/{deviceConfigurationUserStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/userStatuses/{deviceConfigurationUserStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/userStatuses/{deviceConfigurationUserStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/userStatuses/{deviceConfigurationUserStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/userStatuses/{deviceConfigurationUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="f1ca4-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f1ca4-120">Request headers</span></span>
|<span data-ttu-id="f1ca4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f1ca4-121">Header</span></span>|<span data-ttu-id="f1ca4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f1ca4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1ca4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1ca4-123">Authorization</span></span>|<span data-ttu-id="f1ca4-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f1ca4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1ca4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f1ca4-125">Accept</span></span>|<span data-ttu-id="f1ca4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f1ca4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1ca4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f1ca4-127">Request body</span></span>
<span data-ttu-id="f1ca4-128">В тексте запроса добавьте представление объекта [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f1ca4-128">In the request body, supply a JSON representation for the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object.</span></span>

<span data-ttu-id="f1ca4-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="f1ca4-129">The following table shows the properties that are required when you create the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span></span>

|<span data-ttu-id="f1ca4-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f1ca4-130">Property</span></span>|<span data-ttu-id="f1ca4-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f1ca4-131">Type</span></span>|<span data-ttu-id="f1ca4-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f1ca4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1ca4-133">id</span><span class="sxs-lookup"><span data-stu-id="f1ca4-133">id</span></span>|<span data-ttu-id="f1ca4-134">Строка</span><span class="sxs-lookup"><span data-stu-id="f1ca4-134">String</span></span>|<span data-ttu-id="f1ca4-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f1ca4-135">Key of the entity.</span></span>|
|<span data-ttu-id="f1ca4-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="f1ca4-136">userDisplayName</span></span>|<span data-ttu-id="f1ca4-137">String</span><span class="sxs-lookup"><span data-stu-id="f1ca4-137">String</span></span>|<span data-ttu-id="f1ca4-138">Имя пользователя в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="f1ca4-138">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="f1ca4-139">devicesCount</span><span class="sxs-lookup"><span data-stu-id="f1ca4-139">devicesCount</span></span>|<span data-ttu-id="f1ca4-140">Int32</span><span class="sxs-lookup"><span data-stu-id="f1ca4-140">Int32</span></span>|<span data-ttu-id="f1ca4-141">Количество устройств для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="f1ca4-141">Devices count for that user.</span></span>|
|<span data-ttu-id="f1ca4-142">status</span><span class="sxs-lookup"><span data-stu-id="f1ca4-142">status</span></span>|[<span data-ttu-id="f1ca4-143">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="f1ca4-143">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="f1ca4-144">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="f1ca4-144">Compliance status of the policy report.</span></span> <span data-ttu-id="f1ca4-145">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="f1ca4-145">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="f1ca4-146">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="f1ca4-146">lastReportedDateTime</span></span>|<span data-ttu-id="f1ca4-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1ca4-147">DateTimeOffset</span></span>|<span data-ttu-id="f1ca4-148">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="f1ca4-148">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="f1ca4-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f1ca4-149">userPrincipalName</span></span>|<span data-ttu-id="f1ca4-150">String</span><span class="sxs-lookup"><span data-stu-id="f1ca4-150">String</span></span>|<span data-ttu-id="f1ca4-151">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="f1ca4-151">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="f1ca4-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1ca4-152">Response</span></span>
<span data-ttu-id="f1ca4-153">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f1ca4-153">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1ca4-154">Пример</span><span class="sxs-lookup"><span data-stu-id="f1ca4-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1ca4-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="f1ca4-155">Request</span></span>
<span data-ttu-id="f1ca4-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f1ca4-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
Content-type: application/json
Content-length: 290

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStatus",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="f1ca4-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1ca4-157">Response</span></span>
<span data-ttu-id="f1ca4-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f1ca4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 339

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStatus",
  "id": "7e323db2-3db2-7e32-b23d-327eb23d327e",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```




