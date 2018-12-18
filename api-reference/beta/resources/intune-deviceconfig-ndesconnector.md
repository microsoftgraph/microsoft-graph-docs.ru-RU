---
title: Тип ресурса ndesConnector
description: Сущности, который представляет соединителя OnPrem Ndes.
author: tfitzmac
ms.openlocfilehash: e37a20c440546094424d0284bd1d7ffbbeb60bdd
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332293"
---
# <a name="ndesconnector-resource-type"></a>Тип ресурса ndesConnector

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Сущности, который представляет соединителя OnPrem Ndes.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список ndesConnectors](../api/intune-deviceconfig-ndesconnector-list.md)|[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) коллекции|Свойства списка и связей объектов [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) .|
|[Получение ndesConnector](../api/intune-deviceconfig-ndesconnector-get.md)|[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md).|Чтение свойства и связи объекта [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) .|
|[Создание ndesConnector](../api/intune-deviceconfig-ndesconnector-create.md)|[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md).|Создание нового объекта [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) .|
|[Удаление ndesConnector](../api/intune-deviceconfig-ndesconnector-delete.md)|Нет|Удаляет [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md).|
|[Обновление ndesConnector](../api/intune-deviceconfig-ndesconnector-update.md)|[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md).|Обновление свойства объекта [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ NDES соединителя.|
|lastConnectionDateTime|DateTimeOffset|Время последнего подключения для соединителя Ndes|
|state|[ndesConnectorState](../resources/intune-deviceconfig-ndesconnectorstate.md)|Состояние NDES соединителя. Возможные значения: `none`, `active`, `inactive`.|
|displayName|Строка|Понятное имя соединителя Ndes.|

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





