---
title: Тип ресурса iosEasEmailProfileConfiguration
description: Предоставляя конфигурации в этом профиле, вы можете настроить собственный клиент электронной почты на устройствах iOS для связи с сервером Exchange и получать электронную почту, контакты, календарь, напоминания и заметки. Кроме того, вы также можете указать, какой объем электронной почты необходимо синхронизировать, и как часто устройство должно синхронизироваться.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c1aaade5665d86c7498f01d9db361a4b9847cb98
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538947"
---
# <a name="ioseasemailprofileconfiguration-resource-type"></a>Тип ресурса iosEasEmailProfileConfiguration

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Предоставляя конфигурации в этом профиле, вы можете настроить собственный клиент электронной почты на устройствах iOS для связи с сервером Exchange и получать электронную почту, контакты, календарь, напоминания и заметки. Кроме того, вы также можете указать, какой объем электронной почты необходимо синхронизировать, и как часто устройство должно синхронизироваться.


Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Иосеасемаилпрофилеконфигуратионс](../api/intune-deviceconfig-ioseasemailprofileconfiguration-list.md)|Коллекция [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)|Список свойств и связей объектов [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) .|
|[Получение iosEasEmailProfileConfiguration](../api/intune-deviceconfig-ioseasemailprofileconfiguration-get.md)|[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)|Чтение свойств и связей объекта [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) .|
|[Создание iosEasEmailProfileConfiguration](../api/intune-deviceconfig-ioseasemailprofileconfiguration-create.md)|[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)|Создание нового объекта [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) .|
|[Удаление iosEasEmailProfileConfiguration](../api/intune-deviceconfig-ioseasemailprofileconfiguration-delete.md)|Нет|Удаляет объект [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md).|
|[Обновление iosEasEmailProfileConfiguration](../api/intune-deviceconfig-ioseasemailprofileconfiguration-update.md)|[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)|Обновление свойств объекта [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция String|Список тегов областей для этого экземпляра сущности. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|суппортсскопетагс|Логический|Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области. Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия. Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|Применимость выпусков ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|Правило применимости версии ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|Правило применимости режима устройства для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|displayName|Строка|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|usernameSource|[усеремаилсаурце](../resources/intune-deviceconfig-useremailsource.md)|Атрибут username, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве. Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md). Возможные значения: `userPrincipalName`, `primarySmtpAddress`.|
|усернамеаадсаурце|[usernameSource](../resources/intune-deviceconfig-usernamesource.md);|Имя поля AAD, которое будет использоваться для извлечения имени пользователя для профиля электронной почты. Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md). Возможные значения: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.|
|усердомаиннамесаурце|[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md);|Атрибут Усердомаиннаме, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве. Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md). Возможные значения: `fullDomainName`, `netBiosDomainName`.|
|кустомдомаиннаме|String|Значение имени пользовательского домена, используемое при создании профиля электронной почты, перед установкой на устройстве. Наследуется от [еасемаилпрофилеконфигуратионбасе](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)|
|имя_учетной_записи|String|Имя учетной записи.|
|Параметр authenticationmethod|[еасаусентикатионмесод](../resources/intune-deviceconfig-easauthenticationmethod.md)|Способ проверки подлинности для этого профиля электронной почты. Возможные значения: `usernameAndPassword`, `certificate`, `derivedCredential`.|
|блоккмовингмессажестусеремаилаккаунтс|Логический|Указывает, следует ли запретить перемещение сообщений в другие учетные записи электронной почты.|
|блокксендинжемаилфромсирдпартяппс|Логический|Указывает, следует ли запретить отправку сообщений электронной почты от сторонних приложений.|
|блокксинЦингрецентлюседемаиладдрессес|Логический|Указывает, следует ли заблокировать синхронизацию недавно использовавшихся адресов электронной почты (например, при создании нового сообщения электронной почты).|
|дуратионофемаилтосинк|[емаилсинкдуратион](../resources/intune-deviceconfig-emailsyncduration.md)|Длительность времени, в течение которого будет синхронизироваться электронная почта. . Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.|
|емаиладдресссаурце|[усеремаилсаурце](../resources/intune-deviceconfig-useremailsource.md)|Атрибут электронной почты, выбранный из AAD и добавленный в этот профиль перед установкой на устройстве. Возможные значения: `userPrincipalName`, `primarySmtpAddress`.|
|hostName|String|Расположение Exchange (URL-адрес), к которому подключается собственное почтовое приложение.|
|рекуиресмиме|Логический|Указывает, следует ли использовать сертификат S/MIME.|
|смиминаблепермессажесвитч|Логический|Указывает, следует ли разрешить незашифрованные сообщения электронной почты.|
|смиминкриптбидефаултенаблед|Логический|Если задано значение true, то по умолчанию включено шифрование S/MIME.|
|смимесигнинженаблед|Логический|Если для этой учетной записи задано значение true, то подписывание MIME включено.|
|смимесигнингусероверридинаблед|Логический|Если задано значение true, пользователь может включать и отключать подписывание S/MIME.|
|смиминкриптбидефаултусероверридинаблед|Логический|Если задано значение true, пользователь может переключить шифрование по умолчанию.|
|смимесигнингцертификатеусероверридинаблед|Логический|Если задано значение true, пользователь может выбрать удостоверение подписи.|
|смиминкриптионцертификатеусероверридинаблед|Логический|Если задано значение true, пользователь может выбрать удостоверение шифрования S/MIME. |
|рекуирессл|Логический|Указывает, следует ли использовать SSL.|
|усеоаус|Логический|Указывает, должно ли подключение использовать OAuth для проверки подлинности.|
|сигнингцертификатетипе|[emailCertificateType](../resources/intune-deviceconfig-emailcertificatetype.md)|Тип сертификата подписи для этого профиля электронной почты. Возможные значения: `none`, `certificate`, `derivedCredential`.|
|енкриптионцертификатетипе|[emailCertificateType](../resources/intune-deviceconfig-emailcertificatetype.md)|Тип сертификата шифрования для этого профиля электронной почты. Возможные значения: `none`, `certificate`, `derivedCredential`.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|groupAssignments|Коллекция [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|Список назначений групп для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|assignments|Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|Список назначений для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceStatuses|Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Состояние установки конфигурации для каждого устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|userStatuses|Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Состояние установки конфигурации устройств пользователем. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Обзор состояния конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Обзор состояния конфигурации устройств для пользователей. Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceSettingStateSummaries|Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Сводка данных о состоянии настройки конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|Identitycertificate (|[Используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md)|Сертификат удостоверения.|
|смимесигнингцертификате|[iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md);|Сертификат подписи S/MIME.|
|смиминкриптионцертификате|[iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md);|Сертификат шифрования S/MIME.|
|дериведкредентиалсеттингс|[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)|Параметры уровня клиента для производных учетных данных, которые необходимо использовать для проверки подлинности.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosEasEmailProfileConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosEasEmailProfileConfiguration",
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
  "usernameSource": "String",
  "usernameAADSource": "String",
  "userDomainNameSource": "String",
  "customDomainName": "String",
  "accountName": "String",
  "authenticationMethod": "String",
  "blockMovingMessagesToOtherEmailAccounts": true,
  "blockSendingEmailFromThirdPartyApps": true,
  "blockSyncingRecentlyUsedEmailAddresses": true,
  "durationOfEmailToSync": "String",
  "emailAddressSource": "String",
  "hostName": "String",
  "requireSmime": true,
  "smimeEnablePerMessageSwitch": true,
  "smimeEncryptByDefaultEnabled": true,
  "smimeSigningEnabled": true,
  "smimeSigningUserOverrideEnabled": true,
  "smimeEncryptByDefaultUserOverrideEnabled": true,
  "smimeSigningCertificateUserOverrideEnabled": true,
  "smimeEncryptionCertificateUserOverrideEnabled": true,
  "requireSsl": true,
  "useOAuth": true,
  "signingCertificateType": "String",
  "encryptionCertificateType": "String"
}
```



