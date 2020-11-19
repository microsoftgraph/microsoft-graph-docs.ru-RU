---
title: Получение Андроидворкпрофилецертификатепрофилебасе
description: Чтение свойств и связей объекта Андроидворкпрофилецертификатепрофилебасе.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7d91e4c7d774b2c3661943f14bc19db9b6acc763
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49221444"
---
# <a name="get-androidworkprofilecertificateprofilebase"></a><span data-ttu-id="0eb76-103">Получение Андроидворкпрофилецертификатепрофилебасе</span><span class="sxs-lookup"><span data-stu-id="0eb76-103">Get androidWorkProfileCertificateProfileBase</span></span>

<span data-ttu-id="0eb76-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0eb76-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0eb76-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0eb76-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0eb76-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0eb76-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0eb76-107">Чтение свойств и связей объекта [андроидворкпрофилецертификатепрофилебасе](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md) .</span><span class="sxs-lookup"><span data-stu-id="0eb76-107">Read properties and relationships of the [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0eb76-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0eb76-108">Prerequisites</span></span>
<span data-ttu-id="0eb76-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0eb76-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0eb76-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0eb76-111">Permission type</span></span>|<span data-ttu-id="0eb76-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0eb76-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0eb76-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0eb76-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0eb76-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0eb76-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="0eb76-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0eb76-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0eb76-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0eb76-116">Not supported.</span></span>|
|<span data-ttu-id="0eb76-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="0eb76-117">Application</span></span>|<span data-ttu-id="0eb76-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0eb76-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0eb76-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0eb76-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfileVpnConfiguration/identityCertificate
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfileEasEmailProfileBase/identityCertificate
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfileEnterpriseWiFiConfiguration/identityCertificateForClientAuthentication
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0eb76-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0eb76-120">Optional query parameters</span></span>
<span data-ttu-id="0eb76-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0eb76-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0eb76-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0eb76-122">Request headers</span></span>
|<span data-ttu-id="0eb76-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0eb76-123">Header</span></span>|<span data-ttu-id="0eb76-124">Значение</span><span class="sxs-lookup"><span data-stu-id="0eb76-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0eb76-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0eb76-125">Authorization</span></span>|<span data-ttu-id="0eb76-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0eb76-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0eb76-127">Accept</span><span class="sxs-lookup"><span data-stu-id="0eb76-127">Accept</span></span>|<span data-ttu-id="0eb76-128">application/json</span><span class="sxs-lookup"><span data-stu-id="0eb76-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0eb76-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0eb76-129">Request body</span></span>
<span data-ttu-id="0eb76-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0eb76-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0eb76-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="0eb76-131">Response</span></span>
<span data-ttu-id="0eb76-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [андроидворкпрофилецертификатепрофилебасе](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0eb76-132">If successful, this method returns a `200 OK` response code and [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0eb76-133">Пример</span><span class="sxs-lookup"><span data-stu-id="0eb76-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="0eb76-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="0eb76-134">Request</span></span>
<span data-ttu-id="0eb76-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0eb76-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate
```

### <a name="response"></a><span data-ttu-id="0eb76-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="0eb76-136">Response</span></span>
<span data-ttu-id="0eb76-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0eb76-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1734

{
  "value": {
    "@odata.type": "#microsoft.graph.androidWorkProfileCertificateProfileBase",
    "id": "4a559c8b-9c8b-4a55-8b9c-554a8b9c554a",
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
    "subjectAlternativeNameType": "emailAddress"
  }
}
```




