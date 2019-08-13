---
title: Get deviceConfigurationUserStatus
description: Чтение свойств и связей объекта deviceConfigurationUserStatus.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 256e873523dfbf33f8a090647526f8950157b22f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36345808"
---
# <a name="get-deviceconfigurationuserstatus"></a><span data-ttu-id="fcfb0-103">Get deviceConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="fcfb0-103">Get deviceConfigurationUserStatus</span></span>

> <span data-ttu-id="fcfb0-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fcfb0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fcfb0-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fcfb0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fcfb0-106">Чтение свойств и связей объекта [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="fcfb0-106">Read properties and relationships of the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fcfb0-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="fcfb0-107">Prerequisites</span></span>
<span data-ttu-id="fcfb0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fcfb0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fcfb0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fcfb0-110">Permission type</span></span>|<span data-ttu-id="fcfb0-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fcfb0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fcfb0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fcfb0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fcfb0-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fcfb0-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="fcfb0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fcfb0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fcfb0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fcfb0-115">Not supported.</span></span>|
|<span data-ttu-id="fcfb0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fcfb0-116">Application</span></span>|<span data-ttu-id="fcfb0-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fcfb0-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fcfb0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fcfb0-118">HTTP Request</span></span>
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
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/userStatuses/{deviceConfigurationUserStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/userStatuses/{deviceConfigurationUserStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerCertificateProfileBase/rootCertificate/userStatuses/{deviceConfigurationUserStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/userStatuses/{deviceConfigurationUserStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/userStatuses/{deviceConfigurationUserStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fcfb0-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fcfb0-119">Optional query parameters</span></span>
<span data-ttu-id="fcfb0-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fcfb0-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fcfb0-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fcfb0-121">Request headers</span></span>
|<span data-ttu-id="fcfb0-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fcfb0-122">Header</span></span>|<span data-ttu-id="fcfb0-123">Значение</span><span class="sxs-lookup"><span data-stu-id="fcfb0-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fcfb0-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fcfb0-124">Authorization</span></span>|<span data-ttu-id="fcfb0-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fcfb0-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fcfb0-126">Accept</span><span class="sxs-lookup"><span data-stu-id="fcfb0-126">Accept</span></span>|<span data-ttu-id="fcfb0-127">application/json</span><span class="sxs-lookup"><span data-stu-id="fcfb0-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fcfb0-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fcfb0-128">Request body</span></span>
<span data-ttu-id="fcfb0-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fcfb0-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fcfb0-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="fcfb0-130">Response</span></span>
<span data-ttu-id="fcfb0-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="fcfb0-131">If successful, this method returns a `200 OK` response code and [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fcfb0-132">Пример</span><span class="sxs-lookup"><span data-stu-id="fcfb0-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="fcfb0-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="fcfb0-133">Request</span></span>
<span data-ttu-id="fcfb0-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fcfb0-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
```

### <a name="response"></a><span data-ttu-id="fcfb0-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="fcfb0-135">Response</span></span>
<span data-ttu-id="fcfb0-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fcfb0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






