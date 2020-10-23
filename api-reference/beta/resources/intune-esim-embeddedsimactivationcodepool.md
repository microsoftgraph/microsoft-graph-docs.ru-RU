---
title: Тип ресурса Ембеддедсимактиватионкодепул
description: Пул представляет группу встроенных кодов активации SIM-карты.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9791d55a7f98cf9dcc6d18e3cbe8e117efd49dc8
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48697485"
---
# <a name="embeddedsimactivationcodepool-resource-type"></a>Тип ресурса Ембеддедсимактиватионкодепул

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Пул представляет группу встроенных кодов активации SIM-карты.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Ембеддедсимактиватионкодепулс](../api/intune-esim-embeddedsimactivationcodepool-list.md)|Коллекция [ембеддедсимактиватионкодепул](../resources/intune-esim-embeddedsimactivationcodepool.md)|Список свойств и связей объектов [ембеддедсимактиватионкодепул](../resources/intune-esim-embeddedsimactivationcodepool.md) .|
|[Получение Ембеддедсимактиватионкодепул](../api/intune-esim-embeddedsimactivationcodepool-get.md)|[ембеддедсимактиватионкодепул](../resources/intune-esim-embeddedsimactivationcodepool.md)|Чтение свойств и связей объекта [ембеддедсимактиватионкодепул](../resources/intune-esim-embeddedsimactivationcodepool.md) .|
|[Создание Ембеддедсимактиватионкодепул](../api/intune-esim-embeddedsimactivationcodepool-create.md)|[ембеддедсимактиватионкодепул](../resources/intune-esim-embeddedsimactivationcodepool.md)|Создание нового объекта [ембеддедсимактиватионкодепул](../resources/intune-esim-embeddedsimactivationcodepool.md) .|
|[Удаление Ембеддедсимактиватионкодепул](../api/intune-esim-embeddedsimactivationcodepool-delete.md)|Нет|Удаляет объект [ембеддедсимактиватионкодепул](../resources/intune-esim-embeddedsimactivationcodepool.md).|
|[Обновление Ембеддедсимактиватионкодепул](../api/intune-esim-embeddedsimactivationcodepool-update.md)|[ембеддедсимактиватионкодепул](../resources/intune-esim-embeddedsimactivationcodepool.md)|Обновление свойств объекта [ембеддедсимактиватионкодепул](../resources/intune-esim-embeddedsimactivationcodepool.md) .|
|[Действие assign](../api/intune-esim-embeddedsimactivationcodepool-assign.md)|Коллекция [ембеддедсимактиватионкодепулассигнмент](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор для встроенного пула кода активации SIM-карты. Созданное системой значение, назначаемое при создании.|
|displayName|Строка|Имя администратора внедренного пула кода активации SIM-карты.|
|createdDateTime|DateTimeOffset|Время создания внедренного пула кода активации SIM-карты. Созданная сторона службы.|
|modifiedDateTime|DateTimeOffset|Время последнего изменения пула кода активации внедренной SIM-карты. Обновленная сторона службы.|
|активатионкодес|Коллекция [ембеддедсимактиватионкоде](../resources/intune-esim-embeddedsimactivationcode.md)|Коды активации, принадлежащие этому пулу. Это свойство навигации используется для публикации кодов активации в Intune, но не может использоваться для считывания кодов активации из Intune.|
|активатионкодекаунт|Int32|Общее количество кодов активации, относящихся к этому пулу.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|Коллекция [ембеддедсимактиватионкодепулассигнмент](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|Навигационное свойство в список целевых объектов, которым назначен этот пул.|
|deviceStates|Коллекция [ембеддедсимдевицестате](../resources/intune-esim-embeddedsimdevicestate.md)|Свойство навигации для списка состояний устройств для этого пула.|

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





