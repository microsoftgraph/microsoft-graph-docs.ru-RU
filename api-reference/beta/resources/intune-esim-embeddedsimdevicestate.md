---
title: тип ресурса embeddedSIMDeviceState
description: Описывает состояние развертывания встроенного кода активации SIM по отношению к устройству.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0654c71369d9682887d36f02e6cddf1eb9772e0f
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58789907"
---
# <a name="embeddedsimdevicestate-resource-type"></a>тип ресурса embeddedSIMDeviceState

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Описывает состояние развертывания встроенного кода активации SIM по отношению к устройству.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список встроенныхSIMDeviceStates](../api/intune-esim-embeddedsimdevicestate-list.md)|[коллекция embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)|Список свойств и связей встроенных [объектовSIMDeviceState.](../resources/intune-esim-embeddedsimdevicestate.md)|
|[Get embeddedSIMDeviceState](../api/intune-esim-embeddedsimdevicestate-get.md)|[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)|Чтение свойств и связей встроенного [объектаSIMDeviceState.](../resources/intune-esim-embeddedsimdevicestate.md)|
|[Создание встроенных элементовSIMDeviceState](../api/intune-esim-embeddedsimdevicestate-create.md)|[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)|Создайте новый [встроенный объектSIMDeviceState.](../resources/intune-esim-embeddedsimdevicestate.md)|
|[Удаление встроенных элементовSIMDeviceState](../api/intune-esim-embeddedsimdevicestate-delete.md)|Нет|Удаляет [встроенныйSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md).|
|[Update embeddedSIMDeviceState](../api/intune-esim-embeddedsimdevicestate-update.md)|[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)|Обновление свойств встроенного [объектаSIMDeviceState.](../resources/intune-esim-embeddedsimdevicestate.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор для состояния встроенного sim-устройства. Созданное в системе значение, назначенное при его создания.|
|createdDateTime|DateTimeOffset|Время создания состояния встроенного sim-устройства. Сгенерированная сторона службы.|
|modifiedDateTime|DateTimeOffset|Время последнего изменения состояния встроенного SIM-устройства. Обновленная сторона службы.|
|lastSyncDateTime|DateTimeOffset|Время последней регистрации встроенного sim-устройства. Обновленная сторона службы.|
|universalIntegratedCircuitCardIdentifier|Строка|Идентификатор универсальной интегрированной схемной карты (UICCID), определяющий оборудование, на которое будет развернут профиль.|
|deviceName|String|Имя устройства, на которое была предусмотрена подписка, например DESKTOP-JOE|
|userName|String|Имя пользователя, для которого была предусмотрена подписка, например joe@contoso.com|
|state|[embeddedSIMDeviceStateValue](../resources/intune-esim-embeddedsimdevicestatevalue.md)|Состояние операции профиля, примененной к устройству. Возможные значения: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.|
|stateDetails|String|Строковое описание состояния подготовка.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.embeddedSIMDeviceState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.embeddedSIMDeviceState",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "universalIntegratedCircuitCardIdentifier": "String",
  "deviceName": "String",
  "userName": "String",
  "state": "String",
  "stateDetails": "String"
}
```



