---
title: тип ресурса iosKerberosSingleSignOnExtension
description: Представляет профиль одноместного Sign-On kerberos для устройств с iOS.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 888075038454471756b5e2831ed5fd67fafc0636
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/19/2021
ms.locfileid: "60493991"
---
# <a name="ioskerberossinglesignonextension-resource-type"></a>тип ресурса iosKerberosSingleSignOnExtension

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет профиль одноместного Sign-On kerberos для устройств с iOS.


Наследует [от iosSingleSignOnExtension](../resources/intune-deviceconfig-iossinglesignonextension.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|realm|String|Получает или задает имя области, чувствительной к делу, для этого профиля.|
|домены|Коллекция строк|Получает или задает список хостов или доменных имен, для которых расширение приложения выполняет SSO.|
|blockAutomaticLogin|Логический|Включает или отключает использование Keychain.|
|cacheName|String|Получает или задает имя универсальных служб безопасности кэша Kerberos для использования для этого профиля.|
|credentialBundleIdAccessControlList|Коллекция строк|Получает или задает список ID-пакетов приложений, разрешенных для доступа к билету на предоставление билетов Kerberos.|
|domainRealms|Коллекция строк|Получает или задает список областей для настраиваемого сопоставления доменных областей. Области чувствительны к делу.|
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
|requireUserPresence|Логический|Получает или задает, требуется ли проверка подлинности через Touch ID, Face ID или пароль для доступа к записи keychain.|
|activeDirectorySiteCode|String|Получает или задает сайт Active Directory.|
|passwordEnableLocalSync|Логический|Включает или отключает синхронизацию паролей. Это не повлияет на пользователей, входив в систему с мобильной учетной записью на macOS.|
|blockActiveDirectorySiteAutoDiscovery|Логический|Включает или отключает возможность автоматического определения имени сайта расширения Kerberos.|
|passwordChangeUrl|String|Получает или задает URL-адрес, на который будет отправлен пользователь при инициале изменения пароля.|
|signInHelpText|String|Текст, отображаемый пользователю на входе Kerberos в окне. Доступно для устройств с версиями iOS и iPadOS 14 и более поздних версий.|
|managedAppsInBundleIdACLIncluded|Логический|Если установлено true, расширение Kerberos позволяет управляемым приложениям, а все приложения, вступив с удостоверением пакета приложений, могут получить доступ к учетным данным. Если установлено false, расширение Kerberos позволяет всем приложениям получить доступ к учетным данным. Доступно для устройств с версиями iOS и iPadOS 14 и более поздних версий.|

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
  "passwordChangeUrl": "String",
  "signInHelpText": "String",
  "managedAppsInBundleIdACLIncluded": true
}
```



