---
title: Перечисление объектов deviceConfigurationDeviceStatus
description: Список свойств и связей объектов deviceConfigurationDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6b69b1134be87ae098c8b4a9365025401e64d830
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30979615"
---
# <a name="list-deviceconfigurationdevicestatuses"></a><span data-ttu-id="d074f-103">Перечисление объектов deviceConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="d074f-103">List deviceConfigurationDeviceStatuses</span></span>

> <span data-ttu-id="d074f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d074f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d074f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d074f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d074f-106">Список свойств и связей объектов [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="d074f-106">List properties and relationships of the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d074f-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d074f-107">Prerequisites</span></span>
<span data-ttu-id="d074f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d074f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d074f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d074f-110">Permission type</span></span>|<span data-ttu-id="d074f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d074f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d074f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d074f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d074f-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d074f-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d074f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d074f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d074f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d074f-115">Not supported.</span></span>|
|<span data-ttu-id="d074f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d074f-116">Application</span></span>|<span data-ttu-id="d074f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d074f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d074f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d074f-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="d074f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d074f-119">Request headers</span></span>
|<span data-ttu-id="d074f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d074f-120">Header</span></span>|<span data-ttu-id="d074f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d074f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d074f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d074f-122">Authorization</span></span>|<span data-ttu-id="d074f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d074f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d074f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d074f-124">Accept</span></span>|<span data-ttu-id="d074f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d074f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d074f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d074f-126">Request body</span></span>
<span data-ttu-id="d074f-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d074f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d074f-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="d074f-128">Response</span></span>
<span data-ttu-id="d074f-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d074f-129">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d074f-130">Пример</span><span class="sxs-lookup"><span data-stu-id="d074f-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="d074f-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="d074f-131">Request</span></span>
<span data-ttu-id="d074f-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d074f-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
```

### <a name="response"></a><span data-ttu-id="d074f-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="d074f-133">Response</span></span>
<span data-ttu-id="d074f-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d074f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




