---
title: Тип ресурса embeddedSIMDeviceState
description: Описывает состояние развертывания кода активации внедренных диспетчера установки при использовании устройства.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a79453c8d8bcb5682da64ce480f1a2f9f210a673
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415574"
---
# <a name="embeddedsimdevicestate-resource-type"></a>Тип ресурса embeddedSIMDeviceState

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Описывает состояние развертывания кода активации внедренных диспетчера установки при использовании устройства.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список embeddedSIMDeviceStates](../api/intune-esim-embeddedsimdevicestate-list.md)|[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) коллекции|Свойства списка и связей объектов [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) .|
|[Получение embeddedSIMDeviceState](../api/intune-esim-embeddedsimdevicestate-get.md)|[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)|Чтение свойства и связи объекта [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) .|
|[Создание embeddedSIMDeviceState](../api/intune-esim-embeddedsimdevicestate-create.md)|[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)|Создание нового объекта [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) .|
|[Удаление embeddedSIMDeviceState](../api/intune-esim-embeddedsimdevicestate-delete.md)|Нет|Удаляет [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md).|
|[Обновление embeddedSIMDeviceState](../api/intune-esim-embeddedsimdevicestate-update.md)|[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)|Обновление свойства объекта [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для внедренных состояние устройства диспетчера установки. Значение, назначенное при создании создаваемый системой.|
|createdDateTime|DateTimeOffset|Время создания внедренных состояние устройства диспетчера установки. Создан со стороны службы.|
|modifiedDateTime|DateTimeOffset|Время последнего изменения внедренного состояние устройства диспетчера установки. Обновление со стороны службы.|
|lastSyncDateTime|DateTimeOffset|Время, внедренные устройства диспетчера установки последнего возврата. Обновление со стороны службы.|
|universalIntegratedCircuitCardIdentifier|String|Универсальные интегральной карточки идентификатор (UICCID) Идентификация оборудования, на котором профиль — для развертывания.|
|deviceName|String|Имя устройства, к которому был подписки например рабочего СТОЛА ДЖО подготовить к работе|
|userName|String|Имя пользователя, который был подписки подготовлен к например joe@contoso.com|
|state|[embeddedSIMDeviceStateValue](../resources/intune-esim-embeddedsimdevicestatevalue.md)|Состояние операции профилей, применяемые к устройства. Возможные значения: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.|
|stateDetails|String|Строка Описание подготовки состояния.|

## <a name="relationships"></a>Отношения
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




