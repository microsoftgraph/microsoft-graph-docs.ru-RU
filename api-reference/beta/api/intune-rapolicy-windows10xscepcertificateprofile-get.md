---
title: Получить windows10XSCEPCertificateProfile
description: Чтение свойств и связей объекта Windows10XSCEPCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 549e177cd52eecf82a7a437d6f6a2d773f0b65ab664f4347265744764391027e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54136865"
---
# <a name="get-windows10xscepcertificateprofile"></a>Получить windows10XSCEPCertificateProfile

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Чтение свойств и связей [объекта Windows10XSCEPCertificateProfile.](../resources/intune-rapolicy-windows10xscepcertificateprofile.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/resourceAccessProfiles/{deviceManagementResourceAccessProfileBaseId}
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код отклика и `200 OK` [объект Windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
GET https://graph.microsoft.com/beta/deviceManagement/resourceAccessProfiles/{deviceManagementResourceAccessProfileBaseId}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1388

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10XSCEPCertificateProfile",
    "id": "d174d58e-d58e-d174-8ed5-74d18ed574d1",
    "version": 7,
    "displayName": "Display Name value",
    "description": "Description value",
    "creationDateTime": "2017-01-01T00:00:43.1365422-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "certificateStore": "machine",
    "certificateValidityPeriodScale": "months",
    "certificateValidityPeriodValue": 14,
    "extendedKeyUsages": [
      {
        "@odata.type": "microsoft.graph.extendedKeyUsage",
        "name": "Name value",
        "objectIdentifier": "Object Identifier value"
      }
    ],
    "hashAlgorithm": [
      "sha2"
    ],
    "keySize": "size2048",
    "keyStorageProvider": "useTpmKspOtherwiseFail",
    "keyUsage": "digitalSignature",
    "renewalThresholdPercentage": 10,
    "rootCertificateId": "ed919bbc-9bbc-ed91-bc9b-91edbc9b91ed",
    "scepServerUrls": [
      "Scep Server Urls value"
    ],
    "subjectAlternativeNameFormats": [
      {
        "@odata.type": "microsoft.graph.windows10XCustomSubjectAlternativeName",
        "sanType": "emailAddress",
        "name": "Name value"
      }
    ],
    "subjectNameFormatString": "Subject Name Format String value"
  }
}
```




