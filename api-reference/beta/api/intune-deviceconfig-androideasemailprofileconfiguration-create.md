---
title: Создание Андроидеасемаилпрофилеконфигуратион
description: Создание нового объекта Андроидеасемаилпрофилеконфигуратион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e91b5d7442f9e76a27ad34057d8d2b494b10d6ad
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148463"
---
# <a name="create-androideasemailprofileconfiguration"></a>Создание Андроидеасемаилпрофилеконфигуратион

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание нового объекта [андроидеасемаилпрофилеконфигуратион](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Авторизация|Требуется Bearer &lt;маркер&gt;
|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта Андроидеасемаилпрофилеконфигуратион в формате JSON.

В следующей таблице приведены свойства, необходимые при создании Андроидеасемаилпрофилеконфигуратион.

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
|имя_учетной_записи|String|Имя учетной записи Exchange ActiveSync, отображаемое пользователям как имя профиля EAS (этот).|
|Параметр authenticationmethod|[Еасаусентикатионмесод](../resources/intune-deviceconfig-easauthenticationmethod.md)|Способ проверки поДлинности для Exchange ActiveSync. Возможные значения: `usernameAndPassword`, `certificate`.|
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
|usernameSource;|[Андроидусернамесаурце](../resources/intune-deviceconfig-androidusernamesource.md)|Атрибут username, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве. Возможные значения: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.|
|Усердомаиннамесаурце|[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md);|Атрибут Усердомаиннаме, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве. Возможные значения: `fullDomainName`, `netBiosDomainName`.|
|Кустомдомаиннаме|String|Значение имени пользовательского домена, используемое при создании профиля электронной почты, перед установкой на устройстве.|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроидеасемаилпрофилеконфигуратион](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 793

{
  "@odata.type": "#microsoft.graph.androidEasEmailProfileConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountName": "Account Name value",
  "authenticationMethod": "certificate",
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true,
  "syncNotes": true,
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "emailSyncSchedule": "asMessagesArrive",
  "hostName": "Host Name value",
  "requireSmime": true,
  "requireSsl": true,
  "usernameSource": "userPrincipalName",
  "userDomainNameSource": "netBiosDomainName",
  "customDomainName": "Custom Domain Name value"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 965

{
  "@odata.type": "#microsoft.graph.androidEasEmailProfileConfiguration",
  "id": "ee5e5610-5610-ee5e-1056-5eee10565eee",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountName": "Account Name value",
  "authenticationMethod": "certificate",
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true,
  "syncNotes": true,
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "emailSyncSchedule": "asMessagesArrive",
  "hostName": "Host Name value",
  "requireSmime": true,
  "requireSsl": true,
  "usernameSource": "userPrincipalName",
  "userDomainNameSource": "netBiosDomainName",
  "customDomainName": "Custom Domain Name value"
}
```




