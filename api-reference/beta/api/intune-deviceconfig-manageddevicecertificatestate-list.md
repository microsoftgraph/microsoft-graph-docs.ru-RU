---
title: Список managedDeviceCertificateStates
description: Свойства списка и связей объектов managedDeviceCertificateState.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 06081ffaf357a338a23b279462066270c9d0a6a8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411640"
---
# <a name="list-manageddevicecertificatestates"></a><span data-ttu-id="bb170-103">Список managedDeviceCertificateStates</span><span class="sxs-lookup"><span data-stu-id="bb170-103">List managedDeviceCertificateStates</span></span>

> <span data-ttu-id="bb170-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bb170-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bb170-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb170-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bb170-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bb170-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb170-107">Свойства списка и связей объектов [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="bb170-107">List properties and relationships of the [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bb170-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="bb170-108">Prerequisites</span></span>
<span data-ttu-id="bb170-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="bb170-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bb170-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bb170-111">Permission type</span></span>|<span data-ttu-id="bb170-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bb170-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb170-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bb170-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bb170-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="bb170-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="bb170-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bb170-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb170-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb170-116">Not supported.</span></span>|
|<span data-ttu-id="bb170-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bb170-117">Application</span></span>|<span data-ttu-id="bb170-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb170-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb170-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bb170-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidPkcsCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidScepCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosImportedPFXCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSImportedPFXCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidImportedPFXCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfileScepCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkImportedPFXCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkPkcsCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkScepCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10PkcsCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10ImportedPFXCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windowsPhone81ImportedPFXCertificateProfile/managedDeviceCertificateStates
```

## <a name="request-headers"></a><span data-ttu-id="bb170-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bb170-120">Request headers</span></span>
|<span data-ttu-id="bb170-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bb170-121">Header</span></span>|<span data-ttu-id="bb170-122">Значение</span><span class="sxs-lookup"><span data-stu-id="bb170-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb170-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb170-123">Authorization</span></span>|<span data-ttu-id="bb170-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="bb170-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bb170-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bb170-125">Accept</span></span>|<span data-ttu-id="bb170-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bb170-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb170-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bb170-127">Request body</span></span>
<span data-ttu-id="bb170-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bb170-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb170-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb170-129">Response</span></span>
<span data-ttu-id="bb170-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="bb170-130">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb170-131">Пример</span><span class="sxs-lookup"><span data-stu-id="bb170-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="bb170-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="bb170-132">Request</span></span>
<span data-ttu-id="bb170-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bb170-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates
```

### <a name="response"></a><span data-ttu-id="bb170-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb170-134">Response</span></span>
<span data-ttu-id="bb170-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="bb170-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




