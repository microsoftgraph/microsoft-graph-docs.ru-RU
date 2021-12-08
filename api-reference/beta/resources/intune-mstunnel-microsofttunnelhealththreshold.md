---
title: тип ресурсов microsoftTunnelHealthThreshold
description: Сущность, представляюная пороговые значения для здоровья метрики здоровья.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 73ed731fa5ca6fe5efac3ea0b7e7558a5ed75b12
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61337240"
---
# <a name="microsofttunnelhealththreshold-resource-type"></a>тип ресурсов microsoftTunnelHealthThreshold

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность, представляюная пороговые значения для здоровья метрики здоровья.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список microsoftTunnelHealthThresholds](../api/intune-mstunnel-microsofttunnelhealththreshold-list.md)|[коллекция microsoftTunnelHealthThreshold](../resources/intune-mstunnel-microsofttunnelhealththreshold.md)|Список свойств и связей объектов [microsoftTunnelHealthThreshold.](../resources/intune-mstunnel-microsofttunnelhealththreshold.md)|
|[Получите microsoftTunnelHealthThreshold](../api/intune-mstunnel-microsofttunnelhealththreshold-get.md)|[microsoftTunnelHealthThreshold](../resources/intune-mstunnel-microsofttunnelhealththreshold.md)|Чтение свойств и связей объекта [microsoftTunnelHealthThreshold.](../resources/intune-mstunnel-microsofttunnelhealththreshold.md)|
|[Создание microsoftTunnelHealthThreshold](../api/intune-mstunnel-microsofttunnelhealththreshold-create.md)|[microsoftTunnelHealthThreshold](../resources/intune-mstunnel-microsofttunnelhealththreshold.md)|Создайте новый [объект microsoftTunnelHealthThreshold.](../resources/intune-mstunnel-microsofttunnelhealththreshold.md)|
|[Удаление microsoftTunnelHealthThreshold](../api/intune-mstunnel-microsofttunnelhealththreshold-delete.md)|Нет|Удаляет [microsoftTunnelHealthThreshold](../resources/intune-mstunnel-microsofttunnelhealththreshold.md).|
|[Обновление microsoftTunnelHealthThreshold](../api/intune-mstunnel-microsofttunnelhealththreshold-update.md)|[microsoftTunnelHealthThreshold](../resources/intune-mstunnel-microsofttunnelhealththreshold.md)|Обновление свойств объекта [microsoftTunnelHealthThreshold.](../resources/intune-mstunnel-microsofttunnelhealththreshold.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Имя метрик|
|healthyThreshold|Int64|Пороговое значение для здоровья|
|unhealthyThreshold|Int64|Порог для неработоспособного|
|defaultHealthyThreshold|Int64|Пороговое значение по умолчанию для того, чтобы быть здоровым|
|defaultUnhealthyThreshold|Int64|Пороговое значение по умолчанию для неработоспособного|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.microsoftTunnelHealthThreshold"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftTunnelHealthThreshold",
  "id": "String (identifier)",
  "healthyThreshold": 1024,
  "unhealthyThreshold": 1024,
  "defaultHealthyThreshold": 1024,
  "defaultUnhealthyThreshold": 1024
}
```




