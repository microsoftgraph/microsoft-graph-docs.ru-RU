---
title: тип ресурса windowsFirewallRule
description: Правило, управляющее трафиком Windows брандмауэра.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ead732e65cf3119f974f2fa6b29da14cc3dd180b1211dcba1a5dd1db90cc71eb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54251409"
---
# <a name="windowsfirewallrule-resource-type"></a>тип ресурса windowsFirewallRule

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Правило, управляющее трафиком Windows брандмауэра.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Отображаемое имя правила. Не нужно быть уникальным.|
|description|Строка|Описание правила.|
|packageFamilyName|Строка|Семейство пакетов приложения Microsoft Store, на которое влияет правило брандмауэра.|
|filePath|Строка|Полный путь файла приложения, на которое влияет правило брандмауэра.|
|serviceName|Строка|Имя, используемая в случаях, когда служба, а не приложение отправляет или получает трафик.|
|протокол|Int32|Номер 0-255, представляющий протокол IP (TCP = 6, UDP = 17). Если не указано, по умолчанию — все. Допустимые значения от 0 до 255|
|localPortRanges|Коллекция String|Список локальных диапазонов портов. Например, "100-120", "200", "300-320". Если не указано, по умолчанию — все.|
|remotePortRanges|Коллекция String|Список диапазонов удаленных портов. Например, "100-120", "200", "300-320". Если не указано, по умолчанию — все.|
|localAddressRanges|Коллекция String|Список локальных адресов, охваченных правилом. По умолчанию это любой адрес. Допустимые маркеры:<ul><li>"*" указывает любой локальный адрес. Если она присутствует, это должен быть единственный включенный маркер.</li><li>Подсеть можно указать с помощью маски подсети или сетевой префикс. Если не указана ни подсетевая маска, ни сетевой префикс, маска подсети по умолчанию указывает значение 255.255.255.255.255.</li><li>Допустимый адрес IPv6.</li><li>Диапазон адресов IPv4 в формате "начните адрес - конечный адрес" без пробелов.</li><li>Диапазон адресов IPv6 в формате "начните адрес - конечный адрес" без пробелов.</li></ul>|
|remoteAddressRanges|Коллекция String|Список маркеров с указанием удаленных адресов, охваченных правилом. Маркеры являются нечувствительными. По умолчанию это любой адрес. Допустимые маркеры:<ul><li>"*" указывает любой удаленный адрес. Если она присутствует, это должен быть единственный включенный маркер.</li><li>"Defaultgateway"</li><li>"DHCP"</li><li>"DNS"</li><li>"WINS"</li><li>"Интрасеть" (поддерживается Windows версии 1809+)</li><li>"RmtIntranet" (поддерживается Windows версии 1809+)</li><li>"Internet" (поддерживается Windows версии 1809+)</li><li>"Ply2Renders" (поддерживается Windows версии 1809+)</li><li>"LocalSubnet" указывает любой локальный адрес в локальной подсети.</li><li>Подсеть можно указать с помощью маски подсети или сетевой префикс. Если не указана ни подсетевая маска, ни сетевой префикс, маска подсети по умолчанию указывает значение 255.255.255.255.255.</li><li>Допустимый адрес IPv6.</li><li>Диапазон адресов IPv4 в формате "начните адрес - конечный адрес" без пробелов.</li><li>Диапазон адресов IPv6 в формате "начните адрес - конечный адрес" без пробелов.</li></ul>|
|profileTypes|[windowsFirewallRuleNetworkProfileTypes](../resources/intune-deviceconfig-windowsfirewallrulenetworkprofiletypes.md)|Указывает профили, к которым относится правило. Если не указано, по умолчанию — все. Возможные значения: `notConfigured`, `domain`, `private`, `public`.|
|action|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|Действие, применяемая правилом. Если не указано, по умолчанию разрешено. Возможные значения: `notConfigured`, `blocked`, `allowed`.|
|trafficDirection|[windowsFirewallRuleTrafficDirectionType](../resources/intune-deviceconfig-windowsfirewallruletrafficdirectiontype.md)|Направление трафика, для которое включено правило. Если не указано, по умолчанию значение Out. Возможные значения: `notConfigured` , `out` , `in` .|
|interfaceTypes|[windowsFirewallRuleInterfaceTypes](../resources/intune-deviceconfig-windowsfirewallruleinterfacetypes.md)|Типы интерфейса правила. Возможные значения: `notConfigured`, `remoteAccess`, `wireless`, `lan`.|
|edgeTraversal|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|Указывает, включен ли обход края для этого правила или отключен. Параметр EdgeTraversal указывает на то, что определенному входящего трафика разрешено туннель через NATs и другие устройства края с помощью технологии туннеля Teredo. Чтобы этот параметр работал правильно, приложение или служба с правилом входящего брандмауэра должны поддерживать IPv6. Основное применение этого параметра позволяет слушателям на хосте быть глобально адресируемыми с помощью адреса Teredo IPv6. В новых правилах свойство EdgeTraversal отключено по умолчанию. Возможные значения: `notConfigured`, `blocked`, `allowed`.|
|localUserAuthorizations|String|Указывает список авторизованного локального пользователя для контейнера приложений. Это строка в формате Security Descriptor Definition Language (SDDL).|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsFirewallRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsFirewallRule",
  "displayName": "String",
  "description": "String",
  "packageFamilyName": "String",
  "filePath": "String",
  "serviceName": "String",
  "protocol": 1024,
  "localPortRanges": [
    "String"
  ],
  "remotePortRanges": [
    "String"
  ],
  "localAddressRanges": [
    "String"
  ],
  "remoteAddressRanges": [
    "String"
  ],
  "profileTypes": "String",
  "action": "String",
  "trafficDirection": "String",
  "interfaceTypes": "String",
  "edgeTraversal": "String",
  "localUserAuthorizations": "String"
}
```




