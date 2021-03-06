---
title: Тип ресурса Ембеддедсимдевицестате
description: Описание встроенного состояния развертывания кода активации SIM-карты для устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 44f5980881a52428efb655c5f37c8579d445fa84
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49288427"
---
# <a name="embeddedsimdevicestate-resource-type"></a>Тип ресурса Ембеддедсимдевицестате

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Описание встроенного состояния развертывания кода активации SIM-карты для устройства.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Ембеддедсимдевицестатес](../api/intune-esim-embeddedsimdevicestate-list.md)|Коллекция [ембеддедсимдевицестате](../resources/intune-esim-embeddedsimdevicestate.md)|Список свойств и связей объектов [ембеддедсимдевицестате](../resources/intune-esim-embeddedsimdevicestate.md) .|
|[Получение Ембеддедсимдевицестате](../api/intune-esim-embeddedsimdevicestate-get.md)|[ембеддедсимдевицестате](../resources/intune-esim-embeddedsimdevicestate.md)|Чтение свойств и связей объекта [ембеддедсимдевицестате](../resources/intune-esim-embeddedsimdevicestate.md) .|
|[Создание Ембеддедсимдевицестате](../api/intune-esim-embeddedsimdevicestate-create.md)|[ембеддедсимдевицестате](../resources/intune-esim-embeddedsimdevicestate.md)|Создание нового объекта [ембеддедсимдевицестате](../resources/intune-esim-embeddedsimdevicestate.md) .|
|[Удаление Ембеддедсимдевицестате](../api/intune-esim-embeddedsimdevicestate-delete.md)|Нет|Удаляет объект [ембеддедсимдевицестате](../resources/intune-esim-embeddedsimdevicestate.md).|
|[Обновление Ембеддедсимдевицестате](../api/intune-esim-embeddedsimdevicestate-update.md)|[ембеддедсимдевицестате](../resources/intune-esim-embeddedsimdevicestate.md)|Обновление свойств объекта [ембеддедсимдевицестате](../resources/intune-esim-embeddedsimdevicestate.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор состояния встроенного SIM-устройства. Созданное системой значение, назначаемое при создании.|
|createdDateTime|DateTimeOffset|Время создания встроенного состояния SIM-устройства. Созданная сторона службы.|
|modifiedDateTime|DateTimeOffset|Время последнего изменения состояния внедренного SIM-устройства. Обновленная сторона службы.|
|lastSyncDateTime|DateTimeOffset|Время последнего возврата встроенного SIM-устройства. Обновленная сторона службы.|
|универсалинтегратедЦиркуиткардидентифиер|String|Универсальный интегрированный идентификатор карты (УИКЦИД), определяющий оборудование, на котором будет развернут профиль.|
|deviceName|String|Имя устройства, на которое была подготовлена подписка, например DESKTOP — Джо|
|userName|String|Имя пользователя, для которого была подготовлена подписка (например, joe@contoso.com).|
|state|[ембеддедсимдевицестатевалуе](../resources/intune-esim-embeddedsimdevicestatevalue.md)|Состояние операции профиля, примененной к устройству. Возможные значения: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.|
|статедетаилс|String|Строковое описание состояния подготовки.|

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




