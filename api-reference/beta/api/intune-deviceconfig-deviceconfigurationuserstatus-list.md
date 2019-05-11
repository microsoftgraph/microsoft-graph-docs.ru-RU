---
title: Перечисление объектов deviceConfigurationUserStatus
description: Список свойств и связей объектов deviceConfigurationUserStatus.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1ed341e91de907ff6d8b255f5472ff27e1e60081
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33927134"
---
# <a name="list-deviceconfigurationuserstatuses"></a><span data-ttu-id="33eb3-103">Перечисление объектов deviceConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="33eb3-103">List deviceConfigurationUserStatuses</span></span>

> <span data-ttu-id="33eb3-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33eb3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="33eb3-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="33eb3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33eb3-106">Список свойств и связей объектов [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="33eb3-106">List properties and relationships of the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="33eb3-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="33eb3-107">Prerequisites</span></span>
<span data-ttu-id="33eb3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33eb3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33eb3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="33eb3-110">Permission type</span></span>|<span data-ttu-id="33eb3-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="33eb3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="33eb3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="33eb3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="33eb3-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="33eb3-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="33eb3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="33eb3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33eb3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33eb3-115">Not supported.</span></span>|
|<span data-ttu-id="33eb3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="33eb3-116">Application</span></span>|<span data-ttu-id="33eb3-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33eb3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="33eb3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="33eb3-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="33eb3-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="33eb3-119">Request headers</span></span>
|<span data-ttu-id="33eb3-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="33eb3-120">Header</span></span>|<span data-ttu-id="33eb3-121">Значение</span><span class="sxs-lookup"><span data-stu-id="33eb3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="33eb3-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="33eb3-122">Authorization</span></span>|<span data-ttu-id="33eb3-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="33eb3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="33eb3-124">Accept</span><span class="sxs-lookup"><span data-stu-id="33eb3-124">Accept</span></span>|<span data-ttu-id="33eb3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="33eb3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="33eb3-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="33eb3-126">Request body</span></span>
<span data-ttu-id="33eb3-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="33eb3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="33eb3-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="33eb3-128">Response</span></span>
<span data-ttu-id="33eb3-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="33eb3-129">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33eb3-130">Пример</span><span class="sxs-lookup"><span data-stu-id="33eb3-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="33eb3-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="33eb3-131">Request</span></span>
<span data-ttu-id="33eb3-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="33eb3-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses
```

### <a name="response"></a><span data-ttu-id="33eb3-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="33eb3-133">Response</span></span>
<span data-ttu-id="33eb3-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="33eb3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




