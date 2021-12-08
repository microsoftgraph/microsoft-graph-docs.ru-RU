---
title: тип ресурсов microsoftTunnelServer
description: Объект, Microsoft Tunnel представляю
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 507c3d7af22614b96235853e0f5e0351adaf1198
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61336134"
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
|id|String|Id MicrosoftTunnelServer|
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




