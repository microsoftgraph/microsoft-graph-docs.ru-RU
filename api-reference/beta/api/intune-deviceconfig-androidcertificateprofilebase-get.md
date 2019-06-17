---
title: Получение Андроидцертификатепрофилебасе
description: Чтение свойств и связей объекта Андроидцертификатепрофилебасе.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6c410c1a08cb40fadf0c5cc95e511a56f1a38940
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34971712"
---
# <a name="get-androidcertificateprofilebase"></a><span data-ttu-id="53c9e-103">Получение Андроидцертификатепрофилебасе</span><span class="sxs-lookup"><span data-stu-id="53c9e-103">Get androidCertificateProfileBase</span></span>

> <span data-ttu-id="53c9e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53c9e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="53c9e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="53c9e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53c9e-106">Чтение свойств и связей объекта [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md) .</span><span class="sxs-lookup"><span data-stu-id="53c9e-106">Read properties and relationships of the [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="53c9e-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="53c9e-107">Prerequisites</span></span>
<span data-ttu-id="53c9e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53c9e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53c9e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="53c9e-110">Permission type</span></span>|<span data-ttu-id="53c9e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="53c9e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53c9e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="53c9e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="53c9e-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="53c9e-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="53c9e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="53c9e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53c9e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53c9e-115">Not supported.</span></span>|
|<span data-ttu-id="53c9e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="53c9e-116">Application</span></span>|<span data-ttu-id="53c9e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53c9e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="53c9e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="53c9e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidVpnConfiguration/identityCertificate
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidEasEmailProfileConfiguration/identityCertificate
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidEasEmailProfileConfiguration/smimeSigningCertificate
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidEnterpriseWiFiConfiguration/identityCertificateForClientAuthentication
```

## <a name="optional-query-parameters"></a><span data-ttu-id="53c9e-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="53c9e-119">Optional query parameters</span></span>
<span data-ttu-id="53c9e-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="53c9e-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="53c9e-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="53c9e-121">Request headers</span></span>
|<span data-ttu-id="53c9e-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="53c9e-122">Header</span></span>|<span data-ttu-id="53c9e-123">Значение</span><span class="sxs-lookup"><span data-stu-id="53c9e-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53c9e-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="53c9e-124">Authorization</span></span>|<span data-ttu-id="53c9e-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="53c9e-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53c9e-126">Accept</span><span class="sxs-lookup"><span data-stu-id="53c9e-126">Accept</span></span>|<span data-ttu-id="53c9e-127">application/json</span><span class="sxs-lookup"><span data-stu-id="53c9e-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53c9e-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="53c9e-128">Request body</span></span>
<span data-ttu-id="53c9e-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="53c9e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="53c9e-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="53c9e-130">Response</span></span>
<span data-ttu-id="53c9e-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="53c9e-131">If successful, this method returns a `200 OK` response code and [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53c9e-132">Пример</span><span class="sxs-lookup"><span data-stu-id="53c9e-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="53c9e-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="53c9e-133">Request</span></span>
<span data-ttu-id="53c9e-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="53c9e-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidVpnConfiguration/identityCertificate
```

### <a name="response"></a><span data-ttu-id="53c9e-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="53c9e-135">Response</span></span>
<span data-ttu-id="53c9e-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="53c9e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1723

{
  "value": {
    "@odata.type": "#microsoft.graph.androidCertificateProfileBase",
    "id": "76cf241d-241d-76cf-1d24-cf761d24cf76",
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
    "subjectAlternativeNameType": "emailAddress",
    "certificateValidityPeriodValue": 14,
    "certificateValidityPeriodScale": "months",
    "extendedKeyUsages": [
      {
        "@odata.type": "microsoft.graph.extendedKeyUsage",
        "name": "Name value",
        "objectIdentifier": "Object Identifier value"
      }
    ]
  }
}
```





