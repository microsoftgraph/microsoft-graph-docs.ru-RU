---
title: Перечисление объектов deviceConfigurationUserStatus
description: Список свойств и связей объектов deviceConfigurationUserStatus.
author: tfitzmac
ms.openlocfilehash: 3f8c1910cfc06a40b477f8a4010caaf167b060a3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340231"
---
# <a name="list-deviceconfigurationuserstatuses"></a><span data-ttu-id="067cc-103">Перечисление объектов deviceConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="067cc-103">List deviceConfigurationUserStatuses</span></span>

> <span data-ttu-id="067cc-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="067cc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="067cc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="067cc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="067cc-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="067cc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="067cc-107">Список свойств и связей объектов [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="067cc-107">List properties and relationships of the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="067cc-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="067cc-108">Prerequisites</span></span>
<span data-ttu-id="067cc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="067cc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="067cc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="067cc-111">Permission type</span></span>|<span data-ttu-id="067cc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="067cc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="067cc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="067cc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="067cc-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="067cc-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="067cc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="067cc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="067cc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="067cc-116">Not supported.</span></span>|
|<span data-ttu-id="067cc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="067cc-117">Application</span></span>|<span data-ttu-id="067cc-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="067cc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="067cc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="067cc-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="067cc-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="067cc-120">Request headers</span></span>
|<span data-ttu-id="067cc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="067cc-121">Header</span></span>|<span data-ttu-id="067cc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="067cc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="067cc-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="067cc-123">Authorization</span></span>|<span data-ttu-id="067cc-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="067cc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="067cc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="067cc-125">Accept</span></span>|<span data-ttu-id="067cc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="067cc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="067cc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="067cc-127">Request body</span></span>
<span data-ttu-id="067cc-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="067cc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="067cc-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="067cc-129">Response</span></span>
<span data-ttu-id="067cc-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="067cc-130">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="067cc-131">Пример</span><span class="sxs-lookup"><span data-stu-id="067cc-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="067cc-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="067cc-132">Request</span></span>
<span data-ttu-id="067cc-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="067cc-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses
```

### <a name="response"></a><span data-ttu-id="067cc-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="067cc-134">Response</span></span>
<span data-ttu-id="067cc-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="067cc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





