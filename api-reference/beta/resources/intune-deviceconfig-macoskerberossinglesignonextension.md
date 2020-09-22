---
title: Тип ресурса Макоскербероссинглесигнонекстенсион
description: Представляет профиль расширения единого входа Kerberos для устройств macOS.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: af63d68bb0d8dd566ad2f97c26ff2bc73c8460da
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48024117"
---
# <a name="macoskerberossinglesignonextension-resource-type"></a>Тип ресурса Макоскербероссинглесигнонекстенсион

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет профиль расширения единого входа Kerberos для устройств macOS.


Наследуется от [макоссинглесигнонекстенсион](../resources/intune-deviceconfig-macossinglesignonextension.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|область|String|Получает или задает имя области для этого профиля, заданное с учетом регистра.|
|домена|Коллекция String|Получает или задает список имен узлов или доменов, для которых расширение приложения выполняет единый вход.|
|блоккаутоматиклогин|Boolean|Включает или отключает использование цепочки ключей.|
|каченаме|String|Получает или задает универсальное имя службы безопасности для кэша Kerberos, который будет использоваться для этого профиля.|
|кредентиалбундлеидакцессконтроллист|Коллекция String|Получает или задает список идентификаторов пакетов приложений, которым разрешен доступ к билету предоставления билетов Kerberos.|
|домаинреалмс|Коллекция String|Получает или задает список сфер для сопоставления пользовательских областей доменов. В сфере учитывается регистр.|
|исдефаултреалм|Boolean|Если задано значение true, область этого профиля будет выбрана по умолчанию. Необходимо, если настроено несколько профилей типа Kerberos.|
|пассвордблоккмодификатион|Boolean|Включает или отключает смену паролей.|
|passwordExpirationDays|Int32|Переопределяет срок действия пароля по умолчанию (в днях). Для большинства доменов это значение вычисляется автоматически.|
|пассвордекспиратионнотификатиондайс|Int32|Получает или задает количество дней до тех пор, пока пользователь не будет уведомлен о сроке действия пароля (значение по умолчанию — 15).|
|userPrincipalName|String|Получает или задает имя участника, которое будет использоваться для этого профиля. Имя области не обязательно должно быть включено.|
|пассвордрекуиреактиведиректорикомплексити|Boolean|Разрешает или запрещает, должны ли пароли отвечать требованиям сложности Active Directory.|
|passwordPreviousPasswordBlockCount|Int32|Получает или задает количество предыдущих паролей, которые необходимо заблокировать.|
|passwordMinimumLength|Int32|Получает или задает минимальную длину пароля.|
|пассвордминимумажедайс|Int32|Получает или задает минимальное количество дней, пока пользователь не сможет сменить пароль еще раз.|
|пассвордрекуирементсдескриптион|String|Получает или задает описание требований к сложности пароля.|
|рекуиреусерпресенце|Boolean|Получает или задает значение, указывающее, требуется ли проверка подлинности с помощью идентификатора сенсорного экрана, идентификатора лица или секретного кода для доступа к записи цепочки ключей.|
|активедиректориситекоде|String|Получает или задает сайт Active Directory.|
|пассворденаблелокалсинк|Boolean|Включает или отключает синхронизацию паролей. Это не повлияет на пользователей, выполнивших вход в систему с помощью учетной записи мобильного устройства в macOS.|
|блоккактиведиректориситеаутодисковери|Boolean|Включает или отключает, может ли расширение Kerberos автоматически определять имя своего сайта.|
|пассвордчанжеурл|String|Получает или задает URL-адрес, на который будет отправляться пользователь при инициации смены пароля.|

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
  "blockActiveDirectorySiteAutoDiscovery": true,
  "passwordChangeUrl": "String"
}
```






