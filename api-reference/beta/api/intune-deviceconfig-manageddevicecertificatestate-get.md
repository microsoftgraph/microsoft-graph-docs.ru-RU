---
title: Получение managedDeviceCertificateState
description: Чтение свойства и связи объекта managedDeviceCertificateState.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: bc99c6d5277d7c5379721a89d19179a0b8392b6c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967576"
---
# <a name="get-manageddevicecertificatestate"></a><span data-ttu-id="043e4-103">Получение managedDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="043e4-103">Get managedDeviceCertificateState</span></span>

> <span data-ttu-id="043e4-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="043e4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="043e4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="043e4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="043e4-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="043e4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="043e4-107">Чтение свойства и связи объекта [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="043e4-107">Read properties and relationships of the [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="043e4-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="043e4-108">Prerequisites</span></span>
<span data-ttu-id="043e4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="043e4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="043e4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="043e4-111">Permission type</span></span>|<span data-ttu-id="043e4-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="043e4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="043e4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="043e4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="043e4-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="043e4-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="043e4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="043e4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="043e4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="043e4-116">Not supported.</span></span>|
|<span data-ttu-id="043e4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="043e4-117">Application</span></span>|<span data-ttu-id="043e4-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="043e4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="043e4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="043e4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfileScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10PkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10ImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windowsPhone81ImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="043e4-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="043e4-120">Optional query parameters</span></span>
<span data-ttu-id="043e4-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="043e4-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="043e4-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="043e4-122">Request headers</span></span>
|<span data-ttu-id="043e4-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="043e4-123">Header</span></span>|<span data-ttu-id="043e4-124">Значение</span><span class="sxs-lookup"><span data-stu-id="043e4-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="043e4-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="043e4-125">Authorization</span></span>|<span data-ttu-id="043e4-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="043e4-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="043e4-127">Accept</span><span class="sxs-lookup"><span data-stu-id="043e4-127">Accept</span></span>|<span data-ttu-id="043e4-128">application/json</span><span class="sxs-lookup"><span data-stu-id="043e4-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="043e4-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="043e4-129">Request body</span></span>
<span data-ttu-id="043e4-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="043e4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="043e4-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="043e4-131">Response</span></span>
<span data-ttu-id="043e4-132">Успешно завершена, этот метод возвращает `200 OK` объект [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="043e4-132">If successful, this method returns a `200 OK` response code and [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="043e4-133">Пример</span><span class="sxs-lookup"><span data-stu-id="043e4-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="043e4-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="043e4-134">Request</span></span>
<span data-ttu-id="043e4-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="043e4-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
```

### <a name="response"></a><span data-ttu-id="043e4-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="043e4-136">Response</span></span>
<span data-ttu-id="043e4-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="043e4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1637

{
  "value": {
    "@odata.type": "#microsoft.graph.managedDeviceCertificateState",
    "id": "d99bc884-c884-d99b-84c8-9bd984c89bd9",
    "devicePlatform": "androidForWork",
    "certificateKeyUsage": "digitalSignature",
    "certificateValidityPeriodUnits": "months",
    "certificateIssuanceState": "challengeIssued",
    "certificateKeyStorageProvider": "useTpmKspOtherwiseFail",
    "certificateSubjectNameFormat": "commonNameIncludingEmail",
    "certificateSubjectAlternativeNameFormat": "emailAddress",
    "certificateRevokeStatus": "pending",
    "certificateProfileDisplayName": "Certificate Profile Display Name value",
    "deviceDisplayName": "Device Display Name value",
    "userDisplayName": "User Display Name value",
    "certificateExpirationDateTime": "2017-01-01T00:02:14.9489247-08:00",
    "certificateLastIssuanceStateChangedDateTime": "2017-01-01T00:00:27.7468732-08:00",
    "lastCertificateStateChangeDateTime": "2017-01-01T00:01:10.7144639-08:00",
    "certificateIssuer": "Certificate Issuer value",
    "certificateThumbprint": "Certificate Thumbprint value",
    "certificateSerialNumber": "Certificate Serial Number value",
    "certificateKeyLength": 4,
    "certificateEnhancedKeyUsage": "Certificate Enhanced Key Usage value",
    "certificateValidityPeriod": 9,
    "certificateSubjectNameFormatString": "Certificate Subject Name Format String value",
    "certificateSubjectAlternativeNameFormatString": "Certificate Subject Alternative Name Format String value",
    "certificateIssuanceDateTime": "2016-12-31T23:59:41.5044473-08:00",
    "certificateErrorCode": 4
  }
}
```





