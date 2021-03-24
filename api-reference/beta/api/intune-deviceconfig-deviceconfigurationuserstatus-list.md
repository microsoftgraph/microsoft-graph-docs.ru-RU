---
title: Перечисление объектов deviceConfigurationUserStatus
description: Список свойств и связей объектов deviceConfigurationUserStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e69ce1d68d675db4a010a3d6ef17c857d7ffeb80
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51137478"
---
# <a name="list-deviceconfigurationuserstatuses"></a><span data-ttu-id="b2202-103">Перечисление объектов deviceConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="b2202-103">List deviceConfigurationUserStatuses</span></span>

<span data-ttu-id="b2202-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2202-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b2202-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2202-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2202-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b2202-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2202-107">Список свойств и связей объектов [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="b2202-107">List properties and relationships of the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b2202-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b2202-108">Prerequisites</span></span>
<span data-ttu-id="b2202-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2202-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2202-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b2202-111">Permission type</span></span>|<span data-ttu-id="b2202-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b2202-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2202-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b2202-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b2202-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2202-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b2202-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b2202-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2202-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2202-116">Not supported.</span></span>|
|<span data-ttu-id="b2202-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="b2202-117">Application</span></span>|<span data-ttu-id="b2202-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2202-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2202-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b2202-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/userStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/userStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/userStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/userStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/userStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/userStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/userStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/userStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="b2202-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b2202-120">Request headers</span></span>
|<span data-ttu-id="b2202-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b2202-121">Header</span></span>|<span data-ttu-id="b2202-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b2202-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2202-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2202-123">Authorization</span></span>|<span data-ttu-id="b2202-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b2202-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2202-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b2202-125">Accept</span></span>|<span data-ttu-id="b2202-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b2202-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2202-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b2202-127">Request body</span></span>
<span data-ttu-id="b2202-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b2202-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b2202-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2202-129">Response</span></span>
<span data-ttu-id="b2202-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b2202-130">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2202-131">Пример</span><span class="sxs-lookup"><span data-stu-id="b2202-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b2202-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b2202-132">Request</span></span>
<span data-ttu-id="b2202-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b2202-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses
```

### <a name="response"></a><span data-ttu-id="b2202-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2202-134">Response</span></span>
<span data-ttu-id="b2202-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b2202-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 400

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationUserStatus",
      "id": "7e323db2-3db2-7e32-b23d-327eb23d327e",
      "userDisplayName": "User Display Name value",
      "devicesCount": 12,
      "status": "notApplicable",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```




