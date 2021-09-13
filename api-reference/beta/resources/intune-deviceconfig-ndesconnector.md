---
title: Тип ресурса ndesConnector
description: Объект, представляючий соединителя OnPrem Ndes.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 222c675d66fc400c83161377def32420ad81d3fa
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59091652"
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
|[Get ndesConnector](../api/intune-deviceconfig-ndesconnector-get.md)|[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)|Чтение свойств и связей объекта [ndesConnector.](../resources/intune-deviceconfig-ndesconnector.md)|
|[Создание ndesConnector](../api/intune-deviceconfig-ndesconnector-create.md)|[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)|Создайте новый [объект ndesConnector.](../resources/intune-deviceconfig-ndesconnector.md)|
|[Удаление ndesConnector](../api/intune-deviceconfig-ndesconnector-delete.md)|Нет|Удаляет [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md).|
|[Обновление ndesConnector](../api/intune-deviceconfig-ndesconnector-update.md)|[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)|Обновление свойств объекта [ndesConnector.](../resources/intune-deviceconfig-ndesconnector.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ соединиттеля NDES.|
|lastConnectionDateTime|DateTimeOffset|Последнее время подключения для соединитетеля Ndes|
|state|[ndesConnectorState](../resources/intune-deviceconfig-ndesconnectorstate.md)|Состояние соединитетеля Ndes. Возможные значения: `none`, `active`, `inactive`.|
|displayName|String|Дружеское имя соединиттеля Ndes.|

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



