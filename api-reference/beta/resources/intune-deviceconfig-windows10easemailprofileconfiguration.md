---
title: Тип ресурса windows10EasEmailProfileConfiguration
description: Предоставляя конфигурации в этом профиле, вы можете указать, что собственный почтовый клиент (Outlook) на устройствах с Windows 10 должен обмениваться данными с сервером Exchange и получать электронную почту, контакты, календарь и задачи. Кроме того, вы также можете указать, какой объем электронной почты необходимо синхронизировать, и как часто устройство должно синхронизироваться.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 25c4e13c52d825cd9afd32997ae6b38f2b18ab44
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944350"
---
# <a name="windows10easemailprofileconfiguration-resource-type"></a>Тип ресурса windows10EasEmailProfileConfiguration

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Предоставляя конфигурации в этом профиле, вы можете указать, что собственный почтовый клиент (Outlook) на устройствах с Windows 10 должен обмениваться данными с сервером Exchange и получать электронную почту, контакты, календарь и задачи. Кроме того, вы также можете указать, какой объем электронной почты необходимо синхронизировать, и как часто устройство должно синхронизироваться.


Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список windows10EasEmailProfileConfigurations](../api/intune-deviceconfig-windows10easemailprofileconfiguration-list.md)|Коллекция [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md)|Список свойств и связей объектов [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) .|
|[Получение windows10EasEmailProfileConfiguration](../api/intune-deviceconfig-windows10easemailprofileconfiguration-get.md)|[windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md)|Чтение свойств и связей объекта [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) .|
|[Создание windows10EasEmailProfileConfiguration](../api/intune-deviceconfig-windows10easemailprofileconfiguration-create.md)|[windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md)|Создание нового объекта [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) .|
|[Удаление windows10EasEmailProfileConfiguration](../api/intune-deviceconfig-windows10easemailprofileconfiguration-delete.md)|Нет|Удаляет объект [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md).|
|[Обновление windows10EasEmailProfileConfiguration](../api/intune-deviceconfig-windows10easemailprofileconfiguration-update.md)|[windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md)|Обновление свойств объекта [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция строк|Список тегов областей для этого экземпляра сущности. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Суппортсскопетагс|Логический|Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области. Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия. Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|Строка|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|usernameSource|[Усеремаилсаурце](../resources/intune-deviceconfig-useremailsource.md)|Атрибут username, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве. Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md). Возможные значения: `userPrincipalName`, `primarySmtpAddress`.|
|Усернамеаадсаурце|[usernameSource](../resources/intune-deviceconfig-usernamesource.md);|Имя поля AAD, которое будет использоваться для извлечения имени пользователя для профиля электронной почты. Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md). Возможные значения: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.|
|Усердомаиннамесаурце|[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md);|Атрибут Усердомаиннаме, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве. Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md). Возможные значения: `fullDomainName`, `netBiosDomainName`.|
|Кустомдомаиннаме|Строка|Значение имени пользовательского домена, используемое при создании профиля электронной почты, перед установкой на устройстве. Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)|
|имя_учетной_записи|Строка|Имя учетной записи.|
|Синккалендар|Логический|Указывает, следует ли синхронизировать календарь.|
|Синкконтактс|Логический|Указывает, следует ли синхронизировать контакты.|
|Синктаскс|Логический|Указывает, следует ли синхронизировать задачи.|
|Дуратионофемаилтосинк|[Емаилсинкдуратион](../resources/intune-deviceconfig-emailsyncduration.md)|Продолжительность синхронизации электронной почты. Возможные `userDefined`значения:, `oneDay`, `threeDays`, `oneWeek` `twoWeeks`,, `oneMonth`,. `unlimited`|
|Емаиладдресссаурце|[Усеремаилсаурце](../resources/intune-deviceconfig-useremailsource.md)|Атрибут электронной почты, выбранный из AAD и добавленный в этот профиль перед установкой на устройстве. Возможные значения: `userPrincipalName`, `primarySmtpAddress`.|
|Емаилсинксчедуле|[Емаилсинксчедуле](../resources/intune-deviceconfig-emailsyncschedule.md)|Расписание синхронизации электронной почты. Возможные значения: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.|
|hostName|String|Расположение Exchange (URL-адрес), к которому подключается собственное почтовое приложение.|
|Рекуирессл|Логический|Указывает, следует ли использовать SSL.|

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

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10EasEmailProfileConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10EasEmailProfileConfiguration",
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
  "usernameSource": "String",
  "usernameAADSource": "String",
  "userDomainNameSource": "String",
  "customDomainName": "String",
  "accountName": "String",
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true,
  "durationOfEmailToSync": "String",
  "emailAddressSource": "String",
  "emailSyncSchedule": "String",
  "hostName": "String",
  "requireSsl": true
}
```




