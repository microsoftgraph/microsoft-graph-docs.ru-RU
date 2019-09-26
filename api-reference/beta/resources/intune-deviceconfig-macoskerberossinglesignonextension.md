---
title: Тип ресурса Макоскербероссинглесигнонекстенсион
description: Представляет профиль расширения единого входа Kerberos для устройств MacOS.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0e3ffa045508c878d95ee0b7e274de69b64297aa
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37201301"
---
# <a name="macoskerberossinglesignonextension-resource-type"></a>Тип ресурса Макоскербероссинглесигнонекстенсион

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет профиль расширения единого входа Kerberos для устройств MacOS.


Наследуется от [кербероссинглесигнонекстенсион](../resources/intune-deviceconfig-kerberossinglesignonextension.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|область|String.|Получает или задает имя области для этого профиля, заданное с учетом регистра. Наследуется от [кербероссинглесигнонекстенсион](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|домена|Коллекция строк|Получает или задает список имен узлов или доменов, для которых расширение приложения выполняет единый вход. Наследуется от [кербероссинглесигнонекстенсион](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|блоккаутоматиклогин|Boolean.|Включает или отключает использование цепочки ключей. Наследуется от [кербероссинглесигнонекстенсион](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|каченаме|String.|Получает или задает универсальное имя службы безопасности для кэша Kerberos, который будет использоваться для этого профиля. Наследуется от [кербероссинглесигнонекстенсион](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|кредентиалбундлеидакцессконтроллист|Коллекция строк|Получает или задает список идентификаторов пакетов приложений, которым разрешен доступ к билету предоставления билетов Kerberos. Наследуется от [кербероссинглесигнонекстенсион](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|домаинреалмс|Коллекция строк|Получает или задает список сфер для сопоставления пользовательских областей доменов. В сфере учитывается регистр. Наследуется от [кербероссинглесигнонекстенсион](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|исдефаултреалм|Boolean.|Если задано значение true, область этого профиля будет выбрана по умолчанию. Необходимо, если настроено несколько профилей типа Kerberos. Наследуется от [кербероссинглесигнонекстенсион](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|пассвордблоккмодификатион|Boolean.|Включает или отключает смену паролей. Наследуется от [кербероссинглесигнонекстенсион](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|passwordExpirationDays|Int32|Переопределяет срок действия пароля по умолчанию (в днях). Для большинства доменов это значение вычисляется автоматически. Наследуется от [кербероссинглесигнонекстенсион](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|пассвордекспиратионнотификатиондайс|Int32|Получает или задает количество дней до тех пор, пока пользователь не будет уведомлен о сроке действия пароля (значение по умолчанию — 15). Наследуется от [кербероссинглесигнонекстенсион](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|userPrincipalName|String|Получает или задает имя участника, которое будет использоваться для этого профиля. Имя области не обязательно должно быть включено. Наследуется от [кербероссинглесигнонекстенсион](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|пассвордрекуиреактиведиректорикомплексити|Boolean.|Разрешает или запрещает, должны ли пароли отвечать требованиям сложности Active Directory. Наследуется от [кербероссинглесигнонекстенсион](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|passwordPreviousPasswordBlockCount|Int32|Получает или задает количество предыдущих паролей, которые необходимо заблокировать. Наследуется от [кербероссинглесигнонекстенсион](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|passwordMinimumLength|Int32|Получает или задает минимальную длину пароля. Наследуется от [кербероссинглесигнонекстенсион](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|пассвордминимумажедайс|Int32|Получает или задает минимальное количество дней, пока пользователь не сможет сменить пароль еще раз. Наследуется от [кербероссинглесигнонекстенсион](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|пассвордрекуирементсдескриптион|String.|Получает или задает описание требований к сложности пароля. Наследуется от [кербероссинглесигнонекстенсион](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|рекуиреусерпресенце|Boolean.|Получает или задает значение, указывающее, требуется ли проверка подлинности с помощью идентификатора сенсорного экрана, идентификатора лица или секретного кода для доступа к записи цепочки ключей. Наследуется от [кербероссинглесигнонекстенсион](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|активедиректориситекоде|String.|Получает или задает сайт Active Directory. Наследуется от [кербероссинглесигнонекстенсион](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|пассворденаблелокалсинк|Boolean.|Включает или отключает синхронизацию паролей. Это не повлияет на пользователей, выполнивших вход в систему с помощью учетной записи мобильного устройства в macOS. Наследуется от [кербероссинглесигнонекстенсион](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|блоккактиведиректориситеаутодисковери|Boolean.|Включает или отключает, может ли расширение Kerberos автоматически определять имя своего сайта. Наследуется от [кербероссинглесигнонекстенсион](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSKerberosSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSKerberosSingleSignOnExtension",
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
  "blockActiveDirectorySiteAutoDiscovery": true
}
```



