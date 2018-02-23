# <a name="windowsfirewallnetworkprofile-resource-type"></a>Тип ресурса windowsFirewallNetworkProfile

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Политики профилей брандмауэра Windows.
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|firewallEnabled|String|Включение брандмауэра и применение расширенных параметров безопасности. Возможные значения: `notConfigured`, `blocked`, `allowed`.|
|stealthModeBlocked|Boolean|Предотвращение работы сервера в скрытом режиме.|
|incomingTrafficBlocked|Boolean|Настраивает брандмауэр на блокировку всего входящего трафика вне зависимости от параметров политики.|
|unicastResponsesToMulticastBroadcastsBlocked|Boolean|Настраивает брандмауэр на блокировку одноадресных откликов на многоадресный широковещательный трафик.|
|inboundNotificationsBlocked|Boolean|Предотвращает отображение в брандмауэре уведомлений о том, что для приложения заблокирована возможность прослушивания порта.|
|authorizedApplicationRulesFromGroupPolicyMerged|Boolean|Настраивает брандмауэр таким образом, чтобы он объединял правила для авторизованных приложений из групповой политики с правилами из локального хранилища, а не игнорировал правила локального хранилища.|
|globalPortRulesFromGroupPolicyMerged|Boolean|Настраивает брандмауэр таким образом, чтобы он объединял глобальные правила для портов из групповой политики с правилами из локального хранилища, а не игнорировал правила локального хранилища.|
|connectionSecurityRulesFromGroupPolicyMerged|Boolean|Настраивает брандмауэр таким образом, чтобы он объединял правила безопасности подключений из групповой политики с правилами из локального хранилища, а не игнорировал правила локального хранилища.|
|outboundConnectionsBlocked|Boolean|Настраивает брандмауэр на блокировку всех исходящих подключений по умолчанию.|
|inboundConnectionsBlocked|Boolean|Настраивает брандмауэр на блокировку всех входящих подключений по умолчанию.|
|securedPacketExemptionAllowed|Boolean|Настраивает брандмауэр таким образом, чтобы он разрешал главному компьютеру реагировать на незапрошенный сетевой трафик, защищенный с помощью IPsec, даже если для свойства stealthModeBlocked установлено значение True.|
|policyRulesFromGroupPolicyMerged|Boolean|Настраивает брандмауэр таким образом, чтобы он объединял политики правил брандмауэра из групповой политики с политиками из локального хранилища, а не игнорировал правила локального хранилища.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile"
}
-->
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



