---
title: Тип ресурса embeddedSIMActivationCodePool
description: Пул представляет группу внедренных коды активации диспетчера установки.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d6b5d67f90b8f0da701493380b2c3668b6d87f6c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823515"
---
# <a name="embeddedsimactivationcodepool-resource-type"></a>Тип ресурса embeddedSIMActivationCodePool

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Пул представляет группу внедренных коды активации диспетчера установки.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список embeddedSIMActivationCodePools](../api/intune-esim-embeddedsimactivationcodepool-list.md)|[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) коллекции|Свойства списка и связей объектов [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) .|
|[Получение embeddedSIMActivationCodePool](../api/intune-esim-embeddedsimactivationcodepool-get.md)|[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)|Чтение свойства и связи объекта [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) .|
|[Создание embeddedSIMActivationCodePool](../api/intune-esim-embeddedsimactivationcodepool-create.md)|[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)|Создание нового объекта [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) .|
|[Удаление embeddedSIMActivationCodePool](../api/intune-esim-embeddedsimactivationcodepool-delete.md)|Нет|Удаляет [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md).|
|[Обновление embeddedSIMActivationCodePool](../api/intune-esim-embeddedsimactivationcodepool-update.md)|[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)|Обновление свойства объекта [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) .|
|[Действие assign](../api/intune-esim-embeddedsimactivationcodepool-assign.md)|[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) коллекции|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор для внедренных пула кода активации диспетчера установки. Значение, назначенное при создании создаваемый системой.|
|displayName|Строка|Имя группы внедренных диспетчера установки активации кода определенные администратором.|
|createdDateTime|DateTimeOffset|Время создания внедренных пула кода активации диспетчера установки. Создан со стороны службы.|
|modifiedDateTime|DateTimeOffset|Время последнего изменения внедренного пула кода активации диспетчера установки. Обновление со стороны службы.|
|activationCodes|[embeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md) коллекции|Коды активации, которые относятся к этот пул. Это свойство навигации использовать для активации кодов Intune, но не может использоваться для чтения из Intune коды активации.|
|activationCodeCount|Int32|Общее число коды активации, которые относятся к этот пул.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) коллекции|Свойство переходов в список конечных объектов, которым назначена этого пула.|
|deviceStates|[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) коллекции|Навигационные свойства со списком состояния устройств для этого пула.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.embeddedSIMActivationCodePool"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePool",
  "id": "String (identifier)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "activationCodes": [
    {
      "@odata.type": "microsoft.graph.embeddedSIMActivationCode",
      "integratedCircuitCardIdentifier": "String",
      "matchingIdentifier": "String",
      "smdpPlusServerAddress": "String"
    }
  ],
  "activationCodeCount": 1024
}
```





