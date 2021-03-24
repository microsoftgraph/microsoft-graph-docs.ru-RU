---
title: Список windows81SCEPCertificateProfiles
description: Список свойств и связей объектов Windows81SCEPCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 94c71aaf2dda4fb535c56b8847b685d41dc2f451
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51147282"
---
# <a name="list-windows81scepcertificateprofiles"></a><span data-ttu-id="51074-103">Список windows81SCEPCertificateProfiles</span><span class="sxs-lookup"><span data-stu-id="51074-103">List windows81SCEPCertificateProfiles</span></span>

<span data-ttu-id="51074-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51074-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="51074-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51074-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="51074-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="51074-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51074-107">Список свойств и связей объектов [Windows81SCEPCertificateProfile.](../resources/intune-deviceconfig-windows81scepcertificateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="51074-107">List properties and relationships of the [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="51074-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="51074-108">Prerequisites</span></span>
<span data-ttu-id="51074-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51074-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51074-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51074-111">Permission type</span></span>|<span data-ttu-id="51074-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="51074-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51074-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51074-113">Delegated (work or school account)</span></span>|<span data-ttu-id="51074-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51074-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="51074-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51074-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51074-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51074-116">Not supported.</span></span>|
|<span data-ttu-id="51074-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="51074-117">Application</span></span>|<span data-ttu-id="51074-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51074-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="51074-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51074-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="51074-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="51074-120">Request headers</span></span>
|<span data-ttu-id="51074-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="51074-121">Header</span></span>|<span data-ttu-id="51074-122">Значение</span><span class="sxs-lookup"><span data-stu-id="51074-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51074-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="51074-123">Authorization</span></span>|<span data-ttu-id="51074-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="51074-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51074-125">Accept</span><span class="sxs-lookup"><span data-stu-id="51074-125">Accept</span></span>|<span data-ttu-id="51074-126">application/json</span><span class="sxs-lookup"><span data-stu-id="51074-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51074-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="51074-127">Request body</span></span>
<span data-ttu-id="51074-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="51074-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51074-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="51074-129">Response</span></span>
<span data-ttu-id="51074-130">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [Windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="51074-130">If successful, this method returns a `200 OK` response code and a collection of [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51074-131">Пример</span><span class="sxs-lookup"><span data-stu-id="51074-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="51074-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="51074-132">Request</span></span>
<span data-ttu-id="51074-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51074-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="51074-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="51074-134">Response</span></span>
<span data-ttu-id="51074-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="51074-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2473

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows81SCEPCertificateProfile",
      "id": "2daf8af2-8af2-2daf-f28a-af2df28aaf2d",
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
      "renewalThresholdPercentage": 10,
      "keyStorageProvider": "useTpmKspOtherwiseFail",
      "subjectNameFormat": "commonNameIncludingEmail",
      "subjectAlternativeNameType": "emailAddress",
      "certificateValidityPeriodValue": 14,
      "certificateValidityPeriodScale": "months",
      "extendedKeyUsages": [
        {
          "@odata.type": "microsoft.graph.extendedKeyUsage",
          "name": "Name value",
          "objectIdentifier": "Object Identifier value"
        }
      ],
      "customSubjectAlternativeNames": [
        {
          "@odata.type": "microsoft.graph.customSubjectAlternativeName",
          "sanType": "emailAddress",
          "name": "Name value"
        }
      ],
      "scepServerUrls": [
        "Scep Server Urls value"
      ],
      "subjectNameFormatString": "Subject Name Format String value",
      "keyUsage": "digitalSignature",
      "keySize": "size2048",
      "hashAlgorithm": "sha2",
      "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
      "certificateStore": "machine"
    }
  ]
}
```




