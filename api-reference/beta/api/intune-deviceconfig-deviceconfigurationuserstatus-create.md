---
title: Создание объекта deviceConfigurationUserStatus
description: Создание объекта deviceConfigurationUserStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3824eb91797f4bdbdd1ba7b3af1f32e981db13ef
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724864"
---
# <a name="create-deviceconfigurationuserstatus"></a><span data-ttu-id="ec10e-103">Создание объекта deviceConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="ec10e-103">Create deviceConfigurationUserStatus</span></span>

<span data-ttu-id="ec10e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec10e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ec10e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec10e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ec10e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ec10e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec10e-107">Создание объекта [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="ec10e-107">Create a new [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ec10e-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ec10e-108">Prerequisites</span></span>
<span data-ttu-id="ec10e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec10e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec10e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ec10e-111">Permission type</span></span>|<span data-ttu-id="ec10e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ec10e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ec10e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ec10e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ec10e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec10e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ec10e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ec10e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ec10e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec10e-116">Not supported.</span></span>|
|<span data-ttu-id="ec10e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ec10e-117">Application</span></span>|<span data-ttu-id="ec10e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec10e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ec10e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ec10e-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="ec10e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ec10e-120">Request headers</span></span>
|<span data-ttu-id="ec10e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ec10e-121">Header</span></span>|<span data-ttu-id="ec10e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ec10e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ec10e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ec10e-123">Authorization</span></span>|<span data-ttu-id="ec10e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ec10e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ec10e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ec10e-125">Accept</span></span>|<span data-ttu-id="ec10e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ec10e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec10e-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ec10e-127">Request body</span></span>
<span data-ttu-id="ec10e-128">В тексте запроса добавьте представление объекта deviceConfigurationUserStatus в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ec10e-128">In the request body, supply a JSON representation for the deviceConfigurationUserStatus object.</span></span>

<span data-ttu-id="ec10e-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceConfigurationUserStatus.</span><span class="sxs-lookup"><span data-stu-id="ec10e-129">The following table shows the properties that are required when you create the deviceConfigurationUserStatus.</span></span>

|<span data-ttu-id="ec10e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ec10e-130">Property</span></span>|<span data-ttu-id="ec10e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ec10e-131">Type</span></span>|<span data-ttu-id="ec10e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ec10e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec10e-133">id</span><span class="sxs-lookup"><span data-stu-id="ec10e-133">id</span></span>|<span data-ttu-id="ec10e-134">Строка</span><span class="sxs-lookup"><span data-stu-id="ec10e-134">String</span></span>|<span data-ttu-id="ec10e-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ec10e-135">Key of the entity.</span></span>|
|<span data-ttu-id="ec10e-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="ec10e-136">userDisplayName</span></span>|<span data-ttu-id="ec10e-137">String</span><span class="sxs-lookup"><span data-stu-id="ec10e-137">String</span></span>|<span data-ttu-id="ec10e-138">Имя пользователя в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="ec10e-138">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="ec10e-139">devicesCount</span><span class="sxs-lookup"><span data-stu-id="ec10e-139">devicesCount</span></span>|<span data-ttu-id="ec10e-140">Int32</span><span class="sxs-lookup"><span data-stu-id="ec10e-140">Int32</span></span>|<span data-ttu-id="ec10e-141">Количество устройств для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="ec10e-141">Devices count for that user.</span></span>|
|<span data-ttu-id="ec10e-142">status</span><span class="sxs-lookup"><span data-stu-id="ec10e-142">status</span></span>|[<span data-ttu-id="ec10e-143">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="ec10e-143">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="ec10e-144">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="ec10e-144">Compliance status of the policy report.</span></span> <span data-ttu-id="ec10e-145">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="ec10e-145">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="ec10e-146">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="ec10e-146">lastReportedDateTime</span></span>|<span data-ttu-id="ec10e-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec10e-147">DateTimeOffset</span></span>|<span data-ttu-id="ec10e-148">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="ec10e-148">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="ec10e-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ec10e-149">userPrincipalName</span></span>|<span data-ttu-id="ec10e-150">String</span><span class="sxs-lookup"><span data-stu-id="ec10e-150">String</span></span>|<span data-ttu-id="ec10e-151">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="ec10e-151">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="ec10e-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec10e-152">Response</span></span>
<span data-ttu-id="ec10e-153">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ec10e-153">If successful, this method returns a `201 Created` response code and a [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec10e-154">Пример</span><span class="sxs-lookup"><span data-stu-id="ec10e-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="ec10e-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="ec10e-155">Request</span></span>
<span data-ttu-id="ec10e-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ec10e-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ec10e-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec10e-157">Response</span></span>
<span data-ttu-id="ec10e-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ec10e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





