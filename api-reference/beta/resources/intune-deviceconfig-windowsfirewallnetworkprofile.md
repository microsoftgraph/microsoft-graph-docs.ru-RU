---
title: Тип ресурса windowsFirewallNetworkProfile
description: Политики профилей брандмауэра Windows.
author: tfitzmac
ms.openlocfilehash: ff128f004626d846ae27815b656522607cb3a07c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27358361"
---
# <a name="windowsfirewallnetworkprofile-resource-type"></a>Тип ресурса windowsFirewallNetworkProfile

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Политики профилей брандмауэра Windows.
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|firewallEnabled|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|Настройка устройства узла разрешить или заблокировать брандмауэра и принудительное применение повышенной безопасности для сетевого профиля. Возможные значения: `notConfigured`, `blocked`, `allowed`.|
|stealthModeRequired|Boolean.|Разрешить серверу работать в скрытом режиме. Когда StealthModeRequired и StealthModeBlocked являются оба имеет значение true, StealthModeBlocked приоритет.|
|stealthModeBlocked|Boolean|Запретить сервера на работе в скрытом режиме. Когда StealthModeRequired и StealthModeBlocked являются оба имеет значение true, StealthModeBlocked приоритет.|
|incomingTrafficRequired|Boolean.|Настройка брандмауэра для разрешения входящего трафика этих других параметров политики. Когда IncomingTrafficRequired и IncomingTrafficBlocked являются оба имеет значение true, IncomingTrafficBlocked приоритет.|
|incomingTrafficBlocked|Boolean|Настраивает брандмауэр блокирует весь входящий трафик вне зависимости от других параметров политики. Когда IncomingTrafficRequired и IncomingTrafficBlocked являются оба имеет значение true, IncomingTrafficBlocked приоритет.|
|unicastResponsesToMulticastBroadcastsRequired|Boolean.|Настройка брандмауэра, чтобы разрешить одноадресные ответы на многоадресной рассылки широковещательных. Когда UnicastResponsesToMulticastBroadcastsRequired и UnicastResponsesToMulticastBroadcastsBlocked являются оба имеет значение true, UnicastResponsesToMulticastBroadcastsBlocked приоритет.|
|unicastResponsesToMulticastBroadcastsBlocked|Boolean|Настройка брандмауэра для блокировки одноадресные ответы на многоадресной рассылки широковещательного трафика. Когда UnicastResponsesToMulticastBroadcastsRequired и UnicastResponsesToMulticastBroadcastsBlocked являются оба имеет значение true, UnicastResponsesToMulticastBroadcastsBlocked приоритет.|
|inboundNotificationsRequired|Boolean.|Разрешает брандмауэра для отображения уведомления, когда приложение запретом прослушивает порт. Когда InboundNotificationsRequired и InboundNotificationsBlocked являются оба имеет значение true, InboundNotificationsBlocked приоритет.|
|inboundNotificationsBlocked|Boolean|Запрещает отображение уведомлений о блокировании приложения прослушивает порт брандмауэра. Когда InboundNotificationsRequired и InboundNotificationsBlocked являются оба имеет значение true, InboundNotificationsBlocked приоритет.|
|authorizedApplicationRulesFromGroupPolicyMerged|Boolean|Настройка брандмауэра для объединения правил авторизованного приложения из групповой политики с учетными записями из локального хранилища вместо без учета правил локального хранилища. Когда AuthorizedApplicationRulesFromGroupPolicyNotMerged и AuthorizedApplicationRulesFromGroupPolicyMerged являются оба имеет значение true, AuthorizedApplicationRulesFromGroupPolicyMerged приоритет.|
|authorizedApplicationRulesFromGroupPolicyNotMerged|Boolean.|Настраивает брандмауэр для предотвращения слияние авторизованных приложений правила групповой политики с учетными записями из локального хранилища вместо без учета локального хранения правил. Когда AuthorizedApplicationRulesFromGroupPolicyNotMerged и AuthorizedApplicationRulesFromGroupPolicyMerged являются оба имеет значение true, AuthorizedApplicationRulesFromGroupPolicyMerged приоритет.|
|globalPortRulesFromGroupPolicyMerged|Boolean|Настройка брандмауэра для объединения глобальным правила групповой политики с учетными записями из локального хранилища вместо без учета правил локального хранилища. Когда GlobalPortRulesFromGroupPolicyNotMerged и GlobalPortRulesFromGroupPolicyMerged являются оба имеет значение true, GlobalPortRulesFromGroupPolicyMerged приоритет.|
|globalPortRulesFromGroupPolicyNotMerged|Boolean.|Настройка брандмауэра для предотвращения объединение глобальным правила групповой политики с учетными записями из локального хранилища вместо без учета правил локального хранилища. Когда GlobalPortRulesFromGroupPolicyNotMerged и GlobalPortRulesFromGroupPolicyMerged являются оба имеет значение true, GlobalPortRulesFromGroupPolicyMerged приоритет.|
|connectionSecurityRulesFromGroupPolicyMerged|Boolean|Настройка брандмауэра для объединения правил безопасности подключения из групповой политики с учетными записями из локального хранилища вместо без учета правил локального хранилища. Когда ConnectionSecurityRulesFromGroupPolicyNotMerged и ConnectionSecurityRulesFromGroupPolicyMerged являются оба имеет значение true, ConnectionSecurityRulesFromGroupPolicyMerged приоритет.|
|connectionSecurityRulesFromGroupPolicyNotMerged|Boolean.|Настраивает брандмауэр для предотвращения объединение правила безопасности подключения из групповой политики с учетными записями из локального хранилища вместо без учета локального хранения правил. Когда ConnectionSecurityRulesFromGroupPolicyNotMerged и ConnectionSecurityRulesFromGroupPolicyMerged являются оба имеет значение true, ConnectionSecurityRulesFromGroupPolicyMerged приоритет.|
|outboundConnectionsRequired|Boolean.|Настройка брандмауэра, чтобы разрешить всех исходящих подключений по умолчанию. Когда OutboundConnectionsRequired и OutboundConnectionsBlocked являются оба имеет значение true, OutboundConnectionsBlocked приоритет.|
|outboundConnectionsBlocked|Boolean|Настройка брандмауэра для блокирования всех исходящих подключений по умолчанию. Когда OutboundConnectionsRequired и OutboundConnectionsBlocked являются оба имеет значение true, OutboundConnectionsBlocked приоритет.|
|inboundConnectionsRequired|Boolean.|Настройка брандмауэра, чтобы разрешить всех входящих подключений по умолчанию. Когда InboundConnectionsRequired и InboundConnectionsBlocked являются оба имеет значение true, InboundConnectionsBlocked приоритет.|
|inboundConnectionsBlocked|Boolean|Настраивает брандмауэр блокирует все входящие подключения по умолчанию. Когда InboundConnectionsRequired и InboundConnectionsBlocked являются оба имеет значение true, InboundConnectionsBlocked приоритет.|
|securedPacketExemptionAllowed|Boolean|Настраивает брандмауэр, чтобы разрешить главном компьютере реагировать на нежелательных сетевого трафика из защитой трафика по протоколу IPSec даже в том случае, если stealthModeBlocked установлено значение true. Когда SecuredPacketExemptionBlocked и SecuredPacketExemptionAllowed являются оба имеет значение true, SecuredPacketExemptionAllowed приоритет.|
|securedPacketExemptionBlocked|Boolean.|Настраивает брандмауэр блокирует компьютер узла для ответа нежелательных сетевого трафика из защитой трафика по протоколу IPSec даже в том случае, если установлено stealthModeBlocked имеет значение true. Когда SecuredPacketExemptionBlocked и SecuredPacketExemptionAllowed являются оба имеет значение true, SecuredPacketExemptionAllowed приоритет.|
|policyRulesFromGroupPolicyMerged|Boolean|Настройка брандмауэра для объединения правило брандмауэра политик из групповой политики с учетными записями из локального хранилища вместо без учета правил локального хранилища. Когда PolicyRulesFromGroupPolicyNotMerged и PolicyRulesFromGroupPolicyMerged являются оба имеет значение true, PolicyRulesFromGroupPolicyMerged приоритет.|
|policyRulesFromGroupPolicyNotMerged|Boolean.|Настраивает брандмауэр для предотвращения объединение правило брандмауэра политик из групповой политики с учетными записями из локального хранилища вместо без учета локального хранения правил. Когда PolicyRulesFromGroupPolicyNotMerged и PolicyRulesFromGroupPolicyMerged являются оба имеет значение true, PolicyRulesFromGroupPolicyMerged приоритет.|

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





