---
title: Обновление androidForWorkEnterpriseWiFiConfiguration
description: Обновление свойств объекта androidForWorkEnterpriseWiFiConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a55e16ce4d42ed7fed62945ca6896748066b8066
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39928947"
---
# <a name="update-androidforworkenterprisewificonfiguration"></a>Обновление androidForWorkEnterpriseWiFiConfiguration

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Тело запроса
В тексте запроса добавьте представление объекта [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) в формате JSON.

В следующей таблице приведены свойства, необходимые при создании [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция строк|Список тегов областей для этого экземпляра сущности. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|суппортсскопетагс|Boolean|Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области. Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия. Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|Применимость выпусков ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|Правило применимости версии ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|Правило применимости режима устройства для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|displayName|Строка|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|нетворкнаме|Строка|Сетевое имя, унаследованное от [андроидфорворквификонфигуратион](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)|
|SSID|Строка|Это имя сети Wi-Fi, которая отправляется на все устройства. Наследуется от [андроидфорворквификонфигуратион](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)|
|коннектаутоматикалли|Boolean|Подключаться автоматически, если сеть находится в диапазоне. Если задать для этого параметра значение true, запрос пользователя будет пропущен и автоматически подключено устройство к сети Wi/Fi. Наследуется от [андроидфорворквификонфигуратион](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)|
|коннектвхеннетворкнамеишидден|Boolean|Если задано значение true, этот профиль заставляет устройство подключаться к сети, на которой не выполняется трансляция идентификатора SSID на все устройства. Наследуется от [андроидфорворквификонфигуратион](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)|
|вифисекурититипе|[андроидвифисекурититипе](../resources/intune-deviceconfig-androidwifisecuritytype.md)|Указывает, использует ли конечная точка Wi/Fi тип безопасности на основе EAP. Наследуется от [андроидфорворквификонфигуратион](../resources/intune-deviceconfig-androidforworkwificonfiguration.md). Возможные значения: `open`, `wpaEnterprise`, `wpa2Enterprise`.|
|еаптипе|[андроидеаптипе](../resources/intune-deviceconfig-androideaptype.md)|Указывает тип протокола EAP, установленный для конечной точки Wi-Fi (маршрутизатора). Возможные значения: `eapTls`, `eapTtls`, `peap`.|
|Параметр authenticationmethod|[вифиаусентикатионмесод](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|Указывает метод проверки подлинности, который должен использоваться клиентом (устройством), если тип EAP настроен для протокола PEAP или EAP-TTLS. Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`.|
|Свойства innerauthenticationprotocolforeapttls|[нонеапаусентикатионмесодфореапттлстипе](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|Метод проверки подлинности (внутреннее удостоверение), не относящийся к EAP, если тип EAP — EAP-TTLS, а параметр authenticationmethod — имя пользователя и пароль. Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.|
|innerAuthenticationProtocolForPeap|[nonEapAuthenticationMethodForPeap](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|Метод проверки подлинности, отличный от EAP (внутреннее удостоверение), если тип EAP — PEAP, а параметр authenticationmethod — имя пользователя и пароль. Возможные значения: `none`, `microsoftChapVersionTwo`.|
|outerIdentityPrivacyTemporaryValue|Строка|Включите конфиденциальность удостоверений (внешнее удостоверение), если тип EAP настроен для EAP-TTLS или PEAP. Приведенная здесь строка используется для маскирования имени пользователя отдельных пользователей при попытке подключения к сети Wi-Fi.|



## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1545

{
  "@odata.type": "#microsoft.graph.androidForWorkEnterpriseWiFiConfiguration",
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
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "networkName": "Network Name value",
  "ssid": "Ssid value",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "wpaEnterprise",
  "eapType": "eapTtls",
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "innerAuthenticationProtocolForPeap": "microsoftChapVersionTwo",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1717

{
  "@odata.type": "#microsoft.graph.androidForWorkEnterpriseWiFiConfiguration",
  "id": "742d953a-953a-742d-3a95-2d743a952d74",
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
  "networkName": "Network Name value",
  "ssid": "Ssid value",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "wpaEnterprise",
  "eapType": "eapTtls",
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "innerAuthenticationProtocolForPeap": "microsoftChapVersionTwo",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```





