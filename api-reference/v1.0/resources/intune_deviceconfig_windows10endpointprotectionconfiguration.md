# <a name="windows10endpointprotectionconfiguration-resource-type"></a>Тип ресурса windows10EndpointProtectionConfiguration

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

В этой статье описаны объявляемые методы, свойства и связи, которые предоставляются ресурсом Windows10EndpointProtectionConfiguration.

Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов windows10EndpointProtectionConfiguration](../api/intune_deviceconfig_windows10endpointprotectionconfiguration_list.md)|Коллекция [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md)|Перечисление свойств и связей объектов [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md).|
|[Получение объекта windows10EndpointProtectionConfiguration](../api/intune_deviceconfig_windows10endpointprotectionconfiguration_get.md)|[windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md)|Чтение свойств и связей объекта [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md).|
|[Создание объекта windows10EndpointProtectionConfiguration](../api/intune_deviceconfig_windows10endpointprotectionconfiguration_create.md)|[windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md)|Создание объекта [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md).|
|[Удаление объекта windows10EndpointProtectionConfiguration](../api/intune_deviceconfig_windows10endpointprotectionconfiguration_delete.md)|Нет|Удаление объекта [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md).|
|[Обновление объекта windows10EndpointProtectionConfiguration](../api/intune_deviceconfig_windows10endpointprotectionconfiguration_update.md)|[windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md)|Обновление свойств объекта [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|ИД|Строка|Ключ объекта. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|описание|Строка|Указанное администратором описание конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|displayName|Строка|Указанное администратором имя конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|версия|Int32|Версия конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|firewallBlockStatefulFTP|Логический|Блокирует FTP-подключения к устройству с отслеживанием состояния.|
|firewallIdleTimeoutForSecurityAssociationInSeconds|Int32|Настраивает время ожидания для сопоставлений безопасности в секундах от 300 до 3600 включительно. По истечении этого срока сопоставления безопасности перестают действовать и удаляются. Допустимые значения: от 300 до 3600|
|firewallPreSharedKeyEncodingMethod|[firewallPreSharedKeyEncodingMethodType](../resources/intune_deviceconfig_firewallpresharedkeyencodingmethodtype.md)|Выберите кодировку с общим ключом, которую следует использовать. Возможные значения: `deviceDefault`, `none`, `utF8`.|
|firewallIPSecExemptionsAllowNeighborDiscovery|Логический|Настраивает исключения IPSec для разрешения обнаружения соседей. Коды типов ICMP IPv6.|
|firewallIPSecExemptionsAllowICMP|Логический|Настраивает исключения IPSec для разрешения ICMP|
|firewallIPSecExemptionsAllowRouterDiscovery|Логический|Настраивает исключения IPSec для разрешения обнаружения маршрутизаторов. Коды типов ICMP IPv6.|
|firewallIPSecExemptionsAllowDHCP|Логический|Настраивает исключения IPSec для разрешения DHCP-трафика IPv4 и IPv6|
|firewallCertificateRevocationListCheckMethod|[firewallCertificateRevocationListCheckMethodType](../resources/intune_deviceconfig_firewallcertificaterevocationlistcheckmethodtype.md)|Укажите, как будет применяться список отзыва сертификатов. Возможные значения: `deviceDefault`, `none`, `attempt`, `require`.|
|firewallMergeKeyingModuleSettings|Логический|Если модуль ключей поддерживает не весь набор проверки подлинности, дайте ему указание игнорировать только неподдерживаемые пакеты, а не весь набор|
|firewallPacketQueueingMethod|[firewallPacketQueueingMethodType](../resources/intune_deviceconfig_firewallpacketqueueingmethodtype.md)|Настраивает, как будет применяться пакетная очередность в сценарии туннельного шлюза. Возможные значения: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.|
|firewallProfileDomain|[windowsFirewallNetworkProfile](../resources/intune_deviceconfig_windowsfirewallnetworkprofile.md)|Настраивает параметры профиля брандмауэра для доменных сетей|
|firewallProfilePublic|[windowsFirewallNetworkProfile](../resources/intune_deviceconfig_windowsfirewallnetworkprofile.md)|Настраивает параметры профиля брандмауэра для общедоступных сетей|
|firewallProfilePrivate|[windowsFirewallNetworkProfile](../resources/intune_deviceconfig_windowsfirewallnetworkprofile.md)|Настраивает параметры профиля брандмауэра для частных сетей|
|defenderAttackSurfaceReductionExcludedPaths|Коллекция String|Список файлов EXE и папок, которые следует исключить из правил сокращения направлений атак|
|defenderGuardedFoldersAllowedAppPaths|Коллекция String|Список путей к файлам EXE, которым разрешен доступ к защищенным папкам|
|defenderAdditionalGuardedFolders|Коллекция String|Список путей к папкам, которые следует добавить в список защищенных папок|
|defenderExploitProtectionXml|Бинарное|XML-файл с информацией о защите от эксплойтов.|
|defenderExploitProtectionXmlFileName|Строка|Имя файла, из которого получено свойство DefenderExploitProtectionXml.|
|defenderSecurityCenterBlockExploitProtectionOverride|Логический|Указывает, следует ли запретить пользователю переопределять настройки защиты от эксплойтов.|
|appLockerApplicationControl|[appLockerApplicationControlType](../resources/intune_deviceconfig_applockerapplicationcontroltype.md)|Позволяет администратору выбрать, какие типы приложений разрешены на устройствах. Возможные значения: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.|
|smartScreenEnableInShell|Логический|Позволяет ИТ-администраторам настраивать SmartScreen для Windows.|
|smartScreenBlockOverrideForFiles|Логический|Позволяет ИТ-администраторам указывать, могут ли пользователи игнорировать предупреждения SmartScreen и запускать вредоносные файлы.|
|applicationGuardEnabled|Логический|Включение Application Guard в Защитнике Windows|
|applicationGuardBlockFileTransfer|[applicationGuardBlockFileTransferType](../resources/intune_deviceconfig_applicationguardblockfiletransfertype.md)|Позволяет заблокировать передачу изображений и текстовых файлов через буфер обмена. Возможные значения: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.|
|applicationGuardBlockNonEnterpriseContent|Логический|Указывает, следует ли блокировать загрузку некорпоративного контента, например сторонних подключаемых модулей, на корпоративных сайтах.|
|applicationGuardAllowPersistence|Логический|Позволяет разрешить сохранение пользовательских данных в контейнере App Guard (избранное, файлы cookie, веб-пароли и т. д.).|
|applicationGuardForceAuditing|Логический|Эта политика позволяет сохранять журналы и события Windows (попытки входа и выхода, использование привилегий, установка программного обеспечения, системные изменения и т. д.) для обеспечения безопасности и соответствия требованиям.|
|applicationGuardBlockClipboardSharing|[applicationGuardBlockClipboardSharingType](../resources/intune_deviceconfig_applicationguardblockclipboardsharingtype.md)|Позволяет заблокировать обмен данными от основного приложения к контейнеру через буфер обмена. Возможные значения: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.|
|applicationGuardAllowPrintToPDF|Логический|Позволяет разрешить печать в PDF из контейнера.|
|applicationGuardAllowPrintToXPS|Логический|Позволяет разрешить печать в XPS из контейнера.|
|applicationGuardAllowPrintToLocalPrinters|Логический|Позволяет разрешить печать на локальных принтерах из контейнера.|
|applicationGuardAllowPrintToNetworkPrinters|Логический|Позволяет разрешить печать на сетевых принтерах из контейнера.|
|bitLockerDisableWarningForOtherDiskEncryption|Логический|Позволяет администратору отключить предупреждение о другом методе шифрования диска на компьютерах пользователей.|
|bitLockerEnableStorageCardEncryptionOnMobile|Логический|Позволяет администратору требовать включения шифрования с помощью BitLocker. Эта политика действительна только для мобильных устройств.|
|bitLockerEncryptDevice|Логический|Позволяет администратору требовать включения шифрования с помощью BitLocker.|
|bitLockerRemovableDrivePolicy|[bitLockerRemovableDrivePolicy](../resources/intune_deviceconfig_bitlockerremovabledrivepolicy.md)|Политика BitLocker в отношении съемных дисков.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|задания|Коллекция [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)|Список назначений для профиля конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|deviceStatuses|Коллекция [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md)|Состояние установки конфигурации для каждого устройства. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|userStatuses|Коллекция [deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md)|Состояние установки конфигурации устройства пользователем. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|Обзор состояния конфигурации по устройствам. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|Обзор состояния конфигурации устройств по пользователям. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceSettingStateSummaries|Коллекция [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md)|Обзор состояния параметров конфигурации устройств по пользователям. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.deviceConfiguration",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10EndpointProtectionConfiguration"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "firewallBlockStatefulFTP": true,
  "firewallIdleTimeoutForSecurityAssociationInSeconds": 1024,
  "firewallPreSharedKeyEncodingMethod": "String",
  "firewallIPSecExemptionsAllowNeighborDiscovery": true,
  "firewallIPSecExemptionsAllowICMP": true,
  "firewallIPSecExemptionsAllowRouterDiscovery": true,
  "firewallIPSecExemptionsAllowDHCP": true,
  "firewallCertificateRevocationListCheckMethod": "String",
  "firewallMergeKeyingModuleSettings": true,
  "firewallPacketQueueingMethod": "String",
  "firewallProfileDomain": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "String",
    "stealthModeBlocked": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "policyRulesFromGroupPolicyMerged": true
  },
  "firewallProfilePublic": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "String",
    "stealthModeBlocked": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "policyRulesFromGroupPolicyMerged": true
  },
  "firewallProfilePrivate": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "String",
    "stealthModeBlocked": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "policyRulesFromGroupPolicyMerged": true
  },
  "defenderAttackSurfaceReductionExcludedPaths": [
    "String"
  ],
  "defenderGuardedFoldersAllowedAppPaths": [
    "String"
  ],
  "defenderAdditionalGuardedFolders": [
    "String"
  ],
  "defenderExploitProtectionXml": "binary",
  "defenderExploitProtectionXmlFileName": "String",
  "defenderSecurityCenterBlockExploitProtectionOverride": true,
  "appLockerApplicationControl": "String",
  "smartScreenEnableInShell": true,
  "smartScreenBlockOverrideForFiles": true,
  "applicationGuardEnabled": true,
  "applicationGuardBlockFileTransfer": "String",
  "applicationGuardBlockNonEnterpriseContent": true,
  "applicationGuardAllowPersistence": true,
  "applicationGuardForceAuditing": true,
  "applicationGuardBlockClipboardSharing": "String",
  "applicationGuardAllowPrintToPDF": true,
  "applicationGuardAllowPrintToXPS": true,
  "applicationGuardAllowPrintToLocalPrinters": true,
  "applicationGuardAllowPrintToNetworkPrinters": true,
  "bitLockerDisableWarningForOtherDiskEncryption": true,
  "bitLockerEnableStorageCardEncryptionOnMobile": true,
  "bitLockerEncryptDevice": true,
  "bitLockerRemovableDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy",
    "encryptionMethod": "String",
    "requireEncryptionForWriteAccess": true,
    "blockCrossOrganizationWriteAccess": true
  }
}
```








