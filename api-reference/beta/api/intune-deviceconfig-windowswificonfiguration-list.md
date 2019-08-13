---
title: Список Виндовсвификонфигуратионс
description: Список свойств и связей объектов Виндовсвификонфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2640ea1cbc683c2751c6e5713afe51bedbf411c9
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36344093"
---
# <a name="list-windowswificonfigurations"></a>Список Виндовсвификонфигуратионс

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Список свойств и связей объектов [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Тело запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a>Отклик
Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1944

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsWifiConfiguration",
      "id": "8a9e790f-790f-8a9e-0f79-9e8a0f799e8a",
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
      "preSharedKey": "Pre Shared Key value",
      "wifiSecurityType": "wpaPersonal",
      "meteredConnectionLimit": "fixed",
      "ssid": "Ssid value",
      "networkName": "Network Name value",
      "connectAutomatically": true,
      "connectToPreferredNetwork": true,
      "connectWhenNetworkNameIsHidden": true,
      "proxySetting": "manual",
      "proxyManualAddress": "Proxy Manual Address value",
      "proxyManualPort": 15,
      "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
      "forceFIPSCompliance": true
    }
  ]
}
```






