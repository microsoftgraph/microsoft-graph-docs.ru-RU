---
title: тип ресурса androidForWorkNineWorkEasConfiguration
description: Предоставляя конфигурации в этом профиле, вы можете поручить клиенту электронной почты Nine Work на устройствах Android For Work взаимодействовать с сервером Exchange и получать электронную почту, контакты, календарь, задачи и заметки. Кроме того, можно также указать, сколько сообщений электронной почты следует синхронизировать и как часто устройство должно синхронизироваться.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e6c7a9dcb8c3e68fc0384b18f02505a203c50ab9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59106457"
---
# <a name="androidforworknineworkeasconfiguration-resource-type"></a>тип ресурса androidForWorkNineWorkEasConfiguration

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Предоставляя конфигурации в этом профиле, вы можете поручить клиенту электронной почты Nine Work на устройствах Android For Work взаимодействовать с сервером Exchange и получать электронную почту, контакты, календарь, задачи и заметки. Кроме того, можно также указать, сколько сообщений электронной почты следует синхронизировать и как часто устройство должно синхронизироваться.


Наследует [от AndroidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список androidForWorkNineWorkEasConfigurations](../api/intune-deviceconfig-androidforworknineworkeasconfiguration-list.md)|[коллекция androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md)|Список свойств и связей объектов [AndroidForWorkNineWorkEasConfiguration.](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md)|
|[Get AndroidForWorkNineWorkEasConfiguration](../api/intune-deviceconfig-androidforworknineworkeasconfiguration-get.md)|[androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md)|Чтение свойств и связей [объекта AndroidForWorkNineWorkEasConfiguration.](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md)|
|[Создание androidForWorkNineWorkEasConfiguration](../api/intune-deviceconfig-androidforworknineworkeasconfiguration-create.md)|[androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md)|Создайте новый [объект AndroidForWorkNineWorkEasConfiguration.](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md)|
|[Удаление androidForWorkNineWorkEasConfiguration](../api/intune-deviceconfig-androidforworknineworkeasconfiguration-delete.md)|Нет|Удаляет [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md).|
|[Обновление androidForWorkNineWorkEasConfiguration](../api/intune-deviceconfig-androidforworknineworkeasconfiguration-update.md)|[androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md)|Обновите свойства [объекта AndroidForWorkNineWorkEasConfiguration.](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция объектов string|Список тегов области для этого экземпляра Entity. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|supportsScopeTags|Логическое|Указывает, поддерживает ли вся конфигурация устройства назначение тегов области. Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом. Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|Применимость к выпуску ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|Правило применимости версии ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|Правило применимости режима устройства для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|displayName|String|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|authenticationMethod|[easAuthenticationMethod](../resources/intune-deviceconfig-easauthenticationmethod.md)|Метод проверки подлинности для Exchange ActiveSync. Наследуется [от AndroidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md). Возможные значения: `usernameAndPassword`, `certificate`, `derivedCredential`.|
|durationOfEmailToSync|[emailSyncDuration](../resources/intune-deviceconfig-emailsyncduration.md)|Продолжительность времени электронной почты должна быть синхронизирована с. Наследуется [от AndroidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md). Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.|
|emailAddressSource|[userEmailSource](../resources/intune-deviceconfig-useremailsource.md)|Атрибут электронной почты, который выбирается из AAD и вводится в этот профиль перед установкой на устройстве. Наследуется [от AndroidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md). Возможные значения: `userPrincipalName`, `primarySmtpAddress`.|
|hostName|String|Exchange (URL-адрес), к который подключается почтовое приложение. Унаследованный от [AndroidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)|
|requireSsl|Логический|Указывает, следует ли использовать SSL. Унаследованный от [AndroidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)|
|usernameSource|[androidUsernameSource](../resources/intune-deviceconfig-androidusernamesource.md)|Атрибут username, который выбирается из AAD и вводится в этот профиль перед установкой на устройстве. Наследуется [от AndroidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md). Возможные значения: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.|
|syncCalendar|Логическое|Синхронизация календаря. Если установлено ложное, календарь отключается на устройстве.|
|syncContacts|Логическое|Для синхронизации контактов. Если установлено, что на устройстве отключены ложные контакты.|
|syncTasks|Логический|Перегнойные задачи синхронизации. Если установлено, что на устройстве отключены ложные задачи.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|groupAssignments|[коллекция deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|Список назначений групп для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|assignments|Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|Список назначений для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceStatuses|Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Состояние установки конфигурации для каждого устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|userStatuses|Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Состояние установки конфигурации устройства пользователем. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Обзор состояния конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Обзор состояния конфигурации устройств для пользователей. Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceSettingStateSummaries|Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Сводка данных о состоянии настройки конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|identityCertificate|[androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)|Сертификат удостоверения. Унаследованный от [AndroidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidForWorkNineWorkEasConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkNineWorkEasConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "String"
    ],
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "String",
    "maxOSVersion": "String",
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "String",
    "name": "String",
    "ruleType": "String"
  },
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "authenticationMethod": "String",
  "durationOfEmailToSync": "String",
  "emailAddressSource": "String",
  "hostName": "String",
  "requireSsl": true,
  "usernameSource": "String",
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true
}
```



