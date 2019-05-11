---
title: Тип ресурса Андроидеасемаилпрофилеконфигуратион
description: Предоставляя конфигурации в этом профиле, вы можете настроить собственный клиент электронной почты на устройствах KNOX для связи с сервером Exchange и получать электронную почту, контакты, календарь, задачи и заметки. Кроме того, вы также можете указать, какой объем электронной почты необходимо синхронизировать, и как часто устройство должно синхронизироваться.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1fe7905b2c69792e41ebf90fa7578609921a933e
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949033"
---
# <a name="androideasemailprofileconfiguration-resource-type"></a>Тип ресурса Андроидеасемаилпрофилеконфигуратион

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Предоставляя конфигурации в этом профиле, вы можете настроить собственный клиент электронной почты на устройствах KNOX для связи с сервером Exchange и получать электронную почту, контакты, календарь, задачи и заметки. Кроме того, вы также можете указать, какой объем электронной почты необходимо синхронизировать, и как часто устройство должно синхронизироваться.


Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Андроидеасемаилпрофилеконфигуратионс](../api/intune-deviceconfig-androideasemailprofileconfiguration-list.md)|Коллекция [андроидеасемаилпрофилеконфигуратион](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md)|Список свойств и связей объектов [андроидеасемаилпрофилеконфигуратион](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) .|
|[Получение Андроидеасемаилпрофилеконфигуратион](../api/intune-deviceconfig-androideasemailprofileconfiguration-get.md)|[Андроидеасемаилпрофилеконфигуратион](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md)|Чтение свойств и связей объекта [андроидеасемаилпрофилеконфигуратион](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) .|
|[Создание Андроидеасемаилпрофилеконфигуратион](../api/intune-deviceconfig-androideasemailprofileconfiguration-create.md)|[Андроидеасемаилпрофилеконфигуратион](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md)|Создание нового объекта [андроидеасемаилпрофилеконфигуратион](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) .|
|[Удаление Андроидеасемаилпрофилеконфигуратион](../api/intune-deviceconfig-androideasemailprofileconfiguration-delete.md)|Нет|Удаляет объект [андроидеасемаилпрофилеконфигуратион](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md).|
|[Обновление Андроидеасемаилпрофилеконфигуратион](../api/intune-deviceconfig-androideasemailprofileconfiguration-update.md)|[Андроидеасемаилпрофилеконфигуратион](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md)|Обновление свойств объекта [андроидеасемаилпрофилеконфигуратион](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) .|

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
|имя_учетной_записи|Строка|Имя учетной записи Exchange ActiveSync, отображаемое пользователям как имя профиля EAS (этот).|
|Параметр authenticationmethod|[Еасаусентикатионмесод](../resources/intune-deviceconfig-easauthenticationmethod.md)|Способ проверки подлинности для Exchange ActiveSync. Возможные значения: `usernameAndPassword`, `certificate`, `derivedCredential`.|
|Синккалендар|Логический|Включает и выключает синхронизацию календаря. Если для этого устройства задано значение false, календарь отключен.|
|Синкконтактс|Логический|Включает и выключает синхронизацию контактов. Если задано значение false, контакты на устройстве отключены.|
|Синктаскс|Логический|Включает и выключает синхронизацию задач. Если задано значение false, задачи на устройстве отключены.|
|Синкнотес|Логический|Включает и выключает синхронизацию заметок. Если задано значение false, примечания отключаются на устройстве.|
|Дуратионофемаилтосинк|[Емаилсинкдуратион](../resources/intune-deviceconfig-emailsyncduration.md)|Продолжительность синхронизации электронной почты. Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.|
|Емаиладдресссаурце|[Усеремаилсаурце](../resources/intune-deviceconfig-useremailsource.md)|Атрибут электронной почты, выбранный из AAD и добавленный в этот профиль перед установкой на устройстве. Возможные значения: `userPrincipalName`, `primarySmtpAddress`.|
|Емаилсинксчедуле|[Емаилсинксчедуле](../resources/intune-deviceconfig-emailsyncschedule.md)|Расписание синхронизации электронной почты. Возможные значения: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.|
|hostName|String|Расположение Exchange (URL-адрес), к которому подключается исходное почтовое приложение.|
|Рекуиресмиме|Логический|Указывает, следует ли использовать сертификат S/MIME.|
|Рекуирессл|Логический|Указывает, следует ли использовать SSL.|
|usernameSource|[Андроидусернамесаурце](../resources/intune-deviceconfig-androidusernamesource.md)|Атрибут username, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве. Возможные значения: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.|
|Усердомаиннамесаурце|[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md);|Атрибут Усердомаиннаме, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве. Возможные значения: `fullDomainName`, `netBiosDomainName`.|
|Кустомдомаиннаме|Строка|Значение имени пользовательского домена, используемое при создании профиля электронной почты, перед установкой на устройстве.|

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
|Identitycertificate (|[Андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md)|Сертификат удостоверения.|
|Смимесигнингцертификате|[Андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md)|Сертификат подписи S/MIME.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidEasEmailProfileConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidEasEmailProfileConfiguration",
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
  "accountName": "String",
  "authenticationMethod": "String",
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true,
  "syncNotes": true,
  "durationOfEmailToSync": "String",
  "emailAddressSource": "String",
  "emailSyncSchedule": "String",
  "hostName": "String",
  "requireSmime": true,
  "requireSsl": true,
  "usernameSource": "String",
  "userDomainNameSource": "String",
  "customDomainName": "String"
}
```




