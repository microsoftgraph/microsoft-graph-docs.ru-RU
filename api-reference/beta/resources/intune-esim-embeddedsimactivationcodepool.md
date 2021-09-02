---
title: тип ресурса embeddedSIMActivationCodePool
description: Пул представляет собой группу встроенных кодов активации SIM-карт.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9579f4af46ca2b35fde91888ced9973590634095
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58801075"
---
# <a name="embeddedsimactivationcodepool-resource-type"></a>тип ресурса embeddedSIMActivationCodePool

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Пул представляет собой группу встроенных кодов активации SIM-карт.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список встроенныхSIMActivationCodePools](../api/intune-esim-embeddedsimactivationcodepool-list.md)|[коллекция embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)|Список свойств и связей встроенных [объектовSIMActivationCodePool.](../resources/intune-esim-embeddedsimactivationcodepool.md)|
|[Получить встроенныйSIMActivationCodePool](../api/intune-esim-embeddedsimactivationcodepool-get.md)|[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)|Чтение свойств и связей встроенного [объектаSIMActivationCodePool.](../resources/intune-esim-embeddedsimactivationcodepool.md)|
|[Создание встроенныхSIMActivationCodePool](../api/intune-esim-embeddedsimactivationcodepool-create.md)|[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)|Создайте новый [встроенный объектSIMActivationCodePool.](../resources/intune-esim-embeddedsimactivationcodepool.md)|
|[Удаление встроенныхSIMActivationCodePool](../api/intune-esim-embeddedsimactivationcodepool-delete.md)|Нет|Удаляет [встроенныйSIMActivationCodePool.](../resources/intune-esim-embeddedsimactivationcodepool.md)|
|[Обновление встроенныхSIMActivationCodePool](../api/intune-esim-embeddedsimactivationcodepool-update.md)|[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)|Обновление свойств встроенного [объектаSIMActivationCodePool.](../resources/intune-esim-embeddedsimactivationcodepool.md)|
|[Действие assign](../api/intune-esim-embeddedsimactivationcodepool-assign.md)|[коллекция embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор встроенного пула кодов активации SIM. Созданное в системе значение, назначенное при его создания.|
|displayName|Строка|Администратор определил имя встроенного пула кодов активации SIM-карты.|
|createdDateTime|DateTimeOffset|Время создания встроенного пула кодов активации SIM-карты. Сгенерированная сторона службы.|
|modifiedDateTime|DateTimeOffset|Время последнего изменения встроенного пула кодов активации SIM-карты. Обновленная сторона службы.|
|activationCodes|[коллекция embeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md)|Коды активации, которые принадлежат этому пулу. Это свойство навигации используется для публикации кодов активации в Intune, но не может использоваться для чтения кодов активации из Intune.|
|activationCodeCount|Int32|Общее количество кодов активации, которые относятся к этому пулу.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|[коллекция embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)|Свойство навигации к списку целей, которым назначен этот пул.|
|deviceStates|[коллекция embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)|Свойство навигации к списку состояния устройств для этого пула.|

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



