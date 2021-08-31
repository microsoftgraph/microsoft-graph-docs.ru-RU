---
title: Тип ресурса windowsFirewallNetworkProfile
description: Политики профилей брандмауэра Windows.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6bab7f12749d0467ac6435be23ee7a49dac89af6
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58802490"
---
# <a name="windowsfirewallnetworkprofile-resource-type"></a>Тип ресурса windowsFirewallNetworkProfile

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Политики профилей брандмауэра Windows.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|firewallEnabled|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|Настраивает хост-устройство, чтобы разрешить или заблокировать брандмауэр и усовершенствовать правоприменительных мер безопасности для сетевого профиля. Возможные значения: `notConfigured`, `blocked`, `allowed`.|
|stealthModeRequired|Логический|Разрешить серверу работать в режиме стелс. Если stealthModeRequired и StealthModeBlocked являются верными, приоритет отнимает StealthModeBlocked.|
|stealthModeBlocked|Boolean|Запретить работе сервера в режиме стелс. Если stealthModeRequired и StealthModeBlocked являются верными, приоритет отнимает StealthModeBlocked.|
|incomingTrafficRequired|Логический|Настраивает брандмауэр, чтобы разрешить входящий трафик в соответствии с другими настройками политики. Если значение IncomingTrafficRequired и IncomingTrafficBlocked является верным, приоритет отнимает incomingTrafficBlocked.|
|incomingTrafficBlocked|Boolean|Настраивает брандмауэр для блокировки всего входящего трафика независимо от других параметров политики. Если значение IncomingTrafficRequired и IncomingTrafficBlocked является верным, приоритет отнимает incomingTrafficBlocked.|
|unicastResponsesToMulticastBroadcastsRequired|Логический|Настраивает брандмауэр, чтобы разрешить одноуровневые ответы на многокастный трафик трансляции. Когда UnicastResponsesToMulticastBroadcastsRequired и UnicastResponsesToMulticastBroadcastsBlocked являются верными, UnicastResponsesToMulticastBroadcastsBlocked имеет приоритет.|
|unicastResponsesToMulticastBroadcastsBlocked|Boolean|Настраивает брандмауэр, чтобы блокировать одноуровневые ответы на многокастный трафик передачи. Когда UnicastResponsesToMulticastBroadcastsRequired и UnicastResponsesToMulticastBroadcastsBlocked являются верными, UnicastResponsesToMulticastBroadcastsBlocked имеет приоритет.|
|inboundNotificationsRequired|Boolean|Позволяет брандмауэру отображать уведомления, если приложение заблокировано для прослушивания в порту. Если inboundNotificationsRequired и InboundNotificationsBlocked являются верными, значение InboundNotificationsBlocked имеет приоритет.|
|inboundNotificationsBlocked|Boolean|Предотвращает отображение брандмауэром уведомлений при блокировке приложения в порту. Если inboundNotificationsRequired и InboundNotificationsBlocked являются верными, значение InboundNotificationsBlocked имеет приоритет.|
|authorizedApplicationRulesFromGroupPolicyMerged|Boolean|Настраивает брандмауэр для объединения правил авторизованного приложения из групповой политики с правилами локального магазина вместо игнорирования правил локального магазина. Если значение AuthorizedApplicationRulesFromGroupPolicyNotMerged и AuthorizedApplicationRulesFromGroupPolicyMerged являются верными, то в приоритете authorizedApplicationRulesFromGroupPolicyMerged.|
|authorizedApplicationRulesFromGroupPolicyNotMerged|Логический|Настраивает брандмауэр, чтобы предотвратить объединение правил авторизованного приложения из групповой политики с политиками из локального магазина, а не игнорировать правила локального магазина. Если значение AuthorizedApplicationRulesFromGroupPolicyNotMerged и AuthorizedApplicationRulesFromGroupPolicyMerged являются верными, то в приоритете authorizedApplicationRulesFromGroupPolicyMerged.|
|globalPortRulesFromGroupPolicyMerged|Boolean|Настраивает брандмауэр для объединения глобальных правил порта из групповой политики с правилами локального магазина вместо игнорирования правил локального магазина. Если globalPortRulesFromGroupPolicyNotMerged и GlobalPortRulesFromGroupPolicyMerged являются верными, приоритет отнимает GlobalPortRulesFromGroupPolicyMerged.|
|globalPortRulesFromGroupPolicyNotMerged|Логический|Настраивает брандмауэр, чтобы предотвратить объединение глобальных правил порта с групповой политикой с политиками из локального магазина, а не игнорировать правила локального магазина. Если globalPortRulesFromGroupPolicyNotMerged и GlobalPortRulesFromGroupPolicyMerged являются верными, приоритет отнимает GlobalPortRulesFromGroupPolicyMerged.|
|connectionSecurityRulesFromGroupPolicyMerged|Boolean|Настраивает брандмауэр для объединения правил безопасности подключения из групповой политики с правилами локального магазина вместо игнорирования правил локального магазина. Если значение ConnectionSecurityRulesFromGroupPolicyNotMerged и ConnectionSecurityRulesFromGroupPolicyMerged являются верными, приоритет отнимает ConnectionSecurityRulesFromGroupPolicyMerged.|
|connectionSecurityRulesFromGroupPolicyNotMerged|Логический|Настраивает брандмауэр, чтобы предотвратить слияние правил безопасности подключения с групповой политикой с политиками локального магазина, а не игнорировать правила локального магазина. Если значение ConnectionSecurityRulesFromGroupPolicyNotMerged и ConnectionSecurityRulesFromGroupPolicyMerged являются верными, приоритет отнимает ConnectionSecurityRulesFromGroupPolicyMerged.|
|outboundConnectionsRequired|Логический|Настраивает брандмауэр, чтобы разрешить все исходяющие подключения по умолчанию. Когда OutboundConnectionsRequired и OutboundConnectionsBlocked являются верными, OutboundConnectionsBlocked имеет приоритет. Этот параметр будет применен к Windows версии 1809 и выше.|
|outboundConnectionsBlocked|Boolean|Настраивает брандмауэр для блокировки всех исходяющих подключений по умолчанию. Когда OutboundConnectionsRequired и OutboundConnectionsBlocked являются верными, OutboundConnectionsBlocked имеет приоритет. Этот параметр будет применен к Windows версии 1809 и выше.|
|inboundConnectionsRequired|Логический|Настраивает брандмауэр, чтобы разрешить все входящие подключения по умолчанию. Если inboundConnectionsRequired и InboundConnectionsBlocked являются верными, входящиеConnectionsBlocked имеют приоритет.|
|inboundConnectionsBlocked|Boolean|Настраивает брандмауэр для блокировки всех входящих подключений по умолчанию. Если inboundConnectionsRequired и InboundConnectionsBlocked являются верными, входящиеConnectionsBlocked имеют приоритет.|
|securedPacketExemptionAllowed|Boolean|Настраивает брандмауэр, чтобы разрешить хост-компьютеру отвечать на нежелательный сетевой трафик этого трафика, защищенный IPSec, даже если установлено, что stealthModeBlocked является верным. Когда securedPacketExemptionBlocked и SecuredPacketExemptionAllowed являются верными, SecuredPacketExemptionAllowed имеет приоритет.|
|securedPacketExemptionBlocked|Boolean|Настраивает брандмауэр, чтобы заблокировать хост-компьютер, чтобы реагировать на нежелательный сетевой трафик этого трафика, защищенный IPSec, даже если задана истина stealthModeBlocked. Когда securedPacketExemptionBlocked и SecuredPacketExemptionAllowed являются верными, SecuredPacketExemptionAllowed имеет приоритет.|
|policyRulesFromGroupPolicyMerged|Boolean|Настраивает брандмауэр для объединения политик правил брандмауэра из групповой политики с политиками из локального магазина вместо игнорирования правил локального магазина. Если PolicyRulesFromGroupPolicyNotMerged и PolicyRulesFromGroupPolicyMerged являются верными, то PolicyRulesFromGroupPolicyMerged занимает приоритетное место.|
|policyRulesFromGroupPolicyNotMerged|Логический|Настраивает брандмауэр, чтобы исключить объединение политик правил брандмауэра из групповой политики с политиками из локального магазина, а не игнорировать правила локального магазина. Если PolicyRulesFromGroupPolicyNotMerged и PolicyRulesFromGroupPolicyMerged являются верными, то PolicyRulesFromGroupPolicyMerged занимает приоритетное место.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsFirewallNetworkProfile",
  "firewallEnabled": "String",
  "stealthModeRequired": true,
  "stealthModeBlocked": true,
  "incomingTrafficRequired": true,
  "incomingTrafficBlocked": true,
  "unicastResponsesToMulticastBroadcastsRequired": true,
  "unicastResponsesToMulticastBroadcastsBlocked": true,
  "inboundNotificationsRequired": true,
  "inboundNotificationsBlocked": true,
  "authorizedApplicationRulesFromGroupPolicyMerged": true,
  "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
  "globalPortRulesFromGroupPolicyMerged": true,
  "globalPortRulesFromGroupPolicyNotMerged": true,
  "connectionSecurityRulesFromGroupPolicyMerged": true,
  "connectionSecurityRulesFromGroupPolicyNotMerged": true,
  "outboundConnectionsRequired": true,
  "outboundConnectionsBlocked": true,
  "inboundConnectionsRequired": true,
  "inboundConnectionsBlocked": true,
  "securedPacketExemptionAllowed": true,
  "securedPacketExemptionBlocked": true,
  "policyRulesFromGroupPolicyMerged": true,
  "policyRulesFromGroupPolicyNotMerged": true
}
```



