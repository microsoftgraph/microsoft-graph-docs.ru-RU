---
title: Тип ресурса embeddedSIMDeviceState
description: Описывает состояние развертывания кода активации внедренных диспетчера установки при использовании устройства.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ce96250b8c64fc97171ee7721ca44b4cd4579072
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912626"
---
# <a name="embeddedsimdevicestate-resource-type"></a>Тип ресурса embeddedSIMDeviceState

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

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
|id|Строка|Уникальный идентификатор для внедренных состояние устройства диспетчера установки. Значение, назначенное при создании создаваемый системой.|
|createdDateTime|DateTimeOffset|Время создания внедренных состояние устройства диспетчера установки. Создан со стороны службы.|
|modifiedDateTime|DateTimeOffset|Время последнего изменения внедренного состояние устройства диспетчера установки. Обновление со стороны службы.|
|lastSyncDateTime|DateTimeOffset|Время, внедренные устройства диспетчера установки последнего возврата. Обновление со стороны службы.|
|universalIntegratedCircuitCardIdentifier|Строка|Универсальные интегральной карточки идентификатор (UICCID) Идентификация оборудования, на котором профиль — для развертывания.|
|deviceName|String|Имя устройства, к которому был подписки например рабочего СТОЛА ДЖО подготовить к работе|
|userName|String|Имя пользователя, который был подписки подготовлен к например joe@contoso.com|
|state|[embeddedSIMDeviceStateValue](../resources/intune-esim-embeddedsimdevicestatevalue.md)|Состояние операции профилей, применяемые к устройства. Возможные значения: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.|
|stateDetails|Строка|Строка Описание подготовки состояния.|

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





