# <a name="windowsinformationprotection-resource-type"></a>Тип ресурса windowsInformationProtection

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Политика для Windows Information Protection, которая используется для настройки расширенных параметров управления.

Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов windowsInformationProtection](../api/intune_mam_windowsinformationprotection_list.md)|Коллекция объектов [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)|Список свойств и связей объектов [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|[Получение объекта windowsInformationProtection](../api/intune_mam_windowsinformationprotection_get.md)|[windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)|Чтение свойств и связей объекта [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md).|
|[Действие assign](../api/intune_mam_windowsinformationprotection_assign.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Отображаемое имя политики. Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|описание|Строка|Описание политики. Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|createdDateTime|DateTimeOffset|Дата и время создания политики. Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения политики. Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|ИД|Строка|Ключ объекта. Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|версия|Строка|Версия объекта. Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|enforcementLevel|[windowsInformationProtectionEnforcementLevel](../resources/intune_mam_windowsinformationprotectionenforcementlevel.md)|Уровень принудительного применения WIP. Список поддерживаемых значений см. в определении данного перечисления. Возможные значения: `noProtection`, `encryptAndAuditOnly`, `encryptAuditAndPrompt`, `encryptAuditAndBlock`.|
|enterpriseDomain|Строка|Основной корпоративный домен.|
|enterpriseProtectedDomainNames|Коллекция [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)|Список корпоративных доменов, которые необходимо защитить.|
|protectionUnderLockConfigRequired|Логическое|Указывает, следует ли настроить функцию защиты с блокировкой (другое название — шифрование с ПИН-кодом).|
|dataRecoveryCertificate|[windowsInformationProtectionDataRecoveryCertificate](../resources/intune_mam_windowsinformationprotectiondatarecoverycertificate.md)|Указывает сертификат, который можно использовать для восстановления данных из зашифрованных файлов. То же, что сертификат DRA для шифрованной файловой системы (EFS).|
|revokeOnUnenrollDisabled|Логическое|Эта политика определяет, следует ли отзывать ключи WIP при отмене регистрации устройства в службе управления. Если установлено значение 1, ключи не отзываются, а пользователь сохраняет доступ к защищенным файлам после отмены регистрации. Если ключи не отзываются, файлы не очищаются.|
|rightsManagementServicesTemplateId|Guid|GUID шаблона, используемый для шифрования RMS. Шаблон RMS позволяет ИТ-администратору настроить доступ (и его длительность) к защищенному RMS файлу для определенных пользователей.|
|azureRightsManagementServicesAllowed|Логическое|Указывает, разрешать ли шифрование Azure RMS для WIP.|
|iconsVisible|Логическое|Определяет, отображаются ли дополнительные значки поверх значков защищенных файлов WIP в Проводнике и плиток приложений только для предприятий в меню "Пуск". Начиная с Windows 10 версии 1703, этот параметр также определяет, отображается ли значок WIP в заголовке окна защищенного приложения.|
|protectedApps|Коллекция объектов [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)|Защищенные приложения могут получать доступ к корпоративным данным, а обрабатываемые ими данные шифруются.|
|exemptApps|Коллекция [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)|Исключенные приложения также могут получать доступ к корпоративным данным, но обрабатываемые ими данные не шифруются. Это связано с тем, что у некоторых важных корпоративных приложений могут быть проблемы совместимости с зашифрованными данными.|
|enterpriseNetworkDomainNames|Коллекция [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)|Это список доменов, входящих в границы предприятия. Данные, отправляемые из этих доменов на устройство, считаются корпоративными и защищаются. Считается, что отправлять корпоративные данные в эти домены безопасно.|
|enterpriseProxiedDomains|Коллекция [windowsInformationProtectionProxiedDomainCollection](../resources/intune_mam_windowsinformationprotectionproxieddomaincollection.md)|Содержит список корпоративных ресурсов домены, размещенные в облаке, где нужно защищать. Подключения к этим ресурсам считаются корпоративными данными. Если прокси-сервер связан с облачным ресурсом, запросы к облачному ресурсу направляются по корпоративной сети через обозначенный прокси-сервер (порт 80). Используемый для этого прокси-сервер также необходимо настроить с помощью политики EnterpriseInternalProxyServers.|
|enterpriseIPRanges|Коллекция [windowsInformationProtectionIPRangeCollection](../resources/intune_mam_windowsinformationprotectioniprangecollection.md)|Устанавливает диапазоны IP-адресов предприятия, которые определяют компьютеры в корпоративной сети. Данные, поступающие с этих компьютеров, считаются корпоративными и защищаются. Считается, что отправлять корпоративные данные на эти компьютеры безопасно.|
|enterpriseIPRangesAreAuthoritative|Логическое|Логическое значение, которое указывает клиенту принять настроенный список и не использовать эвристику для поиска других подсетей. Значение по умолчанию: false.|
|enterpriseProxyServers|Коллекция [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)|Это список прокси-серверов. Сервер, который не входит в этот список, не считается корпоративным.|
|enterpriseInternalProxyServers|Коллекция [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)|Это список внутренних прокси-серверов, разделенных запятыми (например, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59"). Эти прокси-серверы были настроены администратором для подключения к определенным ресурсам в Интернете. Они считаются корпоративными серверами. Прокси-серверы используются при настройке политики EnterpriseProxiedDomains только для направления трафика на связанные домены через эти прокси-серверы.|
|enterpriseProxyServersAreAuthoritative|Логическое|Логическое значение, которое указывает клиенту принять настроенный список прокси-серверов и не пытаться обнаружить другие рабочие прокси-серверы. Значение по умолчанию: false.|
|neutralDomainResouTranslatedrces|Коллекция [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)|Список доменных имен, которые можно использовать для рабочих или личных ресурсов.|
|indexingEncryptedStoresOrItemsBlocked|Логическое|Этот параметр позволяет разрешить или запретить индексатору службы Windows Search индексировать элементы.|
|smbAutoEncryptedFileExtensions|Коллекция [windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md)|Задает список расширений. Файлы с этими расширениями шифруются при копировании из общей папки SMB в пределах предприятия.|
|isAssigned|Логическое|Указывает, применена ли политика к группам включения.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|protectedAppLockerFiles|Коллекция объектов [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md)|Еще один способ ввести данные о защищенных приложениях с помощью XML-файлов.|
|exemptAppLockerFiles|Коллекция объектов [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md)|Еще один способ ввести данные об исключаемых приложениях с помощью XML-файлов.|
|задания|Коллекция [targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md)|Список групп безопасности, к которым применяется политика.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.managedAppPolicy",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtection"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtection",
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
  "rightsManagementServicesTemplateId": "<Unknown Primitive Type Edm.Guid>",
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








