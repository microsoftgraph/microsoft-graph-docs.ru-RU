---
title: Список Андроиддевицеовнерсцепцертификатепрофилес
description: Список свойств и связей объектов Андроиддевицеовнерсцепцертификатепрофиле.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 96337844542dbc4dc23d9fcd89c8904ea5a64abb
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37534780"
---
# <a name="list-androiddeviceownerscepcertificateprofiles"></a><span data-ttu-id="9bc0d-103">Список Андроиддевицеовнерсцепцертификатепрофилес</span><span class="sxs-lookup"><span data-stu-id="9bc0d-103">List androidDeviceOwnerScepCertificateProfiles</span></span>

> <span data-ttu-id="9bc0d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9bc0d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9bc0d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9bc0d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9bc0d-106">Список свойств и связей объектов [андроиддевицеовнерсцепцертификатепрофиле](../resources/intune-deviceconfig-androiddeviceownerscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="9bc0d-106">List properties and relationships of the [androidDeviceOwnerScepCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerscepcertificateprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9bc0d-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9bc0d-107">Prerequisites</span></span>
<span data-ttu-id="9bc0d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9bc0d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9bc0d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9bc0d-110">Permission type</span></span>|<span data-ttu-id="9bc0d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9bc0d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9bc0d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9bc0d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9bc0d-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9bc0d-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9bc0d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9bc0d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9bc0d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9bc0d-115">Not supported.</span></span>|
|<span data-ttu-id="9bc0d-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="9bc0d-116">Application</span></span>|<span data-ttu-id="9bc0d-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9bc0d-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9bc0d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9bc0d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9bc0d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9bc0d-119">Request headers</span></span>
|<span data-ttu-id="9bc0d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9bc0d-120">Header</span></span>|<span data-ttu-id="9bc0d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9bc0d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9bc0d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9bc0d-122">Authorization</span></span>|<span data-ttu-id="9bc0d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9bc0d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9bc0d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9bc0d-124">Accept</span></span>|<span data-ttu-id="9bc0d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9bc0d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9bc0d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9bc0d-126">Request body</span></span>
<span data-ttu-id="9bc0d-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9bc0d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9bc0d-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="9bc0d-128">Response</span></span>
<span data-ttu-id="9bc0d-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [андроиддевицеовнерсцепцертификатепрофиле](../resources/intune-deviceconfig-androiddeviceownerscepcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9bc0d-129">If successful, this method returns a `200 OK` response code and a collection of [androidDeviceOwnerScepCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerscepcertificateprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9bc0d-130">Пример</span><span class="sxs-lookup"><span data-stu-id="9bc0d-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="9bc0d-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="9bc0d-131">Request</span></span>
<span data-ttu-id="9bc0d-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9bc0d-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="9bc0d-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="9bc0d-133">Response</span></span>
<span data-ttu-id="9bc0d-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9bc0d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2427

{
  "value": [
    {
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
  ]
}
```






