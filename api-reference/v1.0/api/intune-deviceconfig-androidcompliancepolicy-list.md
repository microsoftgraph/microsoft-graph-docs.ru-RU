---
title: Перечисление объектов androidCompliancePolicy
description: Список свойств и связей объектов androidCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 73c88749d683bb582328ee522cfb1832bce3f557
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48083773"
---
# <a name="list-androidcompliancepolicies"></a>Перечисление объектов androidCompliancePolicy

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Список свойств и связей объектов [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).

## <a name="prerequisites"></a>Предварительные условия
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик
При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1476

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidCompliancePolicy",
      "id": "752c820f-820f-752c-0f82-2c750f822c75",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7,
      "passwordRequired": true,
      "passwordMinimumLength": 5,
      "passwordRequiredType": "alphabetic",
      "passwordMinutesOfInactivityBeforeLock": 5,
      "passwordExpirationDays": 6,
      "passwordPreviousPasswordBlockCount": 2,
      "securityPreventInstallAppsFromUnknownSources": true,
      "securityDisableUsbDebugging": true,
      "securityRequireVerifyApps": true,
      "deviceThreatProtectionEnabled": true,
      "deviceThreatProtectionRequiredSecurityLevel": "secured",
      "securityBlockJailbrokenDevices": true,
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value",
      "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
      "storageRequireEncryption": true,
      "securityRequireSafetyNetAttestationBasicIntegrity": true,
      "securityRequireSafetyNetAttestationCertifiedDevice": true,
      "securityRequireGooglePlayServices": true,
      "securityRequireUpToDateSecurityProviders": true,
      "securityRequireCompanyPortalAppIntegrity": true
    }
  ]
}
```









