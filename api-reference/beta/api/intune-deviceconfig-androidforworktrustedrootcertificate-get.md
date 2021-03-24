---
title: Get androidForWorkTrustedRootCertificate
description: Чтение свойств и связей объекта AndroidForWorkTrustedRootCertificate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ffc518199413effed3ab981c4c4e0baccfd899d3
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51138269"
---
# <a name="get-androidforworktrustedrootcertificate"></a><span data-ttu-id="e8a36-103">Get androidForWorkTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="e8a36-103">Get androidForWorkTrustedRootCertificate</span></span>

<span data-ttu-id="e8a36-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8a36-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e8a36-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8a36-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8a36-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e8a36-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8a36-107">Чтение свойств и связей [объекта AndroidForWorkTrustedRootCertificate.](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md)</span><span class="sxs-lookup"><span data-stu-id="e8a36-107">Read properties and relationships of the [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e8a36-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e8a36-108">Prerequisites</span></span>
<span data-ttu-id="e8a36-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8a36-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8a36-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e8a36-111">Permission type</span></span>|<span data-ttu-id="e8a36-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e8a36-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8a36-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e8a36-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e8a36-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8a36-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e8a36-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e8a36-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8a36-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8a36-116">Not supported.</span></span>|
|<span data-ttu-id="e8a36-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="e8a36-117">Application</span></span>|<span data-ttu-id="e8a36-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8a36-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8a36-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e8a36-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkEnterpriseWiFiConfiguration/rootCertificateForServerValidation
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e8a36-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e8a36-120">Optional query parameters</span></span>
<span data-ttu-id="e8a36-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e8a36-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e8a36-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e8a36-122">Request headers</span></span>
|<span data-ttu-id="e8a36-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e8a36-123">Header</span></span>|<span data-ttu-id="e8a36-124">Значение</span><span class="sxs-lookup"><span data-stu-id="e8a36-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8a36-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8a36-125">Authorization</span></span>|<span data-ttu-id="e8a36-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e8a36-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e8a36-127">Accept</span><span class="sxs-lookup"><span data-stu-id="e8a36-127">Accept</span></span>|<span data-ttu-id="e8a36-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e8a36-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8a36-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e8a36-129">Request body</span></span>
<span data-ttu-id="e8a36-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e8a36-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8a36-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8a36-131">Response</span></span>
<span data-ttu-id="e8a36-132">В случае успеха этот метод возвращает код отклика и `200 OK` [объект AndroidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e8a36-132">If successful, this method returns a `200 OK` response code and [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8a36-133">Пример</span><span class="sxs-lookup"><span data-stu-id="e8a36-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="e8a36-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8a36-134">Request</span></span>
<span data-ttu-id="e8a36-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e8a36-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate
```

### <a name="response"></a><span data-ttu-id="e8a36-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8a36-136">Response</span></span>
<span data-ttu-id="e8a36-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e8a36-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1406

{
  "value": {
    "@odata.type": "#microsoft.graph.androidForWorkTrustedRootCertificate",
    "id": "2f78834c-834c-2f78-4c83-782f4c83782f",
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
    "certFileName": "Cert File Name value"
  }
}
```




