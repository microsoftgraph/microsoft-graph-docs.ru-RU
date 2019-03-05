---
title: Тип ресурса windowsFirewallNetworkProfile
description: Политики профилей брандмауэра Windows.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3e52555d8ac9b010028ee3bc716255db8a563e73
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250959"
---
# <a name="windowsfirewallnetworkprofile-resource-type"></a>Тип ресурса windowsFirewallNetworkProfile

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Политики профилей брандмауэра Windows.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|firewallEnabled|[Статеманажементсеттинг](../resources/intune-deviceconfig-statemanagementsetting.md)|НаСтраивает ведущее устройство на разрешение или блокировку брандмауэра и дополнительной безопасности для профиля сети. Возможные значения: `notConfigured`, `blocked`, `allowed`.|
|stealthModeBlocked|Логический|Предотвращение работы сервера в скрытом режиме. Если для Стеалсмодерекуиред и Стеалсмодеблоккед задано значение true, Стеалсмодеблоккед имеет приоритет.|
|incomingTrafficBlocked|Логический|НаСтраивает брандмауэр на блокировку всего входящего трафика независимо от других параметров политики. Если для Инкомингтраффикрекуиред и Инкомингтраффикблоккед задано значение true, Инкомингтраффикблоккед имеет приоритет.|
|unicastResponsesToMulticastBroadcastsBlocked|Логический|НаСтраивает брандмауэр для блокировки одноадресных ответов на многоадресный широковещательный трафик. Если для Уникастреспонсестомултикастброадкастсрекуиред и Уникастреспонсестомултикастброадкастсблоккед задано значение true, UnicastResponsesToMulticastBroadcastsBlocked имеет приоритет.|
|inboundNotificationsBlocked|Логический|Запрещает брандмауэру отображать уведомления, если приложение заблокировано для прослушивания порта. Если для Инбаунднотификатионсрекуиред и Инбаунднотификатионсблоккед задано значение true, Инбаунднотификатионсблоккед имеет приоритет.|
|authorizedApplicationRulesFromGroupPolicyMerged|Логический|НаСтраивает брандмауэр для объединения авторизованных правил приложений из групповой политики с элементами из локального хранилища, а не без учета правил локального хранилища. Если для Аусоризедаппликатионрулесфромграупполицинотмержед и Аусоризедаппликатионрулесфромграупполицимержед задано значение true, AuthorizedApplicationRulesFromGroupPolicyMerged имеет приоритет.|
|globalPortRulesFromGroupPolicyMerged|Логический|НаСтраивает брандмауэр для объединения глобальных правил портов из групповой политики с политиками из локального хранилища, а не без учета правил локального хранилища. Если для Глобалпортрулесфромграупполицинотмержед и Глобалпортрулесфромграупполицимержед задано значение true, GlobalPortRulesFromGroupPolicyMerged имеет приоритет.|
|connectionSecurityRulesFromGroupPolicyMerged|Логический|НаСтраивает брандмауэр для объединения правил безопасности подключений из групповой политики с политиками из локального хранилища, а не без учета правил локального хранилища. Если для Коннектионсекуритирулесфромграупполицинотмержед и Коннектионсекуритирулесфромграупполицимержед задано значение true, ConnectionSecurityRulesFromGroupPolicyMerged имеет приоритет.|
|outboundConnectionsBlocked|Логический|НаСтраивает брандмауэр на блокировку всех исходящих подключений по умолчанию. Если для Аутбаундконнектионсрекуиред и Аутбаундконнектионсблоккед задано значение true, Аутбаундконнектионсблоккед имеет приоритет.|
|inboundConnectionsBlocked|Логический|НаСтраивает брандмауэр на блокировку всех входящих подключений по умолчанию. Если для Инбаундконнектионсрекуиред и Инбаундконнектионсблоккед задано значение true, Инбаундконнектионсблоккед имеет приоритет.|
|securedPacketExemptionAllowed|Логический|НаСтраивает брандмауэр, чтобы разрешить ведущему компьютеру отвечать на нежелательный сетевой трафик этого трафика, защищенный IPSec, даже если для Стеалсмодеблоккед задано значение true. Если для Секуредпаккетексемптионблоккед и Секуредпаккетексемптионалловед задано значение true, Секуредпаккетексемптионалловед имеет приоритет.|
|policyRulesFromGroupPolicyMerged|Boolean|НаСтраивает брандмауэр для объединения политик правил брандмауэра из групповой политики с политиками из локального хранилища, а не без учета правил локального хранилища. Если для Полицирулесфромграупполицинотмержед и Полицирулесфромграупполицимержед задано значение true, Полицирулесфромграупполицимержед имеет приоритет.|

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



