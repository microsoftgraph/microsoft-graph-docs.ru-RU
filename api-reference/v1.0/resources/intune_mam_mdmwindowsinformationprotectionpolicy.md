# <a name="mdmwindowsinformationprotectionpolicy-resource-type"></a>Тип ресурса mdmWindowsInformationProtectionPolicy

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Политика для Windows Information Protection с MDM

Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов MdmWindowsInformationProtectionPolicy](../api/intune_mam_mdmwindowsinformationprotectionpolicy_list.md)|Коллекция [mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md)|Перечисление свойств и связей объектов [mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md).|
|[Получение объекта mdmWindowsInformationProtectionPolicy](../api/intune_mam_mdmwindowsinformationprotectionpolicy_get.md)|[mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md)|Чтение свойств и связей объекта [mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md).|
|[Создание объекта mdmWindowsInformationProtectionPolicy](../api/intune_mam_mdmwindowsinformationprotectionpolicy_create.md)|[mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md)|Создание объекта [mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md).|
|[Удаление объекта mdmWindowsInformationProtectionPolicy](../api/intune_mam_mdmwindowsinformationprotectionpolicy_delete.md)|Нет|Удаление объекта [mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md).|
|[Обновление объекта mdmWindowsInformationProtectionPolicy](../api/intune_mam_mdmwindowsinformationprotectionpolicy_update.md)|[mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md)|Обновление свойств объекта [mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String (строка)|Отображаемое имя политики. Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|description|String (строка)|Описание политики. Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|createdDateTime|DateTimeOffset|Дата и время создания политики. Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения политики. Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|id|String (строка)|Ключ объекта. Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|version|String (строка)|Версия объекта. Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|enforcementLevel|[windowsInformationProtectionEnforcementLevel](../resources/intune_mam_windowsinformationprotectionenforcementlevel.md)|Принудительное применение уровня WIP. См. определение перечисления для поддерживаемых значений, унаследованных от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md). Возможные значения: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.|
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

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|protectedAppLockerFiles|Коллекция [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md)|Еще один способ указания защищенных приложений с помощью xml-файлов. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|exemptAppLockerFiles|Коллекция [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md)|Еще один способ указания исключенных приложений с помощью xml-файлов. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|assignments|Коллекция [targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md)|Список групп безопасности, к которым применяется политика. Наследуется от [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.windowsInformationProtection",
  "@odata.type": "microsoft.graph.mdmWindowsInformationProtectionPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mdmWindowsInformationProtectionPolicy",
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
  "rightsManagementServicesTemplateId": "79199ed9-e50b-4257-8de4-70b9c8685061",
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
  "isAssigned": true
}
```



