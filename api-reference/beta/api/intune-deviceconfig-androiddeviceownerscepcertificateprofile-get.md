---
title: Получение Андроиддевицеовнерсцепцертификатепрофиле
description: Чтение свойств и связей объекта Андроиддевицеовнерсцепцертификатепрофиле.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c0c65b9b8a3b68d0d7edf79781ae8bfa6982d71d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43350675"
---
# <a name="get-androiddeviceownerscepcertificateprofile"></a><span data-ttu-id="5b4bd-103">Получение Андроиддевицеовнерсцепцертификатепрофиле</span><span class="sxs-lookup"><span data-stu-id="5b4bd-103">Get androidDeviceOwnerScepCertificateProfile</span></span>

<span data-ttu-id="5b4bd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b4bd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5b4bd-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b4bd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5b4bd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5b4bd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b4bd-107">Чтение свойств и связей объекта [андроиддевицеовнерсцепцертификатепрофиле](../resources/intune-deviceconfig-androiddeviceownerscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="5b4bd-107">Read properties and relationships of the [androidDeviceOwnerScepCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5b4bd-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5b4bd-108">Prerequisites</span></span>
<span data-ttu-id="5b4bd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b4bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b4bd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5b4bd-111">Permission type</span></span>|<span data-ttu-id="5b4bd-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5b4bd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b4bd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5b4bd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5b4bd-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b4bd-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5b4bd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5b4bd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b4bd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b4bd-116">Not supported.</span></span>|
|<span data-ttu-id="5b4bd-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="5b4bd-117">Application</span></span>|<span data-ttu-id="5b4bd-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b4bd-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b4bd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5b4bd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5b4bd-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5b4bd-120">Optional query parameters</span></span>
<span data-ttu-id="5b4bd-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5b4bd-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5b4bd-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5b4bd-122">Request headers</span></span>
|<span data-ttu-id="5b4bd-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5b4bd-123">Header</span></span>|<span data-ttu-id="5b4bd-124">Значение</span><span class="sxs-lookup"><span data-stu-id="5b4bd-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b4bd-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b4bd-125">Authorization</span></span>|<span data-ttu-id="5b4bd-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5b4bd-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b4bd-127">Accept</span><span class="sxs-lookup"><span data-stu-id="5b4bd-127">Accept</span></span>|<span data-ttu-id="5b4bd-128">application/json</span><span class="sxs-lookup"><span data-stu-id="5b4bd-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b4bd-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5b4bd-129">Request body</span></span>
<span data-ttu-id="5b4bd-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5b4bd-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b4bd-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="5b4bd-131">Response</span></span>
<span data-ttu-id="5b4bd-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [андроиддевицеовнерсцепцертификатепрофиле](../resources/intune-deviceconfig-androiddeviceownerscepcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5b4bd-132">If successful, this method returns a `200 OK` response code and [androidDeviceOwnerScepCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b4bd-133">Пример</span><span class="sxs-lookup"><span data-stu-id="5b4bd-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="5b4bd-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="5b4bd-134">Request</span></span>
<span data-ttu-id="5b4bd-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5b4bd-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="5b4bd-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b4bd-136">Response</span></span>
<span data-ttu-id="5b4bd-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5b4bd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2293

{
  "value": {
    "@odata.type": "#microsoft.graph.androidDeviceOwnerScepCertificateProfile",
    "id": "7d8b9c9a-9c9a-7d8b-9a9c-8b7d9a9c8b7d",
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
    "subjectNameFormat": "commonNameIncludingEmail",
    "certificateValidityPeriodValue": 14,
    "certificateValidityPeriodScale": "months",
    "extendedKeyUsages": [
      {
        "@odata.type": "microsoft.graph.extendedKeyUsage",
        "name": "Name value",
        "objectIdentifier": "Object Identifier value"
      }
    ],
    "subjectAlternativeNameType": "emailAddress",
    "scepServerUrls": [
      "Scep Server Urls value"
    ],
    "subjectNameFormatString": "Subject Name Format String value",
    "keyUsage": "digitalSignature",
    "keySize": "size2048",
    "hashAlgorithm": "sha2",
    "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
    "certificateStore": "machine",
    "customSubjectAlternativeNames": [
      {
        "@odata.type": "microsoft.graph.customSubjectAlternativeName",
        "sanType": "emailAddress",
        "name": "Name value"
      }
    ]
  }
}
```



