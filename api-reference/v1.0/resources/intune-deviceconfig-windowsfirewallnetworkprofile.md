---
title: Тип ресурса windowsFirewallNetworkProfile
description: Политики профилей брандмауэра Windows.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9ed6011844daedc5fe4140b04851605529921c99
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/12/2022
ms.locfileid: "66730002"
---
# <a name="windowsfirewallnetworkprofile-resource-type"></a>Тип ресурса windowsFirewallNetworkProfile

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Политики профилей брандмауэра Windows.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|firewallEnabled|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|Настраивает хост-устройство для разрешения или блокировки брандмауэра и расширенного применения безопасности для сетевого профиля. Возможные значения: `notConfigured`, `blocked`, `allowed`.|
|stealthModeBlocked|Boolean|Запретить работе сервера в скрытом режиме. Если свойства StealthModeRequired и StealthModeBlocked имеют значение true, Свойство StealthModeBlocked имеет приоритет.|
|incomingTrafficBlocked|Boolean|Настраивает брандмауэр для блокировки всего входящего трафика независимо от других параметров политики. Если incomingTrafficRequired и IncomingTrafficBlocked имеют значение true, incomingTrafficBlocked имеет приоритет.|
|unicastResponsesToMulticastBroadcastsBlocked|Boolean|Настраивает брандмауэр для блокировки одноадресных ответов на многоадресный широковещательный трафик. Если свойства UnicastResponsesToMulticastBroadcastsRequired и UnicastResponsesToMulticastBroadcastsBlocked имеют значение true, приоритет имеет UnicastResponsesToMulticastBroadcastsBlocked.|
|inboundNotificationsBlocked|Boolean|Запрещает брандмауэру отображать уведомления, когда приложению запрещено прослушивать порт. Если inboundNotificationsRequired и InboundNotificationsBlocked имеют значение true, InboundNotificationsBlocked имеет приоритет.|
|authorizedApplicationRulesFromGroupPolicyMerged|Boolean|Настраивает брандмауэр для слияния правил авторизованных приложений из групповой политики с правилами из локального хранилища вместо игнорирования правил локального хранилища. Если значения AuthorizedApplicationRulesFromGroupPolicyNotMerged и AuthorizedApplicationRulesFromGroupPolicyMerged имеют значение true, приоритет имеет AuthorizedApplicationRulesFromGroupPolicyMerged.|
|globalPortRulesFromGroupPolicyMerged|Boolean|Настраивает брандмауэр для объединения глобальных правил портов из групповой политики с правилами из локального хранилища вместо игнорирования правил локального хранилища. Если globalPortRulesFromGroupPolicyNotMerged и GlobalPortRulesFromGroupPolicyMerged имеют значение true, GlobalPortRulesFromGroupPolicyMerged имеет приоритет.|
|connectionSecurityRulesFromGroupPolicyMerged|Boolean|Настраивает брандмауэр для объединения правил безопасности подключения из групповой политики с правилами из локального хранилища вместо игнорирования правил локального хранилища. Если значения ConnectionSecurityRulesFromGroupPolicyNotMerged и ConnectionSecurityRulesFromGroupPolicyMerged имеют значение true, приоритет имеет ConnectionSecurityRulesFromGroupPolicyMerged.|
|outboundConnectionsBlocked|Boolean|Настраивает брандмауэр для блокировки всех исходящих подключений по умолчанию. Если параметры OutboundConnectionsRequired и OutboundConnectionsBlocked имеют значение true, outboundConnectionsBlocked имеет приоритет. Этот параметр будет применен к выпускам Windows версии 1809 и более поздних.|
|inboundConnectionsBlocked|Boolean|Настраивает брандмауэр для блокировки всех входящих подключений по умолчанию. Если inboundConnectionsRequired и InboundConnectionsBlocked имеют значение true, то inboundConnectionsBlocked имеет приоритет.|
|securedPacketExemptionAllowed|Boolean|Настраивает брандмауэр, чтобы разрешить хост-компьютеру реагировать на нежелательный сетевой трафик, защищенный IPSec, даже если свойство stealthModeBlocked имеет значение true. Если параметры SecuredPacketExemptionBlocked и SecuredPacketExemptionAllowed имеют значение true, Приоритет имеет SecuredPacketExemptionAllowed.|
|policyRulesFromGroupPolicyMerged|Boolean|Настраивает брандмауэр для слияния политик правил брандмауэра из групповой политики с политиками из локального хранилища вместо игнорирования правил локального хранилища. Если policyRulesFromGroupPolicyNotMerged и PolicyRulesFromGroupPolicyMerged имеют значение true, PolicyRulesFromGroupPolicyMerged имеет приоритет.|

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





