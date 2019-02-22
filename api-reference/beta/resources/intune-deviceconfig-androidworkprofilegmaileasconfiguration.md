---
title: Тип ресурса Андроидворкпрофилегмаилеасконфигуратион
description: Предоставляя конфигурации в этом профиле, вы можете указать клиенту электронной почты Gmail на устройствах рабочих профилей Android возможность обмениваться данными с сервером Exchange и получать электронную почту, контакты, календарь, задачи и заметки. Кроме того, вы также можете указать, какой объем электронной почты необходимо синхронизировать, и как часто устройство должно синхронизироваться.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fed1059d1ad8b64c091ee02d4e26737d30030052
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30152649"
---
# <a name="androidworkprofilegmaileasconfiguration-resource-type"></a>Тип ресурса Андроидворкпрофилегмаилеасконфигуратион

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Предоставляя конфигурации в этом профиле, вы можете указать клиенту электронной почты Gmail на устройствах рабочих профилей Android возможность обмениваться данными с сервером Exchange и получать электронную почту, контакты, календарь, задачи и заметки. Кроме того, вы также можете указать, какой объем электронной почты необходимо синхронизировать, и как часто устройство должно синхронизироваться.


НаСледуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Андроидворкпрофилегмаилеасконфигуратионс](../api/intune-deviceconfig-androidworkprofilegmaileasconfiguration-list.md)|Коллекция [андроидворкпрофилегмаилеасконфигуратион](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md)|Список свойств и связей объектов [андроидворкпрофилегмаилеасконфигуратион](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) .|
|[Получение Андроидворкпрофилегмаилеасконфигуратион](../api/intune-deviceconfig-androidworkprofilegmaileasconfiguration-get.md)|[androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md)|Чтение свойств и связей объекта [андроидворкпрофилегмаилеасконфигуратион](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) .|
|[Создание Андроидворкпрофилегмаилеасконфигуратион](../api/intune-deviceconfig-androidworkprofilegmaileasconfiguration-create.md)|[androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md)|Создание нового объекта [андроидворкпрофилегмаилеасконфигуратион](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) .|
|[Удаление Андроидворкпрофилегмаилеасконфигуратион](../api/intune-deviceconfig-androidworkprofilegmaileasconfiguration-delete.md)|Нет|Удаляет объект [андроидворкпрофилегмаилеасконфигуратион](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md).|
|[Обновление Андроидворкпрофилегмаилеасконфигуратион](../api/intune-deviceconfig-androidworkprofilegmaileasconfiguration-update.md)|[androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md)|Обновление свойств объекта [андроидворкпрофилегмаилеасконфигуратион](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция строк|Список тегов областей для этого экземпляра сущности. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Суппортсскопетагс|Логический|Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области. Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия. Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure. Это свойство доступно только для чтения. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|String|Указанное администратором имя конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Параметр authenticationmethod|[Еасаусентикатионмесод](../resources/intune-deviceconfig-easauthenticationmethod.md)|Способ проверки поДлинности для Exchange ActiveSync. НаСледуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md). Возможные значения: `usernameAndPassword`, `certificate`.|
|Дуратионофемаилтосинк|[Емаилсинкдуратион](../resources/intune-deviceconfig-emailsyncduration.md)|Продолжительность синхронизации электронной почты. НаСледуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md). Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.|
|Емаиладдресссаурце|[Усеремаилсаурце](../resources/intune-deviceconfig-useremailsource.md)|Атрибут электронной почты, выбранный из AAD и добавленный в этот профиль перед установкой на устройстве. НаСледуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md). Возможные значения: `userPrincipalName`, `primarySmtpAddress`.|
|hostName|String|Расположение Exchange (URL-адрес), к которому подключается почтовое приложение. НаСледуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)|
|Рекуирессл|Логический|Указывает, следует ли использовать SSL. НаСледуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)|
|usernameSource;|[Андроидусернамесаурце](../resources/intune-deviceconfig-androidusernamesource.md)|Атрибут username, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве. НаСледуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md). Возможные значения: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|groupAssignments|Коллекция [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|Список назначений групп для профиля конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|assignments|Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|Список назначений для профиля конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatuses|Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Состояние установки конфигурации для каждого устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatuses|Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Состояние установки конфигурации устройств пользователем. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Обзор состояния конфигурации по устройствам. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Обзор состояния конфигурации устройств по пользователям. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceSettingStateSummaries|Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Обзор состояния параметров конфигурации устройств по пользователям. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|Identitycertificate (|[androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)|Сертификат удостоверения. НаСледуется от [андроидворкпрофилиасемаилпрофилебасе](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidWorkProfileGmailEasConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidWorkProfileGmailEasConfiguration",
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
  "authenticationMethod": "String",
  "durationOfEmailToSync": "String",
  "emailAddressSource": "String",
  "hostName": "String",
  "requireSsl": true,
  "usernameSource": "String"
}
```




