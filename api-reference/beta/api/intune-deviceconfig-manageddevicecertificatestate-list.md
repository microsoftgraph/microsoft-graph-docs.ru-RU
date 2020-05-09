---
title: Список Manageddevicecertificatestates к объекту
description: Список свойств и связей объектов Манажеддевицецертификатестате.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e30b0450f9bbf3893d9d38cba3f97483e8221087
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44179125"
---
# <a name="list-manageddevicecertificatestates"></a><span data-ttu-id="458e6-103">Список Manageddevicecertificatestates к объекту</span><span class="sxs-lookup"><span data-stu-id="458e6-103">List managedDeviceCertificateStates</span></span>

<span data-ttu-id="458e6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="458e6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="458e6-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="458e6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="458e6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="458e6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="458e6-107">Список свойств и связей объектов [манажеддевицецертификатестате](../resources/intune-deviceconfig-manageddevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="458e6-107">List properties and relationships of the [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="458e6-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="458e6-108">Prerequisites</span></span>
<span data-ttu-id="458e6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="458e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="458e6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="458e6-111">Permission type</span></span>|<span data-ttu-id="458e6-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="458e6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="458e6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="458e6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="458e6-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="458e6-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="458e6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="458e6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="458e6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="458e6-116">Not supported.</span></span>|
|<span data-ttu-id="458e6-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="458e6-117">Application</span></span>|<span data-ttu-id="458e6-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="458e6-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="458e6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="458e6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidPkcsCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidScepCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosImportedPFXCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidImportedPFXCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerScepCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkImportedPFXCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerImportedPFXCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkPkcsCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkScepCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidWorkProfilePkcsCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidWorkProfileScepCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/microsoft.graph.macOSPkcsCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/microsoft.graph.macOSScepCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/microsoft.graph.macOSImportedPFXCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10PkcsCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10ImportedPFXCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windowsPhone81ImportedPFXCertificateProfile/managedDeviceCertificateStates
```

## <a name="request-headers"></a><span data-ttu-id="458e6-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="458e6-120">Request headers</span></span>
|<span data-ttu-id="458e6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="458e6-121">Header</span></span>|<span data-ttu-id="458e6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="458e6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="458e6-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="458e6-123">Authorization</span></span>|<span data-ttu-id="458e6-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="458e6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="458e6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="458e6-125">Accept</span></span>|<span data-ttu-id="458e6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="458e6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="458e6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="458e6-127">Request body</span></span>
<span data-ttu-id="458e6-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="458e6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="458e6-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="458e6-129">Response</span></span>
<span data-ttu-id="458e6-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [манажеддевицецертификатестате](../resources/intune-deviceconfig-manageddevicecertificatestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="458e6-130">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="458e6-131">Пример</span><span class="sxs-lookup"><span data-stu-id="458e6-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="458e6-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="458e6-132">Request</span></span>
<span data-ttu-id="458e6-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="458e6-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates
```

### <a name="response"></a><span data-ttu-id="458e6-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="458e6-134">Response</span></span>
<span data-ttu-id="458e6-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="458e6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1703

{
  "value": [
    {
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
  ]
}
```



