---
title: тип ресурса macOSKerberosSingleSignOnExtension
description: Представляет профиль расширения типа Kerberos Sign-On для устройств macOS.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9401d3cf92a3f153d7bb1547416d866c2833010a
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60695267"
---
# <a name="macoskerberossinglesignonextension-resource-type"></a>тип ресурса macOSKerberosSingleSignOnExtension

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет профиль расширения типа Kerberos Sign-On для устройств macOS.


Наследует [macOSSingleSignOnExtension](../resources/intune-deviceconfig-macossinglesignonextension.md)

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
|modeCredentialUsed|String|Выберите, как другие процессы используют учетные данные расширения Kerberos.|
|usernameLableCustom|String|Скоро будет обесценить.|
|usernameLabelCustom|String|Эта метка заменяет имя пользователя, показанное в расширении Kerberos. Вы можете ввести имя в соответствие с именем вашей компании или организации. Доступно для устройств с macOS-версиями 11 и более поздней версии.|
|userSetupDelayed|Логический|При наборе true пользователю не будет предложено настроить расширение Kerberos до тех пор, пока расширение не будет включено администратором или не будет получен вызов Kerberos. Доступно для устройств с macOS-версиями 11 и более поздней версии.|
|signInHelpText|String|Текст, отображаемый пользователю на входе Kerberos в окне. Доступно для устройств с версиями iOS и iPadOS 14 и более поздних версий.|
|kerberosAppsInBundleIdACLIncluded|Логический|При наборе True расширение Kerberos позволяет приложениям, вступимым с удостоверением пакета приложений, управляемыми приложениями и стандартными утилитами Kerberos, такими как TicketViewer и klist, получать доступ к учетным данным и использовать их. Доступно для устройств с macOS-версиями 12 и более поздних версий.|
|managedAppsInBundleIdACLIncluded|Логический|Если установлено true, расширение Kerberos позволяет управляемым приложениям, а все приложения, вступив с удостоверением пакета приложений, могут получить доступ к учетным данным. Если установлено false, расширение Kerberos позволяет всем приложениям получить доступ к учетным данным. Доступно для устройств с версиями iOS и iPadOS 14 и более поздних версий.|
|credentialsCacheMonitored|Логический|Если установлено true, учетные данные запрашиваются при следующем вызове Kerberos или изменении сетевого состояния. Когда срок действия учетных данных истек или отсутствует, создается новый учетный данные. Доступно для устройств с macOS-версиями 12 и более поздних версий.|
|singleSignOnExtensionPreferredKDCs|Коллекция строк|Скоро будет обесценить.|
|preferredKDCs|Коллекция строк|Add создает упорядоченный список предпочтительных центров рассылки ключей (KDCs), которые можно использовать для трафика Kerberos. Этот список используется, когда серверы не обнаруживаются с помощью DNS. При обнаружении серверов список используется как для проверки подключения, так и для трафика Kerberos. Если серверы не реагируют, устройство использует обнаружение DNS. Удаление удаляет существующий список, а устройства используют обнаружение DNS. Доступно для устройств с macOS-версиями 12 и более поздних версий.|
|tlsForLDAPRequired|Логический|При наборе True подключения LDAP требуются для использования безопасности транспортного слоя (TLS). Доступно для устройств с macOS-версиями 11 и более поздней версии.|

## <a name="relationships"></a>Связи
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
  "passwordChangeUrl": "String",
  "modeCredentialUsed": "String",
  "usernameLableCustom": "String",
  "usernameLabelCustom": "String",
  "userSetupDelayed": true,
  "signInHelpText": "String",
  "kerberosAppsInBundleIdACLIncluded": true,
  "managedAppsInBundleIdACLIncluded": true,
  "credentialsCacheMonitored": true,
  "singleSignOnExtensionPreferredKDCs": [
    "String"
  ],
  "preferredKDCs": [
    "String"
  ],
  "tlsForLDAPRequired": true
}
```



