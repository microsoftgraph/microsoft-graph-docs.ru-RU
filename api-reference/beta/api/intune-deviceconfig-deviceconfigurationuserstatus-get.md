---
title: Get deviceConfigurationUserStatus
description: Чтение свойств и связей объекта deviceConfigurationUserStatus.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 95af09024416e0af9a39f30a7da10c11bf703ecb
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43433205"
---
# <a name="get-deviceconfigurationuserstatus"></a><span data-ttu-id="bbfbe-103">Get deviceConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="bbfbe-103">Get deviceConfigurationUserStatus</span></span>

<span data-ttu-id="bbfbe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bbfbe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bbfbe-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bbfbe-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bbfbe-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bbfbe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bbfbe-107">Чтение свойств и связей объекта [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="bbfbe-107">Read properties and relationships of the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bbfbe-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="bbfbe-108">Prerequisites</span></span>
<span data-ttu-id="bbfbe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bbfbe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bbfbe-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bbfbe-111">Permission type</span></span>|<span data-ttu-id="bbfbe-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bbfbe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bbfbe-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bbfbe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bbfbe-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="bbfbe-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="bbfbe-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bbfbe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bbfbe-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bbfbe-116">Not supported.</span></span>|
|<span data-ttu-id="bbfbe-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bbfbe-117">Application</span></span>|<span data-ttu-id="bbfbe-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="bbfbe-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bbfbe-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bbfbe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/userStatuses/{deviceConfigurationUserStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/userStatuses/{deviceConfigurationUserStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/userStatuses/{deviceConfigurationUserStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/userStatuses/{deviceConfigurationUserStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/userStatuses/{deviceConfigurationUserStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/userStatuses/{deviceConfigurationUserStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/userStatuses/{deviceConfigurationUserStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/userStatuses/{deviceConfigurationUserStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/userStatuses/{deviceConfigurationUserStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bbfbe-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bbfbe-120">Optional query parameters</span></span>
<span data-ttu-id="bbfbe-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="bbfbe-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bbfbe-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bbfbe-122">Request headers</span></span>
|<span data-ttu-id="bbfbe-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bbfbe-123">Header</span></span>|<span data-ttu-id="bbfbe-124">Значение</span><span class="sxs-lookup"><span data-stu-id="bbfbe-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bbfbe-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bbfbe-125">Authorization</span></span>|<span data-ttu-id="bbfbe-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bbfbe-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bbfbe-127">Accept</span><span class="sxs-lookup"><span data-stu-id="bbfbe-127">Accept</span></span>|<span data-ttu-id="bbfbe-128">application/json</span><span class="sxs-lookup"><span data-stu-id="bbfbe-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bbfbe-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bbfbe-129">Request body</span></span>
<span data-ttu-id="bbfbe-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bbfbe-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bbfbe-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="bbfbe-131">Response</span></span>
<span data-ttu-id="bbfbe-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="bbfbe-132">If successful, this method returns a `200 OK` response code and [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bbfbe-133">Пример</span><span class="sxs-lookup"><span data-stu-id="bbfbe-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="bbfbe-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="bbfbe-134">Request</span></span>
<span data-ttu-id="bbfbe-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bbfbe-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
```

### <a name="response"></a><span data-ttu-id="bbfbe-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="bbfbe-136">Response</span></span>
<span data-ttu-id="bbfbe-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bbfbe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 372

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationUserStatus",
    "id": "7e323db2-3db2-7e32-b23d-327eb23d327e",
    "userDisplayName": "User Display Name value",
    "devicesCount": 12,
    "status": "notApplicable",
    "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
    "userPrincipalName": "User Principal Name value"
  }
}
```



