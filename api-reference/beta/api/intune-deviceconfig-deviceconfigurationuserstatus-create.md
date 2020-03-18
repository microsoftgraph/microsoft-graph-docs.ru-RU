---
title: Создание объекта deviceConfigurationUserStatus
description: Создание объекта deviceConfigurationUserStatus.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 67640f6490b39d7dd6aa9def11194b44a6b3fed9
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42753420"
---
# <a name="create-deviceconfigurationuserstatus"></a><span data-ttu-id="ec271-103">Создание объекта deviceConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="ec271-103">Create deviceConfigurationUserStatus</span></span>

> <span data-ttu-id="ec271-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec271-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ec271-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ec271-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec271-106">Создание объекта [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="ec271-106">Create a new [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ec271-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ec271-107">Prerequisites</span></span>
<span data-ttu-id="ec271-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec271-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec271-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ec271-110">Permission type</span></span>|<span data-ttu-id="ec271-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ec271-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ec271-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ec271-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ec271-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec271-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ec271-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ec271-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ec271-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec271-115">Not supported.</span></span>|
|<span data-ttu-id="ec271-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="ec271-116">Application</span></span>|<span data-ttu-id="ec271-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec271-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ec271-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ec271-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/userStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/userStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/userStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/userStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/userStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/userStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/userStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/userStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="ec271-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ec271-119">Request headers</span></span>
|<span data-ttu-id="ec271-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ec271-120">Header</span></span>|<span data-ttu-id="ec271-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ec271-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ec271-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ec271-122">Authorization</span></span>|<span data-ttu-id="ec271-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ec271-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ec271-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ec271-124">Accept</span></span>|<span data-ttu-id="ec271-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ec271-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec271-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ec271-126">Request body</span></span>
<span data-ttu-id="ec271-127">В тексте запроса добавьте представление объекта deviceConfigurationUserStatus в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ec271-127">In the request body, supply a JSON representation for the deviceConfigurationUserStatus object.</span></span>

<span data-ttu-id="ec271-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceConfigurationUserStatus.</span><span class="sxs-lookup"><span data-stu-id="ec271-128">The following table shows the properties that are required when you create the deviceConfigurationUserStatus.</span></span>

|<span data-ttu-id="ec271-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ec271-129">Property</span></span>|<span data-ttu-id="ec271-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ec271-130">Type</span></span>|<span data-ttu-id="ec271-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ec271-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec271-132">id</span><span class="sxs-lookup"><span data-stu-id="ec271-132">id</span></span>|<span data-ttu-id="ec271-133">Строка</span><span class="sxs-lookup"><span data-stu-id="ec271-133">String</span></span>|<span data-ttu-id="ec271-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ec271-134">Key of the entity.</span></span>|
|<span data-ttu-id="ec271-135">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="ec271-135">userDisplayName</span></span>|<span data-ttu-id="ec271-136">String</span><span class="sxs-lookup"><span data-stu-id="ec271-136">String</span></span>|<span data-ttu-id="ec271-137">Имя пользователя в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="ec271-137">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="ec271-138">devicesCount</span><span class="sxs-lookup"><span data-stu-id="ec271-138">devicesCount</span></span>|<span data-ttu-id="ec271-139">Int32</span><span class="sxs-lookup"><span data-stu-id="ec271-139">Int32</span></span>|<span data-ttu-id="ec271-140">Количество устройств для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="ec271-140">Devices count for that user.</span></span>|
|<span data-ttu-id="ec271-141">status</span><span class="sxs-lookup"><span data-stu-id="ec271-141">status</span></span>|[<span data-ttu-id="ec271-142">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="ec271-142">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="ec271-143">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="ec271-143">Compliance status of the policy report.</span></span> <span data-ttu-id="ec271-144">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="ec271-144">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="ec271-145">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="ec271-145">lastReportedDateTime</span></span>|<span data-ttu-id="ec271-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec271-146">DateTimeOffset</span></span>|<span data-ttu-id="ec271-147">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="ec271-147">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="ec271-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ec271-148">userPrincipalName</span></span>|<span data-ttu-id="ec271-149">String</span><span class="sxs-lookup"><span data-stu-id="ec271-149">String</span></span>|<span data-ttu-id="ec271-150">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="ec271-150">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="ec271-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec271-151">Response</span></span>
<span data-ttu-id="ec271-152">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ec271-152">If successful, this method returns a `201 Created` response code and a [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec271-153">Пример</span><span class="sxs-lookup"><span data-stu-id="ec271-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="ec271-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="ec271-154">Request</span></span>
<span data-ttu-id="ec271-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ec271-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses
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

### <a name="response"></a><span data-ttu-id="ec271-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec271-156">Response</span></span>
<span data-ttu-id="ec271-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ec271-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




