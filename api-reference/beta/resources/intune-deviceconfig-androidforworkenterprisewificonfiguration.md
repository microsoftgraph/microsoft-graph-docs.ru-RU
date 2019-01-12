---
title: Тип ресурса androidForWorkEnterpriseWiFiConfiguration
description: С указанием конфигураций в этом профиле можно указать Android для работы устройства, чтобы подключиться к конечной точке желаемую Wi-Fi. Путем указания типов безопасности и метод проверки подлинности ожидаемого Wi-Fi конечной точкой подключения Wi-Fi можно сделать полностью для конечных пользователей.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9b43e2dd024a22ea1157be7a357be85d5eab1453
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932814"
---
# <a name="androidforworkenterprisewificonfiguration-resource-type"></a>Тип ресурса androidForWorkEnterpriseWiFiConfiguration

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

С указанием конфигураций в этом профиле можно указать Android для работы устройства, чтобы подключиться к конечной точке желаемую Wi-Fi. Путем указания типов безопасности и метод проверки подлинности ожидаемого Wi-Fi конечной точкой подключения Wi-Fi можно сделать полностью для конечных пользователей.

Наследуется от [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список androidForWorkEnterpriseWiFiConfigurations](../api/intune-deviceconfig-androidforworkenterprisewificonfiguration-list.md)|[androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) коллекции|Свойства списка и связей объектов [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) .|
|[Получение androidForWorkEnterpriseWiFiConfiguration](../api/intune-deviceconfig-androidforworkenterprisewificonfiguration-get.md)|[androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md)|Чтение свойства и связи объекта [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) .|
|[Создание androidForWorkEnterpriseWiFiConfiguration](../api/intune-deviceconfig-androidforworkenterprisewificonfiguration-create.md)|[androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md)|Создание нового объекта [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) .|
|[Удаление androidForWorkEnterpriseWiFiConfiguration](../api/intune-deviceconfig-androidforworkenterprisewificonfiguration-delete.md)|Нет|Удаляет [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md).|
|[Обновление androidForWorkEnterpriseWiFiConfiguration](../api/intune-deviceconfig-androidforworkenterprisewificonfiguration-update.md)|[androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md)|Обновление свойства объекта [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция String|Список областей теги для данного экземпляра сущности. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|supportsScopeTags|Boolean|Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия. Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью. Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure. Это свойство доступно только для чтения. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|описание|String|Указанное администратором описание конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|String|Указанное администратором имя конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|networkName|String|Сеть имя наследуется от [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)|
|SSID|String|Это имя в сети Wi-Fi, который передается на все устройства. Наследуется от [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)|
|connectAutomatically|Boolean|Автоматическое подключение, сети, если она в диапазоне. Установка значения true пропустите строке пользователя и автоматически подключаться к сети Wi-Fi устройства. Наследуется от [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)|
|connectWhenNetworkNameIsHidden|Boolean|Когда установлено значение true, этот профиль принудительно устройства для подключения к сети, в которой не передает свое имя SSID для всех устройств. Наследуется от [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)|
|wiFiSecurityType|[androidWiFiSecurityType](../resources/intune-deviceconfig-androidwifisecuritytype.md)|Указывает, используется ли конечная точка Wi-Fi тип безопасности на основе внешних Приложений. Наследуется от [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md). Возможные значения: `open`, `wpaEnterprise`.|
|eapType|[androidEapType](../resources/intune-deviceconfig-androideaptype.md)|Указывает тип протокола EAP на конечной точке Wi-Fi (маршрутизатор). Возможные значения: `eapTls`, `eapTtls`, `peap`.|
|authenticationMethod|[wiFiAuthenticationMethod](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|Указывает метод проверки подлинности клиента (устройств) необходимо использовать при настройке типа EAP PEAP или EAP-TTLS. Возможные значения: `certificate`, `usernameAndPassword`.|
|innerAuthenticationProtocolForEapTtls|[nonEapAuthenticationMethodForEapTtlsType](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|Метод EAP без проверки подлинности (внутреннее удостоверение) при тип EAP — EAP-TTLS и Authenticationmethod — это имя пользователя и пароль. Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.|
|innerAuthenticationProtocolForPeap|[nonEapAuthenticationMethodForPeap](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|Метод EAP без проверки подлинности (внутренний идентификатор) при PEAP — это тип EAP и Authenticationmethod — это имя пользователя и пароль. Возможные значения: `none`, `microsoftChapVersionTwo`.|
|outerIdentityPrivacyTemporaryValue|String|Включите удостоверение конфиденциальности (учетную запись), если тип EAP настроено для EAP-TTLS или PEAP. Строка, представленные здесь используется для скрытие имя пользователя для отдельных пользователей, когда пользователь пытается подключиться к сети Wi-Fi.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) коллекции|Список назначений групп для профиля конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|assignments|Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|Список назначений для профиля конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatuses|Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Состояние установки конфигурации для каждого устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatuses|Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Состояние установки конфигурации устройства пользователем. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Обзор состояния конфигурации по устройствам. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Обзор состояния конфигурации устройств по пользователям. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceSettingStateSummaries|Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Обзор состояния параметров конфигурации устройств по пользователям. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|rootCertificateForServerValidation|[androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md)|Надежные корневой сертификат для проверки сервера, если тип EAP настроено для EAP-TLS, EAP-TTLS или PEAP. Это сертификат, предоставленный в конечную точку Wi-Fi при попытке подключиться к конечной точке Wi-Fi устройства. Устройство (или пользователь), необходимо принять этот сертификат для продолжения попытки подключения.|
|identityCertificateForClientAuthentication|[androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)|Сертификат удостоверения для проверки подлинности клиентов, если тип EAP настроено для EAP-TLS, EAP-TTLS (с проверкой подлинности сертификата) или PEAP (с проверкой подлинности сертификата). Это сертификат клиента к конечной точке Wi-Fi. Сервер проверки подлинности, расположенным за конечной точки Wi-Fi должен принимать этот сертификат, чтобы успешно установить соединение Wi-Fi.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidForWorkEnterpriseWiFiConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkEnterpriseWiFiConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "networkName": "String",
  "ssid": "String",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "String",
  "eapType": "String",
  "authenticationMethod": "String",
  "innerAuthenticationProtocolForEapTtls": "String",
  "innerAuthenticationProtocolForPeap": "String",
  "outerIdentityPrivacyTemporaryValue": "String"
}
```





