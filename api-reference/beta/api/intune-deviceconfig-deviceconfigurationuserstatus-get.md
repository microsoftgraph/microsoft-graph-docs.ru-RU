---
title: Get deviceConfigurationUserStatus
description: Чтение свойств и связей объекта deviceConfigurationUserStatus.
ms.openlocfilehash: 780880ec43d14e33422f590d46a505806ae32389
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077497"
---
# <a name="get-deviceconfigurationuserstatus"></a><span data-ttu-id="cc5d2-103">Get deviceConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="cc5d2-103">Get deviceConfigurationUserStatus</span></span>

> <span data-ttu-id="cc5d2-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cc5d2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cc5d2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc5d2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cc5d2-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="cc5d2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cc5d2-107">Чтение свойств и связей объекта [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="cc5d2-107">Read properties and relationships of the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cc5d2-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="cc5d2-108">Prerequisites</span></span>
<span data-ttu-id="cc5d2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc5d2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc5d2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cc5d2-111">Permission type</span></span>|<span data-ttu-id="cc5d2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cc5d2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cc5d2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cc5d2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cc5d2-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="cc5d2-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="cc5d2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cc5d2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cc5d2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc5d2-116">Not supported.</span></span>|
|<span data-ttu-id="cc5d2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cc5d2-117">Application</span></span>|<span data-ttu-id="cc5d2-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc5d2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cc5d2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cc5d2-119">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="cc5d2-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cc5d2-120">Optional query parameters</span></span>
<span data-ttu-id="cc5d2-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="cc5d2-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="cc5d2-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cc5d2-122">Request headers</span></span>
|<span data-ttu-id="cc5d2-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cc5d2-123">Header</span></span>|<span data-ttu-id="cc5d2-124">Значение</span><span class="sxs-lookup"><span data-stu-id="cc5d2-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cc5d2-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="cc5d2-125">Authorization</span></span>|<span data-ttu-id="cc5d2-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="cc5d2-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cc5d2-127">Accept</span><span class="sxs-lookup"><span data-stu-id="cc5d2-127">Accept</span></span>|<span data-ttu-id="cc5d2-128">application/json</span><span class="sxs-lookup"><span data-stu-id="cc5d2-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cc5d2-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cc5d2-129">Request body</span></span>
<span data-ttu-id="cc5d2-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cc5d2-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cc5d2-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="cc5d2-131">Response</span></span>
<span data-ttu-id="cc5d2-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="cc5d2-132">If successful, this method returns a `200 OK` response code and [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc5d2-133">Пример</span><span class="sxs-lookup"><span data-stu-id="cc5d2-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="cc5d2-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="cc5d2-134">Request</span></span>
<span data-ttu-id="cc5d2-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cc5d2-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
```

### <a name="response"></a><span data-ttu-id="cc5d2-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="cc5d2-136">Response</span></span>
<span data-ttu-id="cc5d2-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="cc5d2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





