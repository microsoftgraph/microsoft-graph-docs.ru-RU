---
title: Обновление объекта deviceConfigurationUserStatus
description: Обновление свойств объекта deviceConfigurationUserStatus.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 181ce76d933bab1c6737db935e29429b22acb6ec
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37168105"
---
# <a name="update-deviceconfigurationuserstatus"></a><span data-ttu-id="46ef7-103">Обновление объекта deviceConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="46ef7-103">Update deviceConfigurationUserStatus</span></span>

> <span data-ttu-id="46ef7-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46ef7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="46ef7-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="46ef7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46ef7-106">Обновление свойств объекта [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="46ef7-106">Update the properties of a [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="46ef7-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="46ef7-107">Prerequisites</span></span>
<span data-ttu-id="46ef7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46ef7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46ef7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="46ef7-110">Permission type</span></span>|<span data-ttu-id="46ef7-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="46ef7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46ef7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="46ef7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="46ef7-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46ef7-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="46ef7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="46ef7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46ef7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46ef7-115">Not supported.</span></span>|
|<span data-ttu-id="46ef7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="46ef7-116">Application</span></span>|<span data-ttu-id="46ef7-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46ef7-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="46ef7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="46ef7-118">HTTP Request</span></span>
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
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/userStatuses/{deviceConfigurationUserStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/userStatuses/{deviceConfigurationUserStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/userStatuses/{deviceConfigurationUserStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/userStatuses/{deviceConfigurationUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="46ef7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="46ef7-119">Request headers</span></span>
|<span data-ttu-id="46ef7-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="46ef7-120">Header</span></span>|<span data-ttu-id="46ef7-121">Значение</span><span class="sxs-lookup"><span data-stu-id="46ef7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46ef7-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="46ef7-122">Authorization</span></span>|<span data-ttu-id="46ef7-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="46ef7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46ef7-124">Accept</span><span class="sxs-lookup"><span data-stu-id="46ef7-124">Accept</span></span>|<span data-ttu-id="46ef7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="46ef7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46ef7-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="46ef7-126">Request body</span></span>
<span data-ttu-id="46ef7-127">В тексте запроса добавьте представление объекта [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="46ef7-127">In the request body, supply a JSON representation for the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object.</span></span>

<span data-ttu-id="46ef7-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="46ef7-128">The following table shows the properties that are required when you create the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span></span>

|<span data-ttu-id="46ef7-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="46ef7-129">Property</span></span>|<span data-ttu-id="46ef7-130">Тип</span><span class="sxs-lookup"><span data-stu-id="46ef7-130">Type</span></span>|<span data-ttu-id="46ef7-131">Описание</span><span class="sxs-lookup"><span data-stu-id="46ef7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46ef7-132">id</span><span class="sxs-lookup"><span data-stu-id="46ef7-132">id</span></span>|<span data-ttu-id="46ef7-133">Строка</span><span class="sxs-lookup"><span data-stu-id="46ef7-133">String</span></span>|<span data-ttu-id="46ef7-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="46ef7-134">Key of the entity.</span></span>|
|<span data-ttu-id="46ef7-135">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="46ef7-135">userDisplayName</span></span>|<span data-ttu-id="46ef7-136">String</span><span class="sxs-lookup"><span data-stu-id="46ef7-136">String</span></span>|<span data-ttu-id="46ef7-137">Имя пользователя в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="46ef7-137">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="46ef7-138">devicesCount</span><span class="sxs-lookup"><span data-stu-id="46ef7-138">devicesCount</span></span>|<span data-ttu-id="46ef7-139">Int32</span><span class="sxs-lookup"><span data-stu-id="46ef7-139">Int32</span></span>|<span data-ttu-id="46ef7-140">Количество устройств для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="46ef7-140">Devices count for that user.</span></span>|
|<span data-ttu-id="46ef7-141">status</span><span class="sxs-lookup"><span data-stu-id="46ef7-141">status</span></span>|[<span data-ttu-id="46ef7-142">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="46ef7-142">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="46ef7-143">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="46ef7-143">Compliance status of the policy report.</span></span> <span data-ttu-id="46ef7-144">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="46ef7-144">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="46ef7-145">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="46ef7-145">lastReportedDateTime</span></span>|<span data-ttu-id="46ef7-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="46ef7-146">DateTimeOffset</span></span>|<span data-ttu-id="46ef7-147">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="46ef7-147">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="46ef7-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="46ef7-148">userPrincipalName</span></span>|<span data-ttu-id="46ef7-149">String</span><span class="sxs-lookup"><span data-stu-id="46ef7-149">String</span></span>|<span data-ttu-id="46ef7-150">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="46ef7-150">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="46ef7-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="46ef7-151">Response</span></span>
<span data-ttu-id="46ef7-152">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="46ef7-152">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46ef7-153">Пример</span><span class="sxs-lookup"><span data-stu-id="46ef7-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="46ef7-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="46ef7-154">Request</span></span>
<span data-ttu-id="46ef7-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="46ef7-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="46ef7-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="46ef7-156">Response</span></span>
<span data-ttu-id="46ef7-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="46ef7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




