---
title: Get deviceConfigurationUserStatus
description: Чтение свойств и связей объекта deviceConfigurationUserStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3e7873a32db68136c33c040ae141647b75f053f8
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174384"
---
# <a name="get-deviceconfigurationuserstatus"></a><span data-ttu-id="c5417-103">Get deviceConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="c5417-103">Get deviceConfigurationUserStatus</span></span>

> <span data-ttu-id="c5417-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5417-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c5417-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c5417-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5417-106">Чтение свойств и связей объекта [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="c5417-106">Read properties and relationships of the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c5417-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="c5417-107">Prerequisites</span></span>
<span data-ttu-id="c5417-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c5417-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c5417-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c5417-110">Permission type</span></span>|<span data-ttu-id="c5417-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c5417-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5417-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c5417-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c5417-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c5417-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c5417-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c5417-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5417-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5417-115">Not supported.</span></span>|
|<span data-ttu-id="c5417-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c5417-116">Application</span></span>|<span data-ttu-id="c5417-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5417-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5417-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c5417-118">HTTP Request</span></span>
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
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/userStatuses/{deviceConfigurationUserStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/userStatuses/{deviceConfigurationUserStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c5417-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c5417-119">Optional query parameters</span></span>
<span data-ttu-id="c5417-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c5417-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c5417-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c5417-121">Request headers</span></span>
|<span data-ttu-id="c5417-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c5417-122">Header</span></span>|<span data-ttu-id="c5417-123">Значение</span><span class="sxs-lookup"><span data-stu-id="c5417-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5417-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5417-124">Authorization</span></span>|<span data-ttu-id="c5417-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c5417-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5417-126">Accept</span><span class="sxs-lookup"><span data-stu-id="c5417-126">Accept</span></span>|<span data-ttu-id="c5417-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c5417-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5417-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c5417-128">Request body</span></span>
<span data-ttu-id="c5417-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c5417-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5417-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="c5417-130">Response</span></span>
<span data-ttu-id="c5417-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c5417-131">If successful, this method returns a `200 OK` response code and [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5417-132">Пример</span><span class="sxs-lookup"><span data-stu-id="c5417-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="c5417-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="c5417-133">Request</span></span>
<span data-ttu-id="c5417-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c5417-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
```

### <a name="response"></a><span data-ttu-id="c5417-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5417-135">Response</span></span>
<span data-ttu-id="c5417-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c5417-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




