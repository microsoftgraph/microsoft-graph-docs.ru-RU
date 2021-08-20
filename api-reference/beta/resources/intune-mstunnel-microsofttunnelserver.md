---
title: тип ресурсов microsoftTunnelServer
description: Объект, Microsoft Tunnel представляю
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ad8186090c30267890e2e1240111edd1a8de5a6eb5c52e452fe9570d32dc319c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54227262"
---
# <a name="microsofttunnelserver-resource-type"></a>тип ресурсов microsoftTunnelServer

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект, Microsoft Tunnel представляю

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список microsoftTunnelServers](../api/intune-mstunnel-microsofttunnelserver-list.md)|[коллекция microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md)|Список свойств и связей объектов [microsoftTunnelServer.](../resources/intune-mstunnel-microsofttunnelserver.md)|
|[Получите microsoftTunnelServer](../api/intune-mstunnel-microsofttunnelserver-get.md)|[microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md)|Чтение свойств и связей объекта [microsoftTunnelServer.](../resources/intune-mstunnel-microsofttunnelserver.md)|
|[Создание microsoftTunnelServer](../api/intune-mstunnel-microsofttunnelserver-create.md)|[microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md)|Создание нового [объекта microsoftTunnelServer.](../resources/intune-mstunnel-microsofttunnelserver.md)|
|[Удаление microsoftTunnelServer](../api/intune-mstunnel-microsofttunnelserver-delete.md)|Нет|Удаляет [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md).|
|[Обновление microsoftTunnelServer](../api/intune-mstunnel-microsofttunnelserver-update.md)|[microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md)|Обновление свойств объекта [microsoftTunnelServer.](../resources/intune-mstunnel-microsofttunnelserver.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Id MicrosoftTunnelServer|
|displayName|Строка|Имя отображения MicrosoftTunnelServer|
|tunnelServerHealthStatus|[microsoftTunnelServerHealthStatus](../resources/intune-mstunnel-microsofttunnelserverhealthstatus.md)|Состояние здоровья MicrosoftTunnelServer. Возможные значения: `unknown`, `healthy`, `unhealthy`, `warning`, `offline`, `upgradeInProgress`, `upgradeFailed`.|
|lastCheckinDateTime|DateTimeOffset|При последней регистрации в MicrosoftTunnelServer|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.microsoftTunnelServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftTunnelServer",
  "id": "String (identifier)",
  "displayName": "String",
  "tunnelServerHealthStatus": "String",
  "lastCheckinDateTime": "String (timestamp)"
}
```




