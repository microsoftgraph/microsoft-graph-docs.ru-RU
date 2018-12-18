---
title: Get deviceConfigurationDeviceOverview
description: Чтение свойств и связей объекта deviceConfigurationDeviceOverview.
author: tfitzmac
ms.openlocfilehash: 2087a92100e69992b3028b7ede45e1c5a64cef82
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312609"
---
# <a name="get-deviceconfigurationdeviceoverview"></a><span data-ttu-id="2e50d-103">Get deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="2e50d-103">Get deviceConfigurationDeviceOverview</span></span>

> <span data-ttu-id="2e50d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2e50d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2e50d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e50d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2e50d-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2e50d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2e50d-107">Чтение свойств и связей объекта [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="2e50d-107">Read properties and relationships of the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2e50d-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="2e50d-108">Prerequisites</span></span>
<span data-ttu-id="2e50d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e50d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e50d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2e50d-111">Permission type</span></span>|<span data-ttu-id="2e50d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2e50d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2e50d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2e50d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2e50d-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2e50d-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2e50d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2e50d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2e50d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e50d-116">Not supported.</span></span>|
|<span data-ttu-id="2e50d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2e50d-117">Application</span></span>|<span data-ttu-id="2e50d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e50d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2e50d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2e50d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/deviceStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/deviceStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/deviceStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/deviceStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/deviceStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceStatusOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2e50d-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2e50d-120">Optional query parameters</span></span>
<span data-ttu-id="2e50d-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2e50d-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="2e50d-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2e50d-122">Request headers</span></span>
|<span data-ttu-id="2e50d-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2e50d-123">Header</span></span>|<span data-ttu-id="2e50d-124">Значение</span><span class="sxs-lookup"><span data-stu-id="2e50d-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2e50d-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2e50d-125">Authorization</span></span>|<span data-ttu-id="2e50d-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="2e50d-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2e50d-127">Accept</span><span class="sxs-lookup"><span data-stu-id="2e50d-127">Accept</span></span>|<span data-ttu-id="2e50d-128">application/json</span><span class="sxs-lookup"><span data-stu-id="2e50d-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e50d-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2e50d-129">Request body</span></span>
<span data-ttu-id="2e50d-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2e50d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2e50d-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="2e50d-131">Response</span></span>
<span data-ttu-id="2e50d-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="2e50d-132">If successful, this method returns a `200 OK` response code and [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e50d-133">Пример</span><span class="sxs-lookup"><span data-stu-id="2e50d-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="2e50d-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="2e50d-134">Request</span></span>
<span data-ttu-id="2e50d-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2e50d-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
```

### <a name="response"></a><span data-ttu-id="2e50d-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="2e50d-136">Response</span></span>
<span data-ttu-id="2e50d-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2e50d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 435

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationDeviceOverview",
    "id": "62d48e3a-8e3a-62d4-3a8e-d4623a8ed462",
    "pendingCount": 12,
    "notApplicableCount": 2,
    "notApplicablePlatformCount": 10,
    "successCount": 12,
    "errorCount": 10,
    "failedCount": 11,
    "conflictCount": 13,
    "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
    "configurationVersion": 4
  }
}
```





