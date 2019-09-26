---
title: Перечисление объектов deviceConfigurationUserStatus
description: Список свойств и связей объектов deviceConfigurationUserStatus.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 013bbcd80438150e4fe08c61f56b9efd491e2494
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37174692"
---
# <a name="list-deviceconfigurationuserstatuses"></a><span data-ttu-id="bc4eb-103">Перечисление объектов deviceConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="bc4eb-103">List deviceConfigurationUserStatuses</span></span>

> <span data-ttu-id="bc4eb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc4eb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bc4eb-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bc4eb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc4eb-106">Список свойств и связей объектов [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="bc4eb-106">List properties and relationships of the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bc4eb-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="bc4eb-107">Prerequisites</span></span>
<span data-ttu-id="bc4eb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc4eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc4eb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bc4eb-110">Permission type</span></span>|<span data-ttu-id="bc4eb-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bc4eb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bc4eb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bc4eb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bc4eb-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="bc4eb-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="bc4eb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bc4eb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bc4eb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc4eb-115">Not supported.</span></span>|
|<span data-ttu-id="bc4eb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bc4eb-116">Application</span></span>|<span data-ttu-id="bc4eb-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="bc4eb-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bc4eb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bc4eb-118">HTTP Request</span></span>
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
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/userStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/userStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/userStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="bc4eb-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bc4eb-119">Request headers</span></span>
|<span data-ttu-id="bc4eb-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bc4eb-120">Header</span></span>|<span data-ttu-id="bc4eb-121">Значение</span><span class="sxs-lookup"><span data-stu-id="bc4eb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bc4eb-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bc4eb-122">Authorization</span></span>|<span data-ttu-id="bc4eb-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bc4eb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bc4eb-124">Accept</span><span class="sxs-lookup"><span data-stu-id="bc4eb-124">Accept</span></span>|<span data-ttu-id="bc4eb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bc4eb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc4eb-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bc4eb-126">Request body</span></span>
<span data-ttu-id="bc4eb-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bc4eb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bc4eb-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="bc4eb-128">Response</span></span>
<span data-ttu-id="bc4eb-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bc4eb-129">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc4eb-130">Пример</span><span class="sxs-lookup"><span data-stu-id="bc4eb-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="bc4eb-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc4eb-131">Request</span></span>
<span data-ttu-id="bc4eb-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bc4eb-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses
```

### <a name="response"></a><span data-ttu-id="bc4eb-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc4eb-133">Response</span></span>
<span data-ttu-id="bc4eb-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bc4eb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




