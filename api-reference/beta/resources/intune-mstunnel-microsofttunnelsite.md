---
title: тип ресурса microsoftTunnelSite
description: Сущность, представляюая Microsoft Tunnel сайт
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4f4ce76a16d63d4d97c7ab27fa74c53fdcdc3408
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61347321"
---
# <a name="microsofttunnelsite-resource-type"></a>тип ресурса microsoftTunnelSite

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность, представляюая Microsoft Tunnel сайт

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список microsoftTunnelSites](../api/intune-mstunnel-microsofttunnelsite-list.md)|[коллекция microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md)|Список свойств и связей объектов [microsoftTunnelSite.](../resources/intune-mstunnel-microsofttunnelsite.md)|
|[Получите microsoftTunnelSite](../api/intune-mstunnel-microsofttunnelsite-get.md)|[microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md)|Чтение свойств и связей объекта [microsoftTunnelSite.](../resources/intune-mstunnel-microsofttunnelsite.md)|
|[Создание microsoftTunnelSite](../api/intune-mstunnel-microsofttunnelsite-create.md)|[microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md)|Создайте новый [объект microsoftTunnelSite.](../resources/intune-mstunnel-microsofttunnelsite.md)|
|[Удаление microsoftTunnelSite](../api/intune-mstunnel-microsofttunnelsite-delete.md)|Нет|Удаляет [microsoftTunnelSite.](../resources/intune-mstunnel-microsofttunnelsite.md)|
|[Обновление microsoftTunnelSite](../api/intune-mstunnel-microsofttunnelsite-update.md)|[microsoftTunnelSite](../resources/intune-mstunnel-microsofttunnelsite.md)|Обновление свойств объекта [microsoftTunnelSite.](../resources/intune-mstunnel-microsofttunnelsite.md)|
|[requestUpgrade action](../api/intune-mstunnel-microsofttunnelsite-requestupgrade.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Id MicrosoftTunnelSite|
|displayName|String|Имя отображения MicrosoftTunnelSite|
|description|Строка|Описание MicrosoftTunnelSite|
|publicAddress|Строка|Имя или IP-адрес общественного домена MicrosoftTunnelSite|
|upgradeWindowUtcOffsetInMinutes|Int32|Зона времени сайта, представленная в качестве минутного смещения от UTC|
|upgradeWindowStartTime|TimeOfDay|Время запуска окна обновления сайта|
|upgradeWindowEndTime|TimeOfDay|Время окончания дня окна обновления сайта|
|upgradeAutomatically|Boolean|Параметр автоматического обновления сайта. True для автоматических обновлений, false для ручного управления|
|upgradeAvailable|Boolean|True, если доступно обновление|
|internalNetworkProbeUrl|String|URL-адрес зонда внутреннего доступа к сети MicrosoftTunnelSite|
|roleScopeTagIds|Коллекция String|Список тегов области для этого экземпляра Entity.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|microsoftTunnelConfiguration|[microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md)|MicrosoftTunnelConfiguration, примененная к этому MicrosoftTunnelSite|
|microsoftTunnelServers|[коллекция microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md)|Список microsoftTunnelServers, зарегистрированных в этом MicrosoftTunnelSite|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.microsoftTunnelSite"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftTunnelSite",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publicAddress": "String",
  "upgradeWindowUtcOffsetInMinutes": 1024,
  "upgradeWindowStartTime": "String (time of day)",
  "upgradeWindowEndTime": "String (time of day)",
  "upgradeAutomatically": true,
  "upgradeAvailable": true,
  "internalNetworkProbeUrl": "String",
  "roleScopeTagIds": [
    "String"
  ]
}
```




