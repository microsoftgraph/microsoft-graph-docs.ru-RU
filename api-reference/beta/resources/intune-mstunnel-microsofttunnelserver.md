---
title: тип ресурсов microsoftTunnelServer
description: Объект, Microsoft Tunnel представляю
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2e20964b09e613c02c0e2483d10aece0439b765a
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58783199"
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
|[действие getHealthMetrics](../api/intune-mstunnel-microsofttunnelserver-gethealthmetrics.md)|[коллекция keyLongValuePair](../resources/intune-shared-keylongvaluepair.md)|Пока не задокументировано.|
|[действие getHealthMetricTimeSeries](../api/intune-mstunnel-microsofttunnelserver-gethealthmetrictimeseries.md)|[коллекция metricTimeSeriesDataPoint](../resources/intune-mstunnel-metrictimeseriesdatapoint.md)|Пока не задокументировано.|
|[createServerLogCollectionRequest action](../api/intune-mstunnel-microsofttunnelserver-createserverlogcollectionrequest.md)|[microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Id MicrosoftTunnelServer|
|displayName|Строка|Имя отображения MicrosoftTunnelServer|
|tunnelServerHealthStatus|[microsoftTunnelServerHealthStatus](../resources/intune-mstunnel-microsofttunnelserverhealthstatus.md)|Состояние здоровья MicrosoftTunnelServer. Возможные значения: `unknown`, `healthy`, `unhealthy`, `warning`, `offline`, `upgradeInProgress`, `upgradeFailed`.|
|lastCheckinDateTime|DateTimeOffset|При последней регистрации в MicrosoftTunnelServer|
|agentImageDigest|Строка|Дайджест текущего образа агента, запущенного на этом сервере |
|serverImageDigest|Строка|Дайджест текущего изображения сервера, запущенного на этом сервере |

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
  "lastCheckinDateTime": "String (timestamp)",
  "agentImageDigest": "String",
  "serverImageDigest": "String"
}
```



