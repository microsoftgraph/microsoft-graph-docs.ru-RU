---
title: Перечисление объектов deviceConfigurationUserStatus
description: Список свойств и связей объектов deviceConfigurationUserStatus.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 70af6972f358ab34d5ce3dff825be7da19923984
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420530"
---
# <a name="list-deviceconfigurationuserstatuses"></a><span data-ttu-id="9b162-103">Перечисление объектов deviceConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="9b162-103">List deviceConfigurationUserStatuses</span></span>

> <span data-ttu-id="9b162-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9b162-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9b162-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b162-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9b162-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9b162-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b162-107">Список свойств и связей объектов [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="9b162-107">List properties and relationships of the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9b162-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9b162-108">Prerequisites</span></span>
<span data-ttu-id="9b162-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="9b162-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9b162-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9b162-111">Permission type</span></span>|<span data-ttu-id="9b162-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9b162-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b162-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9b162-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9b162-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9b162-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9b162-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9b162-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b162-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b162-116">Not supported.</span></span>|
|<span data-ttu-id="9b162-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9b162-117">Application</span></span>|<span data-ttu-id="9b162-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b162-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b162-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9b162-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="9b162-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9b162-120">Request headers</span></span>
|<span data-ttu-id="9b162-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9b162-121">Header</span></span>|<span data-ttu-id="9b162-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9b162-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9b162-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9b162-123">Authorization</span></span>|<span data-ttu-id="9b162-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="9b162-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9b162-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9b162-125">Accept</span></span>|<span data-ttu-id="9b162-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9b162-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b162-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9b162-127">Request body</span></span>
<span data-ttu-id="9b162-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9b162-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9b162-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b162-129">Response</span></span>
<span data-ttu-id="9b162-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9b162-130">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b162-131">Пример</span><span class="sxs-lookup"><span data-stu-id="9b162-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="9b162-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="9b162-132">Request</span></span>
<span data-ttu-id="9b162-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9b162-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses
```

### <a name="response"></a><span data-ttu-id="9b162-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b162-134">Response</span></span>
<span data-ttu-id="9b162-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="9b162-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




