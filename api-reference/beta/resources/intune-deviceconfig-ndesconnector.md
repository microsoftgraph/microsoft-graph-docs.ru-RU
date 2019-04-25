---
title: Тип ресурса Ндесконнектор
description: Сущность, представляющая локальный Соединитель NDES.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3781827d93f1e646becc2ee47de57cbba82dfc63
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554473"
---
# <a name="ndesconnector-resource-type"></a>Тип ресурса Ндесконнектор

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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
|state|[Ндесконнекторстате](../resources/intune-deviceconfig-ndesconnectorstate.md)|Состояние соединителя NDES Connector. Возможные значения: `none`, `active`, `inactive`.|
|displayName|String|Понятное имя соединителя NDES Connector.|

## <a name="relationships"></a>Отношения
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





