---
title: Перечисление объектов deviceConfigurationDeviceStatus
description: Список свойств и связей объектов deviceConfigurationDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ae6a052ce4bd296353ecfc6713958a7e1747409e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27943846"
---
# <a name="list-deviceconfigurationdevicestatuses"></a><span data-ttu-id="835f0-103">Перечисление объектов deviceConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="835f0-103">List deviceConfigurationDeviceStatuses</span></span>

> <span data-ttu-id="835f0-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="835f0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="835f0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="835f0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="835f0-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="835f0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="835f0-107">Список свойств и связей объектов [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="835f0-107">List properties and relationships of the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="835f0-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="835f0-108">Prerequisites</span></span>
<span data-ttu-id="835f0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="835f0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="835f0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="835f0-111">Permission type</span></span>|<span data-ttu-id="835f0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="835f0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="835f0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="835f0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="835f0-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="835f0-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="835f0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="835f0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="835f0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="835f0-116">Not supported.</span></span>|
|<span data-ttu-id="835f0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="835f0-117">Application</span></span>|<span data-ttu-id="835f0-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="835f0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="835f0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="835f0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/deviceStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/deviceStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/deviceStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/deviceStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/deviceStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="835f0-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="835f0-120">Request headers</span></span>
|<span data-ttu-id="835f0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="835f0-121">Header</span></span>|<span data-ttu-id="835f0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="835f0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="835f0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="835f0-123">Authorization</span></span>|<span data-ttu-id="835f0-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="835f0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="835f0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="835f0-125">Accept</span></span>|<span data-ttu-id="835f0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="835f0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="835f0-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="835f0-127">Request body</span></span>
<span data-ttu-id="835f0-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="835f0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="835f0-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="835f0-129">Response</span></span>
<span data-ttu-id="835f0-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="835f0-130">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="835f0-131">Пример</span><span class="sxs-lookup"><span data-stu-id="835f0-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="835f0-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="835f0-132">Request</span></span>
<span data-ttu-id="835f0-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="835f0-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
```

### <a name="response"></a><span data-ttu-id="835f0-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="835f0-134">Response</span></span>
<span data-ttu-id="835f0-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="835f0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 569

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
      "id": "674e98e5-98e5-674e-e598-4e67e5984e67",
      "deviceDisplayName": "Device Display Name value",
      "userName": "User Name value",
      "deviceModel": "Device Model value",
      "platform": 8,
      "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
      "status": "notApplicable",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```





