---
title: Тип ресурса operationalInsightsConnection
description: Представляет специализированное подключение ресурсов, которое связывает рабочую область Log Analytics со службой клиентский компонент Центра обновления Windows для бизнеса.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 07725da7d19cdf4c7fdb232f45823e75ffe37d2d
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/19/2022
ms.locfileid: "66857052"
---
# <a name="operationalinsightsconnection-resource-type"></a>Тип ресурса operationalInsightsConnection

Пространство имен: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет специализированное [подключение ресурсов](../resources/windowsupdates-resourceconnection.md), которое связывает рабочую область Log Analytics со службой клиентский компонент Центра обновления Windows для бизнеса.

Наследуется [от resourceConnection](../resources/windowsupdates-resourceconnection.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление operationalInsightsConnections](../api/windowsupdates-updates-list-resourceconnections-operationalinsightsconnection.md)|[Коллекция microsoft.graph.windowsUpdates.operationalInsightsConnection](../resources/windowsupdates-operationalinsightsconnection.md)|Получение списка объектов [operationalInsightsConnection](../resources/windowsupdates-operationalinsightsconnection.md) и их свойств.|
|[Создание operationalInsightsConnection](../api/windowsupdates-updates-post-resourceconnections-operationalinsightsconnection.md)|[microsoft.graph.windowsUpdates.operationalInsightsConnection](../resources/windowsupdates-operationalinsightsconnection.md)|Создайте объект [operationalInsightsConnection](../resources/windowsupdates-operationalinsightsconnection.md) .|
|[Получение operationalInsightsConnection](../api/windowsupdates-operationalinsightsconnection-get.md)|[microsoft.graph.windowsUpdates.operationalInsightsConnection](../resources/windowsupdates-operationalinsightsconnection.md)|Чтение свойств и связей объекта [operationalInsightsConnection](../resources/windowsupdates-operationalinsightsconnection.md) .|
|[Удаление operationalInsightsConnection](../api/windowsupdates-operationalinsightsconnection-delete.md)|Нет|Удаление объекта [operationalInsightsConnection](../resources/windowsupdates-operationalinsightsconnection.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|azureResourceGroupName|Строка|Имя группы ресурсов Azure, содержащего рабочую область Log Analytics.|
|azureSubscriptionId|String|Идентификатор подписки Azure, содержащий рабочую область Log Analytics.|
|id|String|Идентификатор подключения к ресурсу. Ключ. Значение null не допускается. Только для чтения. Возвращается по умолчанию.|
|state|microsoft.graph.windowsUpdates.resourceConnectionState|Состояние соединения. Допустимые значения: `connected`, `notAuthorized`, `notFound`, `unknownFutureValue`.|
|workspaceName|String|Имя рабочей области Log Analytics.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.operationalInsightsConnection",
  "baseType": "microsoft.graph.windowsUpdates.resourceConnection",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.operationalInsightsConnection",
  "azureResourceGroupName": "String",  
  "azureSubscriptionId": "String",
  "id": "String (identifier)",
  "state": "String",
  "workspaceName": "String"
}
```

