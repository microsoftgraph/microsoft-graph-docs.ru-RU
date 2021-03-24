---
title: Список iosEduDeviceConfigurations
description: Список свойств и связей объектов iosEduDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9c40cb4b105115e4f5cad6aae2f876f0583c36ed
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51129889"
---
# <a name="list-iosedudeviceconfigurations"></a>Список iosEduDeviceConfigurations

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Список свойств и связей объектов [iosEduDeviceConfiguration.](../resources/intune-deviceconfig-iosedudeviceconfiguration.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированное (рабочая или учебная учетная запись)|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All|
|Делегированное (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) в теле ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
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




