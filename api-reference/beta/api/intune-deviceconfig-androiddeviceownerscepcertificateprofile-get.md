---
title: Получение Андроиддевицеовнерсцепцертификатепрофиле
description: Чтение свойств и связей объекта Андроиддевицеовнерсцепцертификатепрофиле.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c6b3e382d7ebcf0d76ccc342c0b4f9157e3bba69
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38084968"
---
# <a name="get-androiddeviceownerscepcertificateprofile"></a><span data-ttu-id="38a0f-103">Получение Андроиддевицеовнерсцепцертификатепрофиле</span><span class="sxs-lookup"><span data-stu-id="38a0f-103">Get androidDeviceOwnerScepCertificateProfile</span></span>

> <span data-ttu-id="38a0f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38a0f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="38a0f-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="38a0f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38a0f-106">Чтение свойств и связей объекта [андроиддевицеовнерсцепцертификатепрофиле](../resources/intune-deviceconfig-androiddeviceownerscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="38a0f-106">Read properties and relationships of the [androidDeviceOwnerScepCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="38a0f-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="38a0f-107">Prerequisites</span></span>
<span data-ttu-id="38a0f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38a0f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38a0f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="38a0f-110">Permission type</span></span>|<span data-ttu-id="38a0f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="38a0f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="38a0f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="38a0f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="38a0f-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="38a0f-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="38a0f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="38a0f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38a0f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38a0f-115">Not supported.</span></span>|
|<span data-ttu-id="38a0f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="38a0f-116">Application</span></span>|<span data-ttu-id="38a0f-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="38a0f-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="38a0f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="38a0f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="38a0f-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="38a0f-119">Optional query parameters</span></span>
<span data-ttu-id="38a0f-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="38a0f-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="38a0f-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="38a0f-121">Request headers</span></span>
|<span data-ttu-id="38a0f-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="38a0f-122">Header</span></span>|<span data-ttu-id="38a0f-123">Значение</span><span class="sxs-lookup"><span data-stu-id="38a0f-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="38a0f-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="38a0f-124">Authorization</span></span>|<span data-ttu-id="38a0f-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="38a0f-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="38a0f-126">Accept</span><span class="sxs-lookup"><span data-stu-id="38a0f-126">Accept</span></span>|<span data-ttu-id="38a0f-127">application/json</span><span class="sxs-lookup"><span data-stu-id="38a0f-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="38a0f-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="38a0f-128">Request body</span></span>
<span data-ttu-id="38a0f-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="38a0f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="38a0f-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="38a0f-130">Response</span></span>
<span data-ttu-id="38a0f-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [андроиддевицеовнерсцепцертификатепрофиле](../resources/intune-deviceconfig-androiddeviceownerscepcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="38a0f-131">If successful, this method returns a `200 OK` response code and [androidDeviceOwnerScepCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38a0f-132">Пример</span><span class="sxs-lookup"><span data-stu-id="38a0f-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="38a0f-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="38a0f-133">Request</span></span>
<span data-ttu-id="38a0f-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="38a0f-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="38a0f-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="38a0f-135">Response</span></span>
<span data-ttu-id="38a0f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="38a0f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






