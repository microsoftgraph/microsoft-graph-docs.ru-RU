---
title: Тип ресурса ndesConnector
description: Объект, представляючий соединителя OnPrem Ndes.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 20f58e58b36abe69ecdb9ef24da990516d8ea01ed37cf3ad3fba44e6f708fdb8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54198250"
---
# <a name="ndesconnector-resource-type"></a>Тип ресурса ndesConnector

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект, представляючий соединителя OnPrem Ndes.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список ndesConnectors](../api/intune-deviceconfig-ndesconnector-list.md)|[Коллекция ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)|Список свойств и связей объектов [ndesConnector.](../resources/intune-deviceconfig-ndesconnector.md)|
|[Get ndesConnector](../api/intune-deviceconfig-ndesconnector-get.md)|[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md).|Чтение свойств и связей объекта [ndesConnector.](../resources/intune-deviceconfig-ndesconnector.md)|
|[Создание ndesConnector](../api/intune-deviceconfig-ndesconnector-create.md)|[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md).|Создайте новый [объект ndesConnector.](../resources/intune-deviceconfig-ndesconnector.md)|
|[Удаление ndesConnector](../api/intune-deviceconfig-ndesconnector-delete.md)|Нет|Удаляет [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md).|
|[Обновление ndesConnector](../api/intune-deviceconfig-ndesconnector-update.md)|[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md).|Обновление свойств объекта [ndesConnector.](../resources/intune-deviceconfig-ndesconnector.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ соединиттеля NDES.|
|lastConnectionDateTime|DateTimeOffset|Последнее время подключения для соединитетеля Ndes|
|state|[ndesConnectorState](../resources/intune-deviceconfig-ndesconnectorstate.md)|Состояние соединитетеля Ndes. Возможные значения: `none`, `active`, `inactive`.|
|displayName|Строка|Дружеское имя соединиттеля Ndes.|

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




