---
title: Обновление объекта deviceConfigurationUserStatus
description: Обновление свойств объекта deviceConfigurationUserStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5f94b349f7d48069ed6b9b61a420f2e431ff819f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078887"
---
# <a name="update-deviceconfigurationuserstatus"></a><span data-ttu-id="80368-103">Обновление объекта deviceConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="80368-103">Update deviceConfigurationUserStatus</span></span>

<span data-ttu-id="80368-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80368-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="80368-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="80368-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="80368-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="80368-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80368-107">Обновление свойств объекта [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="80368-107">Update the properties of a [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="80368-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="80368-108">Prerequisites</span></span>
<span data-ttu-id="80368-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80368-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80368-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="80368-111">Permission type</span></span>|<span data-ttu-id="80368-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="80368-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="80368-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="80368-113">Delegated (work or school account)</span></span>|<span data-ttu-id="80368-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80368-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="80368-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="80368-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80368-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="80368-116">Not supported.</span></span>|
|<span data-ttu-id="80368-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="80368-117">Application</span></span>|<span data-ttu-id="80368-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80368-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="80368-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="80368-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="80368-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="80368-120">Request headers</span></span>
|<span data-ttu-id="80368-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="80368-121">Header</span></span>|<span data-ttu-id="80368-122">Значение</span><span class="sxs-lookup"><span data-stu-id="80368-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="80368-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="80368-123">Authorization</span></span>|<span data-ttu-id="80368-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="80368-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="80368-125">Accept</span><span class="sxs-lookup"><span data-stu-id="80368-125">Accept</span></span>|<span data-ttu-id="80368-126">application/json</span><span class="sxs-lookup"><span data-stu-id="80368-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="80368-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="80368-127">Request body</span></span>
<span data-ttu-id="80368-128">В тексте запроса добавьте представление объекта [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="80368-128">In the request body, supply a JSON representation for the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object.</span></span>

<span data-ttu-id="80368-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="80368-129">The following table shows the properties that are required when you create the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span></span>

|<span data-ttu-id="80368-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="80368-130">Property</span></span>|<span data-ttu-id="80368-131">Тип</span><span class="sxs-lookup"><span data-stu-id="80368-131">Type</span></span>|<span data-ttu-id="80368-132">Описание</span><span class="sxs-lookup"><span data-stu-id="80368-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80368-133">id</span><span class="sxs-lookup"><span data-stu-id="80368-133">id</span></span>|<span data-ttu-id="80368-134">String</span><span class="sxs-lookup"><span data-stu-id="80368-134">String</span></span>|<span data-ttu-id="80368-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="80368-135">Key of the entity.</span></span>|
|<span data-ttu-id="80368-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="80368-136">userDisplayName</span></span>|<span data-ttu-id="80368-137">String</span><span class="sxs-lookup"><span data-stu-id="80368-137">String</span></span>|<span data-ttu-id="80368-138">Имя пользователя в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="80368-138">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="80368-139">devicesCount</span><span class="sxs-lookup"><span data-stu-id="80368-139">devicesCount</span></span>|<span data-ttu-id="80368-140">Int32</span><span class="sxs-lookup"><span data-stu-id="80368-140">Int32</span></span>|<span data-ttu-id="80368-141">Количество устройств для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="80368-141">Devices count for that user.</span></span>|
|<span data-ttu-id="80368-142">status</span><span class="sxs-lookup"><span data-stu-id="80368-142">status</span></span>|[<span data-ttu-id="80368-143">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="80368-143">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="80368-144">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="80368-144">Compliance status of the policy report.</span></span> <span data-ttu-id="80368-145">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="80368-145">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="80368-146">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="80368-146">lastReportedDateTime</span></span>|<span data-ttu-id="80368-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80368-147">DateTimeOffset</span></span>|<span data-ttu-id="80368-148">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="80368-148">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="80368-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="80368-149">userPrincipalName</span></span>|<span data-ttu-id="80368-150">String</span><span class="sxs-lookup"><span data-stu-id="80368-150">String</span></span>|<span data-ttu-id="80368-151">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="80368-151">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="80368-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="80368-152">Response</span></span>
<span data-ttu-id="80368-153">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="80368-153">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80368-154">Пример</span><span class="sxs-lookup"><span data-stu-id="80368-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="80368-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="80368-155">Request</span></span>
<span data-ttu-id="80368-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="80368-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="80368-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="80368-157">Response</span></span>
<span data-ttu-id="80368-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="80368-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






