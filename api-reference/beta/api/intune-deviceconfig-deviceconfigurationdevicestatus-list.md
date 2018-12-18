---
title: Перечисление объектов deviceConfigurationDeviceStatus
description: Список свойств и связей объектов deviceConfigurationDeviceStatus.
author: tfitzmac
ms.openlocfilehash: 2ec7116917891e29798a71b2cb36a75a7468fe1b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336570"
---
# <a name="list-deviceconfigurationdevicestatuses"></a><span data-ttu-id="06a6f-103">Перечисление объектов deviceConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="06a6f-103">List deviceConfigurationDeviceStatuses</span></span>

> <span data-ttu-id="06a6f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="06a6f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="06a6f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06a6f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="06a6f-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="06a6f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="06a6f-107">Список свойств и связей объектов [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="06a6f-107">List properties and relationships of the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="06a6f-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="06a6f-108">Prerequisites</span></span>
<span data-ttu-id="06a6f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06a6f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06a6f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="06a6f-111">Permission type</span></span>|<span data-ttu-id="06a6f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="06a6f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06a6f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="06a6f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="06a6f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="06a6f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="06a6f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="06a6f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06a6f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06a6f-116">Not supported.</span></span>|
|<span data-ttu-id="06a6f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="06a6f-117">Application</span></span>|<span data-ttu-id="06a6f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06a6f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="06a6f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="06a6f-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="06a6f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="06a6f-120">Request headers</span></span>
|<span data-ttu-id="06a6f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="06a6f-121">Header</span></span>|<span data-ttu-id="06a6f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="06a6f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06a6f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="06a6f-123">Authorization</span></span>|<span data-ttu-id="06a6f-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="06a6f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06a6f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="06a6f-125">Accept</span></span>|<span data-ttu-id="06a6f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="06a6f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06a6f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="06a6f-127">Request body</span></span>
<span data-ttu-id="06a6f-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="06a6f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06a6f-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="06a6f-129">Response</span></span>
<span data-ttu-id="06a6f-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="06a6f-130">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06a6f-131">Пример</span><span class="sxs-lookup"><span data-stu-id="06a6f-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="06a6f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="06a6f-132">Request</span></span>
<span data-ttu-id="06a6f-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="06a6f-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
```

### <a name="response"></a><span data-ttu-id="06a6f-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="06a6f-134">Response</span></span>
<span data-ttu-id="06a6f-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="06a6f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





