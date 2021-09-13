---
title: тип ресурса kerberosSingleSignOnExtension
description: Представляет профиль расширения типа Kerberos Sign-On.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fbac237df1c2d4a1b466d675751b67b71c1ba94e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59127229"
---
# <a name="kerberossinglesignonextension-resource-type"></a>тип ресурса kerberosSingleSignOnExtension

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет профиль расширения типа Kerberos Sign-On.


Наследует [от singleSignOnExtension](../resources/intune-deviceconfig-singlesignonextension.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|realm|String|Получает или задает имя области, чувствительной к делу, для этого профиля.|
|домены|Коллекция объектов string|Получает или задает список хостов или доменных имен, для которых расширение приложения выполняет SSO.|
|blockAutomaticLogin|Логическое|Включает или отключает использование Keychain.|
|cacheName|String|Получает или задает имя универсальных служб безопасности кэша Kerberos для использования для этого профиля.|
|credentialBundleIdAccessControlList|Коллекция объектов string|Получает или задает список ID-пакетов приложений, разрешенных для доступа к билету на предоставление билетов Kerberos.|
|domainRealms|Коллекция объектов string|Получает или задает список областей для настраиваемого сопоставления доменных областей. Области чувствительны к делу.|
|isDefaultRealm|Логический|Если значение true, область этого профиля будет выбрана по умолчанию. Необходимо, если настроено несколько профилей типа Kerberos.|
|passwordBlockModification|Логический|Включает или отключает изменения пароля.|
|passwordExpirationDays|Int32|Переопределяет срок действия пароля по умолчанию за несколько дней. Для большинства доменов это значение вычисляется автоматически.|
|passwordExpirationNotificationDays|Int32|Получает или задает количество дней до уведомления пользователя о том, что срок действия пароля истекает (по умолчанию — 15).|
|userPrincipalName|String|Получает или задает имя пользователя, которое необходимо использовать для этого профиля. Имя области не нужно включать.|
|passwordRequireActiveDirectoryComplexity|Логический|Включает или отключает, должны ли пароли соответствовать требованиям active Directory по сложности.|
|passwordPreviousPasswordBlockCount|Int32|Получает или задает количество предыдущих паролей для блокировки.|
|passwordMinimumLength|Int32|Получает или задает минимальную длину пароля.|
|passwordMinimumAgeDays|Int32|Получает или задает минимальное количество дней, пока пользователь не сможет изменить пароль снова.|
|passwordRequirementsDescription|String|Получает или задает описание требований к сложности пароля.|
|requireUserPresence|Логическое|Получает или задает, требуется ли проверка подлинности через Touch ID, Face ID или пароль для доступа к записи keychain.|
|activeDirectorySiteCode|String|Получает или задает сайт Active Directory.|
|passwordEnableLocalSync|Логическое|Включает или отключает синхронизацию паролей. Это не повлияет на пользователей, входив в систему с мобильной учетной записью на macOS.|
|blockActiveDirectorySiteAutoDiscovery|Логическое|Включает или отключает возможность автоматического определения имени сайта расширения Kerberos.|
|passwordChangeUrl|String|Получает или задает URL-адрес, на который будет отправлен пользователь при инициале изменения пароля.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.kerberosSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.kerberosSingleSignOnExtension",
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



