---
title: Тип ресурса Иоскербероссинглесигнонекстенсион
description: Представляет профиль расширения единого входа Kerberos для устройств с iOS.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: dcc8b8eecbee0794699736929c68bb4b28de0bed
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955542"
---
# <a name="ioskerberossinglesignonextension-resource-type"></a>Тип ресурса Иоскербероссинглесигнонекстенсион

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет профиль расширения единого входа Kerberos для устройств с iOS.


Наследуется от [кербероссинглесигнонекстенсион](../resources/intune-deviceconfig-kerberossinglesignonextension.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|область|Строка|Получает или задает имя области для этого профиля, заданное с учетом регистра. Наследуется от [кербероссинглесигнонекстенсион](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|домена|Коллекция строк|Получает или задает список имен узлов или доменов, для которых расширение приложения выполняет единый вход. Наследуется от [кербероссинглесигнонекстенсион](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|блоккаутоматиклогин|Boolean|Включает или отключает использование цепочки ключей. Наследуется от [кербероссинглесигнонекстенсион](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|каченаме|Строка|Получает или задает универсальное имя службы безопасности для кэша Kerberos, который будет использоваться для этого профиля. Наследуется от [кербероссинглесигнонекстенсион](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|кредентиалбундлеидакцессконтроллист|Коллекция строк|Получает или задает список идентификаторов пакетов приложений, которым разрешен доступ к билету предоставления билетов Kerberos. Наследуется от [кербероссинглесигнонекстенсион](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|домаинреалмс|Коллекция строк|Получает или задает список сфер для сопоставления пользовательских областей доменов. В сфере учитывается регистр. Наследуется от [кербероссинглесигнонекстенсион](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|исдефаултреалм|Boolean|Если задано значение true, область этого профиля будет выбрана по умолчанию. Необходимо, если настроено несколько профилей типа Kerberos. Наследуется от [кербероссинглесигнонекстенсион](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|пассвордблоккмодификатион|Boolean|Включает или отключает смену паролей. Наследуется от [кербероссинглесигнонекстенсион](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|passwordExpirationDays|Int32|Переопределяет срок действия пароля по умолчанию (в днях). Для большинства доменов это значение вычисляется автоматически. Наследуется от [кербероссинглесигнонекстенсион](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|пассвордекспиратионнотификатиондайс|Int32|Получает или задает количество дней до тех пор, пока пользователь не будет уведомлен о сроке действия пароля (значение по умолчанию — 15). Наследуется от [кербероссинглесигнонекстенсион](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|userPrincipalName|String|Получает или задает имя участника, которое будет использоваться для этого профиля. Имя области не обязательно должно быть включено. Наследуется от [кербероссинглесигнонекстенсион](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|пассвордрекуиреактиведиректорикомплексити|Boolean|Разрешает или запрещает, должны ли пароли отвечать требованиям сложности Active Directory. Наследуется от [кербероссинглесигнонекстенсион](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|passwordPreviousPasswordBlockCount|Int32|Получает или задает количество предыдущих паролей, которые необходимо заблокировать. Наследуется от [кербероссинглесигнонекстенсион](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|passwordMinimumLength|Int32|Получает или задает минимальную длину пароля. Наследуется от [кербероссинглесигнонекстенсион](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|пассвордминимумажедайс|Int32|Получает или задает минимальное количество дней, пока пользователь не сможет сменить пароль еще раз. Наследуется от [кербероссинглесигнонекстенсион](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|пассвордрекуирементсдескриптион|Строка|Получает или задает описание требований к сложности пароля. Наследуется от [кербероссинглесигнонекстенсион](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|рекуиреусерпресенце|Boolean|Получает или задает значение, указывающее, требуется ли проверка подлинности с помощью идентификатора сенсорного экрана, идентификатора лица или секретного кода для доступа к записи цепочки ключей. Наследуется от [кербероссинглесигнонекстенсион](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|активедиректориситекоде|Строка|Получает или задает сайт Active Directory. Наследуется от [кербероссинглесигнонекстенсион](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|пассворденаблелокалсинк|Boolean|Включает или отключает синхронизацию паролей. Это не повлияет на пользователей, выполнивших вход в систему с помощью учетной записи мобильного устройства в macOS. Наследуется от [кербероссинглесигнонекстенсион](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|блоккактиведиректориситеаутодисковери|Boolean|Включает или отключает, может ли расширение Kerberos автоматически определять имя своего сайта. Наследуется от [кербероссинглесигнонекстенсион](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|пассвордчанжеурл|Строка|Получает или задает URL-адрес, на который будет отправляться пользователь при инициации смены пароля. Наследуется от [кербероссинглесигнонекстенсион](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosKerberosSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosKerberosSingleSignOnExtension",
  "realm": "String",
  "domains": [
    "String"
  ],
  "blockAutomaticLogin": true,
  "cacheName": "String",
  "credentialBundleIdAccessControlList": [
    "String"
  ],
  "domainRealms": [
    "String"
  ],
  "isDefaultRealm": true,
  "passwordBlockModification": true,
  "passwordExpirationDays": 1024,
  "passwordExpirationNotificationDays": 1024,
  "userPrincipalName": "String",
  "passwordRequireActiveDirectoryComplexity": true,
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinimumAgeDays": 1024,
  "passwordRequirementsDescription": "String",
  "requireUserPresence": true,
  "activeDirectorySiteCode": "String",
  "passwordEnableLocalSync": true,
  "blockActiveDirectorySiteAutoDiscovery": true,
  "passwordChangeUrl": "String"
}
```



