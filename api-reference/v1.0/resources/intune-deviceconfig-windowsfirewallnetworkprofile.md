---
title: Тип ресурса windowsFirewallNetworkProfile
description: Политики профилей брандмауэра Windows.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 75e76e0cd4789f8e2f760d0bdc423fe15378ed67
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867034"
---
# <a name="windowsfirewallnetworkprofile-resource-type"></a>Тип ресурса windowsFirewallNetworkProfile

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Политики профилей брандмауэра Windows.
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|firewallEnabled|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|Настройка устройства узла разрешить или заблокировать брандмауэра и принудительное применение повышенной безопасности для сетевого профиля. Возможные значения: `notConfigured`, `blocked`, `allowed`.|
|stealthModeBlocked|Boolean|Запретить сервера на работе в скрытом режиме. Когда StealthModeRequired и StealthModeBlocked являются оба имеет значение true, StealthModeBlocked приоритет.|
|incomingTrafficBlocked|Boolean|Настраивает брандмауэр блокирует весь входящий трафик вне зависимости от других параметров политики. Когда IncomingTrafficRequired и IncomingTrafficBlocked являются оба имеет значение true, IncomingTrafficBlocked приоритет.|
|unicastResponsesToMulticastBroadcastsBlocked|Boolean|Настройка брандмауэра для блокировки одноадресные ответы на многоадресной рассылки широковещательного трафика. Когда UnicastResponsesToMulticastBroadcastsRequired и UnicastResponsesToMulticastBroadcastsBlocked являются оба имеет значение true, UnicastResponsesToMulticastBroadcastsBlocked приоритет.|
|inboundNotificationsBlocked|Boolean|Запрещает отображение уведомлений о блокировании приложения прослушивает порт брандмауэра. Когда InboundNotificationsRequired и InboundNotificationsBlocked являются оба имеет значение true, InboundNotificationsBlocked приоритет.|
|authorizedApplicationRulesFromGroupPolicyMerged|Boolean|Настройка брандмауэра для объединения правил авторизованного приложения из групповой политики с учетными записями из локального хранилища вместо без учета правил локального хранилища. Когда AuthorizedApplicationRulesFromGroupPolicyNotMerged и AuthorizedApplicationRulesFromGroupPolicyMerged являются оба имеет значение true, AuthorizedApplicationRulesFromGroupPolicyMerged приоритет.|
|globalPortRulesFromGroupPolicyMerged|Boolean|Настройка брандмауэра для объединения глобальным правила групповой политики с учетными записями из локального хранилища вместо без учета правил локального хранилища. Когда GlobalPortRulesFromGroupPolicyNotMerged и GlobalPortRulesFromGroupPolicyMerged являются оба имеет значение true, GlobalPortRulesFromGroupPolicyMerged приоритет.|
|connectionSecurityRulesFromGroupPolicyMerged|Boolean|Настройка брандмауэра для объединения правил безопасности подключения из групповой политики с учетными записями из локального хранилища вместо без учета правил локального хранилища. Когда ConnectionSecurityRulesFromGroupPolicyNotMerged и ConnectionSecurityRulesFromGroupPolicyMerged являются оба имеет значение true, ConnectionSecurityRulesFromGroupPolicyMerged приоритет.|
|outboundConnectionsBlocked|Boolean|Настройка брандмауэра для блокирования всех исходящих подключений по умолчанию. Когда OutboundConnectionsRequired и OutboundConnectionsBlocked являются оба имеет значение true, OutboundConnectionsBlocked приоритет.|
|inboundConnectionsBlocked|Boolean|Настраивает брандмауэр блокирует все входящие подключения по умолчанию. Когда InboundConnectionsRequired и InboundConnectionsBlocked являются оба имеет значение true, InboundConnectionsBlocked приоритет.|
|securedPacketExemptionAllowed|Boolean|Настраивает брандмауэр, чтобы разрешить главном компьютере реагировать на нежелательных сетевого трафика из защитой трафика по протоколу IPSec даже в том случае, если stealthModeBlocked установлено значение true. Когда SecuredPacketExemptionBlocked и SecuredPacketExemptionAllowed являются оба имеет значение true, SecuredPacketExemptionAllowed приоритет.|
|policyRulesFromGroupPolicyMerged|Boolean|Настройка брандмауэра для объединения правило брандмауэра политик из групповой политики с учетными записями из локального хранилища вместо без учета правил локального хранилища. Когда PolicyRulesFromGroupPolicyNotMerged и PolicyRulesFromGroupPolicyMerged являются оба имеет значение true, PolicyRulesFromGroupPolicyMerged приоритет.|

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



