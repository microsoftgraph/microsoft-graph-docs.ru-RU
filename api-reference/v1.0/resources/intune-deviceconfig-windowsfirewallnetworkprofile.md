---
title: Тип ресурса windowsFirewallNetworkProfile
description: Политики профилей брандмауэра Windows.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3aa50d75a7e692e8393a6c01f46aaf4f3dc88912
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59072164"
---
# <a name="windowsfirewallnetworkprofile-resource-type"></a>Тип ресурса windowsFirewallNetworkProfile

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Политики профилей брандмауэра Windows.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|firewallEnabled|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|Настраивает хост-устройство, чтобы разрешить или заблокировать брандмауэр и усовершенствовать правоприменительных мер безопасности для сетевого профиля. Возможные значения: `notConfigured`, `blocked`, `allowed`.|
|stealthModeBlocked|Boolean|Запретить работе сервера в режиме стелс. Если stealthModeRequired и StealthModeBlocked являются верными, приоритет отнимает StealthModeBlocked.|
|incomingTrafficBlocked|Boolean|Настраивает брандмауэр для блокировки всего входящего трафика независимо от других параметров политики. Если значение IncomingTrafficRequired и IncomingTrafficBlocked является верным, приоритет отнимает incomingTrafficBlocked.|
|unicastResponsesToMulticastBroadcastsBlocked|Boolean|Настраивает брандмауэр, чтобы блокировать одноуровневые ответы на многокастный трафик передачи. Когда UnicastResponsesToMulticastBroadcastsRequired и UnicastResponsesToMulticastBroadcastsBlocked являются верными, UnicastResponsesToMulticastBroadcastsBlocked имеет приоритет.|
|inboundNotificationsBlocked|Boolean|Предотвращает отображение брандмауэром уведомлений при блокировке приложения в порту. Если inboundNotificationsRequired и InboundNotificationsBlocked являются верными, значение InboundNotificationsBlocked имеет приоритет.|
|authorizedApplicationRulesFromGroupPolicyMerged|Boolean|Настраивает брандмауэр для объединения правил авторизованного приложения из групповой политики с правилами локального магазина вместо игнорирования правил локального магазина. Если значение AuthorizedApplicationRulesFromGroupPolicyNotMerged и AuthorizedApplicationRulesFromGroupPolicyMerged являются верными, то в приоритете authorizedApplicationRulesFromGroupPolicyMerged.|
|globalPortRulesFromGroupPolicyMerged|Boolean|Настраивает брандмауэр для объединения глобальных правил порта из групповой политики с правилами локального магазина вместо игнорирования правил локального магазина. Если globalPortRulesFromGroupPolicyNotMerged и GlobalPortRulesFromGroupPolicyMerged являются верными, приоритет отнимает GlobalPortRulesFromGroupPolicyMerged.|
|connectionSecurityRulesFromGroupPolicyMerged|Boolean|Настраивает брандмауэр для объединения правил безопасности подключения из групповой политики с правилами локального магазина вместо игнорирования правил локального магазина. Если значение ConnectionSecurityRulesFromGroupPolicyNotMerged и ConnectionSecurityRulesFromGroupPolicyMerged являются верными, приоритет отнимает ConnectionSecurityRulesFromGroupPolicyMerged.|
|outboundConnectionsBlocked|Boolean|Настраивает брандмауэр для блокировки всех исходяющих подключений по умолчанию. Когда OutboundConnectionsRequired и OutboundConnectionsBlocked являются верными, OutboundConnectionsBlocked имеет приоритет. Этот параметр будет применен к Windows версии 1809 и выше.|
|inboundConnectionsBlocked|Boolean|Настраивает брандмауэр для блокировки всех входящих подключений по умолчанию. Если inboundConnectionsRequired и InboundConnectionsBlocked являются верными, входящиеConnectionsBlocked имеют приоритет.|
|securedPacketExemptionAllowed|Boolean|Настраивает брандмауэр, чтобы разрешить хост-компьютеру отвечать на нежелательный сетевой трафик этого трафика, защищенный IPSec, даже если установлено, что stealthModeBlocked является верным. Когда securedPacketExemptionBlocked и SecuredPacketExemptionAllowed являются верными, SecuredPacketExemptionAllowed имеет приоритет.|
|policyRulesFromGroupPolicyMerged|Boolean|Настраивает брандмауэр для объединения политик правил брандмауэра из групповой политики с политиками из локального магазина вместо игнорирования правил локального магазина. Если PolicyRulesFromGroupPolicyNotMerged и PolicyRulesFromGroupPolicyMerged являются верными, то PolicyRulesFromGroupPolicyMerged занимает приоритетное место.|

## <a name="relationships"></a>Отношения
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




