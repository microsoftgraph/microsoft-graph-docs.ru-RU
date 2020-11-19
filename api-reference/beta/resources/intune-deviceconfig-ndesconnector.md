---
title: Тип ресурса Ндесконнектор
description: Сущность, представляющая локальный Соединитель NDES.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 36d41032e98253f81a409665fb35b7e25f672053
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49273328"
---
# <a name="ndesconnector-resource-type"></a>Тип ресурса Ндесконнектор

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность, представляющая локальный Соединитель NDES.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Ндесконнекторс](../api/intune-deviceconfig-ndesconnector-list.md)|Коллекция [ндесконнектор](../resources/intune-deviceconfig-ndesconnector.md)|Список свойств и связей объектов [ндесконнектор](../resources/intune-deviceconfig-ndesconnector.md) .|
|[Получение Ндесконнектор](../api/intune-deviceconfig-ndesconnector-get.md)|[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md).|Чтение свойств и связей объекта [ндесконнектор](../resources/intune-deviceconfig-ndesconnector.md) .|
|[Создание Ндесконнектор](../api/intune-deviceconfig-ndesconnector-create.md)|[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md).|Создание нового объекта [ндесконнектор](../resources/intune-deviceconfig-ndesconnector.md) .|
|[Удаление Ндесконнектор](../api/intune-deviceconfig-ndesconnector-delete.md)|Нет|Удаляет объект [ндесконнектор](../resources/intune-deviceconfig-ndesconnector.md).|
|[Обновление Ндесконнектор](../api/intune-deviceconfig-ndesconnector-update.md)|[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md).|Обновление свойств объекта [ндесконнектор](../resources/intune-deviceconfig-ndesconnector.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ соединителя NDES Connector.|
|lastConnectionDateTime|DateTimeOffset|Время последнего подключения для соединителя NDES Connector|
|state|[ндесконнекторстате](../resources/intune-deviceconfig-ndesconnectorstate.md)|Состояние соединителя NDES Connector. Возможные значения: `none`, `active`, `inactive`.|
|displayName|String|Понятное имя соединителя NDES Connector.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ndesConnector"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.ndesConnector",
  "id": "String (identifier)",
  "lastConnectionDateTime": "String (timestamp)",
  "state": "String",
  "displayName": "String"
}
```




