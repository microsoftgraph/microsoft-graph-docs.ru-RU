# <a name="windowsinformationprotectionpolicy-resource-type"></a>Тип ресурса windowsInformationProtectionPolicy

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Политика для Windows Information Protection без MDM

Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов WindowsInformationProtectionPolicy](../api/intune_mam_windowsinformationprotectionpolicy_list.md)|Коллекция [windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md)|Перечисление свойств и связей объектов [windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md).|
|[Получение объекта windowsInformationProtectionPolicy](../api/intune_mam_windowsinformationprotectionpolicy_get.md)|[windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md)|Чтение свойств и связей объекта [windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md).|
|[Создание объекта windowsInformationProtectionPolicy](../api/intune_mam_windowsinformationprotectionpolicy_create.md)|[windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md)|Создание объекта [windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md).|
|[Удаление объекта windowsInformationProtectionPolicy](../api/intune_mam_windowsinformationprotectionpolicy_delete.md)|Нет|Удаление объекта [windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md).|
|[Обновление объекта windowsInformationProtectionPolicy](../api/intune_mam_windowsinformationprotectionpolicy_update.md)|[windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md)|Обновление свойств объекта [windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String (строка)|Отображаемое имя политики. Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|описание|String (строка)|Описание политики. Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|createdDateTime|DateTimeOffset|Дата и время создания политики. Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения политики. Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|ид|String (строка)|Ключ объекта. Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|версия|String (строка)|Версия объекта. Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|enforcementLevel|[windowsInformationProtectionEnforcementLevel](../resources/intune_mam_windowsinformationprotectionenforcementlevel.md)|Уровень применения WIP. Поддерживаемые значения см. в определении Enum. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md). Возможные значения: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.|
|enterpriseDomain|String (строка)|Основной домен предприятия. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|enterpriseProtectedDomainNames|Коллекция [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)|Список доменов предприятия, подлежащих защите. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|protectionUnderLockConfigRequired|Boolean (логический)|Указывает, следует ли настроить функцию защиты с блокировкой (другое название — шифрование с ПИН-кодом). Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|dataRecoveryCertificate|[windowsInformationProtectionDataRecoveryCertificate](../resources/intune_mam_windowsinformationprotectiondatarecoverycertificate.md)|Указывает сертификат, который можно использовать для восстановления данных из зашифрованных файлов. То же, что сертификат DRA для шифрованной файловой системы (EFS). Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|revokeOnUnenrollDisabled|Boolean (логический)|Эта политика определяет, следует ли отзывать ключи WIP при отмене регистрации устройства в службе управления. Если установлено значение 1, ключи не отзываются, а пользователь сохраняет доступ к защищенным файлам после отмены регистрации. Если не отзывать ключи, отзываемые файлы не будут удаляться. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|rightsManagementServicesTemplateId|Guid|GUID шаблона, используемый для шифрования RMS. Шаблон RMS позволяет ИТ-администратору настроить доступ к защищенному RMS файлу. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|azureRightsManagementServicesAllowed|Boolean (логический)|Указывает, разрешено ли шифрование Azure RMS для WIP. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|iconsVisible|Boolean (логический)|Определяет, отображаются ли дополнительные значки поверх значков защищенных файлов в Проводнике и плиток корпоративных приложений в меню "Пуск". Начиная с Windows 10 версии 1703, этот параметр также определяет, виден ли значок WIP в заголовке окна защищенного приложения. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|protectedApps|Коллекция [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)|Защищенные приложения могут получать доступ к корпоративным данным, а обрабатываемые ими данные шифруются. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|exemptApps|Коллекция [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)|Исключенные приложения также могут получать доступ к корпоративным данным, но обрабатываемые ими данные не шифруются. Это связано с тем, что у некоторых важных корпоративных приложений могут быть проблемы совместимости с зашифрованными данными. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|enterpriseNetworkDomainNames|Коллекция [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)|Это список доменов, входящих в границы предприятия. Данные, отправляемые из этих доменов на устройство, считаются корпоративными и защищаются. Считается, что отправлять корпоративные данные в эти домены безопасно. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|enterpriseProxiedDomains|Коллекция [windowsInformationProtectionProxiedDomainCollection](../resources/intune_mam_windowsinformationprotectionproxieddomaincollection.md)|Содержит список корпоративных ресурсов домены, размещенные в облаке, где нужно защищать. Подключения к этим ресурсам считаются корпоративными данными. Если прокси-сервер связан с облачным ресурсом, запросы к облачному ресурсу направляются по корпоративной сети через обозначенный прокси-сервер (порт 80). Используемый для этого прокси-сервер также необходимо настроить с помощью политики EnterpriseInternalProxyServers. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|enterpriseIPRanges|Коллекция [windowsInformationProtectionIPRangeCollection](../resources/intune_mam_windowsinformationprotectioniprangecollection.md)|Устанавливает диапазоны IP-адресов предприятия, которые определяют компьютеры в корпоративной сети. Данные, поступающие с этих компьютеров, считаются корпоративными и защищаются. Считается, что отправлять корпоративные данные на эти компьютеры безопасно. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|enterpriseIPRangesAreAuthoritative|Boolean (логический)|Логическое значение, которое указывает клиенту принять настроенный список и не использовать эвристику для поиска других подсетей. Значение по умолчанию — false. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|enterpriseProxyServers|Коллекция [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)|Это список прокси-серверов. Если сервера нет в этом списке, он не считается корпоративным. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|enterpriseInternalProxyServers|Коллекция [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)|Это список внутренних прокси-серверов, разделенных запятыми (например, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59"). Эти прокси-серверы были настроены администратором для подключения к определенным ресурсам в Интернете. Они считаются корпоративными серверами. Прокси-серверы используются при настройке политики EnterpriseProxiedDomains только для направления трафика на связанные домены через эти прокси-серверы. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|enterpriseProxyServersAreAuthoritative|Boolean (логический)|Логическое значение, которое указывает клиенту принять настроенный список прокси-серверов и не пытаться обнаружить другие рабочие прокси-серверы. Значение по умолчанию — false. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|neutralDomainResources|Коллекция [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)|Список доменных имен, которые можно использовать для рабочего или личного ресурса. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|indexingEncryptedStoresOrItemsBlocked|Boolean (логический)|Этот параметр позволяет разрешить или запретить индексатору службы Windows Search индексировать элементы. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|smbAutoEncryptedFileExtensions|Коллекция [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)|Задает список расширений. Файлы с этими расширениями шифруются при копировании из общей папки SMB в пределах предприятия. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|isAssigned|Boolean (логический)|Указывает, применена ли политика к группам включения. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|revokeOnMdmHandoffDisabled|Boolean (логический)|Новое свойство в RS2, документация готовится.|
|mdmEnrollmentUrl|String (строка)|URL-адрес регистрации в системе MDM.|
|windowsHelloForBusinessBlocked|Boolean (логический)|Логическое значение, которое определяет Windows Hello для бизнеса как способ входа в Windows.|
|pinMinimumLength|Int32|Целое число, которое определяет минимальное количество символов в ПИН-коде. Значение по умолчанию — 4. Для этого параметра политики можно установить значение в диапазоне от 4 до 127 (или числа, заданного в параметре политики "Максимальная длина ПИН-кода", если оно меньше).|
|pinUppercaseLetters|[windowsInformationProtectionPinCharacterRequirements](../resources/intune_mam_windowsinformationprotectionpincharacterrequirements.md)|Целочисленное значение, которое настраивает использование прописных букв в PIN-коде Windows Hello for Business. По умолчанию используется NotAllow. Возможные значения:: `notAllow`, `requireAtLeastOne`, `allow`.|
|pinLowercaseLetters|[windowsInformationProtectionPinCharacterRequirements](../resources/intune_mam_windowsinformationprotectionpincharacterrequirements.md)|Целочисленное значение, которое настраивает использование строчных букв в PIN-коде Windows Hello for Business. По умолчанию используется NotAllow. Возможные значения: `notAllow`, `requireAtLeastOne`, `allow`.|
|pinSpecialCharacters|[windowsInformationProtectionPinCharacterRequirements](../resources/intune_mam_windowsinformationprotectionpincharacterrequirements.md)|Целое число, которое настраивает использование специальных знаков в ПИН-коде Windows Hello для бизнеса. Действительные специальные знаки для ПИН-жестов Windows Hello для бизнеса: " # $ % & ' ( ) * + , - . / : ; < = > ? @ \[ \ \] ^ _ ` { | } ~. По умолчанию NotAllow. Возможные значения: `notAllow`, `requireAtLeastOne`, `allow`.|
|pinExpirationDays|Int32|Целое число указывает срок действия ПИН-кода (в днях), по истечении которого система требует его изменения. Для этого параметра политики можно установить значение в диапазоне от 730 до 0. Если для этой политики установлено значение 0, срок действия ПИН-кода пользователя никогда не истекает. Этот узел добавлен в Windows 10 версии 1511. Значение по умолчанию — 0.|
|numberOfPastPinsRemembered|Int32|Целое число, указывающее количество предыдущих ПИН-кодов, связанных с учетной записью пользователя, повторное использование которых необходимо запретить. Для этого параметра политики можно установить значение в диапазоне от 50 до 0. Если для этой политики установлено значение 0, хранение предыдущих ПИН-кодов не требуется. Этот узел добавлен в Windows 10 версии 1511. Значение по умолчанию — 0.|
|passwordMaximumAttemptCount|Int32|Количество неудачных попыток аутентификации до очистки устройства. Значение 0 отключает функцию очистки устройства. Значение — целое число, которое лежит в диапазоне X, где 4 <= X <= 16 для компьютеров и 0 <= X <= 999 для мобильных устройств.|
|minutesOfInactivityBeforeDeviceLock|Int32|Указывает максимальное время простоя устройства (в минутах), по истечении которого оно блокируется ПИН-кодом или паролем.   Значение — целое число, которое лежит в диапазоне X, где 0 <= X <= 999.|
|daysWithoutContactBeforeUnenroll|Int32|Время с момента последнего подключения к Интернету до очистки данных приложения (в днях) |

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|protectedAppLockerFiles|Коллекция [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md)|Еще один способ указания защищенных приложений с помощью xml-файлов. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|exemptAppLockerFiles|Коллекция [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md)|Еще один способ указания исключенных приложений с помощью xml-файлов. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|задания|Коллекция [targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md)|Список групп безопасности, к которым применяется политика. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.windowsInformationProtection",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtectionPolicy"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionPolicy",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "version": "String",
  "enforcementLevel": "String",
  "enterpriseDomain": "String",
  "enterpriseProtectedDomainNames": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "protectionUnderLockConfigRequired": true,
  "dataRecoveryCertificate": {
    "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
    "subjectName": "String",
    "description": "String",
    "expirationDateTime": "String (timestamp)",
    "certificate": "binary"
  },
  "revokeOnUnenrollDisabled": true,
  "rightsManagementServicesTemplateId": "guid",
  "azureRightsManagementServicesAllowed": true,
  "iconsVisible": true,
  "protectedApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionApp",
      "displayName": "String",
      "description": "String",
      "publisherName": "String",
      "productName": "String",
      "denied": true
    }
  ],
  "exemptApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionApp",
      "displayName": "String",
      "description": "String",
      "publisherName": "String",
      "productName": "String",
      "denied": true
    }
  ],
  "enterpriseNetworkDomainNames": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "enterpriseProxiedDomains": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionProxiedDomainCollection",
      "displayName": "String",
      "proxiedDomains": [
        {
          "@odata.type": "microsoft.graph.proxiedDomain",
          "ipAddressOrFQDN": "String",
          "proxy": "String"
        }
      ]
    }
  ],
  "enterpriseIPRanges": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionIPRangeCollection",
      "displayName": "String",
      "ranges": [
        {
          "@odata.type": "microsoft.graph.iPv6Range",
          "lowerAddress": "String",
          "upperAddress": "String"
        }
      ]
    }
  ],
  "enterpriseIPRangesAreAuthoritative": true,
  "enterpriseProxyServers": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "enterpriseInternalProxyServers": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "enterpriseProxyServersAreAuthoritative": true,
  "neutralDomainResources": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "indexingEncryptedStoresOrItemsBlocked": true,
  "smbAutoEncryptedFileExtensions": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "isAssigned": true,
  "revokeOnMdmHandoffDisabled": true,
  "mdmEnrollmentUrl": "String",
  "windowsHelloForBusinessBlocked": true,
  "pinMinimumLength": 1024,
  "pinUppercaseLetters": "String",
  "pinLowercaseLetters": "String",
  "pinSpecialCharacters": "String",
  "pinExpirationDays": 1024,
  "numberOfPastPinsRemembered": 1024,
  "passwordMaximumAttemptCount": 1024,
  "minutesOfInactivityBeforeDeviceLock": 1024,
  "daysWithoutContactBeforeUnenroll": 1024
}
```








