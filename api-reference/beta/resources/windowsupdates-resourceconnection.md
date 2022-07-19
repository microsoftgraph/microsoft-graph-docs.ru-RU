---
title: Тип ресурса resourceConnection
description: Представляет подключения к внешним ресурсам, из которых будут создаваться более специализированные подключения.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: dd21fba95209dbcc1ce5f868b98fa818fe34b254
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/19/2022
ms.locfileid: "66857051"
---
# <a name="resourceconnection-resource-type"></a>Тип ресурса resourceConnection

Пространство имен: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет подключения к внешним ресурсам, из которых будут создаваться более специализированные подключения, такие как [operationalInsightsConnection](../resources/windowsupdates-operationalinsightsconnection.md) .

Это абстрактный тип.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление resourceConnections](../api/windowsupdates-updates-list-resourceconnections.md)|[Коллекция microsoft.graph.windowsUpdates.resourceConnection](../resources/windowsupdates-resourceconnection.md)|Получение списка объектов [resourceConnection](../resources/windowsupdates-resourceconnection.md) и их свойств.|
|[Получение resourceConnection](../api/windowsupdates-resourceconnection-get.md)|[microsoft.graph.windowsUpdates.resourceConnection](../resources/windowsupdates-resourceconnection.md)|Чтение свойств и связей объекта [resourceConnection](../resources/windowsupdates-resourceconnection.md) .|
|[Удаление resourceConnection](../api/windowsupdates-resourceconnection-delete.md)|Нет|Удаление объекта [resourceConnection](../resources/windowsupdates-resourceconnection.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор подключения к ресурсу. Ключ. Значение null не допускается. Только для чтения. Возвращается по умолчанию.|
|state|microsoft.graph.windowsUpdates.resourceConnectionState|Состояние соединения. Допустимые значения: `connected`, `notAuthorized`, `notFound`, `unknownFutureValue`.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.resourceConnection",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.resourceConnection",
  "id": "String (identifier)",
  "state": "String"
}
```

