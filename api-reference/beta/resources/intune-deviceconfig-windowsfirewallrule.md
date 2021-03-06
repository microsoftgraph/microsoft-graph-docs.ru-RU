---
title: Тип ресурса Виндовсфиреваллруле
description: Правило, контролирующее трафик через брандмауэр Windows.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0ac5437bc95a726ed036de84f3c9a209d01aca31
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49215354"
---
# <a name="windowsfirewallrule-resource-type"></a>Тип ресурса Виндовсфиреваллруле

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Правило, контролирующее трафик через брандмауэр Windows.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Отображаемое имя правила. Не обязательно должны быть уникальными.|
|description|String|Описание правила.|
|паккажефамилинаме|String|Имя семейства пакетов приложения Microsoft Store, на которое влияет правило брандмауэра.|
|Пути|String|Полный путь к файлу приложения, на который влияет правило брандмауэра.|
|Служба|String|Имя, используемое в случаях, когда служба, а не приложение, отправляет или получает трафик.|
|Protocol|Int32|0-255 число, представляющее протокол IP (TCP = 6, UDP = 17). Если этот параметр не указан, используется значение по умолчанию ALL. Допустимые значения — от 0 до 255|
|локалпортранжес|Коллекция строк|Список диапазонов локальных портов. Например, "100-120", "200", "300-320". Если этот параметр не указан, используется значение по умолчанию ALL.|
|ремотепортранжес|Коллекция строк|Список диапазонов удаленных портов. Например, "100-120", "200", "300-320". Если этот параметр не указан, используется значение по умолчанию ALL.|
|локаладдрессранжес|Коллекция строк|Список локальных адресов, охваченных правилом. Значение по умолчанию — любой адрес. Допустимыми являются следующие маркеры:<ul><li>"*" обозначает любой локальный адрес. Если этот параметр задан, он должен быть единственным включенным маркером.</li><li>Подсеть можно указать либо с помощью маски подсети, либо с помощью нотации префикса сети. Если не указана ни маска подсети, ни префикс сети, маска подсети устанавливается по умолчанию 255.255.255.255.</li><li>Допустимый IPv6-адрес.</li><li>Диапазон IPv4-адресов в формате "начальный адрес-конечный адрес" без пробелов.</li><li>Диапазон IPv6-адресов в формате "начальный адрес-конечный адрес" без пробелов.</li></ul>|
|ремотеаддрессранжес|Коллекция строк|Список маркеров, указывающих удаленные адреса, покрытые правилом. Маркеры не зависят от регистра символов. Значение по умолчанию — любой адрес. Допустимыми являются следующие маркеры:<ul><li>"*" обозначает любой удаленный адрес. Если этот параметр задан, он должен быть единственным включенным маркером.</li><li>"Дефаултгатевай"</li><li>-</li><li>Служба</li><li>WINS</li><li>"Интрасеть" (поддерживается в версиях Windows 1809 +)</li><li>"Рмтинтранет" (поддерживается в версиях Windows 1809 +)</li><li>"Интернет" (поддерживается в версиях Windows 1809 +)</li><li>"Ply2Renders" (поддерживается в версиях Windows 1809 +)</li><li>"Локалсубнет" указывает на любой локальный адрес в локальной подсети.</li><li>Подсеть можно указать либо с помощью маски подсети, либо с помощью нотации префикса сети. Если не указана ни маска подсети, ни префикс сети, маска подсети устанавливается по умолчанию 255.255.255.255.</li><li>Допустимый IPv6-адрес.</li><li>Диапазон IPv4-адресов в формате "начальный адрес-конечный адрес" без пробелов.</li><li>Диапазон IPv6-адресов в формате "начальный адрес-конечный адрес" без пробелов.</li></ul>|
|профилетипес|[windowsFirewallRuleNetworkProfileTypes](../resources/intune-deviceconfig-windowsfirewallrulenetworkprofiletypes.md)|Задает профили, к которым относится правило. Если этот параметр не указан, используется значение по умолчанию ALL. Возможные значения: `notConfigured`, `domain`, `private`, `public`.|
|action|[статеманажементсеттинг](../resources/intune-deviceconfig-statemanagementsetting.md)|Действие, которое применяет правило. Если этот параметр не указан, разрешено значение по умолчанию. Возможные значения: `notConfigured`, `blocked`, `allowed`.|
|траффикдиректион|[windowsFirewallRuleTrafficDirectionType](../resources/intune-deviceconfig-windowsfirewallruletrafficdirectiontype.md)|Направление трафика, для которого включено правило. Если этот параметр не указан, используется значение по умолчанию out. Возможные значения: `notConfigured` , `out` , `in` .|
|интерфацетипес|[windowsFirewallRuleInterfaceTypes](../resources/intune-deviceconfig-windowsfirewallruleinterfacetypes.md)|Типы интерфейсов правила. Возможные значения: `notConfigured`, `remoteAccess`, `wireless`, `lan`.|
|еджетраверсал|[статеманажементсеттинг](../resources/intune-deviceconfig-statemanagementsetting.md)|Указывает, включено или отключено обход узлов для этого правила. Параметр Еджетраверсал указывает на то, что определенный входящий трафик может проходить туннели через NAT и другие пограничные устройства, использующие технологию туннелирования Teredo. Чтобы этот параметр работал правильно, приложение или служба с правилом брандмауэра для входящих подключений должны поддерживать IPv6. Основное приложение этого параметра позволяет прослушивателям узла быть глобальными адресами через IPv6-адрес Teredo. По умолчанию в новых правилах отключено свойство Еджетраверсал. Возможные значения: `notConfigured`, `blocked`, `allowed`.|
|локалусераусоризатионс|String|Указывает список авторизованных локальных пользователей для контейнера приложения. Это строка в формате языка определения дескрипторов безопасности (SDDL).|

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




