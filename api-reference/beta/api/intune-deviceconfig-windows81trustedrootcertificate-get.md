---
title: Получение windows81TrustedRootCertificate
description: Чтение свойств и связей объекта windows81TrustedRootCertificate.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ccf67e057486c4574756d6e51b19e3f2f7d65d3d
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37187053"
---
# <a name="get-windows81trustedrootcertificate"></a><span data-ttu-id="b1d13-103">Получение windows81TrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="b1d13-103">Get windows81TrustedRootCertificate</span></span>

> <span data-ttu-id="b1d13-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1d13-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1d13-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b1d13-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1d13-106">Чтение свойств и связей объекта [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="b1d13-106">Read properties and relationships of the [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b1d13-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b1d13-107">Prerequisites</span></span>
<span data-ttu-id="b1d13-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1d13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1d13-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b1d13-110">Permission type</span></span>|<span data-ttu-id="b1d13-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b1d13-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1d13-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b1d13-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b1d13-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b1d13-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b1d13-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b1d13-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1d13-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1d13-115">Not supported.</span></span>|
|<span data-ttu-id="b1d13-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b1d13-116">Application</span></span>|<span data-ttu-id="b1d13-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b1d13-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1d13-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b1d13-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/rootCertificate
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b1d13-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b1d13-119">Optional query parameters</span></span>
<span data-ttu-id="b1d13-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b1d13-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b1d13-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b1d13-121">Request headers</span></span>
|<span data-ttu-id="b1d13-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b1d13-122">Header</span></span>|<span data-ttu-id="b1d13-123">Значение</span><span class="sxs-lookup"><span data-stu-id="b1d13-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1d13-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b1d13-124">Authorization</span></span>|<span data-ttu-id="b1d13-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b1d13-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1d13-126">Accept</span><span class="sxs-lookup"><span data-stu-id="b1d13-126">Accept</span></span>|<span data-ttu-id="b1d13-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b1d13-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1d13-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b1d13-128">Request body</span></span>
<span data-ttu-id="b1d13-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b1d13-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b1d13-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="b1d13-130">Response</span></span>
<span data-ttu-id="b1d13-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b1d13-131">If successful, this method returns a `200 OK` response code and [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1d13-132">Пример</span><span class="sxs-lookup"><span data-stu-id="b1d13-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="b1d13-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b1d13-133">Request</span></span>
<span data-ttu-id="b1d13-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b1d13-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}
```

### <a name="response"></a><span data-ttu-id="b1d13-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1d13-135">Response</span></span>
<span data-ttu-id="b1d13-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b1d13-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1459

{
  "value": {
    "@odata.type": "#microsoft.graph.windows81TrustedRootCertificate",
    "id": "3fb588f9-88f9-3fb5-f988-b53ff988b53f",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "deviceManagementApplicabilityRuleOsEdition": {
      "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
      "osEditionTypes": [
        "windows10EnterpriseN"
      ],
      "name": "Name value",
      "ruleType": "exclude"
    },
    "deviceManagementApplicabilityRuleOsVersion": {
      "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
      "minOSVersion": "Min OSVersion value",
      "maxOSVersion": "Max OSVersion value",
      "name": "Name value",
      "ruleType": "exclude"
    },
    "deviceManagementApplicabilityRuleDeviceMode": {
      "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
      "deviceMode": "sModeConfiguration",
      "name": "Name value",
      "ruleType": "exclude"
    },
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
    "certFileName": "Cert File Name value",
    "destinationStore": "computerCertStoreIntermediate"
  }
}
```




