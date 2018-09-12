# <a name="windowsfirewallnetworkprofile-resource-type"></a>Тип ресурса windowsFirewallNetworkProfile

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Политики профилей брандмауэра Windows.
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|firewallEnabled|[stateManagementSetting](../resources/intune_deviceconfig_statemanagementsetting.md)|Настройка главного устройства, чтобы разрешить или заблокировать брандмауэр, и принудительное применение повышенной безопасности для сетевого профиля. Возможные значения: `notConfigured`, `blocked`, `allowed`.|
|stealthModeBlocked|Логический|Предотвращение работы сервера в скрытом режиме. Когда оба свойства StealthModeRequired и StealthModeBlocked имеют значение true, приоритет имеет StealthModeBlocked.|
|incomingTrafficBlocked|Логический|Настройка брандмауэра на блокировку всего входящего трафика независимо от параметров политики. Когда оба свойства IncomingTrafficRequired и IncomingTrafficBlocked имеют значение true, приоритет имеет IncomingTrafficBlocked.|
|unicastResponsesToMulticastBroadcastsBlocked|Логический|Настраивает брандмауэр на блокировку одноадресных откликов на многоадресный широковещательный трафик. Когда оба свойства UnicastResponsesToMulticastBroadcastsRequired и UnicastResponsesToMulticastBroadcastsBlocked имеют значение true, приоритет имеет UnicastResponsesToMulticastBroadcastsBlocked.|
|inboundNotificationsBlocked|Логический|Предотвращает отображение в брандмауэре уведомлений о том, что для приложения заблокирована возможность прослушивания порта. Когда оба свойства InboundNotificationsRequired и InboundNotificationsBlocked имеют значение true, приоритет имеет InboundNotificationsBlocked.|
|authorizedApplicationRulesFromGroupPolicyMerged|Логический|Настройка брандмауэра таким образом, чтобы он объединял правила для авторизованных приложений из групповой политики с правилами из локального хранилища, а не игнорировал правила локального хранилища. Когда оба свойства AuthorizedApplicationRulesFromGroupPolicyNotMerged и AuthorizedApplicationRulesFromGroupPolicyMerged имеют значение true, приоритет имеет AuthorizedApplicationRulesFromGroupPolicyMerged.|
|globalPortRulesFromGroupPolicyMerged|Логический|Настраивает брандмауэр таким образом, чтобы он объединял глобальные правила для портов из групповой политики с правилами из локального хранилища, а не игнорировал правила локального хранилища. Когда оба свойства GlobalPortRulesFromGroupPolicyNotMerged и GlobalPortRulesFromGroupPolicyMerged имеют значение true, приоритет имеет GlobalPortRulesFromGroupPolicyMerged.|
|connectionSecurityRulesFromGroupPolicyMerged|Логический|Настраивает брандмауэр таким образом, чтобы он объединял правила безопасности подключений из групповой политики с правилами из локального хранилища, а не игнорировал правила локального хранилища. Когда оба свойства ConnectionSecurityRulesFromGroupPolicyNotMerged и ConnectionSecurityRulesFromGroupPolicyMerged имеют значение true, приоритет имеет ConnectionSecurityRulesFromGroupPolicyMerged.|
|outboundConnectionsBlocked|Логический|Настраивает брандмауэр на блокировку всех исходящих подключений по умолчанию. Когда оба свойства OutboundConnectionsRequired и OutboundConnectionsBlocked имеют значение true, приоритет имеет OutboundConnectionsBlocked.|
|inboundConnectionsBlocked|Логический|Настраивает брандмауэр на блокировку всех входящих подключений по умолчанию. Когда оба свойства InboundConnectionsRequired и InboundConnectionsBlocked имеют значение true, приоритет имеет InboundConnectionsBlocked.|
|securedPacketExemptionAllowed|Логический|Настраивает брандмауэр таким образом, чтобы он разрешал главному компьютеру реагировать на незапрошенный сетевой трафик, защищенный с помощью IPsec, даже если для свойства stealthModeBlocked установлено значение True. Когда оба свойства SecuredPacketExemptionBlocked и SecuredPacketExemptionAllowed имеют значение true, приоритет имеет SecuredPacketExemptionAllowed.|
|policyRulesFromGroupPolicyMerged|Логический|Настраивает брандмауэр таким образом, чтобы он объединял политики правил брандмауэра из групповой политики с политиками из локального хранилища, а не игнорировал правила локального хранилища. Когда оба свойства PolicyRulesFromGroupPolicyNotMerged и PolicyRulesFromGroupPolicyMerged имеют значение true, приоритет имеет PolicyRulesFromGroupPolicyMerged.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsFirewallNetworkProfile",
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
}
```








