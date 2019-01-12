---
title: Перечисление объектов deviceConfigurationUserStatus
description: Список свойств и связей объектов deviceConfigurationUserStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c44f984aab21a2155ce2f93fd25f82752f8aa7c7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27943146"
---
# <a name="list-deviceconfigurationuserstatuses"></a><span data-ttu-id="2df37-103">Перечисление объектов deviceConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="2df37-103">List deviceConfigurationUserStatuses</span></span>

> <span data-ttu-id="2df37-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2df37-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2df37-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2df37-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2df37-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2df37-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2df37-107">Список свойств и связей объектов [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="2df37-107">List properties and relationships of the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2df37-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2df37-108">Prerequisites</span></span>
<span data-ttu-id="2df37-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2df37-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2df37-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2df37-111">Permission type</span></span>|<span data-ttu-id="2df37-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2df37-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2df37-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2df37-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2df37-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2df37-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2df37-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2df37-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2df37-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2df37-116">Not supported.</span></span>|
|<span data-ttu-id="2df37-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2df37-117">Application</span></span>|<span data-ttu-id="2df37-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2df37-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2df37-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2df37-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="2df37-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2df37-120">Request headers</span></span>
|<span data-ttu-id="2df37-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2df37-121">Header</span></span>|<span data-ttu-id="2df37-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2df37-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2df37-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2df37-123">Authorization</span></span>|<span data-ttu-id="2df37-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="2df37-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2df37-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2df37-125">Accept</span></span>|<span data-ttu-id="2df37-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2df37-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2df37-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2df37-127">Request body</span></span>
<span data-ttu-id="2df37-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2df37-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2df37-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="2df37-129">Response</span></span>
<span data-ttu-id="2df37-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2df37-130">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2df37-131">Пример</span><span class="sxs-lookup"><span data-stu-id="2df37-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="2df37-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="2df37-132">Request</span></span>
<span data-ttu-id="2df37-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2df37-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses
```

### <a name="response"></a><span data-ttu-id="2df37-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="2df37-134">Response</span></span>
<span data-ttu-id="2df37-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2df37-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





