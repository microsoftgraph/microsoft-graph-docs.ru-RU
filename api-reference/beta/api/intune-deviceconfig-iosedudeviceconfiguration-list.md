---
title: Список Иоседудевицеконфигуратионс
description: Список свойств и связей объектов Иоседудевицеконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5af1d18f61cfcb37afbd3144e27a1b7528d9bdf7
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39948944"
---
# <a name="list-iosedudeviceconfigurations"></a><span data-ttu-id="3faef-103">Список Иоседудевицеконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="3faef-103">List iosEduDeviceConfigurations</span></span>

> <span data-ttu-id="3faef-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3faef-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3faef-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3faef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3faef-106">Список свойств и связей объектов [иоседудевицеконфигуратион](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="3faef-106">List properties and relationships of the [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3faef-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3faef-107">Prerequisites</span></span>
<span data-ttu-id="3faef-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3faef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3faef-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3faef-110">Permission type</span></span>|<span data-ttu-id="3faef-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3faef-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3faef-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3faef-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3faef-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3faef-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="3faef-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3faef-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3faef-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3faef-115">Not supported.</span></span>|
|<span data-ttu-id="3faef-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3faef-116">Application</span></span>|<span data-ttu-id="3faef-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3faef-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3faef-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3faef-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3faef-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3faef-119">Request headers</span></span>
|<span data-ttu-id="3faef-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3faef-120">Header</span></span>|<span data-ttu-id="3faef-121">Значение</span><span class="sxs-lookup"><span data-stu-id="3faef-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3faef-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3faef-122">Authorization</span></span>|<span data-ttu-id="3faef-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3faef-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3faef-124">Accept</span><span class="sxs-lookup"><span data-stu-id="3faef-124">Accept</span></span>|<span data-ttu-id="3faef-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3faef-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3faef-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3faef-126">Request body</span></span>
<span data-ttu-id="3faef-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3faef-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3faef-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="3faef-128">Response</span></span>
<span data-ttu-id="3faef-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [иоседудевицеконфигуратион](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3faef-129">If successful, this method returns a `200 OK` response code and a collection of [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3faef-130">Пример</span><span class="sxs-lookup"><span data-stu-id="3faef-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="3faef-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="3faef-131">Request</span></span>
<span data-ttu-id="3faef-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3faef-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="3faef-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="3faef-133">Response</span></span>
<span data-ttu-id="3faef-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3faef-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3148

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosEduDeviceConfiguration",
      "id": "4c5df9b6-f9b6-4c5d-b6f9-5d4cb6f95d4c",
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
      "teacherCertificateSettings": {
        "@odata.type": "microsoft.graph.iosEduCertificateSettings",
        "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
        "certFileName": "Cert File Name value",
        "certificationAuthority": "Certification Authority value",
        "certificationAuthorityName": "Certification Authority Name value",
        "certificateTemplateName": "Certificate Template Name value",
        "renewalThresholdPercentage": 10,
        "certificateValidityPeriodValue": 14,
        "certificateValidityPeriodScale": "months"
      },
      "studentCertificateSettings": {
        "@odata.type": "microsoft.graph.iosEduCertificateSettings",
        "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
        "certFileName": "Cert File Name value",
        "certificationAuthority": "Certification Authority value",
        "certificationAuthorityName": "Certification Authority Name value",
        "certificateTemplateName": "Certificate Template Name value",
        "renewalThresholdPercentage": 10,
        "certificateValidityPeriodValue": 14,
        "certificateValidityPeriodScale": "months"
      },
      "deviceCertificateSettings": {
        "@odata.type": "microsoft.graph.iosEduCertificateSettings",
        "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
        "certFileName": "Cert File Name value",
        "certificationAuthority": "Certification Authority value",
        "certificationAuthorityName": "Certification Authority Name value",
        "certificateTemplateName": "Certificate Template Name value",
        "renewalThresholdPercentage": 10,
        "certificateValidityPeriodValue": 14,
        "certificateValidityPeriodScale": "months"
      }
    }
  ]
}
```





