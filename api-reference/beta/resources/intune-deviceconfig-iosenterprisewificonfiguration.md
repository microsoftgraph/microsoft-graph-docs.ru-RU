---
title: Тип ресурса iosEnterpriseWiFiConfiguration
description: Предоставляя конфигурации в этом профиле, вы можете указать устройству iOS подключаться к желаемой конечной точке Wi/Fi. Указав способ проверки подлинности и типы безопасности, ожидаемые конечной точкой Wi/Fi, можно легко установить соединение Wi/Fi для конечного пользователя.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bc9e2a06eaf5a63fc9b3d11db9f7d3cad61ef5b7
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946513"
---
# <a name="iosenterprisewificonfiguration-resource-type"></a>Тип ресурса iosEnterpriseWiFiConfiguration

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Предоставляя конфигурации в этом профиле, вы можете указать устройству iOS подключаться к желаемой конечной точке Wi/Fi. Указав способ проверки подлинности и типы безопасности, ожидаемые конечной точкой Wi/Fi, можно легко установить соединение Wi/Fi для конечного пользователя.


Наследуется от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Иосентерприсевификонфигуратионс](../api/intune-deviceconfig-iosenterprisewificonfiguration-list.md)|Коллекция [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)|Список свойств и связей объектов [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) .|
|[Получение iosEnterpriseWiFiConfiguration](../api/intune-deviceconfig-iosenterprisewificonfiguration-get.md)|[iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)|Чтение свойств и связей объекта [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) .|
|[Создание iosEnterpriseWiFiConfiguration](../api/intune-deviceconfig-iosenterprisewificonfiguration-create.md)|[iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)|Создание нового объекта [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) .|
|[Удаление iosEnterpriseWiFiConfiguration](../api/intune-deviceconfig-iosenterprisewificonfiguration-delete.md)|Нет|Удаляет объект [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md).|
|[Обновление iosEnterpriseWiFiConfiguration](../api/intune-deviceconfig-iosenterprisewificonfiguration-update.md)|[iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)|Обновление свойств объекта [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция строк|Список тегов областей для этого экземпляра сущности. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Суппортсскопетагс|Логический|Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области. Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия. Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|Строка|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Нетворкнаме|Строка|Сетевое имя, унаследованное от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|
|SSID|Строка|Это имя сети Wi-Fi, которая отправляется на все устройства. Наследуется от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|
|Коннектаутоматикалли|Логический|Подключаться автоматически, если сеть находится в диапазоне. Если задать для этого параметра значение true, запрос пользователя будет пропущен и автоматически подключено устройство к сети Wi/Fi. Наследуется от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|
|Коннектвхеннетворкнамеишидден|Логический|Подключаться, если сеть не ведет вещание своего имени (SSID). Если задано значение true, этот профиль заставляет устройство подключаться к сети, на которой не выполняется трансляция идентификатора SSID на все устройства. Наследуется от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|
|Вифисекурититипе|[Вифисекурититипе](../resources/intune-deviceconfig-wifisecuritytype.md)|Указывает, использует ли конечная точка Wi/Fi тип безопасности на основе EAP. Наследуется от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md). Возможные значения: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.|
|proxySettings|[Вифипроксисеттинг](../resources/intune-deviceconfig-wifiproxysetting.md)|Тип прокси-сервера для этого подключения Wi-Fi наследуется от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md). Возможные значения: `none`, `manual`, `automatic`.|
|Проксимануаладдресс|Строка|IP-адрес или DNS-имя узла прокси-сервера при выборе конфигурации вручную. Наследуется от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|
|Проксимануалпорт|Int32|Порт прокси-сервера при выборе конфигурации вручную. Наследуется от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|
|Проксяутоматикконфигуратионурл|Строка|URL-адрес скрипта автоматической настройки прокси-сервера при выборе параметра Автоматическая настройка. Обычно это URL-адрес файла PAC (Автонастройка прокси-сервера). Наследуется от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|
|preSharedKey|Строка|Это предварительно общий ключ для частной сети Wi-Fi WPA. Наследуется от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|
|Еаптипе|[Еаптипе](../resources/intune-deviceconfig-eaptype.md)|Протокол расширенной проверки подлинности (EAP). Указывает тип протокола EAP, установленный для конечной точки Wi-Fi (маршрутизатора). Возможные значения: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.|
|Еапфастконфигуратион|[Еапфастконфигуратион](../resources/intune-deviceconfig-eapfastconfiguration.md)|Параметр конфигурации EAP-FAST, когда EAP-FAST выбран тип EAP. Возможные значения: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.|
|Трустедсерверцертификатенамес|Коллекция строк|Имена сертификатов доверенных серверов, когда тип EAP настроен для EAP-TLS/TTLS/FAST или PEAP. Это общее имя, используемое в сертификатах, выдаваемых доверенным центром сертификации (CA). Если вы предоставляете эти сведения, вы можете обходить диалоговое окно динамического доверия, отображаемое на устройствах конечных пользователей, когда они подключаются к сети Wi-Fi.|
|Параметр authenticationmethod|[Вифиаусентикатионмесод](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|Метод проверки подлинности, когда тип EAP настроен для протокола PEAP или EAP-TTLS. Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`.|
|Свойства innerauthenticationprotocolforeapttls|[Нонеапаусентикатионмесодфореапттлстипе](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|Метод проверки подлинности, отличный от EAP, если тип EAP — EAP-TTLS, а параметр authenticationmethod — имя пользователя и пароль. Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.|
|outerIdentityPrivacyTemporaryValue|Строка|Включите конфиденциальность удостоверений (внешнее удостоверение), если тип EAP настроен для EAP-TTLS, EAP-FAST или PEAP. Это свойство маскирует имена пользователей с введенным текстом. Например, если вы используете анонимный доступ, все пользователи, которые проходят проверку подлинности с помощью этого подключения Wi-Fi, с помощью действительного имени пользователя отображаются как anonymous.|
|Усернамеформатстринг|Строка|Строка формата имени пользователя, используемая для построения имени пользователя для подключения к Wi-Fi|
|Пассвордформатстринг|Строка|Строка формата пароля, используемая для создания пароля подключения к Wi-Fi|

## <a name="relationships"></a>Связи
|Отношение|Тип|Описание|
|:---|:---|:---|
|groupAssignments|Коллекция [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|Список назначений групп для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|assignments|Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|Список назначений для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatuses|Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Состояние установки конфигурации для каждого устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatuses|Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Состояние установки конфигурации устройств пользователем. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Обзор состояния конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Обзор состояния конфигурации устройств для пользователей. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceSettingStateSummaries|Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Сводка данных о состоянии настройки конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Рутцертификатесфорсервервалидатион|Коллекция [иострустедрутцертификате](../resources/intune-deviceconfig-iostrustedrootcertificate.md)|Доверенные корневые сертификаты для проверки сервера, если тип EAP настроен для EAP-TLS/TTLS/FAST или PEAP. Если указать это значение, нет необходимости предоставлять Трустедсерверцертификатенамес и наоборот.|
|Идентитицертификатефорклиентаусентикатион|[Используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md)|Сертификат удостоверения для проверки подлинности клиента, если тип EAP настроен для EAP-TLS, EAP-TTLS (с проверкой подлинности с помощью сертификата) или PEAP (с проверкой подлинности сертификата).|
|Дериведкредентиалсеттингс|[Девицеманажементдериведкредентиалсеттингс](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md)|Параметры уровня клиента для производных учетных данных, которые необходимо использовать для проверки подлинности.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosEnterpriseWiFiConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosEnterpriseWiFiConfiguration",
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
  "proxySettings": "String",
  "proxyManualAddress": "String",
  "proxyManualPort": 1024,
  "proxyAutomaticConfigurationUrl": "String",
  "preSharedKey": "String",
  "eapType": "String",
  "eapFastConfiguration": "String",
  "trustedServerCertificateNames": [
    "String"
  ],
  "authenticationMethod": "String",
  "innerAuthenticationProtocolForEapTtls": "String",
  "outerIdentityPrivacyTemporaryValue": "String",
  "usernameFormatString": "String",
  "passwordFormatString": "String"
}
```




