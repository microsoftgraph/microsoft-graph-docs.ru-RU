---
title: тип ресурса certificateConnectorDetails
description: Объект используется для получения сведений о соединители сертификатов Intune.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2dd74a003add77fffd029153fc9295b603ce3eef
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61338955"
---
# <a name="certificateconnectordetails-resource-type"></a>тип ресурса certificateConnectorDetails

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект используется для получения сведений о соединители сертификатов Intune.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Сертификат ListConnectorDetailses](../api/intune-raimportcerts-certificateconnectordetails-list.md)|[коллекция certificateConnectorDetails](../resources/intune-raimportcerts-certificateconnectordetails.md)|Список свойств и связей объектов [certificateConnectorDetails.](../resources/intune-raimportcerts-certificateconnectordetails.md)|
|[Получить сертификатConnectorDetails](../api/intune-raimportcerts-certificateconnectordetails-get.md)|[certificateConnectorDetails](../resources/intune-raimportcerts-certificateconnectordetails.md)|Чтение свойств и связей объекта [certificateConnectorDetails.](../resources/intune-raimportcerts-certificateconnectordetails.md)|
|[Создание certificateConnectorDetails](../api/intune-raimportcerts-certificateconnectordetails-create.md)|[certificateConnectorDetails](../resources/intune-raimportcerts-certificateconnectordetails.md)|Создайте новый [объект certificateConnectorDetails.](../resources/intune-raimportcerts-certificateconnectordetails.md)|
|[Удаление сертификатаConnectorDetails](../api/intune-raimportcerts-certificateconnectordetails-delete.md)|Нет|Удаляет [сертификатConnectorDetails](../resources/intune-raimportcerts-certificateconnectordetails.md).|
|[Обновление сертификатаConnectorDetails](../api/intune-raimportcerts-certificateconnectordetails-update.md)|[certificateConnectorDetails](../resources/intune-raimportcerts-certificateconnectordetails.md)|Обновление свойств объекта [certificateConnectorDetails.](../resources/intune-raimportcerts-certificateconnectordetails.md)|
|[действие getHealthMetrics](../api/intune-raimportcerts-certificateconnectordetails-gethealthmetrics.md)|[коллекция keyLongValuePair](../resources/intune-shared-keylongvaluepair.md)|Пока не задокументировано.|
|[действие getHealthMetricTimeSeries](../api/intune-raimportcerts-certificateconnectordetails-gethealthmetrictimeseries.md)|[коллекция certificateConnectorHealthMetricValue](../resources/intune-raimportcerts-certificateconnectorhealthmetricvalue.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для этого набора ConnectorDetails.|
|connectorName|Строка|Имя соединитетеля (за набор во время регистрации).|
|machineName|Строка|Имя компьютера, на которого размещена эта служба соединитела.|
|enrollmentDateTime|DateTimeOffset|Дата и время регистрации этого соединитетеля.|
|lastCheckinDateTime|DateTimeOffset|Дата и время последнего подключения этого соединитетеля к службе.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.certificateConnectorDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.certificateConnectorDetails",
  "id": "String (identifier)",
  "connectorName": "String",
  "machineName": "String",
  "enrollmentDateTime": "String (timestamp)",
  "lastCheckinDateTime": "String (timestamp)"
}
```




